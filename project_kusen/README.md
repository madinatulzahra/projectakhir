# 🪵 Rizz Furniture

Rizz Furniture adalah website company profile dan katalog produk digital yang dibangun menggunakan PHP native, MySQL, dan Bootstrap 5. Website ini dirancang untuk membantu usaha furniture dan interior lokal memiliki kehadiran digital yang profesional, modern, dan mudah dikelola.

---

## Tentang Website

Website ini terdiri dari dua bagian utama — halaman publik untuk pengunjung, dan panel admin untuk pengelolaan konten.

Di sisi pengunjung, halaman beranda menampilkan hero section dengan layout split antara teks dan gambar, dilengkapi floating card yang menampilkan statistik bisnis seperti jumlah project selesai dan tahun pengalaman. Di bawahnya terdapat strip statistik, kemudian section produk unggulan yang menggunakan layout featured — satu produk besar di kiri dan grid produk di bawahnya. Setiap kartu produk memiliki badge label seperti "Terlaris" atau "Baru", dan saat kursor diarahkan ke gambar produk akan muncul overlay dengan tombol pesan yang langsung terhubung ke WhatsApp dengan teks otomatis berisi nama dan harga produk.

Website ini juga memiliki section timeline proses kerja yang menampilkan alur dari konsultasi, desain, produksi, hingga pemasangan dalam format visual yang mudah dipahami. Ada pula section testimoni dari pelanggan yang sudah menggunakan layanan, lengkap dengan nama, lokasi, dan status terverifikasi.

Halaman Tentang menampilkan profil perusahaan dengan layout asimetris — gambar yang keluar dari batas container di sisi kiri, dan konten teks beserta statistik pencapaian di sisi kanan. Di halaman ini juga terdapat section keunggulan dan visi misi perusahaan.

Halaman Produk menampilkan seluruh katalog produk dalam grid tiga kolom, masing-masing dengan gambar, nama, harga, deskripsi singkat, dan tombol pesan via WhatsApp.

Halaman Kontak menyediakan informasi lengkap berupa alamat, nomor WhatsApp, dan jam operasional, disertai peta Google Maps yang langsung menunjukkan lokasi UIN Siber Syekh Nurjati Cirebon. Di semua halaman terdapat floating WhatsApp button yang selalu terlihat, serta tombol kembali ke atas yang muncul saat pengguna scroll ke bawah.

---

## Panel Admin

Panel admin dapat diakses melalui halaman login yang dilindungi dengan autentikasi session. Setelah masuk, admin akan melihat dashboard yang menampilkan tiga kartu statistik — total produk, rating toko, dan status katalog — masing-masing dilengkapi grafik sparkline kecil.

Admin dapat mengelola seluruh produk melalui halaman Data Produk yang menggunakan DataTables dengan fitur pencarian dan pagination otomatis. Untuk menambah produk baru, tersedia form lengkap dengan preview gambar sebelum diunggah, validasi format file (JPG, PNG, WEBP), dan batas ukuran maksimal 5MB. Admin juga bisa mengedit produk yang sudah ada — termasuk mengganti gambar, di mana gambar lama akan otomatis terhapus. Untuk menghapus produk, sistem menampilkan konfirmasi menggunakan SweetAlert2 agar tidak terjadi penghapusan yang tidak disengaja.

Sidebar navigasi admin dapat diakses di semua ukuran layar termasuk mobile, dengan highlight otomatis pada halaman yang sedang aktif.

---

## Keamanan

Sistem ini menerapkan beberapa lapisan keamanan dasar: prepared statement untuk mencegah SQL injection di semua query yang melibatkan input pengguna, pengecekan session di setiap halaman admin, whitelist halaman di index.php untuk mencegah path traversal, dan htmlspecialchars di semua output data untuk mencegah XSS.

---

## Teknologi

PHP · MySQL · Bootstrap 5 · Font Awesome · AOS.js · SweetAlert2 · DataTables · Plus Jakarta Sans · XAMPP

---

## Instalasi

1. Clone repositori dan pindahkan ke folder `htdocs` XAMPP
2. Jalankan Apache dan MySQL di XAMPP Control Panel
3. Buka phpMyAdmin, buat database `db_kusen`, lalu import file `database/db_kusen.sql`
4. Buka `http://localhost/project_kusen/` di browser
5. Akses admin di `http://localhost/project_kusen/admin/auth/login.php` dengan username `admin` dan password `admin123`

---

Dibuat dengan ❤️ oleh [Nama Anda]
