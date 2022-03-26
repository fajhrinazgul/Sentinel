#### MySQL -> My Structured Query Language

#### MySQL Database Command

#### ```;``` digunakan untuk mengakhiri perintah dari query command

Membuat database
```sql
-- Membuat Database Sekolah
CREATE DATABASE Sekolah;
```
Menggunakan database
```SQL
-- Memakai Database Sekolah
USE Sekolah;
```
Menghapus database
```SQL
-- Menghapus database sekolah
DROP DATABASE sekolah;
```
Menampilkan database yang ada
```SQL
-- Perhatikan ! Apabila ingin menampilkan daftar database atau table, selalu akhiri dengan tambahan s
SHOW DATABASES;
```
Menampilkan daftar table dalam suatu database
```SQL
SHOW tables;
```
Membuat table
```SQL
CREATE TABLE siswa(
  nisn int not null primary key auto_increment;
  nama varchar(50) not null,
  tempat_lahir varchar(10) not null,
  tanggal_lahir data not null,
  alamat text not null,
  agama int not null
  );
```
Menghapus data dalam table
```SQL
TRUNCATE TABLE siswa;
```
Menghapus table
```SQL
DROP TABLE siswa;
```
Merubah table
```SQL
-- Menambah column baru
ALTER TABLE siswa add varian int;
-- Menghapus column baru
ALTER TABLE siswa DROP varian;
-- Merubah tipe data
ALTER TABLE siswa MODIFY agama varchar(10);
```
Memasukkan data
```SQL
INSERT INTO siswa VALUES(1,'Budi','Riau','2022-01-01','Planet Namek','Islam');
```
Menampilkan data
```SQL
-- Menampilkan seluruh data
SELECT * FROM siswa;
```
Menampilkan data dengan kondisi tertentu
```SQL
-- Menampilkan data seluruh siswa dengan jenis kelamin Perempuan
SELECT * FROM siswa WHERE jekel = 'Perempuan';
```
Menampilkan n-data
```SQL
-- Menampilkan 5 data teratas dari tabel siswa
SELECT * FROM siswa LIMIT 5;
```
