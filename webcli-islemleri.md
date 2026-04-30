<img width="725" height="412" alt="image" src="https://github.com/user-attachments/assets/f6454b7b-0143-4ee9-b958-c80256cb262e" />



## Sunucu Güncelleme:

```bash
sudo apt update -y && sudo apt upgrade -y
```
## Paketleri İndirelim :

```bash
sudo apt install htop ca-certificates zlib1g-dev libncurses5-dev libgdbm-dev libnss3-dev tmux iptables curl nvme-cli git wget make jq libleveldb-dev build-essential pkg-config ncdu tar snap clang bsdmainutils lsb-release libssl-dev libreadline-dev libffi-dev jq gcc screen file unzip lz4 -y
```

## Screen Açalım:
```bash
screen -S ngrok
```
- Yep yeni bir temiz sayfa açıcak.

## Ngrok İndirelim

- Çoğunuz diğer projeler ile aşina olmuşsunuzdur ama bilmiyorsanız sitesine gidip kayıt olup - mail doğrulamasını yapmalısınız.
- Site: https://dashboard.ngrok.com

- Linux olan sayfaya gelin: 

<img width="1381" height="352" alt="image" src="https://github.com/user-attachments/assets/df7231fd-81fe-4861-82a2-71e5d2e9391d" />


- Snap İle İndiriyoruz:

```bash
snap install ngrok
```

<img width="572" height="45" alt="image" src="https://github.com/user-attachments/assets/708d14f8-c9c4-4dd0-a840-0a864ecd6aa7" />


- Böyle oldu ise inmiş demektir Biraz sürebilir.

<img width="1025" height="563" alt="image" src="https://github.com/user-attachments/assets/881d9d8f-a7fd-4835-90bc-6c17e3b34a1d" />

- Siteden Kendinizdeki komutu kopyalayıp sunucuda yapıştırıp girin.

<img width="829" height="79" alt="image" src="https://github.com/user-attachments/assets/f3754378-ffee-4f64-a371-012032a9036b" />

- Böyle oldu ise başarılı tertemiz.

```bash
ngrok http 8420
```

- Bu komutu girdikten sonra port yönlendirme aktif olacak ve bize bir site linki vericek. Buradan sanki sunucuda o porta girmişiz gibi işlem yapabileceğiz.

<img width="1012" height="419" alt="image" src="https://github.com/user-attachments/assets/a7efd0b5-aa7f-49e9-8ac3-c6034cc1e987" />

- Buradaki linki kopyalayıp yada termius kullanıyorsanız üstüne tıklayıp kendi tarayıcınızda girin. 

- CTRL'ye basılıp tutup sırasıyla A ve D yapıp screenden çıkın.

## Webcli indirelim

```bash
sudo apt install g++ libssl-dev make
```

```bash
git clone https://github.com/octra-labs/webcli.git
```

```bash
cd webcli
```
```bash
chmod +x setup.sh
./setup.sh
./octra_wallet
```
<img width="385" height="142" alt="image" src="https://github.com/user-attachments/assets/ca66220c-61ea-4559-8c77-93af61250227" />

## Web'e Girelim:

- Ngrok sayfasından gittiğiniz siteyi yenileyin - octra webcli sizi karşılayacak.

<img width="1302" height="841" alt="image" src="https://github.com/user-attachments/assets/f80e994e-3085-4b3d-a6e9-53ffe01aac2a" />

- İmport'a basın.

<img width="549" height="400" alt="image" src="https://github.com/user-attachments/assets/c81fa32a-4635-45a8-b6fb-44bb549554e0" />

- Cüzdan kelimeleri yada privatekeyinizi girin. 

<img width="673" height="518" alt="image" src="https://github.com/user-attachments/assets/4c3dac8c-1d62-4480-bdca-92150a8e31ca" />


- 6 Hane dijital pin oluşturun. Set pin'e basın.

<img width="1012" height="471" alt="image" src="https://github.com/user-attachments/assets/88c6768f-a1d7-43d2-89b3-8c958249deb6" />

Paneliniz açılacak.

<img width="1180" height="425" alt="image" src="https://github.com/user-attachments/assets/7a50eeb9-1f34-4ede-b9af-01493cfbd197" />

- Sağ üstten apps'e basın.
- Açılan sayfada bridgeye basın sizi yönlendirecek.

<img width="544" height="214" alt="image" src="https://github.com/user-attachments/assets/bb9d0a36-092e-4bac-be8c-c16325d4789e" />

- Metamask bağlıyoruz. 
- oct -> woct olan sayfada olacağız.

<img width="572" height="811" alt="image" src="https://github.com/user-attachments/assets/ae43fe97-b0d9-442c-9dad-7706ea6bc176" />

<img width="401" height="374" alt="image" src="https://github.com/user-attachments/assets/06bb9d75-a47f-472d-8fbe-4d8be2d28964" />

- Tam miktar max yapmayın hata verdi 434.050505 deydi düz 434 yaptım onay verdi.
- Onay veriyoruz.

<img width="590" height="696" alt="image" src="https://github.com/user-attachments/assets/6b36a2c4-e95a-4005-b033-bf982ae75976" />

- Claim butonuna basıp ETH ağında claimliyoruz.


<img width="385" height="784" alt="image" src="https://github.com/user-attachments/assets/294ca279-969d-48fa-aa71-ee078e08263a" />

- Claimed oldu ve cüzdana geçti.

<img width="460" height="233" alt="image" src="https://github.com/user-attachments/assets/7577cdf8-5436-45a4-b6a5-78fe1d137a97" />
