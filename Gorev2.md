![image](https://github.com/user-attachments/assets/0d8ec782-edf6-4ce2-a75b-4ee08589afe7)

## 1. Server Güncelleme : 

```bash
sudo apt update -y && sudo apt upgrade -y
```
## 2. Paketleri İndirelim:

```bash
sudo apt install htop ca-certificates zlib1g-dev libncurses5-dev libgdbm-dev libnss3-dev tmux iptables curl nvme-cli git wget make jq libleveldb-dev build-essential pkg-config ncdu tar clang bsdmainutils lsb-release libssl-dev libreadline-dev libffi-dev jq gcc screen file nano btop unzip lz4 -y
```

## 3. Python / Yarn / Git : 

```bash
sudo apt update && sudo apt install -y python3 python3-venv python3-pip git yarn && curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add - && echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list && sudo apt update && sudo apt install -y yarn
```

## Screen Nolur Nolmaz ;

```bash
screen -S octragorev2
```

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

![image](https://github.com/user-attachments/assets/d8331cf8-8587-4463-b171-3a79b3451bb6)


## Token Gönderme : 

![image](https://github.com/user-attachments/assets/662833be-3130-4ca6-b975-5a82f68752ec)

- 1 Yazıp Enterleyin.
- Göndereceğiniz adresi yazın.
- Bana Gönderebilirsiniz : oct4Nngm5EW6NFPViHcMo8FeDziyMnqWQUpgf6eBoxHe15w

![image](https://github.com/user-attachments/assets/7022ab5e-f035-4b61-9b40-b0087054f98a)

- Miktaryı ayarlayın ; 

![image](https://github.com/user-attachments/assets/23e3f3e0-059d-4c4f-a8bc-2a1e9a724fa3)

- Y yazıp enterleyin - Enter'a basıp ana panele geri dönebilirsiniz. 

![image](https://github.com/user-attachments/assets/e05bba4c-06f2-4383-b0b0-c967420f8e6d)


- Screenden çıkmak içni CTRL A ve D yapabilirsiniz.
