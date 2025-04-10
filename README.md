# 🗺️ SHORTEST PATH WITH DJIKSTRA ALGORITHM Kampus UNIB

Proyek ini menampilkan rute terpendek antar lokasi di lingkungan Kampus Universitas Bengkulu menggunakan **algoritma Dijkstra** dan data **OpenRouteService (ORS)**. Visualisasi dilakukan dengan peta interaktif menggunakan `folium`.

---

## 📌 Fitur

- ✅ Menentukan rute terpendek menggunakan **algoritma Dijkstra**
- ✅ Menggunakan **jarak nyata** via OpenRouteService API
- ✅ Menampilkan peta interaktif dengan **marker lokasi & jalur rute**
- ✅ Menampilkan **rute alternatif** dari ORS
- ✅ Estimasi **jarak dan waktu tempuh** tiap rute

---

## 🧰 Teknologi

- Python 3.x
- [OpenRouteService](https://openrouteservice.org/)
- `openrouteservice` (client API)
- `folium` (peta interaktif)
- `heapq` (priority queue untuk Dijkstra)

---

## 🗺️ Lokasi yang Didukung

Beberapa titik penting dalam graf:
- Rektorat
- Perpustakaan
- Danau UNIB
- LPTIK
- GSG
- Gedung B1, B2, B3 & B4
- Stadion UNIB
- Gedung FKIP
- GLT
- Dekanat Teknik
- LAB Teknik
- LAB Terpadu Teknik

> 📌 Lokasi dan koneksi dapat diperluas sesuai kebutuhan dengan menambahkan ke dictionary `locations` dan `graph`.

---

## ⚙️ Cara Kerja

1. **Lokasi Kampus** ditentukan dalam koordinat longitude & latitude.
2. **Graf koneksi** antar lokasi dibuat manual berdasarkan realita jalan.
3. **Jarak antar lokasi** dihitung secara dinamis menggunakan ORS.
4. **Algoritma Dijkstra** digunakan untuk mencari rute terpendek.
5. **Peta ditampilkan** dengan marker lokasi dan jalur rute.
6. **Perbandingan** rute alternatif ditampilkan menggunakan ORS.

---

## 🚀 Cara Menjalankan

1. **Clone Repository (jika dari GitHub)**  
   ```bash
   git clone https://github.com/username/nama-repo.git
   cd nama-repo

   Install Library yang Dibutuhkan
Pastikan Python 3.x sudah terinstal. Jalankan perintah berikut untuk menginstal dependensi:

      pip install openrouteservice folium
Dapatkan API Key dari OpenRouteService

      Kunjungi: https://openrouteservice.org/sign-up/

Daftar akun (gratis)

Setelah login, masuk ke dashboard dan salin API Key milikmu

Masukkan API Key ke dalam kode
Buka file Python utama, lalu temukan dan ubah bagian berikut:

      python
      import openrouteservice

# Ganti 'API_KEY_ANDA' dengan API key kamu sendiri
      client = openrouteservice.Client(key='API_KEY_ANDA')
Jalankan Program
Jalankan file Python menggunakan terminal, Jupyter Notebook, atau Google Colab.

