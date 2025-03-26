# cPan - cPanel & WHM Account Cracker

## 🚀 Overview
**cPan** adalah alat yang dirancang untuk melakukan pencarian akun cPanel dan WHM secara otomatis. Dengan menggunakan multi-threading, alat ini dapat dengan cepat memeriksa berbagai domain/IP untuk menemukan kredensial yang valid.

> **⚠ Disclaimer:**
> Alat ini hanya untuk tujuan edukasi dan pengujian keamanan di lingkungan yang Anda miliki atau memiliki izin eksplisit untuk diuji. Penyalahgunaan alat ini dapat melanggar hukum. Gunakan dengan bijak!

## 🎯 Features
- 🔍 **Pendeteksian cPanel & WHM** di port 2083 dan 2087.
- 🔑 **Brute-force login** dengan daftar username dan password.
- ⚡ **Multi-threading** untuk eksekusi yang lebih cepat.
- 📄 **Menyimpan hasil** ke dalam folder `Results/`.

## 📥 Installation & Usage

### 1️⃣ Install Dependencies
Pastikan Python sudah terinstall di sistem Anda. Jika belum, unduh dan instal dari [python.org](https://www.python.org/downloads/).

Kemudian, instal dependensi yang diperlukan:
```bash
pip install -r requirements.txt
```

### 2️⃣ Menjalankan cPan
```bash
python cPanel.py
```

Setelah menjalankan skrip, Anda akan diminta untuk memasukkan:
- **DOMAIN/IP LIST:** File yang berisi daftar domain/IP target.
- **WORDLIST(KREDENSIAL):** File yang berisi daftar password yang akan dicoba.
- **THREAD:** Jumlah thread untuk mempercepat proses.

### 3️⃣ Contoh Penggunaan
```bash
DOMAIN/IP LIST: wordlist.txt
WORDLIST (KREDENSIAL): kredensial.txt
THREAD: 2
```

## 📂 Directory Structure
```
├── cpan.py  # Main script
├── lib/
│   ├── test.txt  # Default wordlist
├── Results/
│   ├── cPanel.txt  # Hasil pencarian cPanel
│   ├── WHM.txt  # Hasil pencarian WHM
│   ├── Cracked.txt  # Akun yang berhasil ditemukan
├── requirements.txt  # Library yang dibutuhkan
```

## 🛠 Dependencies
- `requests`
- `bs4` (BeautifulSoup)
- `colorama`
- `concurrent.futures`

## 📜 License
Proyek ini dirilis di bawah lisensi **MIT**. Silakan gunakan dengan tanggung jawab.

## 📬 Contact
Jika ada pertanyaan atau saran, silakan kunjungi repository:
[**GitHub Repository**](https://github.com/Finsiii/cpan)

🔥 **Happy Hacking** 🔥
