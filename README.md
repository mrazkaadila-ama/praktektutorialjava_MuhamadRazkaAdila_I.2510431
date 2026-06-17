# Java CRUD Siswa

Aplikasi desktop berbasis Java Swing untuk mengelola data siswa menggunakan konsep CRUD (Create, Read, Update, Delete) dan database MySQL.

## Deskripsi

Project ini dibuat menggunakan Java dan NetBeans IDE sebagai media pembelajaran koneksi database menggunakan JDBC. Aplikasi memungkinkan pengguna untuk menambah, melihat, mengubah, dan menghapus data siswa melalui antarmuka GUI (Graphical User Interface).

## Fitur

✅ Menampilkan data siswa dari database

✅ Menambahkan data siswa

✅ Mengubah data siswa

✅ Menghapus data siswa

✅ Reset form input

✅ Menampilkan data pada JTable

✅ Koneksi database menggunakan JDBC

## Data yang Dikelola

- NIS
- Nama
- Jurusan
- Jenis Kelamin
- Alamat

### Pilihan Jurusan

- Rekayasa Perangkat Lunak (RPL)
- Teknik Komputer dan Jaringan (TKJ)
- Multimedia

### Pilihan Jenis Kelamin

- Laki-laki
- Perempuan

## Teknologi yang Digunakan

- Java
- Java Swing
- JDBC
- MySQL
- NetBeans IDE

## Struktur Project

```text
Java CRUD
│
├── src
│   ├── koneksi
│   │   └── koneksi.java
│   │
│   └── tutorialjava
│       └── FormSiswa.java
│
├── build
├── nbproject
├── test
├── build.xml
└── manifest.mf
```

## Struktur Database

### Membuat Database

```sql
CREATE DATABASE tutorialjava;
```

### Menggunakan Database

```sql
USE tutorialjava;
```

### Membuat Tabel Students

```sql
CREATE TABLE students (
    nis VARCHAR(20) PRIMARY KEY,
    nama VARCHAR(100) NOT NULL,
    jurusan VARCHAR(100) NOT NULL,
    jk VARCHAR(20) NOT NULL,
    alamat TEXT
);
```

## Konfigurasi Database

File:

```text
src/koneksi/koneksi.java
```

Konfigurasi koneksi:

```java
Connection koneksi = DriverManager.getConnection(
    "jdbc:mysql://localhost/tutorialjava",
    "root",
    ""
);
```

Pastikan:

- MySQL berjalan
- Database `tutorialjava` sudah dibuat
- Tabel `students` sudah tersedia

## Cara Menjalankan Project

### Clone Repository

```bash
git clone https://github.com/mrazkaadila-ama/praktektutorialjava_MuhamadRazkaAdila_I.2510431.git
```

### Buka di NetBeans

1. Jalankan NetBeans IDE
2. Pilih Open Project
3. Pilih folder project Java CRUD
4. Klik Open

### Jalankan Database

- Aktifkan Apache dan MySQL melalui XAMPP
- Buat database dan tabel sesuai struktur di atas

### Run Project

Klik:

```text
Run Project (F6)
```

atau

```text
Run File (Shift + F6)
```

## Tampilan Aplikasi

Form terdiri dari:

- Input NIS
- Input Nama
- ComboBox Jurusan
- ComboBox Jenis Kelamin
- Input Alamat
- Tombol Simpan
- Tombol Update
- Tombol Hapus
- Tombol Reset
- Tabel Data Siswa

## Author

**Muhamad Razka Adila**

NIM: **I.2510431**

## Repository

https://github.com/mrazkaadila-ama/praktektutorialjava_MuhamadRazkaAdila_I.2510431

## Lisensi

Project ini dibuat untuk keperluan pembelajaran dan praktikum pemrograman Java.
