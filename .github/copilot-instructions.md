<!--
Petunjuk singkat dan praktis untuk agen AI yang mengerjakan repositori ini.
File ini dihasilkan/diubah oleh asisten otomatis. Jaga ringkas (20–50 baris).
-->
# Instruksi Copilot — Halaman-Error

Tujuan
- Repositori ini berisi kumpulan halaman error statis berbahasa Indonesia yang berdiri sendiri: `400.html`, `401.html`, `403.html`, `404.html`, `500.html`.

Gambaran umum
- Setiap file adalah halaman HTML statis lengkap dengan CSS inline dan sedikit JavaScript inline. File ini dimaksudkan untuk dilayani sebagai aset statis (tidak ada sistem build).

Perubahan yang wajar dan alasan
- Lakukan perubahan kecil dan fokus: pembaruan teks (Bahasa Indonesia), penyesuaian warna/spasi, perbaikan aksesibilitas, atau perbaikan JS kecil (placeholder pencarian, animasi).
- Hindari menambahkan framework, bundler, atau dependensi berat — proyek ini sengaja minimal.

Konvensi & pola (contoh spesifik)
- Bahasa: Semua konten harus tetap berbahasa Indonesia. Contoh: judul di `404.html` adalah "Halaman Tidak Ditemukan".
- Struktur: Halaman memakai kelas umum yang konsisten: `.container`, `.error-code`, `.buttons`, `.floating-elements`. Gunakan kembali kelas ini saat menyesuaikan tampilan.
- CSS: Ditulis inline pada setiap file di dalam tag `<style>` — preferensi: ubah lokal per halaman daripada memindahkan ke stylesheet global, kecuali Anda juga memperbarui semua halaman dan menambahkan README migrasi.
- JS: Skrip kecil inline untuk efek UI (lihat `404.html` untuk efek ketik dan logika tombol pencarian). Jaga perubahan JS tetap kecil dan terisolasi.

Alur kerja pengembang
- Tidak ada langkah build: buka file HTML di browser (double-click) atau gunakan ekstensi Live Server di editor untuk preview.
- Git: gunakan alur commit/PR biasa. Deskripsikan perubahan copy/branding di deskripsi PR.

Titik integrasi
- File ini adalah aset statis untuk webserver atau pipeline deploy. Jika mengubah nama file atau path, pastikan konfigurasi server/deploy yang menggunakan file ini diperbarui.
- Jika berencana menambahkan stylesheet bersama atau bundler, sertakan rencana migrasi (update semua halaman, README, dan catat perubahan path).

Yang tidak boleh dilakukan
- Jangan ubah repositori menjadi proyek framework (React/Vue/Angular) atau tambahkan dependensi besar.
- Jangan ubah bahasa ke Inggris atau mencampur bahasa antar halaman.

Contoh cepat untuk agen
- Mengubah teks: edit elemen `<h1>` atau `<p>` pada file yang relevan, pertahankan kelas CSS yang ada.
- Menyesuaikan warna: ubah gradient pada selector `body` dan sesuaikan warna `.error-code` untuk kontras.
- Memperbaiki pencarian di `404.html`: cari komentar `// Efek pencarian` dalam skrip; pastikan placeholder dan validasi minimal tetap berbahasa Indonesia.

File penting
- `400.html`, `401.html`, `403.html`, `404.html`, `500.html` — contoh struktur, pola CSS, dan snippet JS kecil.

Jika butuh lebih
- Untuk perubahan besar (shared stylesheet, build step, atau testing), buka issue dengan rencana migrasi dan catatan file yang akan diubah.

Selesai