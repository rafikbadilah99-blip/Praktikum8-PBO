# 📝 Modul Praktikum 8 - Pemrograman Berbasis Objek (Java)

Repositori ini berisi implementasi kode untuk **Praktikum 8** dalam mata kuliah **Pemrograman Berbasis Objek (PBO)**. Praktikum ini berfokus pada konsep dasar OOP tingkat lanjut dalam bahasa pemrograman Java, meliputi **Polimorfisme (Upcasting & Overriding)**, **Abstract Class**, dan **Multiple Interface**.

---

## 📌 Daftar Isi

- [Konsep Materi](#-konsep-materi)
- [Struktur Repositori](#-struktur-repositori)
- [Penjelasan Kode & Contoh Output](#-penjelasan-kode--contoh-output)
  - [1. Polimorfisme (Hewan)](#1-polimorfisme-hewan)
  - [2. Abstract Class (Bangun Datar)](#2-abstract-class-bangun-datar)
  - [3. Multiple Interface (Smartphone)](#3-multiple-interface-smartphone)
- [Cara Menjalankan Kode](#-cara-menjalankan-kode)
- [Author](#-author)

---

## 💡 Konsep Materi

1. **Polimorfisme & Dynamic Binding**

   Polimorfisme adalah kemampuan suatu objek untuk memiliki banyak bentuk. Metode yang dipanggil ditentukan secara dinamis saat program berjalan (*runtime*), bergantung pada objek sebenarnya yang menempati memori. Konsep ini berkaitan dengan *upcasting*, *method overriding*, dan *dynamic binding*.

2. **Abstract Class**

   *Abstract class* adalah kelas abstrak yang tidak dapat diinstansiasi secara langsung menggunakan kata kunci `new`. Kelas ini berfungsi sebagai cetak biru (*blueprint*) bagi subclass yang mewarisinya. Subclass harus mengimplementasikan *abstract method* yang diwariskan, kecuali subclass tersebut juga dideklarasikan sebagai abstrak.

3. **Interface**

   *Interface* merupakan kontrak perilaku (*behavioral contract*) yang mendefinisikan metode yang perlu diimplementasikan oleh suatu kelas. Java mendukung implementasi beberapa interface sekaligus menggunakan kata kunci `implements`, sehingga sebuah kelas dapat memiliki berbagai kemampuan dari beberapa interface.

---

## 📁 Struktur Repositori

```text
src/
└── com/
    └── praktikum8/
        ├── Hewan.java
        ├── Kucing.java
        ├── Anjing.java
        ├── PoliTester.java
        ├── BangunDatar.java
        ├── Lingkaran.java
        ├── TesBangunDatar.java
        ├── AlatElektronik.java
        ├── Kamera.java
        ├── Smartphone.java
        └── TesSmartphone.java
```

---

## 💻 Penjelasan Kode & Contoh Output

### 1. Polimorfisme (Hewan)

Program ini mendemonstrasikan polimorfisme melalui pemanggilan metode `bersuara()` pada array bertipe superclass `Hewan[]` yang berisi objek dari beberapa subclass, yaitu `Kucing` dan `Anjing`.

Teknik *upcasting* memungkinkan objek subclass diperlakukan sebagai objek superclass. Dengan *method overriding* dan *dynamic binding*, metode yang dijalankan menyesuaikan tipe objek sebenarnya saat program berjalan.

**File terkait:** `Hewan.java`, `Kucing.java`, `Anjing.java`, dan `PoliTester.java`.

**Contoh Output:**

```text
Hewan ini mengeluarkan suara yang tidak spesifik.
Kucing: Meow meow!
Anjing: Guk guk!
```

### 2. Abstract Class (Bangun Datar)

Program ini mendemonstrasikan penggunaan *abstract class* `BangunDatar` yang memiliki atribut bersama berupa `warna`, *concrete method* `cetakWarna()`, dan *abstract method* `hitungLuas()` yang diimplementasikan oleh subclass `Lingkaran`.

Konsep ini memungkinkan kelas abstrak menyediakan atribut dan perilaku umum, sementara subclass memberikan implementasi khusus sesuai kebutuhan.

**File terkait:** `BangunDatar.java`, `Lingkaran.java`, dan `TesBangunDatar.java`.

**Contoh Output:**

```text
Warna bangun ini adalah: Merah
Luas lingkaran: 78.53981633974483
```

### 3. Multiple Interface (Smartphone)

Program ini mendemonstrasikan implementasi beberapa interface sekaligus dalam Java. Kelas `Smartphone` mengimplementasikan dua interface, yaitu `AlatElektronik` dan `Kamera`.

Dengan pendekatan ini, kelas `Smartphone` dapat menyediakan beberapa perilaku sekaligus, seperti menyalakan perangkat, mengambil foto, dan mematikan perangkat.

**File terkait:** `AlatElektronik.java`, `Kamera.java`, `Smartphone.java`, dan `TesSmartphone.java`.

**Contoh Output:**

```text
Samsung menyala. Booting OS...
Cekrek! Foto berhasil disimpan di galeri Samsung.
Samsung dimatikan. Goodbye.
```

---

## 🚀 Cara Menjalankan Kode

Pastikan Java Development Kit (JDK) sudah terpasang di komputer. Periksa instalasi Java melalui terminal dengan perintah berikut:

```bash
java -version
javac -version
```

### 1. Clone Repositori

Unduh repositori dari GitHub dan masuk ke direktori proyek.

```bash
git clone https://github.com/rafikbadilah99-blip/Praktikum8-PBO.git
cd Praktikum8-PBO
```

### 2. Kompilasi Berkas Java

Buat direktori `bin` untuk menyimpan hasil kompilasi, kemudian kompilasi seluruh berkas Java.

```bash
mkdir -p bin
javac -d bin src/com/praktikum8/*.java
```

### 3. Jalankan Program

Setelah proses kompilasi berhasil, jalankan masing-masing kelas penguji berikut.

**Pengujian Polimorfisme:**

```bash
java -cp bin com.praktikum8.PoliTester
```

**Pengujian Abstract Class:**

```bash
java -cp bin com.praktikum8.TesBangunDatar
```

**Pengujian Multiple Interface:**

```bash
java -cp bin com.praktikum8.TesSmartphone
```

---

## 👤 Author

- **Nama:** Rafik Badilah
- **NIM:** L0325009
- **Kelas:** Semester 3 (A)

---

*Praktikum 8 — Pemrograman Berbasis Objek (PBO) | Java*
