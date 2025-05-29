# Aplikasi Pomodoro Timer dengan Pelacakan Sesi (Firebase)

Aplikasi web sederhana ini membantu Anda menerapkan Teknik Pomodoro untuk meningkatkan fokus dan produktivitas. Aplikasi ini dilengkapi dengan fitur login menggunakan email/password, pelacakan riwayat sesi, dan notifikasi suara di akhir setiap sesi.

## Apa itu Teknik Pomodoro?

Teknik Pomodoro adalah metode manajemen waktu yang dikembangkan oleh Francesco Cirillo pada akhir tahun 1980-an. Teknik ini menggunakan timer untuk memecah pekerjaan menjadi interval-interval, biasanya berdurasi 25 menit, yang dipisahkan oleh istirahat pendek. Setiap interval kerja ini dikenal sebagai "pomodoro", dari kata Italia untuk "tomat", setelah Cirillo menggunakan timer dapur berbentuk tomat saat masih menjadi mahasiswa.

**Prinsip Dasar Teknik Pomodoro:**

1.  **Pilih Tugas:** Tentukan tugas yang ingin Anda kerjakan.
2.  **Atur Timer Pomodoro:** Atur timer ke durasi standar, biasanya 25 menit.
3.  **Kerjakan Tugas:** Fokus penuh pada tugas tersebut hingga timer berbunyi. Hindari semua gangguan.
4.  **Akhiri Pekerjaan Saat Timer Berbunyi:** Tandai bahwa satu pomodoro telah selesai.
5.  **Istirahat Pendek:** Ambil istirahat pendek, biasanya 5 menit. Selama istirahat, lakukan sesuatu yang tidak berhubungan dengan pekerjaan (misalnya, peregangan, minum air).
6.  **Ulangi:** Setelah istirahat pendek, mulai pomodoro berikutnya.
7.  **Istirahat Panjang:** Setelah menyelesaikan empat pomodoro, ambil istirahat yang lebih panjang, biasanya 15-30 menit.

**Manfaat Teknik Pomodoro:**

* Meningkatkan fokus dan konsentrasi.
* Mengurangi kelelahan mental.
* Meningkatkan kesadaran akan waktu yang dihabiskan.
* Membantu mengatasi prokrastinasi.
* Memecah tugas besar menjadi bagian-bagian yang lebih mudah dikelola.

## Cara Menggunakan Aplikasi Ini

Aplikasi ini dirancang agar mudah digunakan. Berikut adalah langkah-langkahnya:

### 1. Login atau Buat Akun

* **Email yang Diizinkan:** Aplikasi ini saat ini dikonfigurasi untuk mengizinkan pendaftaran dan login hanya untuk alamat email tertentu. Pastikan email Anda termasuk dalam daftar yang diizinkan oleh administrator aplikasi (jika Anda bukan administratornya).
* **Pendaftaran (Sign Up):**
    1.  Masukkan alamat email Anda yang valid dan diizinkan.
    2.  Masukkan password (minimal 6 karakter).
    3.  Klik tombol **"Sign Up"**.
* **Login:**
    1.  Masukkan alamat email yang sudah terdaftar dan diizinkan.
    2.  Masukkan password Anda.
    3.  Klik tombol **"Login"**.

    Jika login atau pendaftaran gagal karena email tidak diizinkan atau kredensial salah, pesan error akan muncul.

### 2. Tampilan Utama Aplikasi Pomodoro

Setelah berhasil login, Anda akan melihat antarmuka utama Pomodoro Timer:

* **Informasi Pengguna:** Di pojok kanan atas, Anda akan melihat email Anda dan tombol **"Logout"**.
* **Timer Display:** Menampilkan sisa waktu sesi saat ini (format MM:SS).
* **Tombol Mode:**
    * **Pomodoro:** Mengatur timer untuk sesi kerja (default 25 menit).
    * **Istirahat Pendek:** Mengatur timer untuk istirahat pendek (default 5 menit).
    * **Istirahat Panjang:** Mengatur timer untuk istirahat panjang (default 15 menit, biasanya diambil setelah 4 sesi Pomodoro).
