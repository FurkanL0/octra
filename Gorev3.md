
![image](https://github.com/user-attachments/assets/0d8ec782-edf6-4ce2-a75b-4ee08589afe7)

## 1. Temiz Olması Açısından Sıfır Kurulum : 

```bash
screene -r octragorev2
```

- CTRL C ile durdurun.

- Exit Komutu ile screen'i kapatın
```bash
exit
```

- Eski Dosyaları Uçuralım ; 

```bash
cd
```
```bash
rm -rf octra_pre_client
```

## Screen Nolur Nolmaz ;

```bash
screen -S octragorev3
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


## Cüzdan Bilgilerini

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
