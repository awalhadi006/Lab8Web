# Lab8Web
<h1> Langkah-langkah Praktikum </h1>

<p>
<ol>
  <li><b>Menjalankan MySQL Server</b></br>
    Untuk menjalankan MySQL Server dari menu XAMPP Control.
    
  ![Screenshot_248](https://user-images.githubusercontent.com/24362384/120874994-9b58ee00-c5d3-11eb-9bba-739cd27196ba.png)

  <li><b>Mengakses MySQL Client menggunakan PHP MyAdmin</b></br>
  Pastikan webserver Apache dan MySQL server sudah dijalankan. Kemudian buka melalui browser : http://localhost/phpmyadmin/

![Screenshot_249](https://user-images.githubusercontent.com/24362384/120875049-e5da6a80-c5d3-11eb-8d90-8164be037532.png)

  <li><b>Membuat Database</b></br>
  
  ```php
  CREATE DATABASE latihan1;
  ```
  
  ![Screenshot_250](https://user-images.githubusercontent.com/24362384/120875068-00acdf00-c5d4-11eb-9dff-264cf5326b12.png)

  ![Screenshot_251](https://user-images.githubusercontent.com/24362384/120875078-220dcb00-c5d4-11eb-81c2-3db37b35721b.png)

  <li><b>Membuat table</b></br>
  
  ```php
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
  
  ![Screenshot_252](https://user-images.githubusercontent.com/24362384/120875081-26d27f00-c5d4-11eb-8e5c-9f5e73ceabdc.png)

  ![Screenshot_253](https://user-images.githubusercontent.com/24362384/120875083-29cd6f80-c5d4-11eb-9929-0e9d18e6e0ac.png)

  <li><b>Menambahkan Data</b></br>
 
 ```php
 INSERT INTO data_barang (kategori, nama, gambar, harga_beli, harga_jual, stok)
VALUES ('Elektronik', 'HP Samsung Android', 'hp_samsung.jpg', 2000000, 2400000, 5),
('Elektronik', 'HP Xiaomi Android', 'hp_xiaomi.jpg', 1000000, 1400000, 5),
('Elektronik', 'HP OPPO Android', 'hp_oppo.jpg', 1800000, 2300000, 5);
```

![Screenshot_254](https://user-images.githubusercontent.com/24362384/120875099-45d11100-c5d4-11eb-8af8-23a9644af383.png)

![Screenshot_255](https://user-images.githubusercontent.com/24362384/120875106-49649800-c5d4-11eb-8d6e-8ae9f2fd5078.png)

  <li><b>Membuat Program CRUD</b></br>
  Buat folder <b>lab8_php_database</b> pada root directory web server (C:\xampp\htdocs)
  
 ![Screenshot_256](https://user-images.githubusercontent.com/24362384/120875143-89c41600-c5d4-11eb-8fc5-847dc2d85bc4.png)

  Kemudian untuk mengakses directory tersebut pada web server dengan mengakses URL: http://localhost/lab8_php_database/
  
  ![Screenshot_257](https://user-images.githubusercontent.com/24362384/120875183-c3951c80-c5d4-11eb-9e9c-d6b7ac6ae180.png)

  <li><b>Membuat file koneksi database</b></br>
  Buat file baru dengan nama <b>koneksi.php</b>
  
![Screenshot_258](https://user-images.githubusercontent.com/24362384/120875202-e32c4500-c5d4-11eb-9c18-5415709003bc.png)

  Buka melalui browser untuk menguji koneksi database (untuk menampilkan pesan koneksi berhasil, <b><i>uncomment</b></i> pada perintah {echo "koneksi berhasil"};
  
![Screenshot_259](https://user-images.githubusercontent.com/24362384/120875208-e6bfcc00-c5d4-11eb-8a59-0c6a9d808997.png)

  <li><b>Membuat file index untuk menampilkan data</b> <b><i>(Read)</i></b></br>
  Buat file baru dengan nama <b>index.php</b>

![Screenshot_261](https://user-images.githubusercontent.com/24362384/120875288-503fda80-c5d5-11eb-9d00-b59df39a88b9.png)

![Screenshot_260](https://user-images.githubusercontent.com/24362384/120875291-546bf800-c5d5-11eb-8b0d-8fe6d7e9b5e5.png)

  <li><b>Menambah Data</b> <b><i>(Create)</i></b></br>
  Buat file baru dengan nama <b>tambah.php</b>
  
  ![Screenshot_266](https://user-images.githubusercontent.com/24362384/120875325-85e4c380-c5d5-11eb-9eb6-856600f47a78.png)
  
![Screenshot_267](https://user-images.githubusercontent.com/24362384/120875328-87ae8700-c5d5-11eb-8e35-e0118caf801d.png)

![Screenshot_268](https://user-images.githubusercontent.com/24362384/120875330-88471d80-c5d5-11eb-932e-2c77b78bbcb0.png)

  <li><b>Mengubah Data</b> <b><i>(Update)</i></b></br>
  Buat file baru dengan nama <b>ubah.php</b>

![Screenshot_269](https://user-images.githubusercontent.com/24362384/120875355-a90f7300-c5d5-11eb-83e4-306c3fd51e32.png)

![Screenshot_270](https://user-images.githubusercontent.com/24362384/120875358-ab71cd00-c5d5-11eb-9fe3-7aea61436cb5.png)

![Screenshot_271](https://user-images.githubusercontent.com/24362384/120875361-aca2fa00-c5d5-11eb-9eca-398a46129328.png)

   <li><b>Menghapus Data</b> <b><i>(Delete)</i></b></br>
  Buat file baru dengan nama <b>hapus.php</b>
  
  ![Screenshot_272](https://user-images.githubusercontent.com/24362384/120875387-c80e0500-c5d5-11eb-95fc-faf0a7524c11.png)

![Screenshot_273](https://user-images.githubusercontent.com/24362384/120875389-cb08f580-c5d5-11eb-8e62-fafd62a10ac0.png)

![Screenshot_274](https://user-images.githubusercontent.com/24362384/120875390-ccd2b900-c5d5-11eb-8e00-aa90da21fb92.png)

  
