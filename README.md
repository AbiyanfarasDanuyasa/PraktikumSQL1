# PraktikumSQL1
# Latihan 2
```
NAMA         : Abiyanfaras Danuyasa
NIM          : 312210103
KELAS        : TI.22.A2
MATA KULIAH  : BASIS DATA
```
# tugas praktikum
# 1. langkah pertama buat terlebih dahulu database dengan nama latihan2.
untuk membuat database gunakan perintah sebagai berikut:
```
create database [nama_database]
contohnya
create database latihan2
```
lalu, setelah kita membuat database selanjutnya kita masuk kedalam database tersebut dengan perintah sebagai berikut:
```
use latihan2;
```
![gambar2](https://user-images.githubusercontent.com/115562487/231254714-bec3b9ad-1b8f-47a4-8b05-99461ed2b962.png)
# 2. buat sebuah tabel dengan nama biodata seperti nama, alamat didalam database latihan2.
untuk membuat table gunakan perintah sebagai berikut:
```
CREATE TABLE nama_tabel (nama_field1 tipe _data(ukuran), nama_field2 tipe_data(ukuran), ..., nama_fieldn tipe_data(ukuran));
CREATE TABLE biodata (nama VACHAR (15), alamat TEXT);
```
![gambar1](https://user-images.githubusercontent.com/115562487/231254804-bb7535b2-269b-427e-afd2-55ef21d12958.png)
# 3. tambahkan sebuah kolom keterangan (varchar 15), sebagai kolom trakhir.
 
untuk menambahkan kolom terakhir yaitu deangan sering digunakan kata after, contoh:
```
alter table biodata add column keterangan varchar (15) after phone;
```
![gambar3](https://user-images.githubusercontent.com/115562487/231254929-05244682-9dc0-4a09-b09a-e1e8a6cb8356.png)
# 4. tambahkan kolom id(int11) di awal (sebagai kolom pertama).
untuk menambahkan kolom pertama yaitu dengan perintah sebagai berikut:
```
alter table biodata add column id(int11) first;
```
![gambar4](https://user-images.githubusercontent.com/115562487/231255019-64e6413f-41c8-443a-883a-4f5c0def3d7d.png)
# 5. sisipkan sebuah kolom dengan nama phone (varchar 15) setelah kolom alamat.
untuk menambahkan kolom setelah kolom lain yaitu dengan perintah after
![gambar5](https://user-images.githubusercontent.com/115562487/231255076-dd1a9482-4b2d-45f6-97af-d67daef97b07.png)
# 6. ubah tipe data kolom id menjadi char(11).
untuk mengubah type data yaitu dengan perintah sebagai berikut:
```
alter table [nama_table] modify nama_field tipe_data_baru(ukuran);
```
![gambar6](https://user-images.githubusercontent.com/115562487/231255166-ad4ab63e-bb03-43d0-98d7-d0277c1cb5a3.png)
# 7. ubah nama kolom phone menjadi hp(varchar20).
untuk mengubah kolom yaitu dengan perintah sebagai berikut:
```
ALTER TABLE [nama_tabel] CHANGE nama_field_lama nama_field_baru tipe_data(ukuran);
```
![gambar7](https://user-images.githubusercontent.com/115562487/231255241-036c4d49-1bff-4ec5-bb12-c35e9da0f7b0.png)
# 8.tambahkan kolom email setelah kolom hp 
![gambar8](https://user-images.githubusercontent.com/115562487/231255353-438adebf-d95c-4bb8-97be-d96dda38fa37.png)
# 9. hapus kolom keterangan dari table.
untuk menghapus kolom dari dable yaitu dengan perintah sebagai berikut:
```
alter table [nama_table] drop_field;
```
![gambar9](https://user-images.githubusercontent.com/115562487/231255534-7e61ab49-81f9-48e8-ae71-e09138c094c9.png)
# 10. ganti nama table menjadi data_mahasiswa.
untuk mengganti nama table yaitu dengan perintah sebagai berikut:
```
alter table [nama_table] rename [nama_table_baru]
```
![gambar10](https://user-images.githubusercontent.com/115562487/231255683-76f18cc0-634e-4790-8451-c85dbbd67141.png)
# 11. ganti nama field id menjadi nim.
![gambar11](https://user-images.githubusercontent.com/115562487/231255788-aa400efa-663b-4c2c-854a-d4464f3747ad.png)
# 12. jadikan nim sebagai primary key.
untuk menambahkan index atau key, gunakan perintah sebagai berikut:
-tipe
-primary key
-unique key 
-fulltext
```
ALTER TABLE [nama_tabel] ADD [INDEX|PRIMARY KEY] (nama_field);
```
![gambar12](https://user-images.githubusercontent.com/115562487/231255898-26c682e8-bb9d-446c-aeb0-8f051d78862f.png)
# 13. jadikan kolom email sebagai
perintahnya sama seperti diatas, hanya saja diganti menjadi unique key.
![gambar13](https://user-images.githubusercontent.com/115562487/231255990-dfaeeaf9-8efd-449d-9ce5-4123951bfb17.png)
# evaluasi dan pertanyaan 
1. tulis semua printah-perintah SQL percobaan di pdf praktikum 1 beserta outputnya!
sql dll
* membuat database
```
create database latihan2
```
![gambar2](https://user-images.githubusercontent.com/115562487/231256652-d07dfe0c-d112-4b53-89f4-863f1da23329.png)
* membuat table 
```
create biodata (nama varchar (15), alamat text)
```


![gambar1](https://user-images.githubusercontent.com/115562487/231256727-e15f368a-3718-414b-9a4f-cd2e717a526c.png)



* menambah kolom 
```
alter table biodata add column keterangan text after alamat;
```


![gambar3](https://user-images.githubusercontent.com/115562487/231257250-db7a1782-f6e3-4cc6-bc04-e4c7e9adbaef.png)

@@ -147,23 +152,35 @@ alter table biodata add column keterangan text after alamat;
```
alter table biodata add column id int first;
```



![gambar4](https://user-images.githubusercontent.com/115562487/231257383-a08188ce-8d88-47ae-b02f-74e01d2d3698.png)



* mengubah nama kolom 
* mengubah nama kolom



![gambar7](https://user-images.githubusercontent.com/115562487/231257563-37a9fa8a-44fe-4bec-9c7f-ceea9739de89.png)



* mengubah tipe data 



![gambar6](https://user-images.githubusercontent.com/115562487/231257706-48aecc58-9e3e-4c3e-a649-916890b7de8d.png)



* menghapus kolom 



![gambar9](https://user-images.githubusercontent.com/115562487/231257829-c5cb1343-d512-4161-b876-b70ff2919a1e.png)




2. apa maksud dari int(11)?
int(11) adalah nama tipe datanya yaitu integer dan memiliki panjang 11 karakter



3. ketika melihat struktur table dengan perintah desc, ada kolom null yang berisi yes dan no, apa maksudnya?
maksudnya yaitu untuk menjelaskan bahwa pada record yang harus diisi. sedangkan yes bisa tidak diisi
