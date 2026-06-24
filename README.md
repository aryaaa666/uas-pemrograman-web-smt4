# uas-pemrograman-web-smt4
# Sistem Manajemen Data Mahasiswa
## Tugas UAS Web 2
# Nama arya zhalna nugraha
# Nim 312410371
# Kelas I241C
## Deskripsi
Aplikasi ini merupakan proyek Tugas UAS Mata Kuliah Web 2 yang dibuat menggunakan CodeIgniter 4 sebagai backend dan frontend berbasis web. Aplikasi digunakan untuk mengelola data mahasiswa dengan fitur CRUD (Create, Read, Update, Delete).

---

## Fitur
- Login Admin
- Dashboard
- Tambah Data Mahasiswa
- Lihat Data Mahasiswa
- Edit Data Mahasiswa
- Hapus Data Mahasiswa
- Pencarian Data Mahasiswa
- API Backend menggunakan CodeIgniter 4

---

## Teknologi yang Digunakan
- PHP 8.2+
- CodeIgniter 4
- MySQL / MariaDB
- HTML
- CSS
- JavaScript
- Bootstrap
- XAMPP

---

## Struktur Folder

```
web2_uas/
│
├── backend-api/
│   ├── app/
│   ├── public/
│   ├── writable/
│   ├── vendor/
│   └── ...
│
├── frontend/
│
├── database/
│   └── web2_uas.sql
│
└── README.md
```

---

## Cara Instalasi

### 1. Install XAMPP
Gunakan XAMPP dengan PHP versi 8.2 atau lebih baru.

### 2. Copy Project
Copy folder project ke:

```
C:\xampp\htdocs\
```

Sehingga menjadi:

```
C:\xampp\htdocs\web2_uas
```

---

### 3. Jalankan XAMPP

Start:

- Apache
- MySQL

---

### 4. Import Database

1. Buka

```
http://localhost/phpmyadmin
```

2. Buat database

```
web2_uas
```

3. Import file

```
web2_uas.sql
```

---

### 5. Konfigurasi Database

Buka file

```
backend-api/.env
```

atau

```
backend-api/app/Config/Database.php
```

Sesuaikan konfigurasi:

```
database.default.hostname = localhost
database.default.database = web2_uas
database.default.username = root
database.default.password =
database.default.DBDriver = MySQLi
```

---

### 6. Jalankan Backend

Masuk ke folder backend:

```
cd C:\xampp\htdocs\web2_uas\backend-api
```

Kemudian jalankan:

```
php spark serve
```

atau

```
C:\xampp\php\php.exe spark serve
```

Backend akan berjalan pada:

```
http://localhost:8080
```

---

### 7. Jalankan Frontend

Jika menggunakan Vite:

```
cd frontend
npm install
npm run dev
```

Jika frontend berupa HTML biasa:

```
http://localhost/web2_uas/frontend
```

---

## Database

Nama Database:

```
web2_uas
```

Import file:

```
web2_uas.sql
```

---

## ERD

Database terdiri dari tabel utama:

- users
- mahasiswa

Relasi:

```
users (1)
     │
     └─────────────< mahasiswa (N)
```

---

## Akun Login

```
Username : admin
Password : admin123
```

*(Sesuaikan jika berbeda pada database.)*

---

## Author

**Nama:** ....................................

**NIM:** .....................................

**Mata Kuliah:** Web 2

**Universitas:** ....................................
