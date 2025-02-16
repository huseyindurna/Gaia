# Gaia
![gaia-xp](https://github.com/user-attachments/assets/778179af-821a-43b0-a218-4c336094b80f)
## Gerekli Donanım
CPU: 4 çekirdekli işlemci

RAM: 8 GB bellek

Depolama: 10 GB boş alan

## Altdaki Linkden Kayıt Olalım
* https://gaianet.ai/reward?invite_code=RmB158

## Kurulum

Paketleri Güncelle
```shell
sudo apt update && sudo apt upgrade -y
```
Python Yükle
```shell
sudo apt install -y python3-pip
sudo apt install pip
sudo apt install -y build-essential libssl-dev libffi-dev python3-dev
```

Gaia Node Kur
```shell
curl -sSfL 'https://github.com/GaiaNet-AI/gaianet-node/releases/latest/download/install.sh' | bash
```
```shell
source /root/.bashrc
```

```shell
gaianet init --config https://raw.githubusercontent.com/GaiaNet-AI/node-configs/main/qwen2-0.5b-instruct/config.json
```
Düğümü Başlatalım
```shell
gaianet start
```
Node ID ve Device ID bilgilerini veriyor bunları siteye giriyoruz
```shell
gaianet info
```
https://www.gaianet.ai/setting/nodes sayfasından

![image](https://github.com/user-attachments/assets/9a13aa64-cf12-408a-8fe2-66d489c3fe54)
![image](https://github.com/user-attachments/assets/35315860-b7d3-48f1-9476-b38970877fb5)

Domain’e Katılıcaz

```shell
gaianet stop
gaianet config --domain gaia.domains
gaianet init
gaianet start
```

![image](https://github.com/user-attachments/assets/4db12949-5b49-45b1-bf17-2c16b0137335)

Join Domain seçeneğini seçin. Sonraki adımları takip edin.
pengu.gaia.domain adlı domain’i arayın ve katılın.

Sohbet Botunu Çalıştırma 
API Anahtarı Oluşturun ve Bunu saklayın :
https://www.gaianet.ai/setting/gaia-api-keys 

Aşağıdaki komutu sunucunda çalıştır
```shell
curl -L -o gaiabot.py https://raw.githubusercontent.com/huseyindurna/Gaia/refs/heads/main/gaiabot.py
```

Sunucuda bir screen açarak botu arka planda çalıştır
Kullanmadığımız zamanlarda da çalışması için oto text bot kuracağız.


```shell
screen -S gaia
```
```shell
python3 gaiabot.py
```

requests Hatası Alanlar 
```shell
pip install requests
```
```shell
python3 gaiabot.py
```
Gaia API anahtarınızı gir. 

Screen’den çıkmak için Ctrl + A + D tuşlarına basın.

Buradan Base ağında reeddem yapın EXP'lerinizi
https://www.gaianet.ai/reward-summary 
![image](https://github.com/user-attachments/assets/387620ef-88e9-414b-9e2f-d5252cc0abf8)

#Puanlar her 24 saat bir sürede güncellenecektir.

## Gerekli Olabilecek Bazı Komutlar
 Screen Girmek için
 
```shell
screen -r gaia
```

Durdurmak için CTRL+C 

Screen'i Silmek için

```shell
screen -X -S screen-ismi quit
```


