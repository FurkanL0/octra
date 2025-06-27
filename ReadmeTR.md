![image](https://github.com/user-attachments/assets/0d8ec782-edf6-4ce2-a75b-4ee08589afe7)

## 1. Server Update : 

```bash
sudo apt update -y && sudo apt upgrade -y
```
## 2. Install Packages:

```bash
sudo apt install htop ca-certificates zlib1g-dev libncurses5-dev libgdbm-dev libnss3-dev tmux iptables curl nvme-cli git wget make jq libleveldb-dev build-essential pkg-config ncdu tar clang bsdmainutils lsb-release libssl-dev libreadline-dev libffi-dev jq gcc screen file nano btop unzip lz4 -y
```

## 3. Dosyaları Çekelim ; 

```bash
wget https://github.com/octra-labs/wallet-gen/releases/download/v4/wallet-generator-linux-x64.tar.gz
```
```bash
tar -xzf wallet-generator-linux-x64.tar.gz
```
```bash
./wallet-generator
```
