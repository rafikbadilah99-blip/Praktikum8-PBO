# 📝 Modul Praktikum 8 - Pemrograman Berbasis Objek (Java)

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
```
---

## 💻 Penjelasan Kode & Contoh Output

**1. Polimorfisme (Hewan)**
Mendemonstrasikan pemanggilan method bersuara() pada array bertipe superclass (Hewan[]) yang diisi oleh berbagai elemen subclass (Kucing dan Anjing) melalui teknik upcasting.

File terkait: Hewan.java, Kucing.java, Anjing.java, PoliTester.java
```text
📤 Output PoliTester:
Hewan ini mengeluarkan suara yang tidak spesifik.
Kucing: Meow meow!
Anjing: Guk guk!
```

**2. Abstract Class (Bangun Datar)**
Mendemonstrasikan penerapan abstract class BangunDatar yang memiliki atribut bersama (warna), concrete method (cetakWarna()), dan abstract method (hitungLuas()) yang diturunkan ke kelas Lingkaran.
*File terkait: BangunDatar.java, Lingkaran.java, TesBangunDatar.java*
```text
📤 Output TesBangunDatar:
Warna bangun ini adalah: Merah
Luas lingkaran: 78.53981633974483
```

**3. Multiple Interface (Smartphone)**
Mendemonstrasikan multiple inheritance di Java. Kelas Smartphone mengimplementasikan dua interface sekaligus, yaitu AlatElektronik dan Kamera.
```text
*File terkait: AlatElektronik.java, Kamera.java, Smartphone.java, TesSmartphone.java*
📤 Output TesSmartphone:
Samsung menyala. Booting OS...
Cekrek! Foto berhasil disimpan di galeri Samsung.
Samsung dimatikan. Goodbye.
```
---

## 🚀 Cara Menjalankan Kode

Melalui Terminal / Command Line
1. Clone repositori ini:
git clone
cd **praktikum8-pbo**
2. 
