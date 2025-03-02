![17321472629448090425316459222952](https://github.com/user-attachments/assets/800db8e1-b67b-4520-ab64-a6e8d173b89c)

# SQL_injection v2
## Fitur Utama
- **Pengujian SQL Injection**: Menguji apakah sebuah situs web rentan terhadap SQL Injection.
- **Pengujian HTTPS**: Memastikan situs web menggunakan HTTPS untuk enkripsi yang lebih aman.
- **Pemeriksaan Header Keamanan**: Memverifikasi apakah situs web memiliki header keamanan yang sesuai.
- **Deteksi Formulir Input**: Memeriksa apakah situs web memiliki formulir input yang bisa jadi rentan terhadap serangan.
- **Bot Pengujian Keamanan**: Bot yang dapat menjawab pertanyaan terkait pengujian keamanan dan memberikan petunjuk.

## Prasyarat
Pastikan kamu memiliki Python 3.x yang terinstal. kamu dapat memeriksanya dengan menjalankan:

```bash
python --version
```
## Instalasi pustaka 
menginstal beberapa pustaka eksternal.
```bash
pip install flask
pip install requests
pip install beautifulsoup4
apt install git
git clone https://github.com/Cyberheroess/SQL_injectionCh.git
cd SQL_injectionCh
python main.py
```
## jika memgalami error 
lakukan instalasi seperti berikut
```bash
pip install -r requirements.txt
git clone https://github.com/Cyberheroess/SQL_injectionCh.git
cd SQL_injectionCh
python main.py
```
## Mengakses dan Menguji API
Aplikasi ini menyediakan beberapa endpoint API yang dapat diuji. Berikut adalah cara untuk mengaksesnya menggunakan curl.

## Menguji Website
Untuk menguji keamanan sebuah website (HTTPS, header keamanan, dan form input), kirim permintaan POST ke endpoint /test_website:

```bash
curl -X POST http://127.0.0.1:5000/test_website -H "Content-Type: application/json" -d '{"url": "http://example.com"}'
```
### Menguji SQL Injection
Untuk menguji kerentanannya terhadap SQL Injection, kirim permintaan POST ke endpoint /test_sql_injection:

```bash
curl -X POST http://127.0.0.1:5000/test_sql_injection -H "Content-Type: application/json" -d '{"url": "http://(url web)"}'
```
### Berinteraksi dengan Bot
Bot dapat memberikan bantuan atau instruksi terkait pengujian keamanan. Kirim pesan ke endpoint /bot menggunakan permintaan POST:

```bash
curl -X POST http://127.0.0.1:5000/bot -H "Content-Type: application/json" -d '{"message": "halo"}'
```


