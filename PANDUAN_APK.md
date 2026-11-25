# Membuat APK dengan PWABuilder (opsional)

Aplikasi ini sudah bisa dipasang langsung dari browser (lihat README.md). APK hanya perlu bila Anda ingin berkas .apk untuk dibagikan.

## Syarat
- Aplikasi sudah di-hosting dengan **HTTPS** (GitHub Pages atau Vercel). PWABuilder tidak bisa memakai berkas lokal.
- Paket ini (versi APK) sudah memuat ikon maskable dan screenshot yang diminta PWABuilder.

## Langkah
1. Unggah isi folder paket ini ke GitHub Pages/Vercel, lalu buka alamatnya untuk memastikan aplikasi berjalan.
2. Buka **pwabuilder.com**, tempel alamat aplikasi Anda, ketuk **Start**.
3. Tunggu skor selesai. Manifest dan service worker seharusnya terbaca (hijau). Bila ada peringatan, ketuk untuk detailnya.
4. Ketuk **Package for Stores → Android**. Isi:
   - **Package ID**: nama unik, contoh `id.web.namaanda.koreksiljk` (tidak bisa diubah setelah dipublikasikan).
   - **App name**: Koreksi Lembar Jawab. **Short name**: Koreksi LJK.
   - **Signing key**: pilih *New* lalu **simpan berkas keystore dan sandinya** di tempat aman. Tanpa itu Anda tidak bisa memperbarui aplikasi.
5. Unduh paket. Berkas `.apk` bisa dipasang langsung di HP Android (izinkan "pasang dari sumber tidak dikenal").

## Catatan
- Tanpa pengaturan *Digital Asset Links*, aplikasi tampil dengan bilah alamat di bagian atas. Petunjuk membuat `assetlinks.json` ada di dalam paket dari PWABuilder.
- Izin kamera akan diminta saat pertama kali memotret.
- Pembaruan aplikasi cukup dengan mengunggah ulang situs; APK memuat versi terbaru dari alamat Anda.
- Saya belum menguji pemasangan APK pada HP sungguhan. Coba di satu HP dulu sebelum dibagikan.
