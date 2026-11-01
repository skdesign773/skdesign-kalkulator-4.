SKDESIGN Kalkulator - PWA siap diunggah

PERBAIKAN:
- manifest.json dilengkapi identitas, scope, start_url, warna, dan ikon 192/512 px.
- sw.js melakukan precache file aplikasi, cache aset, fallback offline, dan pembersihan cache versi lama.
- Ditambahkan ikon aplikasi serta metadata Android/iOS pada index.html.

CARA MEMASANG DI HP ANDROID:
1. Ekstrak ZIP ini.
2. Unggah SELURUH isi folder (index.html, manifest.json, sw.js, dan folder icons) ke hosting HTTPS.
   Contoh: GitHub Pages, Netlify, atau hosting web milik sendiri.
3. Buka alamat website tersebut di Google Chrome pada HP.
4. Tunggu halaman selesai dimuat, lalu pilih menu ⋮ > Instal aplikasi / Tambahkan ke layar utama.
5. Buka aplikasi minimal sekali saat online agar file aplikasi tersimpan di cache. Setelah itu halaman utama dapat dibuka offline.

CATATAN PENTING:
- PWA dan Service Worker tidak dapat dipasang normal jika index.html dibuka langsung dari file manager (file://).
- Hosting harus menggunakan HTTPS (localhost hanya untuk pengujian).
- Semua produk dan riwayat tetap disimpan di localStorage browser/perangkat yang digunakan.
- Jika ikon atau versi lama masih muncul, tutup aplikasi lalu muat ulang website. Cache versi lama akan dibersihkan oleh service worker baru.
