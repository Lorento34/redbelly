![1_kNm5E2XtpiKdacDmywA8-w](https://github.com/Lorento34/redbelly/assets/84406096/fdb0c843-b7ff-44e1-86be-a1dd0d3cc03f)


<details>
<summary>Redbelly Network Sosyal Medya Linkleri</summary>

|                  |
| ---------------- |
| [Discord](https://discord.gg/vbJ6w5E5)
| [Twitter](https://twitter.com/RedbellyNetwork)
| [Websitesi](https://www.redbelly.network/)
| [Medium](https://medium.com/@redbellyblockchain)
| [Telegram](https://t.me/redbellychat)
| [Telegram Türkçe Kanal](https://t.me/redbellyturkey)

</details>



------

# Donanım Gereksinimleri

<b> Redbelly Network düğümünü (Node) çalıştırmak için minumum donanım gereksinimleri </b>

| Donanım | Gereksinim |
| ------------- | ---------------- |
Cpu | 8-core Cpu
Mimari | x86-64 (x64, x86_64, AMD64, ve Intel 64)
Ram | 16 GB
İşletim Sistemi | Ubuntu 22.04.2 LTS ya da üst sürümler (x86-64)
Depolama | 400 GB
Ağ Bant Genişliği | 40 Mbps
TCP bağlantı noktaları | 8545, 8546, 1111 ve 1888 (Önerilen)



Arkadaşlar rehber biraz uzun olacak üstün körü anlatıp geçtiğimde biliyorum ki telegramda birçok kişi anlayamayacak ve nasıl olduğunu soracak ya da birçok kişi hata alacak. Bu karışıklığın önüne geçmek için ve aramıza yeni katılanları da düşünerek ayrıntılı ve resimli bir rehber hazırlıyorum. Rehberde ki adımları dikkatlice okuyup, takip ederseniz sorunsuz bir şekilde kurulumu tamamlayabilirsiniz. Bu arada aşağıda kullanacağımız siteleri Türkçe'ye çevirip eee burada böyle bir şey yok demeyin. İngilizce olarak kullanın böylece aşağıda ki resimlerle senkronize gidebilirsiniz. Ben bu rehbere göre yaptım ve çalışıyor. Kurulum 3 adımdan oluşacak. Domain satın alma, domain için dns yapılandırılması ve düğüm (node) kurulumu.

---

# Domain Satın Alma
Bunun için ben <a href="https://www.godaddy.com/en-ie"><b>```Godaddy```</b></a> platformunu kullandım. Kullanımı basit ve fiyat olarak uygun domainler var. 50-60 TL’ye domain alabilirsiniz. Ama siz istediğiniz platformu kullanabilirsiniz ya da önceden aldığınız bir domain varsa onu da kullanabilirsiniz. Ama ben size <a href="https://www.godaddy.com/en-ie"><b>```Godaddy```</b></a> üzerinden dns yönlendirme işlemlerini anlatacağım. Eğer bu konuya yabancıysanız sizde domaini <a href="https://www.godaddy.com/en-ie"><b>```Godaddy```</b></a> üzerinden satın alıp, kafanız karışmadan aşağıda ki rehbere göre işlemleri yapabilirsiniz. Domaini satın almadan önce mutlaka üyelik açın çünkü daha sonra bir sorun olduğunda müşteri temsilcisiyle daha rahat iletişim kurabilirsiniz. Domain satın alma kısmı zaten basit olduğu için onu anlatmıyorum. Ama domaini satın alırken sepete ekledikten sonra ödeme kısmında bir takım ekstra özellikler eklemek isteyip istemediğinizi soracak hepsini reddedin ve sadece domaini satın alın 1 yıllık. Satın almayı yaptığınızı varsayarak 2. adım olan dns yönlendirme işlemine geçiyoruz.

# Dns Yönlendirme

1- Bu işlem için <a href="https://dash.cloudflare.com/sign-up"><b>```Cloudflare```</b></a>  sitesine gidin ve üyelik oluşturun. Mailinize gelen doğrulama linkine tıklayarak mail adresinizi doğrulayın.

![1](https://github.com/Lorento34/redbelly/assets/84406096/67acac57-f871-4846-835b-b802496fa812)

2- Sizi şöyle bir ekran karşılıyacak. ```Add a website or application``` yazan butona tıklıyoruz...


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
- 2- ```Name (required)``` Domain adresinizi yazacaksınız. Https, www gibi şeyler yazmayın. Aşağıda ki gibi olsun.
- 3- ```IPv4 address (required)``` Ip adresinizi yazacaksınız.
- 4- ```Proxy Status``` kapalı olacak. Aşağıda ki gibi.
  
Tüm bu ayarlamaları yaptıktan sonra ```Save``` butonuna tıklayın ve ardından ```Continue``` butonuna tıklayınız...

![6](https://github.com/Lorento34/redbelly/assets/84406096/84431f9a-8996-4a82-8b45-c196f34ee4c1)

7-	Burada size Cloudflare nameservers (Ad sunucular) verecek. Bunları bir metin belgesine kaydedin. Bunlar birazdan lazım olacak! Dns yönlendirmesini yapmak için <a href="https://www.godaddy.com/en-ie"><b>```Godaddy```</b></a> sitesine gidin…


![7](https://github.com/Lorento34/redbelly/assets/84406096/bdae7a85-0b75-45ae-af5d-43c289796e53)



8-	Godaddy platformuna giriş yaptıktan sonra sağ üst köşede profilinize girin sonra ```My Products``` tıklayın.


![8](https://github.com/Lorento34/redbelly/assets/84406096/0cf68c5c-b205-412d-ab0c-4e26329ad1ba)

9-	Burada Dns'ye tıklayın ve bir sonra ki adımda Dns ayarlarını yapılandıracağız.


![9](https://github.com/Lorento34/redbelly/assets/84406096/96ddd156-cefa-4fa8-9a5b-1b77f90f1660)



10-	```Nameservers```tıklayın, ardından ```Change Nameservers``` tıklayın ve bir sonra ki adımda Cloudflare sitesinden kopyaladığınız nameservers kaydedeceğiz.


![10](https://github.com/Lorento34/redbelly/assets/84406096/6df7bcf2-3f7a-432a-af90-9832f6d00edf)


11- Burada ```I'll use my own nameservers``` seçeneğini işaretleyin. Ve aşağıda ki gibi Cloudflare’den kopyaladığınız nameservers’i değiştirin, ardından ```Save``` butonuna tıklayarak kaydedin.



![11](https://github.com/Lorento34/redbelly/assets/84406096/ebe040a0-6c24-4e12-be24-71f501ac3016)

12- Düğüm (Node) kurulumuna başlamadan önce domaninizin dns yönlendirilmesinin tamamlanması gerekiyor. Yoksa düğüm (Node) kurulumu sırasında domaine sertifika alma kısmında hata alacaksınız. <a href="https://dnschecker.org/"><b>```Dns Checker```</b></a>sitesine gidip, takip edebilirsiniz. Arama kısmına domaininizin adını yazın aşağıda ki resimde ki gibi dünya haritasında hepsinin yeşil bir şekilde onaylı olması gerekiyor. Yarısı onaylı, yarısı kırmızı çarpı işareti varsa beklemeniz gerekiyor. Bu bekleme süresi 15-20 dakika olabilir. Dns yönlendirilmesi tamamlandıktan sonra düğüm (Node) kurulumuna geçebilirsiniz.

![12](https://github.com/Lorento34/redbelly/assets/84406096/63175717-a9fe-49c9-ae59-aef3d090f2c6)


---


<h1>Düğüm (Node) Kurulumu</h1>


1- Paket listenizini güncelleyin.

```Ballerina
sudo apt update
```

2- Certbot yardımcı programını sunucuya yükleyin.

```BASIC
sudo apt install snapd
```
```Awk
sudo snap install --classic certbot
```
```AutoIt
sudo ln -s /snap/bin/certbot /usr/bin/certbot
```

3- DNS/FQDN'nizi doğrulamak ve sertifikayı vermek için certbot tarafından kullanılacak olan 80 numaralı bağlantı noktasında hiçbir işlemin çalışmadığından emin olun.

```AutoHotkey
apt install net-tools
```

```Asymptote
netstat -an | grep 80
```

4- Bu komut önemli çünkü domain adresinize sertifika alacaksınız ve kullanacağınız komut sonrası size bir çıktı verecek onu bir metin belgesine kaydedin çünkü ileride kullanacaksınız. Aşağıda ki komutu bir metin belgesine kaydedin. Ardından ```xxx@mail.com``` ve ```domainadresiniz.com```’u kendi bilgilerinize göre düzenleyin.

> [!CAUTION]
> - Aşağıda ki komutu kesinlikle kendi bilgilerinize göre düzenleyin :bangbang:
> - Komutu kendi bilginize göre düzenledikten sonra sunucuda tek tek değil, bir bütün olarak çalıştırın :bangbang:

```Swift
email=xxx@mail.com
fqn=domainadresiniz.com
sudo certbot certonly --standalone -d $fqn. --non-interactive --agree-tos -m $email
sudo chown -R $USER:$USER /etc/letsencrypt/
```

> [!CAUTION]
> - Aşağıda ki çıktı örnektir. Sarı ile işaretli komutları kendi bilgilerinize göre düzenliyeceksiniz :bangbang:
> - Mavi ile işaretli sertifika ```fullchain.pem``` ve key ```privkey.pem``` çıktılarını metin belgesine kaydedin ileride kullanacağız  :bangbang:


![Ekran görüntüsü 2024-03-09 223513](https://github.com/Lorento34/redbelly/assets/84406096/8848743d-3e85-49a3-a728-7bf159a05772)



5- Bağımlılıkları yükleme/yükseltme

```Assembly
sudo apt-get update
```
```AspectJ
sudo apt-get install -y cron curl unzip
```
```AsciiDoc
sudo DEBIAN_FRONTEND=noninteractive apt-get -y upgrade
```

6- Redbelly düğüm (Node) kurulumunu tamamlamadan önce belirli dosyaları sunucuya yüklemeniz gerekiyor.

-	[Rbbc](https://drive.google.com/file/d/1gg3uHXYV0CnZJns49N1WdRiC-4wec21P/view?usp=sharing) dosyasını indirin.

- [Genesis.json](https://drive.google.com/file/d/1GTBBKs0IZZcDiOc_TldAwCzVu8D9wt3L/view?usp=drive_link) dosyasını indirin.
  
Daha sonra bu indirdiğiniz iki dosyayı ```winscp``` ya da ```termius``` gibi uygulamalar kullanarak sunucunuzun ```/root``` dizinine atın. Yani bilmeyen arkadaşlar için şöyle anlatayım, ```winscp``` ya da ```termius``` ile sunucuya bağlandıktan sonra hiçbir klasöre ya da başka bir yere girmeden ilk giriş yaptığınız yere atacaksınız dosyaları.


![image](https://github.com/Lorento34/redbelly/assets/84406096/f2c67bc3-e2f5-4541-a62a-ae2b6dd37e54)




7- Güvenlik duvarı yapılandıracağız. Aşağıdaki UFW komutlarını kullanarak ```<b>80, 8545, 1888 ve 1111</b>``` numaralı bağlantı noktalarına izin vermemiz gerekiyor.

```Sieve
sudo ufw enable
sudo ufw allow 22
sudo ufw allow 80
sudo ufw allow 8545
sudo ufw allow 1888
sudo ufw allow 1111
```

8- Config dosyasını yapılandıracağız.

```Apex
nano config.yaml
```

9- Aşağıda ki komutu metin belgesine kaydedin. Ardından <b>```kendi bilgilerinize```</b> göre değişiklikler yapacaksınız.

> [!CAUTION]
> - Aşağıda ki komut örnektir. Kesinlikle kendi bilgilerinize göre düzenleyin :bangbang:
> - Domain adresiniz aşağıda ki gibi olacak. Yani başında www, http ya da sonunda nokta, / gibi semboller olmayacak :bangbang:
> - Metamask adresinizin private keyini vereceksiniz bundan dolayı kesinlikle bu işlem için yeni bir metamask hesabı açın ve onu kullanın :bangbang:
> - Değiştireceğiniz kısımlar şöyle;```ip: Domain adresiniz```, ```id: Size verilen Numara```, ```privateKeyHex: Metamask adresinizin private keyi```

Komutu düzenledikten sonra komutun hepsini bir bütün halinde sunucunuza yapıştırın.```ctrl + o``` , ardından ```enter``` çıkış yapmak için ```ctrl + x```

```Processing
ip: sakultaroll.app
id: 33
genesisContracts:
  bootstrapContractsRegistryAddress: 0xDAFEA492D9c6733ae3d56b7Ed1ADB60692c98Bc5
consensusPort: 1888
grpcPort: 1111
privateKeyHex: ef71578b448ee9b9a7c112e4567d9j654e94gge164109bf820034f467h1903Bjk
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


10- observe.sh dosyasını yapılandıracağız.

```Antlers
nano observe.sh
```

11- Hata almamak için dikkatli okumanızı rica ediyorum. Aşağıda ki komutu metin belgesine kaydedin. Kendi bilgilerinize göre değiştireceğiniz 2 kısım var. 
Bunlar; ```<PATH TO SSL CERTIFICATE>``` ve ```<PATH TO SSL CERTIFICATE KEY>```
Aşağıda ki komutta ```<PATH TO SSL CERTIFICATE>``` ve ```<PATH TO SSL CERTIFICATE KEY>``` bulacaksınız ve 4. adımda size kaydetmenizi söylediğim sertifika ve key çıktılarıyla değiştireceksiniz.

Size örnek olması açısından aşağıda ki ekran görüntüsünde olduğu gibi kendi bilgilerinize göre düzenleyeceksiniz. Ayrıca boşluklara dikkat edin, fazladan bir şey silmeyin.

![image](https://github.com/Lorento34/redbelly/assets/84406096/0058f98a-f0aa-4fd6-a20d-493717cfd8c3)


```Mask
#!/bin/sh
# filename: observe.sh
if [ ! -d rbn ]; then
  echo "rbn doesnt exist. Initialising redbelly"
  mkdir -p rbn
  mkdir -p consensus
  cp config.yaml ./consensus

  ./binaries/rbbc init --datadir=rbn --standalone
  rm -rf ./rbn/database/chaindata
  rm -rf ./rbn/database/nodes
  mkdir -p ./rbn/genesis
  cp genesis.json ./rbn/genesis
else
  echo "rbn already exists. continuing with existing setup"
  cp config.yaml ./consensus
fi


# Run EVM
rm -f log
./binaries/rbbc run --datadir=rbn --consensus.dir=consensus --tls --consensus.tls --tls.cert=<PATH TO SSL CERTIFICATE> --tls.key=<PATH TO SSL CERTIFICATE KEY> --http --http.addr=0.0.0.0 --http.corsdomain=* --http.vhosts=* --http.port=8545 --http.api eth,net,web3,rbn --ws --ws.addr=0.0.0.0 --ws.port=8546 --ws.origins="*" --ws.api eth,net,web3,rbn --threshold=200 --timeout=500 --logging.level info --mode production --consensus.type dbft --config.file config.yaml --bootstrap.tries=10 --bootstrap.wait=10 --recovery.tries=10 --recovery.wait=10
```


12- Start-rbn.sh dosyasını yapılandıracağız.

```Alloy
nano start-rbn.sh
```

13- Aşağıda ki komutta bir değişiklik yapmadan direkt sunucuda çalıştırın.

```Boo
#!/bin/sh
# filename: start-rbn.sh
mkdir -p binaries
mkdir -p consensus
chmod +x rbbc
cp rbbc binaries/rbbc
mkdir -p logs
nohup ./observe.sh > ./logs/rbbcLogs 2>&1 &
```

14- Kurlumun bu kadar. Şimdi sadece düğümü (Node) çalıştırmaya geldi sıra. Aşğıda ki komutları sırasıyla sunucuda çalıştırın. Komutlar herhangi bir çıktı vermeyecek. Eğer yukarıda anlatılan talimatları iyi okuyup, eksiksiz yaptıysanız sorunsuz çalışacaktır düğüm (Node)

```ActionScript
chmod +x observe.sh
```

```ATS
chmod +x start-rbn.sh
```

```ASL
./start-rbn.sh
```

# Yararlı Komutlar

1- Logları kontrol etmek için aşağıda ki komutu kullanın.

```APL
tail -f $HOME/logs/rbbcLogs
```

![Ekran görüntüsü 2024-03-08 233819](https://github.com/Lorento34/redbelly/assets/84406096/b4d55ac5-12bf-4180-87b1-c146a4a548d4)


2- Düğümün (Node) senkronize olup olmadığını kontol etmek için aşağıda ki komutu kullanın. Bu komutta ```kendi bilginize``` göre değiştireceğiniz kısım domain adresini yazan yer. Yani ```https://domainadresin.com``` yazan yere kendi domain adresinizi yazın.

```ANTLR
echo $(( 16#$(curl -s https://domainadresin.com:8545 -X POST -H "Content-Type: application/json" --data '{"method":"eth_getBlockByNumber","params":["latest",false],"id":1,"jsonrpc":"2.0"}' | jq -r .result.number | sed 's/0x//') ))
```

![Ekran görüntüsü 2024-03-08 233709](https://github.com/Lorento34/redbelly/assets/84406096/da591976-3334-497c-88cb-aaee10914cc9)

3- Düğüme (Node) reset atmak için aşağıda ki komutları kullanın.

- Aşağıda ki komut Rbbc'yi kapatmak için size bir rakam verecek.

```AMPL
pgrep rbbc
```

![image](https://github.com/Lorento34/redbelly/assets/84406096/0059fd7c-4f0c-4b75-9905-d37c5be99055)


- Size verilen rakam ile rbbc'yi kapatıyoruz. ```Örnek``` kullanım şöyle ```kill 2727``` olacak. Siz kendinize göre düzenleyeceksiniz.

```AL
kill ****
```

![image](https://github.com/Lorento34/redbelly/assets/84406096/af6adbd2-1982-4d22-9f49-c5aa737a1885)


- Düğümü (Node) tekrardan başlatıyoruz.

```AIDL
chmod +x observe.sh
```

```ABNF
chmod +x start-rbn.sh
```

```ABAP
./start-rbn.sh
```

- Son olarak logları kontrol edelim.
  
```4D
tail -f $HOME/logs/rbbcLogs
```

![image](https://github.com/Lorento34/redbelly/assets/84406096/cfc002a0-52cb-4fd5-86ed-871402bc438e)





