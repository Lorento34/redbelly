![1_kNm5E2XtpiKdacDmywA8-w](https://github.com/Lorento34/redbelly/assets/84406096/fdb0c843-b7ff-44e1-86be-a1dd0d3cc03f)

| Redbelly Network Sosyal Medya Linkleri|
| ---------------- |
| [Discord](https://discord.gg/vbJ6w5E5)
| [Twitter](https://twitter.com/RedbellyNetwork)
| [Websitesi](https://www.redbelly.network/)
| [Medium](https://medium.com/@redbellyblockchain)
| [Telegram](https://t.me/redbellychat)
| [Telegram Tükçe Kanal](https://t.me/redbellyturkey)


# tree-sitter-ruby

[![CI][ci]](https://github.com/tree-sitter/tree-sitter-ruby/actions/workflows/ci.yml)
[![discord][discord]](https://discord.gg/vbJ6w5E5m)
[![matrix][matrix]](https://matrix.to/#/#tree-sitter-chat:matrix.org)
[![crates][crates]](https://crates.io/crates/tree-sitter-ruby)
[![npm][npm]](https://www.npmjs.com/package/tree-sitter-ruby)

Ruby grammar for [tree-sitter](https://github.com/tree-sitter/tree-sitter).

#### References

- [AST Format of the Whitequark parser](https://github.com/whitequark/parser/blob/master/doc/AST_FORMAT.md)

[ci]: https://img.shields.io/github/actions/workflow/status/tree-sitter/tree-sitter-ruby/ci.yml?logo=github&label=CI
[discord]: https://img.shields.io/discord/1063097320771698699?logo=discord&label=discord
[matrix]: https://img.shields.io/matrix/tree-sitter-chat%3Amatrix.org?logo=matrix&label=matrix
[npm]: https://img.shields.io/npm/v/tree-sitter-ruby?logo=npm
[crates]: https://img.shields.io/crates/v/tree-sitter-ruby?logo=rust

------

# Donanım Gereksinimleri

<b> Redbelly Network düğümünü (Node) çalıştırmak için minimum donanım gereksinimleri </b>

| Donanım | Gereksinim |
| ------------- | ---------------- |
Cpu | 8-core Cpu
Mimari | x86-64 (x64, x86_64, AMD64, ve Intel 64)
Ram | 16 GB
İşletim Sistemi | Ubuntu 22.04.2 LTS ya da üst sürümler (x86-64)
Depolama | 1 TB
Ağ Bant Genişliği | 40 Mbps
TCP bağlantı noktaları | 8545, 8546, 1111 ve 1888 (Önerilen)



Arkadaşlar rehber biraz uzun olacak üstün körü anlatıp geçtiğimde biliyorum ki telegramda birçok kişi anlayamayacak ve nasıl olduğunu soracak ya da birçok kişi hata alacak. Bu karışıklığın önüne geçmek için ve aramıza yeni katılanları da düşünerek ayrıntılı ve resimli bir rehber hazırlıyorum. Rehberde ki adımları dikkatlice okuyup, takip ederseniz sorunsuz bir şekilde kurulumu tamamlayabilirsiniz. Bu arada aşağıda kullanacağımız siteleri Türkçe'ye çevirip eee burada böyle bir şey yok demeyin. İngilizce olarak kullanın böylece aşağıda ki resimlerle senkronize gidebilirsiniz. Ben bu rehbere göre yaptım ve çalışıyor. Kurulum 3 adımdan oluşacak. Domain satın alma, domain için dns yapılandırılması ve düğüm (node) kurulumu.

[![CI][ci]](https://github.com/tree-sitter/tree-sitter-ruby/actions/workflows/ci.yml)
[![discord][discord]](https://discord.gg/w7nTvsVJhm)
[![matrix][matrix]](https://matrix.to/#/#tree-sitter-chat:matrix.org)
[![crates][crates]](https://crates.io/crates/tree-sitter-ruby)
[![npm][npm]](https://www.npmjs.com/package/tree-sitter-ruby)

---

# Domain Satın Alma
Bunun için ben <a href="https://www.godaddy.com/en-ie">__Godaddy__</a> platformunu kullandım. Kullanımı basit ve fiyat olarak uygun domainler var. 50-60 TL’ye domain alabilirsiniz. Ama siz istediğiniz platformu kullanabilirsiniz ya da önceden aldığınız bir domain varsa onu da kullanabilirsiniz. Ama ben size <a href="https://www.godaddy.com/en-ie"><b>Godaddy</b></a> üzerinden dns yönlendirme işlemlerini anlatacağım. Eğer bu konuya yabancıysanız sizde domaini <a href="https://www.godaddy.com/en-ie"><b>Godaddy</b></a> üzerinden satın alıp, kafanız karışmadan aşağıda ki rehbere göre işlemleri yapabilirsiniz. Domaini satın almadan önce mutlaka üyelik açın çünkü daha sonra bir sorun olduğunda müşteri temsilcisiyle daha rahat iletişim kurabilirsiniz. Domain satın alma kısmı zaten basit olduğu için onu anlatmıyorum. Ama domaini satın alırken sepete ekledikten sonra ödeme kısmında bir takım ekstra özellikler eklemek isteyip istemediğinizi soracak hepsini reddedin ve sadece domaini satın alın 1 yıllık. Satın almayı yaptığınızı varsayarak 2. adım olan dns yönlendirme işlemine geçiyoruz.

# Dns Yönlendirme

#### 1- Bu işlem için <a href="https://dash.cloudflare.com/sign-up">Cloudflare</a>  sitesine gidin ve üyelik oluşturun. Mailinize gelen doğrulama linkine tıklayarak mail adresinizi doğrulayın.

![1](https://github.com/Lorento34/redbelly/assets/84406096/67acac57-f871-4846-835b-b802496fa812)

#### 2- Sizi şöyle bir ekran karşılıyacak. ```Add a website or application``` yazan butona tıklıyoruz...


![2](https://github.com/Lorento34/redbelly/assets/84406096/dad248d4-43ae-40f0-b1ae-2d0a844983fb)


3- Bir sonra ki adımda şöyle bir ekran gelecek. ```Enter domain name``` yazan yere satın aldığınız domainin adını yazın. Domainin başında https, www gibi şeyler yazmayın. Aşağıda ki gibi olsun. Sonra ```Enter``` butonuna tıklıyoruz...



![3](https://github.com/Lorento34/redbelly/assets/84406096/449e4065-3656-46f4-9504-28dd66bb2fe0)


4- Bu kısımda planı seçeceğiz. Cloudflare’e bize ücretli ve ücretsiz planlar sunuyor. Biz en aşağıda ki ```Free``` seçeceğiz. Bu ücretsiz plan. Daha sonra ```Continue``` butonuna tıklıyoruz...



<p align="center">
  <img width="588" height="683" src="https://i.imgur.com/VAXfZMW.png">
</p>



5- Bir sonra ki ekranda hazır ayarlar gelirse -ki bazen gelmiyor- hepsini ```Delete``` tıklayarak siliyoruz. Hepsini sildikten sonra ```Add record``` yazan yere tıklıyoruz…


![5](https://github.com/Lorento34/redbelly/assets/84406096/208dcaa7-1438-447e-9c1a-76038db184be)


6- Bu sayfada dikkat etmeniz gereken ve ayarlama yapmanız gereken 4 kısım var. Sayılarla belirttim.
- 1- ```Type``` A seçeceksiniz.
- 2- Domain adresinizi yazacaksınız. Https, www gibi şeyler yazmayın. Aşağıda ki gibi olsun.
- 3- Ip adresinizi yazacaksınız.
- 4- ```Proxy Status``` kapatacaksınız. Aşağıda ki gibi olacak.
  
Tüm bu ayarlamaları yaptıktan sonra ```Save``` butonuna tıklayın ve ardından ```Continue``` butonuna tıklayınız...

![6](https://github.com/Lorento34/redbelly/assets/84406096/84431f9a-8996-4a82-8b45-c196f34ee4c1)

7-	Burada size Cloudflare nameservers (Ad sunucular) verecek. Bunları bir metin belgesine kaydedin. Bunlar birazdan lazım olacak! Dns yönlendirmesini yapmak için <a href="https://www.godaddy.com/en-ie">```Godaddy```</a> sitesine gidin…


![7](https://github.com/Lorento34/redbelly/assets/84406096/bdae7a85-0b75-45ae-af5d-43c289796e53)



8-	Godaddy platformuna giriş yaptıktan sonra sağ üst köşede profilinize girin sonra ```My Products``` tıklayın.


![8](https://github.com/Lorento34/redbelly/assets/84406096/0cf68c5c-b205-412d-ab0c-4e26329ad1ba)

9-	Burada Dns'ye tıklayın ve bir sonra ki adımda Dns ayarlarını yapılandıracağız.


![9](https://github.com/Lorento34/redbelly/assets/84406096/96ddd156-cefa-4fa8-9a5b-1b77f90f1660)



10-	```Nameservers```tıklayın, ardından ```Change Nameservers``` tıklayın ve bir sonra ki adımda Cloudflare sitesinden kopyaladığınız nameservers kaydedeceğiz.


![10](https://github.com/Lorento34/redbelly/assets/84406096/6df7bcf2-3f7a-432a-af90-9832f6d00edf)


11- Burada ```I'll use my own nameservers``` seçeneğini işaretleyin. Ve aşağıda ki gibi Cloudflare’den kopyaladığınız nameservers’i değiştirin, ardından ```Save``` butonuna tıklayarak kaydedin.



![11](https://github.com/Lorento34/redbelly/assets/84406096/ebe040a0-6c24-4e12-be24-71f501ac3016)

12- Düğüm (Node) kurulumuna başlamadan önce domaninizin dns yönlendirilmesinin tamamlanması gerekiyor. Yoksa düğüm (Node) kurulumu sırasında domaine sertifika alma kısmında hata alacaksınız. <a href="https://dnschecker.org/">Dns Checker</a>sitesine gidip, takip edebilirsiniz. Arama kısmına domaininizin adını yazın aşağıda ki resimde ki gibi dünya haritasında hepsinin yeşil bir şekilde onaylı olması gerekiyor. Yarısı onaylı, yarısı kırmızı çarpı işareti varsa beklemeniz gerekiyor. Bu bekleme süresi 15-20 dakika olabilir. Dns yönlendirilmesi tamamlandıktan sonra düğüm (Node) kurulumuna geçebilirsiniz.

![12](https://github.com/Lorento34/redbelly/assets/84406096/63175717-a9fe-49c9-ae59-aef3d090f2c6)


---


<h1>Düğüm (Node) Kurulumu</h1>


1- Paket listenizin güncelleyin.

```ruby
sudo apt update
```

2- Certbot yardımcı programını sunucuya yükleyin.

```ruby
sudo apt install snapd
```
```ruby
sudo snap install --classic certbot
```
```ruby
sudo ln -s /snap/bin/certbot /usr/bin/certbot
```

3- DNS/FQDN'nizi doğrulamak ve sertifikayı vermek için certbot tarafından kullanılacak olan 80 numaralı bağlantı noktasında hiçbir işlemin çalışmadığından emin olun.

```ruby
apt install net-tools
```

```ruby
netstat -an | grep 80
```

4- Aşağıda ki komutu bir metin belgesine kaydedin. Ardından ```xxx@mail.com``` ve ```domainadresiniz.com```’u kendi bilgilerinize göre değiştirin. Aşağıda ki bilgilere göre çalıştırmayın bu komutu kesinlikle! Bu komutu girdikten sonra domaininize sertifika almış olacaksınız.

> [!CAUTION]
> - Aşağıda ki komutu kesinlikle kendi bilgilerinize göre değiştirin :bangbang:
> - Komutları sunucuda tek tek değil komple olarak kopyalayıp çalıştıracaksınız :bangbang:

```ruby
email=xxx@mail.com
fqn=domainadresiniz.com
sudo certbot certonly --standalone -d $fqn. --non-interactive --agree-tos -m $email
sudo chown -R $USER:$USER /etc/letsencrypt/
```

5- Bağımlılıkları yükleme/yükseltme

```ruby
sudo apt-get update
```
```ruby
sudo apt-get install -y cron curl unzip
```
```ruby
sudo DEBIAN_FRONTEND=noninteractive apt-get -y upgrade
```

6- Redbelly düğüm (Node) kurulumunu tamamlamadan önce belirli dosyaları sunucuya yüklemeniz gerekiyor.

-	[Rbbc](https://drive.google.com/file/d/1gg3uHXYV0CnZJns49N1WdRiC-4wec21P/view?usp=sharing) dosyasını indirin.

- [Genesis.json](https://drive.google.com/file/d/1GTBBKs0IZZcDiOc_TldAwCzVu8D9wt3L/view?usp=drive_link) dosyasını indirin.
  
Daha sonra bu indirdiğiniz iki dosyayı winscp ya da termius gibi uygulamalar kullanarak sunucunuzun kök dizinine atın. Kök dizinden kastım sunucuya bağlandıktan sonra hiçbir klasöre ya da başka bir yere girmeden ilk giriş yaptığınız yere atacaksınız.

7- Güvenlik duvarı yapılandıracağız. Aşağıdaki UFW komutlarını kullanarak ```<b>80, 8545, 1888 ve 1111</b>``` numaralı bağlantı noktalarına izin vermemiz gerekiyor.

```ruby
sudo ufw enable
sudo ufw allow 22
sudo ufw allow 80
sudo ufw allow 8545
sudo ufw allow 1888
sudo ufw allow 1111
```

8- Config dosyasını yapılandıracağız.

```YAML
nano config.yaml
```

9- Aşağıda ki komutu metin belgesine kaydedin. Ardından <b>```kendi bilgilerinize```</b> göre değişiklikler yapacaksınız.

> [!CAUTION]
> - Aşağıda ki komut örnektir. Kesinlikle kendi bilgilerinize göre düzenleyin :bangbang:
> - Domain adresiniz aşağıda ki gibi olacak. Yani başında www, http ya da sonunda nokta, / gibi semboller olmayacak :bangbang:
> - Metamask adresinizin private keyini vereceğiniz için kesinlikle bu işlem için yeni bir metamask hesabı açın ve onu kullanın :bangbang:
> - Değiştireceğiniz kısımlar şöyle;```ip: Domain adresiniz```, ```id: Size verilen Numara```, ```privateKeyHex: Metamask adresinizin private keyi```

Komutu düzenledikten sonra komutun hepsin sunucunuza yapıştırın. ```Ctrl + o``` , enter ve ```ctrl + x``` yaparak çıkış yapın. 

```YAML
ip: lorento.app
id: 33
genesisContracts:
  bootstrapContractsRegistryAddress: 0xDAFEA492D9c6733ae3d56b7Ed1ADB60692c98Bc5
consensusPort: 1888
grpcPort: 1111
privateKeyHex: ef71578b448ee9b9a7c112e4567d9j654e94gge164109bf820034f467h1903bjk
poolConfig:
  initCap: 5
  maxCap: 30
  idleTimeout: 180
clientKeepAliveConfig:
  keepAliveTime: 1
  keepAliveTimeOut: 20
serverKeepAliveConfig:
  serverKeepAliveTime: 70
  serverKeepAliveTimeOut: 10
  minTime: 60
rpcPoolConfig:
  maxOpenCount: 1
  maxIdleCount: 1
  maxIdleTime: 30
```






# Yararlı Komutlar

1- Logları kontrol etmek için aşağıda ki komutu kullanın.
```ruby
tail -f $HOME/logs/rbbcLogs
```

![Ekran görüntüsü 2024-03-08 233819](https://github.com/Lorento34/redbelly/assets/84406096/b4d55ac5-12bf-4180-87b1-c146a4a548d4)


2- Düğümün (Node) senkronize olup olmadığını kontol için aşağıda ki komutu kullanın. Burada ki domain https://domainadresin.com:8545 bilgisine kendi domain adresinizi yazın.

```ruby
echo $(( 16#$(curl -s https://domainadresin.com:8545 -X POST -H "Content-Type: application/json" --data '{"method":"eth_getBlockByNumber","params":["latest",false],"id":1,"jsonrpc":"2.0"}' | jq -r .result.number | sed 's/0x//') ))
```

![Ekran görüntüsü 2024-03-08 233709](https://github.com/Lorento34/redbelly/assets/84406096/da591976-3334-497c-88cb-aaee10914cc9)

3- Düğüme (Node) reset atmak için aşağıda ki komutları kullanın.

- Rbbc'i kapatmak için aşağıda ki komutla sayısını öğreniyoruz.

```ruby
pgrep rbbc
```

![image](https://github.com/Lorento34/redbelly/assets/84406096/0059fd7c-4f0c-4b75-9905-d37c5be99055)


- Size veren sayı ile rbbc'yi kapatıyoruz. __Örnek__ kullanım şöyle ```kill 2727``` olacak. Siz kendinize göre düzenleyeceksiniz.

```ruby
kill ****
```

![image](https://github.com/Lorento34/redbelly/assets/84406096/af6adbd2-1982-4d22-9f49-c5aa737a1885)


- Düğümü (Node) tekrardan başlatıyoruz.

```ruby
./start-rbn.sh
```
![image](https://github.com/Lorento34/redbelly/assets/84406096/d95fda32-b887-49c9-98d8-a6f0708f3ba3)

- Son olarak logları kontrol edelim.
  
```ruby
tail -f $HOME/logs/rbbcLogs
```

![image](https://github.com/Lorento34/redbelly/assets/84406096/cfc002a0-52cb-4fd5-86ed-871402bc438e)





