# Destinopedia - Panduan Rancangan dan Pemasangan

## 1. Struktur situs
```
Cover (nama web | kolom search | tombol Wish list/bookmark)
 └─ Menu 7 benua: Asia, Afrika, Amerika Utara, Amerika Selatan, Antartika, Eropa, Australia
     └─ Daftar negara
         ├─ Fakta singkat (ibu kota, mata uang, bahasa)
         ├─ Bulan terbaik berkunjung
         ├─ Destinasi wisata (bisa disimpan ke wish list)
         ├─ Makanan tradisional
         ├─ Minuman tradisional
         └─ Tips dan pengetahuan lain
```

## 2. Isi folder
| File | Fungsi |
|---|---|
| index.html | Halaman cover dan kerangka |
| style.css | Tampilan (mendukung HP dan mode gelap) |
| data.js | Seluruh data benua, negara, destinasi, kuliner. Ini file yang Anda perbanyak |
| app.js | Menu benua, pencarian, wish list (disimpan di browser) |

## 3. Pasang di GitHub Pages
1. Buat akun di github.com, lalu klik **New repository** dan beri nama `destinopedia` (Public).
2. Klik **uploading an existing file**, unggah keempat file (bukan file zip-nya), lalu **Commit changes**.
3. Buka **Settings > Pages**. Pada *Source* pilih **Deploy from a branch**, branch `main`, folder `/ (root)`, klik **Save**.
4. Tunggu 1-2 menit. Alamat situs: `https://NAMA-USER.github.io/destinopedia/`

## 4. Tampilkan di Google Sites
1. Buka sites.google.com dan buat situs baru, beri judul **Destinopedia**.
2. Di panel kanan pilih **Sematkan (Embed) > Dengan URL**, tempel alamat GitHub Pages di atas.
3. Ubah ukuran kotak sematan sampai memenuhi lebar dan tinggi halaman. Jadikan itu halaman Beranda.
4. (Opsional) Buat satu halaman per benua di Google Sites dengan menyematkan `.../destinopedia/#asia`, `#afrika`, `#eropa`, dan seterusnya.
5. Klik **Publikasikan**.

Catatan: wish list tersimpan di browser tiap pengunjung. Jika tombol Simpan tidak bekerja di dalam sematan Google Sites, buka alamat GitHub Pages langsung (beberapa browser memblokir penyimpanan pada konten tersemat).

## 5. Menambah negara
Buka `data.js` di GitHub (ikon pensil), salin satu blok negara di dalam benuanya, isi datanya, lalu Commit. Situs ikut diperbarui otomatis.
Data bawaan hanya contoh (200 entri yang mencakup hampir seluruh negara dan wilayah di semua benua, termasuk yang punya peringatan perjalanan). Isi sisa negara secara bertahap, dan periksa ulang bulan terbaik serta aturan visa dari sumber resmi.
