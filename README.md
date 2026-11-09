# Proyek Inventaris Toko - Aplikasi Daftar Produk Toko

Repositori ini berisi kode sumber aplikasi desktop berbasis Java dan JavaFX untuk pencatatan inventaris produk toko. Proyek ini dibuat untuk memenuhi tugas individu pemrograman berorientasi objek dan antarmuka grafis (GUI).

## Identitas Mahasiswa
* Nama: Rizky Pratama
* NIM: 2508475
* Program Studi: Mekatronika dan Kecerdasan Buatan

## Deskripsi Sistem
Aplikasi Daftar Produk Toko dibangun menggunakan sistem build Apache Maven dan menerapkan pola arsitektur MVC (Model, View, Controller). Aplikasi ini berfungsi untuk mencatat data produk ke dalam memori selama program berjalan, menampilkannya ke dalam tabel, melakukan pencarian data, serta melihat rincian dari setiap produk.

 Setiap produk yang dicatat memiliki empat atribut utama:
1. Kode produk (dibuat otomatis secara berurutan seperti PR001, PR002, dan seterusnya).
2. Nama produk.
3. Kategori produk (Makanan atau Minuman).
4. Harga produk.

## Fitur Utama
1. Formulir Tambah Produk: Halaman untuk memasukkan nama produk, memilih kategori (Makanan atau Minuman), dan mengisi harga produk. Dilengkapi validasi untuk menolak input apabila nama produk kosong atau harga kurang dari maupun sama dengan nol.
2. Tabel Daftar Produk: Menampilkan seluruh produk yang tersimpan dalam bentuk tabel dengan kolom kode produk, nama produk, kategori, dan harga.
3. Pencarian Produk: Fitur pencarian berdasarkan nama produk melalui kolom input dan tombol Cari, dilengkapi tombol Reset untuk menampilkan kembali seluruh data.
4. Halaman Detail Produk: Menampilkan rincian informasi lengkap dari satu objek produk yang dipilih pengguna pada tabel maupun setelah menyimpan produk baru.

## Struktur Proyek
* `kelas.MainApp`: Kelas utama untuk menjalankan aplikasi JavaFX.
* `kelas.Navigator`: Pengatur perpindahan halaman antarmuka (Form, Daftar, dan Detail) serta pengirim konteks data antar halaman.
* `kelas.model.Produk`: Kelas model dengan atribut private, constructor bervalidasi, dan metode getter.
* `kelas.data.DataProduk`: Kelas penyimpan daftar produk di memori menggunakan ObservableList.
* `kelas.controller`: Berisi `FormController`, `DaftarController`, dan `DetailController` yang menghubungkan tampilan FXML dengan logika program.
* `resources/kelas`: Berisi file tata letak antarmuka (`form.fxml`, `daftar.fxml`, `detail.fxml`) serta file desain tampilan (`styles/app.css`).

<img width="957" height="562" alt="Screenshot 2026-11-09 174245" src="https://github.com/user-attachments/assets/d44b7502-82fe-452a-999c-bbce91bd9330" />
<img width="959" height="563" alt="Screenshot 2026-11-09 174301" src="https://github.com/user-attachments/assets/1393803d-2e02-4849-9f71-42d5ece2f05b" />
<img width="959" height="562" alt="Screenshot 2026-11-09 174313" src="https://github.com/user-attachments/assets/74e3c3c4-12d6-4183-8d83-155c788fcfc7" />



## Spesifikasi dan Cara Menjalankan
* Bahasa Pemrograman: Java 17
* Framework UI: JavaFX 21
* Build Tool: Apache Maven
* IDE: Apache NetBeans

Untuk menjalankan program, buka proyek ini di Apache NetBeans lalu jalankan perintah Run Project (atau melalui terminal dengan perintah `mvn clean javafx:run`).
