![image](https://github.com/user-attachments/assets/0d8ec782-edf6-4ce2-a75b-4ee08589afe7)

## CodeSpace ; 


#### 1 - Github üzerinde Repo Oluşturun ; 

<img width="582" height="290" alt="image" src="https://github.com/user-attachments/assets/941e87f4-95b8-4c11-8e5d-41838bf53c6a" />


#### 2- Private Olsun - Readme.md Tik'i açık olsun ; 

<img src="https://github.com/user-attachments/assets/b0938a6d-3243-4bff-9e8c-7ddecca50f8c" width="450px" alt="u">


#### 3- CodeSpace ; 

- Link : https://github.com/codespaces

<img width="337" height="289" alt="image" src="https://github.com/user-attachments/assets/4acc9502-d644-4c75-8b32-49685e12c5dd" />

#### 4 - Açtığınız Repo'yu Seçin - Diğerleri Aynı Kalabilir ; 

<img width="813" height="536" alt="image" src="https://github.com/user-attachments/assets/1924ece8-8999-494f-a844-ce0fdb20bf18" />

- Artık Paneldesiniz ; 
<img src="https://github.com/user-attachments/assets/4a61a1c9-21e4-4981-be85-22af2ae9d906" width="450px" alt="u">


## 1. Server Güncelleme : 

```bash
sudo apt update -y && sudo apt upgrade -y
```
## 2. Paketleri İndirelim:

```bash
sudo apt install htop ca-certificates zlib1g-dev libncurses5-dev libgdbm-dev libnss3-dev tmux iptables curl nvme-cli git wget make jq libleveldb-dev build-essential pkg-config ncdu tar clang bsdmainutils lsb-release libssl-dev libreadline-dev libffi-dev jq gcc screen file nano btop unzip lz4 -y
```

## Tek Komut Cüzdan Kurulum - https://github.com/zunxbt'a Aittir. CodeSpace Kuranlar İçin ; 

- Size direkt cüzdan bilgilerinizi vericek kaydedin.

```bash
curl -sSL https://raw.githubusercontent.com/zunxbt/octra-wallet-cli/refs/heads/main/start.sh -o start.sh && chmod +x start.sh && ./start.sh
```

<img width="1305" height="221" alt="image" src="https://github.com/user-attachments/assets/f2595888-3042-4496-b72a-390ee5b0fe7e" />

- Enter.

<img width="661" height="261" alt="image" src="https://github.com/user-attachments/assets/7f24318a-bbc5-4f59-a907-ed22286ee8a1" />

- Cüzdan Bilgerini tümüyle kayıt edin.

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

## Dosyaları Çekelim ; 


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

- 1 Yazıp Enterleyin.
- Göndereceğiniz adresi yazın.
- Bana Gönderebilirsiniz : oct4Nngm5EW6NFPViHcMo8FeDziyMnqWQUpgf6eBoxHe15w

<img width="242" height="236" alt="image" src="https://github.com/user-attachments/assets/8ea0e5ff-f8a4-4db4-8cea-8af5638e114d" />


- Miktaryı ayarlayın ; 

<img src="https://github.com/user-attachments/assets/23e3f3e0-059d-4c4f-a8bc-2a1e9a724fa3" width="450px" alt="u">

- Y yazıp enterleyin - Enter'a basıp ana panele geri dönebilirsiniz. 

<img src="https://github.com/user-attachments/assets/e05bba4c-06f2-4383-b0b0-c967420f8e6d" width="450px" alt="u">

- Screenden çıkmak içni CTRL A ve D yapabilirsiniz.
 

#### Encrypt ; 

- 4'ü seçiyoruz.

<img src="https://github.com/user-attachments/assets/8920f291-664b-4e45-949b-7c37c7e11215" width="450px" alt="u">

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
