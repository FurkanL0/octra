
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

- Snap İle İndiriyoruz:

```bash
snap install ngrok
```

<img width="1025" height="563" alt="image" src="https://github.com/user-attachments/assets/881d9d8f-a7fd-4835-90bc-6c17e3b34a1d" />

- Kendinizdeki komutu kopyalayıp sunucuda yapıştırıp girin.


```bash
ngrok http 8420
```

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

