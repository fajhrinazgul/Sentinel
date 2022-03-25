#### MySQL -> My Structured Query Language

#### MySQL Database Command

#### ```;``` digunakan untuk mengakhiri perintah dari query command

1. Membuat database
```sql
-- Membuat Database Sekolah
CREATE DATABASE Sekolah;
```
2. Menggunakan database
```SQL
-- Memakai Database Sekolah
USE Sekolah;
```
3. Menghapus database
```SQL
-- Menghapus database sekolah
DROP DATABASE sekolah;
```
5. Menampilkan database yang ada
```SQL
-- Perhatikan ! Apabila ingin menampilkan daftar database atau table, selalu akhiri dengan tambahan s
SHOW DATABASES;
```
7. Membuat table
```SQL
CREATE TABLE siswa(
  nisn int not null primary key auto_increment;
  nama varchar(50) not null,
  tempat_lahir varchar(10) not null,
  tanggal_lahir data not null,
  alamat text not null,
  agama varchar(10) not null);
```
9. Menghapus table
10. Merubah table
11. Memasukkan data
12. Menampilkan data
```SQL
-- Menampilkan seluruh data
SELECT * FROM siswa;
```
10. Menampilkan data dengan kondisi tertentu
```SQL
-- Menampilkan data seluruh siswa dengan jenis kelamin Perempuan
SELECT * FROM siswa WHERE jekel = 'Perempuan';
```
11. Menampilkan n-data
```SQL
-- Menampilkan 5 data teratas dari tabel siswa
SELECT * FROM siswa LIMIT 5
```
