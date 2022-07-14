# Sui-Devnet
Ağustos ayında Sui ödüllü node testneti başlayacak. Şuan Devnete katılanlar discorda IP veriyor belki bir eleme yaparlar o yüzden devnete katılacağım.

Not:Çok ufak bir güncelleme geldi. Eğer daha önce devnete katılıp Http ile başlayan IP adresinizi discorda verdiyeseniz tekrar yapmanıza gerek yok. IP discorda gönderdikten sonra Sui kurduğunuz sunucuyu silebilirsiniz boş yere para vermeyin.

Not:@Ruesandora0 'dan forkladım

![sui devnet](https://user-images.githubusercontent.com/98783018/178501237-0a49f928-6f4b-4038-82ba-04cb0c50f579.png)

Sistem Gereksinimleri

**CPUs: 2**

**RAM: 8GB**

**Depolama: 50GB**

Sudo Kurulumu
```
sudo apt install
```

_Bir Screen Oluşturalım_

```
screen -S sui
```

Full nodeumuzu yükleyelim **(15-20dk sürebilir**)
```
wget -O sui.sh https://raw.githubusercontent.com/kj89/testnet_manuals/main/sui/sui.sh && chmod +x sui.sh && ./sui.sh
```

Kurulum Sonrası Alacağınız çıktı Resimdeki Gibi Olmalı (Güncelleme sonrası adım)

<img width="815" alt="kurulum sonrasi" src="https://user-images.githubusercontent.com/98783018/178959488-eb452991-502f-416b-a40d-e478be4c5625.png">

Bu Çıktıdaki hhtp ile başlayan ve 9000 ile biten yere kadar kopyalayıp discorda atıyoruz gerisi hep aynı

Daha Sonra [Discorda](https://discord.gg/DznV3tVp) Gidiyoruz Ve Resimdeki Kanala Resimdeki Gibi IP Adresimizi Bırakıyoruz

Discord Link:https://discord.gg/DznV3tVp

![aplication](https://user-images.githubusercontent.com/98783018/178503597-36defc84-15d9-4d09-bffa-f2d62fc5be1d.png)

**Not: #pick-a-role role kanalından da kanalından istediğiniz rolü alın**

![role seç](https://user-images.githubusercontent.com/98783018/178504268-1cfb9938-b757-4e05-b9f7-381e97407f2f.png)

Node Durumunu Kontrol etmek için

https://node.sui.zvalid.com/

Log Kontrol

```
journalctl -u suid -f -o cat
```
Node silmek için:
```
sudo systemctl stop suid
sudo systemctl disable suid
sudo rm -rf ~/sui /var/sui/
sudo rm /etc/systemd/system/suid.service
```

Node durumunu kontrol:

```
service suid status
```
Node Reset

```
sudo systemctl restart suid
```

Node durdurma

```
sudo systemctl stop suid
```

**Sosyal Medya Hesaplarımız**

https://linktr.ee/lossnode

[Youtube](https://www.youtube.com/c/Cryptoloss1)

