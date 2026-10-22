# LAPORAN ETS PEMROGRAMAN WEB - PERPUSTAKAAN UNIVERSITAS (LibraryReg)

5025251095 - Alessandro Almaz Filemon

<img width="8943" height="3353" alt="Group 4" src="https://github.com/user-attachments/assets/c20d3b00-f40a-4182-a03c-b10abb812b31" />

**Link Website:**
https://libraryreg-5025251095.netlify.app/

# 1. Deskripsi dan Ruang Lingkup Pekerjaan
1.1 Deskripsi Sistem

Sebuah perpustakaan perguruan tinggi saat ini masih menghadapi kendala akibat proses pendaftaran anggota secara manual menggunakan formulir kertas. Hal ini berdampak pada tingginya antrean pendaftaran, risiko kesalahan pencatatan data, kesulitan pencarian informasi anggota, serta lambatnya proses pembuatan kartu anggota.

Untuk mengatasinya, dikembangkan aplikasi berbasis web bernama LibraryReg. Pada tahap pengembangan ini, fokus utama ada pada pengembangan front-end. Pengelolaan data anggota disimpan secara sementara menggunakan JavaScript dan fitur localStorage pada browser tanpa bergantung pada backend atau database server terlebih dahulu.

1.2 Ruang Lingkup Pekerjaan

Pengerjaan proyek ini mencakup ruang lingkup sebagai berikut:
- Landing Page (Home): Page utama informasi dan navigasi perpustakaan. Disertakan pilihan login sebagai Calon Anggota dan Admin.
- Page Tentang: Page berisikan informasi umum tentang perpustakaan.
- Page Layanan: Page berisikan informasi layanan yang diberikaan oleh perpustakaan.
- Page Formulir Pendaftaran Online: Page berisi form input data pendaftaran anggota baru perpus dengan validasi data.
- Pengelolaan Data Anggota: Bagian frontend bagi petugas/administrator dalam mengelola, mencari, dan melihat detail anggota. (Calon Anggota tidak bisa mengedit detail anggota lain).
- Page Penyimpanan Data Lokal: Pengintegrasian localStorage untuk mempertahankan data anggota setelah reload halaman.
- Implementasi & Publikasi: Penulisan kode frontend serta penerapan publikasi web deployment dengan menggunakan netlify.


# 2. Rancangan Halaman dan Struktur Menu

2.1 Struktur Menu dan Navigasi

Aplikasi LibraryReg menggunakan struktur navigasi yang terbagi menjadi dua tergantung perannya:

Navigasi Calon Anggota:
        - Beranda / Landing Page
        - Header (Logo & Nama Perpustakaan)
        - Hero Section
        - Layanan
        - Keunggulan & Fasilitas
        - Statistik
        - Footer (Kontak & Jam Layanan)
        - Formulir Pendaftaran

Navigasi Petugas Perpustakaan:
        - Pengelolaan Data Anggota

2.2 Arsitektur Rancangan Halaman

2.2.1 Landing Page (Home)
Tujuan: memberikan informasi awal dan mengarahkan pengunjung ke layanan perpustakaan.
- Header dengan logo dan nama perpustakaan.
- Hero section dengan judul, deskripsi, dan tombol ajakan.
- Informasi layanan perpustakaan secara singkat.
- Keunggulan dan fasilitas perpustakaan secara singkat.
- Statistik ilustratif jumlah koleksi dan anggota.
- Footer berisi kontak dan informasi jam layanan.
- Login sebagai Calon Anggota atau Admin (Tambahan)

2.2.2 Page Tentang
- Header dengan logo dan nama perpustakaan.
- Hero section dengan judul, deskripsi, dan tombol ajakan.
- Informasi sejarah perpustakaan secara rinci.
- Statistik ilustratif jumlah koleksi dan anggota secara rinci.
- Footer berisi kontak dan informasi jam layanan.

2.2.3 Page Layanan
- Header dengan logo dan nama perpustakaan.
- Hero section dengan judul, deskripsi, dan tombol ajakan.
- Informasi layanan perpustakaan secara rinci.
- Keunggulan dan fasilitas perpustakaan secara rinci.
- Footer berisi kontak dan informasi jam layanan.

2.2.4 Pengelolaan Menu Navigasi
Tujuan: memudahkan pengguna berpindah antarbagian aplikasi.
- Beranda
- Tentang Perpustakaan
- Layanan
- Daftar Anggota
- Pendaftaran Anggota
- Login Administrator

2.2.5 Formulir Pendaftaran Online
Tujuan: menggantikan formulir kertas dengan formulir digital.
- Jenis Keanggotaan: Mahasiswa, Dosen, atau Tenaga kependidikan (Terkhusus Dosen dan Tenaga Pendidik tidak bisa mengisi Fakultas, Departemen, dan Program Studi)
- Nama Lengkap
- NRP/NIDN (Dosen)/NITK (Tenaga Kependidikan)
- Fakultas
- Departemen
- Program Studi
- Alamat Tinggal
- Nomor telepon
- Email
Formulir memiliki validasi kolom wajib, format email, dan keunikan nomor induk. Setelah berhasil, data ditambahkan ke daftar anggota pada sisi front end.

2.2.4 Halaman Pengelolaan Anggota
Tujuan: membantu Admin mengelola data anggota melalui antarmuka web.
- Menampilkan tabel daftar anggota.
- Mencari anggota berdasarkan nama atau NRP/NIDN/NITK.
- Melihat detail anggota.
- Mengedit data anggota.
- Menghapus data dengan dialog konfirmasi.
- Menampilkan notifikasi keberhasilan atau kesalahan.
- Menyimpan data pada localStorage agar tetap tersedia setelah halaman dimuat ulang di browser yang sama.

# 3. Desain UI Landing Page

3.1 Tata Letak & Komponen Visual
Desain antarmuka Landing Page dirancang secara responsif dan intuitif dengan komponen berikut:

<img width="9983" height="6699" alt="DESAIN HOME PAGE" src="https://github.com/user-attachments/assets/ded01107-9432-4884-b5ec-3f3cefc21742" />

# 4. Implementasi dan Publis Web yang dibuat

4.1 Implementasi Kode

4.1.1 Cuplikan Kode HTML (index/Home)
<img width="785" height="497" alt="image" src="https://github.com/user-attachments/assets/6b82c0cb-f624-4676-b9cf-c951b35caea9" />

4.1.2 Cuplikan Kode CSS
<img width="658" height="611" alt="image" src="https://github.com/user-attachments/assets/c59d06b1-8fda-4798-8cb7-cad5bf18740e" />

4.1.3 Cuplikan Kode JavaScript (kelola)
<img width="685" height="622" alt="image" src="https://github.com/user-attachments/assets/deaaeec0-d064-4223-ad52-6575ca09e8d6" />

4.2 Publish Web

4.2.1 Publish Web pada netlify
https://libraryreg-5025251095.netlify.app/
