#### MySQL -> My Structured Query Language

#### MySQL Database Command

1. Membuat database
```sql
-- Membuat Database Sekolah
-- QUERY - CREATE DATABASE databasename;
CREATE DATABASE Sekolah;
```
2. Menggunakan database
```SQL
-- Memakai Database Sekolah
-- QUERY - USE databasename;
USE Sekolah;
```
3. Menghapus database
4. Menampilkan database yang ada
5. Membuat table
6. Menghapus table
7. Merubah table
8. Memasukkan data
9. Menampilkan data
10. Menampilkan data dengan kondisi tertentu
```SQL
-- Menampilkan data seluruh siswa dengan jenis kelamin Perempuan
SELECT * FROM siswa WHERE jekel = 'Perempuan';
```
12. Menampilkan n-data
```SQL
-- Menampilkan 5 data teratas dari tabel siswa
SELECT * FROM siswa LIMIT 5
```
