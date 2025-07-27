
![image](https://github.com/user-attachments/assets/0d8ec782-edf6-4ce2-a75b-4ee08589afe7)

## 1. Server Güncelleme : 

```bash
sudo apt update -y && sudo apt upgrade -y
```
## 2. Paketleri İndirelim:

```bash
sudo apt install htop ca-certificates zlib1g-dev libncurses5-dev libgdbm-dev libnss3-dev tmux iptables curl nvme-cli git wget make jq libleveldb-dev build-essential pkg-config ncdu tar clang bsdmainutils lsb-release libssl-dev libreadline-dev libffi-dev jq gcc screen file nano btop unzip lz4 -y
```

## 3. Rust ; 

```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

- 1 Enter.

```bash
source $HOME/.cargo/env
```

## 4. Buildliyelim ; 

```bash
git clone https://github.com/octra-labs/ocs01-test.git
cd ocs01-test
cargo build --release
```

<img width="599" height="184" alt="image" src="https://github.com/user-attachments/assets/1e8cf79a-b9ab-4f5a-a34e-81cf383ef2a6" />


## 5. Kopyalama ; 
```bash
cp EI/exec_interface.json .
```

<img width="497" height="147" alt="image" src="https://github.com/user-attachments/assets/1dc46574-f2f7-4c2e-af99-aa5512ff42cc" />


## Cüzdanı İçeri Atalım ; 

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

## Çalıştıralım ; 

```bash
./target/release/ocs01-test
```

<img width="538" height="380" alt="image" src="https://github.com/user-attachments/assets/aa2bb395-6240-4e18-8a92-5191474fffce" />


```bash
1. greeting: Bir mesaj alma fonksiyonu.
2. contract info: Sözleşmenin tanımını (açıklamasını) alma fonksiyonu.
3. claim 1 token: Belirli bir adrese bir kez token (dijital para birimi) talep etme fonksiyonu.
4. check token balance: Token bakiyesini kontrol etme fonksiyonu.
5. dot product: İki vektörün noktasal çarpımını hesaplama fonksiyonu.
6. vector magnitude: Bir vektörün büyüklüğünü (uzunluğunu) hesaplama fonksiyonu.
7. power: Bir sayının üssünü hesaplama.
8. factorial: Faktöriyel hesaplama.
9. fibonacci number: Fibonacci serisinden bir sayı bulma.
10. greatest common divisor: İki sayının en büyük ortak bölenini bulma.
11. check if number is prime: Bir sayının asal olup olmadığını kontrol etme.
12. 2x2 matrix determinant: 2x2 matrisin determinantını hesaplama.
13. linear interpolation: Doğrusal enterpolasyon yapma.
14. modular exponentiation: Modüler üs alma işlemi.
0. exit: Programdan çıkma.
```

- 1 ve 3 Yaptım.

- 1 ; 

<img width="626" height="434" alt="Gw4_7lcWAAAZ34o" src="https://github.com/user-attachments/assets/b0710c41-7c92-4142-ac6e-721b0e4a45bb" />

- 2 ; 

<img width="551" height="508" alt="image" src="https://github.com/user-attachments/assets/2ebfbf1f-d364-4b86-b93d-74ada0a06f87" />


- Komuta bastıktan sonra Enter'e basmanız yeterli.
