# Lab8Web
## Praktikum-8
## PHP dan DataBase MySQL
## Langkah Langkah Praktikum
### Menjalankan MySQL server
Untuk menjalankan MySQL Server dari menu XAMPP Contol.

![ss1](/image/ss1.png)
### Mengakses MySQL Client menggunakan PHP MyAdmin
Pastikan webserver Apache dan MySQL server sudah dijalankan. Kemudian buka
melalui browser: http://localhost/phpmyadmin/


### Membuat Database: Studi Kasus Data Barang
- Membuat Database 
```
Create Database latihan1;
```
- Membuat Table 
```
CREATE TABLE data_barang (
    id_barang int(10) auto_increment Primary Key,
    kategori varchar(30),
    nama varchar(30),
    gambar varchar(100),
    harga_beli decimal(10,0),
    harga_jual decimal(10,0),
    stok int(4)
);
```
![ss2](/image/ss2.png)
### Menambahkan Data 
```
INSERT INTO data_barang (kategori, nama, gambar, harga_beli, harga_jual, stok)
VALUES ('Elektronik', 'HP Samsung Android', 'hp_samsung.jpg', 2000000, 2400000, 5),
('Elektronik', 'HP Xiaomi Android', 'hp_xiaomi.jpg', 1000000, 1400000, 5),
('Elektronik', 'HP OPPO Android', 'hp_oppo.jpg', 1800000, 2300000, 5);
```
![ss3](/image/ss3.png)
### Membuat Program CRUD
Buat folder lab8_php_database pada root directory web server (d:\xampp\htdocs)
![ss4](/image/ss4.png)

- Kemudian untuk mengakses direktory tersebut pada web server dengan mengakses URL:
http://localhost/lab8_php_database/
![ss5](/image/ss5.png)

### Membuat file koneksi database
Buat file baru dengan nama koneksi.php
![koneksi](/image/koneksi.png)
![ss6](/image/ss6.png)
Buka melalui browser untuk menguji koneksi database (untuk menyampilkan pesan
koneksi berhasil, uncomment pada perintah echo “koneksi berhasil”;

### Membuat File Index untuk menampilkan data(Read)
Buat File baru dengan nama index.php
![index](/image/index.png)
![ss7](/image/ss7.png)

### Menambahkan Data Create
Buat File dengan nama tambah.php
![tambah](/image/tambah.png)
![ss8](/image/ss8.png)

### Menambahkan Data Update
Buat file dangan nama ubah.php
![ubah](/image/ubah.png)
![ss9](/image/ss9.png)

### Menghapus Data (Delete)
Buat file dengan nama hapus.php
![hapus](/image/hapus.png)

### Menambahkan CSS untuk merapihkan file PHP
![css](/image/css.png)

