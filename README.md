# TikTokShop & Shopee Style E-Commerce (100% Frontend)

Website E-Commerce ringan berbasis Single Page Application murni menggunakan **HTML**, **Tailwind CSS (via CDN)**, dan **Vanilla JavaScript**. Seluruh data disimpan secara lokal menggunakan **LocalStorage** sehingga sangat mudah dijalankan tanpa database server.

---

## 🚀 Cara Install & Menjalankan di Lokal / Acode (HP)
1. Buat folder baru di perangkat Anda (atau di aplikasi **Acode** di HP Android).
2. Simpan 3 file utama di dalam folder tersebut:
   - `index.html`
   - `admin.html`
   - `README.md`
3. Buka file `index.html` menggunakan browser langsung (Double click atau buka via Live Server di VS Code / buka file langsung di Chrome Android / Acode preview).

---

## 🌐 Cara Deploy ke GitHub Pages (Gratis)
1. Buat repository baru di [GitHub](https://github.com/).
2. Upload / Push ketiga file (`index.html`, `admin.html`, `README.md`) ke branch utama (`main` atau `master`).
3. Masuk ke menu **Settings** repository Anda di GitHub.
4. Pilih menu **Pages** di sidebar kiri.
5. Pada bagian **Build and deployment**, pilih Source: **Deploy from a branch**, lalu pilih branch `main` dan folder `/ (root)`. Klik **Save**.
6. Dalam beberapa detik, GitHub akan memberikan link live website Anda!

---

## 🔑 Akses Halaman Admin
- Buka `index.html`, lalu klik tombol **"Masuk Admin"** di pojok kanan atas (atau langsung akses `admin.html`).
- **Default Login Admin:**
  - **Username:** `admin`
  - **Password:** `admin123`

---

## ⚙️ Cara Kerja & Aturan LocalStorage
Website ini menggunakan 5 key utama di LocalStorage untuk mengelola seluruh ekosistem toko:
1. `db_produk`: Menyimpan daftar produk (Nama, Harga, Stok, Kategori, Gambar) yang dikelola melalui menu Admin Input/View.
2. `db_cart`: Menyimpan produk yang sedang dimasukkan customer ke dalam keranjang belanja.
3. `db_transaksi`: Menyimpan riwayat transaksi saat customer melakukan checkout. Stok produk otomatis berkurang dan total checkout masuk ke saldo toko.
4. `db_saldo`: Menyimpan akumulasi omset/saldo toko bersih yang bisa ditarik melalui menu Penarikan Saldo Admin.
5. `db_penarikan`: Menyimpan riwayat pengajuan penarikan dana dengan status awal "Menunggu".
# toko.html