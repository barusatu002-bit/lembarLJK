# Koreksi Lembar Jawab

Aplikasi web (PWA) untuk mengoreksi lembar jawab pilihan ganda dari foto HP. Semua pemrosesan terjadi di HP; foto tidak dikirim ke mana pun.
Dibuat oleh Aras Hidayat, S.Pd · SMA Negeri 3 Paloh.

## Isi paket
`index.html` · `sw.js` · `manifest.webmanifest` · `icons/` · `lembar/` (PDF A4 dan F4) · `README.md`

## 1. Unggah ke GitHub Pages
1. Buat repositori baru di github.com (publik), misalnya `koreksi-ljk`.
2. Ketuk **Add file → Upload files**, lalu seret **seluruh isi** folder paket (bukan folder induknya) dan **Commit**.
3. Buka **Settings → Pages**, pilih **Deploy from a branch**, cabang `main`, folder `/ (root)`, lalu **Save**.
4. Tunggu 1–2 menit. Alamatnya: `https://NAMA-ANDA.github.io/koreksi-ljk/`.
Vercel juga bisa: impor repositori yang sama tanpa pengaturan tambahan.
Untuk memperbarui, unggah ulang berkas; aplikasi memuat ulang sendiri saat versi baru aktif (menunggu bila ada lembar yang belum disimpan).

## 2. Memasang di HP
- **Android (Chrome):** buka alamat aplikasi → menu ⋮ → **Pasang aplikasi** / **Tambahkan ke layar utama**.
- **iPhone (Safari):** buka alamat → ketuk **Bagikan** → **Tambah ke Layar Utama**. Gunakan Safari, bukan Chrome.
- **Laptop:** buka di Chrome/Edge; bisa dipasang lewat ikon di bilah alamat.
Setelah dibuka sekali, aplikasi tetap jalan tanpa internet.

## 3. Mencetak lembar jawab
1. Di aplikasi: **Pengaturan → Lembar Jawab → Unduh A4** atau **Unduh F4**.
2. Cetak **skala 100% (Actual size)**, jangan "Fit to page". Cetak hitam putih, tanpa tepi dihapus.
3. Satu kertas (landscape) dipotong 3 lembar di garis potong kecil. Tiap lembar memuat 50 soal A–E dan 4 kotak hitam di sudut. Lembar tanpa 4 kotak tidak dibaca. Ujian 40 soal memakai lembar yang sama; 10 soal terakhir diabaikan.
4. Siswa menghitamkan **satu** bulatan penuh per soal dengan pensil 2B dan menulis nama.

## 4. Cara pakai (tiga langkah)
1. **Pengaturan:** isi jenis ujian, mapel, kelas, jumlah soal; lalu isi **Kunci Jawaban** (ketuk, tempel teks, atau pindai lembar kunci).
2. **Pindai:** ketuk **Buka kamera** dan arahkan ke kertas utuh (3 lembar) atau satu lembar. Foto diambil otomatis saat stabil; tombol putih untuk manual. Bisa juga pilih foto dari galeri. Isi nama siswa, periksa soal bertanda **cek ulang** (kotak putus-putus kuning), lalu **Simpan hasil**.
3. **Hasil:** lihat peringkat, analisis soal, dan detail siswa; **Ekspor CSV** untuk Excel (pemisah titik koma). Di **Riwayat** ada cadangan data.

Tips foto: cahaya cukup dan merata, HP sejajar kertas, keempat kotak hitam tiap lembar terlihat, jangan ada bayangan tangan.
Data tersimpan di browser HP Anda. **Ekspor cadangan** secara berkala; menghapus data browser akan menghapus hasil.

## Keputusan dan batas yang perlu diketahui
- Soal yang ragu-ragu (isian tipis, bekas hapus) ditandai **cek ulang** dan tidak dihitung benar sampai Anda tentukan. Isian ganda ditandai kuning dan dihitung salah.
- Nama siswa yang sama tidak menimpa data; otomatis menjadi "Nama (2)".
- Diuji dengan foto sintetis dan simulasi cetak PDF (nol salah baca tanpa tanda). **Belum diuji** pada HP sungguhan, hasil cetak printer, dan tulisan tangan nyata.
- **Sebelum dipakai ujian sungguhan, uji 5–10 lembar asli** dari kelas Anda: bandingkan hasil aplikasi dengan koreksi manual, dengan berbagai pensil, cahaya, dan HP.
