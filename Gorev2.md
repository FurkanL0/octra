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

```bash
{
  "priv": "cüzdanprivatekeyiniburayayaz",
  "addr": "octilebaslayancuzdanadresiniz",
  "rpc": "https://octra.network"
}
```
