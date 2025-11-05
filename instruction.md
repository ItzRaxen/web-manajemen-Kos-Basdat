Buatkan sebuah Prototipe Visual (Mockup) Aplikasi Web Manajemen Kos yang statis, modern, dan responsif.

Tujuan:
Aplikasi ini berfungsi sebagai demo visual (mockup) untuk sistem manajemen internal "Kos Gacor". Tujuannya adalah untuk menunjukkan tampilan (UI/UX) aplikasi kepada 2 tipe pengguna: Pemilik dan Penghuni.

PENTING: Aplikasi ini statis (tidak fungsional). Tidak ada backend (PHP) dan tidak ada koneksi database. Semua data di-hardcode (dummy data).

Spesifikasi Teknis:

Teknologi: Murni HTML, Tailwind CSS, dan JavaScript (hanya untuk interaksi UI seperti menu mobile atau modal).

Database: Tidak ada. Semua data (nama pengguna, riwayat pembayaran, contoh chat) ditulis langsung di dalam tag HTML sebagai data dummy.

Frontend: Gunakan Tailwind CSS (muat melalui CDN di header setiap file).

Font: Gunakan Google Font 'Inter'.

Autentikasi: Simulasi Login. Tidak ada validasi.

Struktur File (Multi-Halaman HTML):

login.html (Halaman formulir login palsu).

index-penghuni.html (Dashboard Penghuni).

index-pemilik.html (Dashboard Pemilik).

pembayaran.html (Riwayat pembayaran - statis).

laporan-penghuni.html (Formulir & riwayat laporan - statis).

laporan-pemilik.html (Tabel laporan untuk pemilik - statis).

pesan-penghuni.html (Tampilan chat - statis).

pesan-pemilik.html (Tampilan chat - statis).

pengumuman.html (Daftar pengumuman - statis).

kelola-kamar-pemilik.html (Tabel kamar - statis).

script.js (Untuk interaktivitas frontend seperti hamburger menu).

Struktur Fungsional per Halaman (Mockup):

1. Komponen Berulang (Navbar & Footer):

Setiap file .html (kecuali login.html) harus memiliki Navbar dan Footer yang identik (copy-paste).

Navbar: Harus sticky dengan nama "Kos Gacor".

Tautan di Navbar harus mengarah ke file .html yang sesuai (misal: "Dashboard" -> index-penghuni.html, "Laporan" -> laporan-penghuni.html).

Harus ada tombol "Logout" yang mengarah kembali ke login.html.

2. login.html:

Formulir login (email, password).

Wajib: Sediakan dua tombol:

Tombol "Login sebagai Penghuni" (Saat diklik, arahkan ke index-penghuni.html).

Tombol "Login sebagai Pemilik" (Saat diklik, arahkan ke index-pemilik.html).

Tidak perlu ada validasi JavaScript.

3. index-penghuni.html (Dashboard Penghuni):

Tampilkan "Selamat datang, [Nama Penghuni Dummy, misal: Andi Pratama]".

Tampilkan info kamar (hardcode): "Kamar A1 - Tipe Deluxe".

Tampilkan status pembayaran terakhir (hardcode): "Pembayaran Bulan Ini: LUNAS".

Tampilkan shortcut (tombol) yang mengarah ke laporan-penghuni.html dan pengumuman.html.

4. index-pemilik.html (Dashboard Pemilik):

Tampilkan "Selamat datang, [Nama Pemilik Dummy, misal: Budi Santoso]".

Tampilkan ringkasan statis (hardcode):

Kartu "Okupansi": 8 / 10 Kamar Terisi.

Kartu "Laporan Baru": 2 Laporan Belum Diproses.

Kartu "Pesan Baru": 3 Pesan Belum Dibaca.

5. laporan-penghuni.html (Laporan Kerusakan - Penghuni):

Tampilkan formulir statis untuk membuat laporan baru (Judul Laporan, Deskripsi). Tombol "Kirim" tidak perlu berfungsi.

Di bawah formulir, tampilkan tabel dummy (hardcode) riwayat laporan:

"AC Bocor" | Status: "Sedang Dikerjakan"

"Lampu Mati" | Status: "Selesai"

6. laporan-pemilik.html (Laporan Kerusakan - Pemilik):

Tampilkan tabel dummy (hardcode) dari semua laporan:

"Andi (A1) - AC Bocor" | Status: "Sedang Dikerjakan"

"Siti (B2) - Kran Air Rusak" | Status: "Belum Dikerjakan"

Tampilkan tombol palsu "Ubah Status" di samping setiap item (tidak perlu fungsional).

7. pesan-penghuni.html (Chat - Penghuni):

Buat layout aplikasi chat.

Di sidebar kiri, tampilkan kontak (hardcode): "Pemilik Kos (Budi Santoso)".

Di area chat utama, tampilkan percakapan dummy (hardcode):

(Anda) "Pak, AC saya bocor."

(Pemilik) "Baik, akan segera dicek teknisi."

Di bagian bawah, tampilkan kotak input pesan dan tombol "Kirim" (tidak fungsional).

8. pembayaran.html (Riwayat Pembayaran - Penghuni):

Tampilkan tabel dummy (hardcode) riwayat pembayaran:

"Mei 2025" | Rp 1.500.000 | Status: "Lunas"

"April 2025" | Rp 1.500.000 | Status: "Lunas"

"Maret 2025" | Rp 1.500.000 | Status: "Lunas"

9. pengumuman.html (Pengumuman):

Tampilkan daftar pengumuman dummy (hardcode) dalam bentuk kartu, diurutkan dari yang terbaru.

Contoh: "Perbaikan WiFi (10 Mei 2025)", "Kerja Bakti Bulanan (5 Mei 2025)".

Jika ini halaman untuk pemilik (pengumuman-pemilik.html), tambahkan tombol palsu "Buat Pengumuman Baru".
