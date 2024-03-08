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


<h1>Domain Satın Alma:<h6>
Bunun için ben Godaddy platformunu kullandım. Kullanımı basit ve fiyat olarak uygun domainler var. 50-60 TL’ye domain alabilirsiniz. Ama siz istediğiniz platformu kullanabilirsiniz ya da önceden aldığınız bir domain varsa onu da kullanabilirsiniz. Ama ben size godaddy üzerinden dns yönlendirme işlemlerini anlatacağım. Eğer bu konuya yabancıysanız sizde domaini godaddy üzerinden satın alıp, kafanız karışmadan aşağıda ki rehbere göre işlemleri yapabilirsiniz. Domaini satın almadan önce mutlaka üyelik açın çünkü daha sonra bir sorun olduğunda müşteri temsilcisiyle daha rahat iletişim kurabilirsiniz. Domain satın alma kısmı zaten basit olduğu için onu anlatmıyorum. Ama domaini satın alırken sepete ekledikten sonra ödeme kısmında bir takım ekstra özellikler eklemek isteyip istemediğinizi soracak hepsini reddedin ve sadece domaini satın alın 1 yıllık. Satın almayı yaptığınızı varsayarak 2. adım olan dns yönlendirme işlemine geçiyoruz.

<h1>Dns Yönlendirme:<h6>

1- Bu işlem için <a href="https://dash.cloudflare.com/sign-up">Cloudflare</a>  sitesine gidin ve üyelik oluşturun. Mailinize gelen doğrulama linkine tıklayarak mail adresinizi doğrulayın.

![1](https://github.com/Lorento34/redbelly/assets/84406096/67acac57-f871-4846-835b-b802496fa812)

2-	Sizi şöyle bir ekran karşılıyacak. ```‘’Add a website or application’’``` yazan butona tıklayın.


![2](https://github.com/Lorento34/redbelly/assets/84406096/dad248d4-43ae-40f0-b1ae-2d0a844983fb)


















