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
6. Menampilkan daftar table dalam suatu database
```SQL
SHOW tables;
```
7. Membuat table
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
9. Menghapus table
10. Merubah table
```SQL
-- Menambah column baru
ALTER TABLE siswa add varian int;
-- Menghapus column baru
ALTER TABLE siswa DROP varian;
-- Merubah tipe data
ALTER TABLE siswa MODIFY agama varchar(10);
```
12. Memasukkan data
13. Menampilkan data
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
