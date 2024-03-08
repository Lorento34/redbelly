![1_kNm5E2XtpiKdacDmywA8-w](https://github.com/Lorento34/redbelly/assets/84406096/fdb0c843-b7ff-44e1-86be-a1dd0d3cc03f)

<h1>Donanım Gereksinimleri<h6>

Redbelly Network düğümünü (Node) çalıştırmak için minimum donanım gereksinimleri

- Cpu : 8-core Cpu
- Mimari: - x86-64 (Bunun haricinde x64, x86_64, AMD64, ve Intel 64)
- Ram: 16 GB
- İşletim Sistemi: Ubuntu 22.04.2 LTS ya da üst sürümler (x86-64)
- Depolama: 1 TB
- Ağ Bant Genişliği: 40 Mbps
- TCP bağlantı noktaları: 8545, 8546, 1111 ve 1888 (Önerilir)


Arkadaşlar rehber biraz uzun olacak üstün körü anlatıp geçtiğimde biliyorum ki telegramda birçok kişi anlayamayacak ve nasıl olduğunu soracak ya da birçok kişi hata alacak. Bu karışıklığın önüne geçmek için ve aramıza yeni katılanları da düşünerek ayrıntılı ve resimli bir rehber hazırlıyorum. Rehberde ki adımları dikkatlice okuyup, takip ederseniz sorunsuz bir şekilde kurulumu tamamlayabilirsiniz. Ben bu rehbere göre yaptım ve çalışıyor. Kurulum 3 adımdan oluşacak. Bunlar, domain satın alma, domain için Dns yapılandırılması ve düğüm (node) kurulumu.


<h1>Domain Satın Alma<h6>
Bunun için ben <a href="https://www.godaddy.com/en-ie">Godaddy</a> platformunu kullandım. Kullanımı basit ve fiyat olarak uygun domainler var. 50-60 TL’ye domain alabilirsiniz. Ama siz istediğiniz platformu kullanabilirsiniz ya da önceden aldığınız bir domain varsa onu da kullanabilirsiniz. Ama ben size godaddy üzerinden dns yönlendirme işlemlerini anlatacağım. Eğer bu konuya yabancıysanız sizde domaini godaddy üzerinden satın alıp, kafanız karışmadan aşağıda ki rehbere göre işlemleri yapabilirsiniz. Domaini satın almadan önce mutlaka üyelik açın çünkü daha sonra bir sorun olduğunda müşteri temsilcisiyle daha rahat iletişim kurabilirsiniz. Domain satın alma kısmı zaten basit olduğu için onu anlatmıyorum. Ama domaini satın alırken sepete ekledikten sonra ödeme kısmında bir takım ekstra özellikler eklemek isteyip istemediğinizi soracak hepsini reddedin ve sadece domaini satın alın 1 yıllık. Satın almayı yaptığınızı varsayarak 2. adım olan dns yönlendirme işlemine geçiyoruz.

<h1>Dns Yönlendirme</h1>

1- Bu işlem için <a href="https://dash.cloudflare.com/sign-up">Cloudflare</a>  sitesine gidin ve üyelik oluşturun. Mailinize gelen doğrulama linkine tıklayarak mail adresinizi doğrulayın.

![1](https://github.com/Lorento34/redbelly/assets/84406096/67acac57-f871-4846-835b-b802496fa812)

2- Sizi şöyle bir ekran karşılıyacak. ```Add a website or application``` yazan butona tıklayın.


![2](https://github.com/Lorento34/redbelly/assets/84406096/dad248d4-43ae-40f0-b1ae-2d0a844983fb)


3- Bir sonra ki adımda şöyle bir ekran gelecek. ```Enter domain name``` yazan yere satin aldığınız domain adını yazın. Domainin başında https, www gibi şeyler yazmayın. Aşağıda ki gibi olsun. Sonra ```Enter``` butonuna tıklayı ve devam edin…



![3](https://github.com/Lorento34/redbelly/assets/84406096/449e4065-3656-46f4-9504-28dd66bb2fe0)


4- Bu kısımda planı seçeceğiz. Cloudflare’nin verdiği hizmetler paralı olduğu için bazı planlar var. Ama biz en aşağıda ki ```free``` seçeceğiz. Bu ücretsiz plan. Daha sonra ```Continue``` butonuna tıklıyoruz ve devam ediyoruz…



![4](https://github.com/Lorento34/redbelly/assets/84406096/49b525d3-9558-4ba7-b6fa-c706290c3b26)


5- Bir sonra ki ekranda hazır ayarlar gelirse -ki bazen gelmiyor- hepsini ```Delete``` tıklayarak Silin. Hepsini sildikten sonra ```Add record``` yazan yere tıklayın…


![5](https://github.com/Lorento34/redbelly/assets/84406096/208dcaa7-1438-447e-9c1a-76038db184be)


6- Bu sayfada dikkat etmeniz gereken ve ayarlama yapmanız gereken 4 kısım var. Numara ile belirttim.
- 1- ```Type``` A seçeceksiniz
- 2- Domain adresinizi yazacaksınız. Https, www gibi şeyler yazmayın. Aşağıda ki gibi olsun.
- 3- Ip adresinizi yazacaksınız.
- 4- ```Proxy Status``` kapatacaksınız. Aşağıda ki gibi olacak.
  
Tüm bu ayarlamaları yaptıktan sonra ```Save``` butonuna tıklayın ve ardından ```Continue``` butonuna tıklayıp devam edin…

![6](https://github.com/Lorento34/redbelly/assets/84406096/84431f9a-8996-4a82-8b45-c196f34ee4c1)



Düğüm (Node) Kurulumu


1-Aşağıdaki komutu kullanarak paket listenizin güncel olduğundan emin olun

```sudo apt update```

2- Aşağıdaki komutu kullanarak certbot yardımcı programını sisteminize yükleyin 

```sudo apt install snapd```
```sudo snap install --classic certbot```
```sudo ln -s /snap/bin/certbot /usr/bin/certbot```

3- DNS/FQDN'nizi doğrulamak ve sertifikayı vermek için certbot tarafından kullanılacak olan 80 numaralı bağlantı noktasında hiçbir işlemin çalışmadığından emin olun

```apt install net-tools```
```netstat -an | grep 80```

4- Aşağıda ki komutu komple kopyalayın ve bir metin belgesine kaydedin. Ardından xxx@mail.com ve domainadresiniz.com’u kendi bilgilerinize göre değiştirin. Aşağıda ki bilgilere göre çalıştırmayın bu komutu kesinlikle! Bu komutu girdikten sonra domaininize sertifika almış olacaksınız.

👉 Önemli Not:   Aşağıda ki komutu kesinlikle kendi bilgilerinize göre değiştirin!!!
👉 Önemli Not 2: Komutları sunucuda tek tek değil komple olarak kopyalayıp çalıştıracaksınız!

```
email=xxx@mail.com
fqn=domainadresiniz.com
sudo certbot certonly --standalone -d $fqn. --non-interactive --agree-tos -m $email
sudo chown -R $USER:$USER /etc/letsencrypt/```


