# 📝 Modul Praktikum 8 - Pemrograman Berbasis Objek (Java)

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![OOP](https://img.shields.io/badge/OOP-Polymorphism%20%26%20Abstraction-blue?style=for-the-badge)

Repositori ini berisi implementasi kode untuk **Praktikum 8** dalam mata kuliah *Pemrograman Berbasis Objek (PBO)*. Praktikum ini berfokus pada konsep dasar OOP tingkat lanjut di bahasa pemrograman Java, meliputi **Polimorfisme (Upcasting & Overriding)**, **Abstract Class**, dan **Multiple Interface**.

---

## 📌 Daftar Isi
- [Konsep Materi](#-konsep-materi)
- [Struktur Repositori](#-struktur-repositori)
- [Penjelasan Kode & Contoh Output](#-penjelasan-kode--contoh-output)
  - [1. Polimorfisme (Hewan)](#1-polimorfisme-hewan)
  - [2. Abstract Class (Bangun Datar)](#2-abstract-class-bangun-datar)
  - [3. Multiple Interface (Smartphone)](#3-multiple-interface-smartphone)
- [Cara Menjalankan Kode](#-cara-menjalankan-kode)

---

## 💡 Konsep Materi

1. **Polimorfisme & Dynamic Binding**: Kemampuan suatu objek untuk memiliki banyak bentuk. Metode yang dipanggil ditentukan secara dinamis saat runtime (*late binding*) tergantung pada objek sebenarnya yang menempati memori.
2. **Abstract Class**: Kelas abstrak yang tidak dapat diinstansiasi secara langsung (`new`). Digunakan sebagai cetak biru (*blueprint*) untuk subclass yang harus meng-override *abstract method*-nya.
3. **Interface**: Kontrak perilaku (*behavioral contract*) penuh. Java mendukung *multiple inheritance* menggunakan interface melalui kata kunci `implements`.

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
