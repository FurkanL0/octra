![image](https://github.com/user-attachments/assets/0d8ec782-edf6-4ce2-a75b-4ee08589afe7)

## 1. Server Güncelleme : 

```bash
sudo apt update -y && sudo apt upgrade -y
```
## 2. Paketleri İndirelim:

```bash
sudo apt install htop ca-certificates zlib1g-dev libncurses5-dev libgdbm-dev libnss3-dev tmux iptables curl nvme-cli git wget make jq libleveldb-dev build-essential pkg-config ncdu tar clang bsdmainutils lsb-release libssl-dev libreadline-dev libffi-dev jq gcc screen file nano btop unzip lz4 -y
```

## Tek Komut Kurulum - https://github.com/zunxbt'a Aittir.

- Size direkt cüzdan bilgilerinizi vericek kaydedin.

```bash
curl -sSL https://raw.githubusercontent.com/zunxbt/octra-wallet-cli/refs/heads/main/start.sh -o start.sh && chmod +x start.sh && ./start.sh
```

## Normal Projenin Verdiğ Şekilde Kurulum ; 

```bash
wget https://github.com/octra-labs/wallet-gen/releases/download/v4/wallet-generator-linux-x64.tar.gz
```
```bash
tar -xzf wallet-generator-linux-x64.tar.gz
```

```bash
chmod +x wallet-generator
```
```bash
screen -S octra
```
```bash
./wallet-generator
```
<img src="https://github.com/user-attachments/assets/115f5773-e2f2-4b05-9ee2-21b0fadc571e" width="450px" alt="u">

## Panele Giriş : 
- Herhangi bir tarayıcından girebilirsiniz.
- sunucu ip adresiniz :8888
- Örnek : 1.1.1.1:8888

<img src="https://github.com/user-attachments/assets/3c337032-40db-4371-a41f-55b06848ff55" width="450px" alt="u">

#### Generate Wallet'a Basın : 

<img src="https://github.com/user-attachments/assets/490ec720-f4ed-43eb-8f32-f7f8c5f89161" width="450px" alt="u">

- Size Verdiği Bilgileri Tümüyle Kaydedin : 

<img src="https://github.com/user-attachments/assets/fe14c60d-8119-418a-a64b-5e7580ee8c71" width="450px" alt="u">

- Ayrıca Size Verdiği Dosya İsmi İlede bilgileri alabilirsiniz : 

```bash
cat dosyaismi.txt
```

<img src="https://github.com/user-attachments/assets/c3c0b274-c6bb-4d94-98b0-4040b9801016" width="450px" alt="u">

## Faucet : 

- Link : https://faucet.octra.network/
- Validatör değiliz kutuyu işaretlemeyin.

<img src="https://github.com/user-attachments/assets/555cb20c-800e-484c-9b68-a99ff9d0b9fe" width="450px" alt="u">

- 👇

<img src="https://github.com/user-attachments/assets/bf0cf164-5d87-4fa0-b78d-3a2158ed614f" width="450px" alt="u">

- Explorer Linkinden Doğrulama Yapın Confirmed Olsun : 

<img src="https://github.com/user-attachments/assets/83b41d6b-49ae-43b1-b7fb-3eb6be61fc67" width="450px" alt="u">

- İşiniz bitince başkaları port'tan birşeyler denemesin diye CTRL + C ile durdurabilirsiniz.


# Cüzdan TX İşlemleri ; 

## 4. Dosyaları Çekelim ; 


```bash
git clone https://github.com/octra-labs/octra_pre_client.git
cd octra_pre_client
```
```bash
python3 -m venv venv
source venv/bin/activate
```
```bash
pip install -r requirements.txt
cp wallet.json.example wallet.json
```

#### Dosya Düzenleme ;

```bash
nano wallet.json
```

![image](https://github.com/user-attachments/assets/8b31183c-1bb1-4038-bda5-1a4eb36f063d)


- Private Key B64 olacak. Cüzdan oluştururken kaydettiğimiz bilgilerde yazıyor.


```bash
{
  "priv": "cüzdanprivatekeyiniburayayaz",
  "addr": "octilebaslayancuzdanadresiniz",
  "rpc": "https://octra.network"
}
```

- CTRL X - CTRL Y - Enter Kayıt edecek.

## Başlatalım : 
```bash
./run.sh
```

## Gorevler : 

#### Encrypt ; 

- 4'ü seçiyoruz.

![image](https://github.com/user-attachments/assets/8920f291-664b-4e45-949b-7c37c7e11215)

- İstediğimiz miktarı encrypt ediyoruz. Encrypt olması için tx'in geçmesi gerekiyor 2-3 dk bekletebilir.

![image](https://github.com/user-attachments/assets/43151f30-2013-48b5-ab94-d6342f6ab7c5)

#### Private Transfer ; 

- 6'yı seçiyoruz.

![image](https://github.com/user-attachments/assets/615af0c0-2d44-40a0-97f2-0251f530b3fe)

- Göndereceğimiz kişinin adresini yazıyoruz - hata almaması için karşı tarafın normal OCT testnette bir tx göndermesi gerekiyor - boş hesaplara gitmiyor.

![image](https://github.com/user-attachments/assets/176021da-9ad5-40e1-aee6-01faa3e54d42)

#### Private Transfer'i Claimleme - Karşı Taraf - Yada Size Gelen Transfer ; 

- 7'yi seçiyoruz.

![image](https://github.com/user-attachments/assets/e9f18189-c2a4-4ed3-b741-af1e3994b546)

- İşlemin numarasını yazıp enterleyin , claimleyin.

![image](https://github.com/user-attachments/assets/cb3a3506-4d24-469f-aafb-78730589adab)

#### DeCrypt ; 

- 5 'i seçiyoruz.

![image](https://github.com/user-attachments/assets/339c7639-d1dd-413a-aec5-88d6da71843d)

- Decrypt edeceğimiz miktarı yazıp onaylıyoruz.

![image](https://github.com/user-attachments/assets/990181e1-6f92-4c02-ba3d-59734a164eb5)