* **Tombol Kontrol Timer:**
    * **Mulai:** Memulai timer untuk mode yang dipilih.
    * **Jeda:** Menjeda timer yang sedang berjalan.
    * **Atur Ulang:** Mengatur ulang timer ke durasi awal mode yang dipilih.
* **Tombol Hentikan Suara:** Tombol ini akan muncul saat notifikasi suara bel berbunyi di akhir sesi. Klik tombol ini untuk menghentikan suara dan melanjutkan ke mode sesi berikutnya.
* **Input Tugas:** (Hanya relevan untuk mode Pomodoro) Masukkan nama atau deskripsi singkat tugas yang sedang Anda kerjakan. Ini akan disimpan dalam riwayat sesi Anda.
* **Riwayat Sesi:** Menampilkan daftar 10 sesi Pomodoro terakhir yang telah Anda selesaikan, beserta nama tugas dan waktunya.

### 3. Memulai Sesi Pomodoro

1.  **Pilih Mode:** Klik tombol mode yang sesuai (misalnya, "Pomodoro").
2.  **Masukkan Nama Tugas:** Jika dalam mode "Pomodoro", ketikkan tugas yang akan Anda kerjakan di kolom "Apa yang sedang Anda kerjakan?".
3.  **Mulai Timer:** Klik tombol **"Mulai"**. Timer akan mulai menghitung mundur.
4.  **Fokus pada Tugas:** Kerjakan tugas Anda tanpa gangguan hingga timer berbunyi.

### 4. Akhir Sesi dan Notifikasi

* Ketika timer mencapai 00:00:
    * Notifikasi visual (jika diizinkan oleh browser) akan muncul.
    * Suara bel akan berbunyi secara berulang.
    * Tombol **"Hentikan Suara"** akan muncul.
* Klik tombol **"Hentikan Suara"**:
    * Suara bel akan berhenti.
    * Aplikasi akan secara otomatis beralih ke mode berikutnya (misalnya, dari Pomodoro ke Istirahat Pendek, atau dari Istirahat Pendek/Panjang kembali ke Pomodoro).
    * Timer untuk mode baru tersebut akan dimulai secara otomatis.

### 5. Istirahat

* Saat timer istirahat (pendek atau panjang) berjalan, gunakan waktu ini untuk benar-benar beristirahat dari pekerjaan Anda.
* Ketika timer istirahat berakhir, proses notifikasi suara dan tombol "Hentikan Suara" akan sama seperti akhir sesi Pomodoro. Setelah suara dihentikan, aplikasi akan kembali ke mode "Pomodoro" dan memulai timer.

### 6. Melihat Riwayat

* Sesi Pomodoro yang selesai (beserta nama tugasnya) akan otomatis tercatat di bagian "Riwayat Sesi". Ini membantu Anda melacak produktivitas Anda.

### 7. Logout

* Jika Anda ingin keluar dari aplikasi, klik tombol **"Logout"** di bagian informasi pengguna.

## Konfigurasi (Untuk Pengembang/Administrator)

* **Konfigurasi Firebase:** Pastikan Anda telah memasukkan detail konfigurasi proyek Firebase Anda di dalam kode (variabel `firebaseConfig`).
* **Daftar Email yang Diizinkan (`allowedEmails`):**
    * Di dalam file HTML (bagian `<script>`), terdapat array JavaScript bernama `allowedEmails`.
    * Edit array ini untuk menambahkan atau menghapus alamat email yang diizinkan untuk mendaftar dan login ke aplikasi.
        ```javascript
        const allowedEmails = [
            "email_anda@example.com",
            "rekan_kerja@example.com"
            // Tambahkan email lain di sini
        ];
        ```
    * **Catatan Keamanan:** Untuk aplikasi produksi dengan kebutuhan keamanan yang lebih tinggi, daftar email ini sebaiknya tidak disimpan langsung di kode klien. Pertimbangkan penggunaan Firebase Cloud Functions atau database terpisah untuk manajemen daftar akses yang lebih aman.

Selamat menggunakan Aplikasi Pomodoro Timer ini untuk meningkatkan fokus dan produktivitas Anda!

