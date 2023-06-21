# Deskripsi Tugas Latihan 12 DPBO 2023

- Ubahlah hasil dari Latihan Praktikum 7 menjadi MVP atau MVVM dan berikan alasannya.

## Penjelasan Kenapa Menggunakan MVVM

Alasan utama mengapa saya menggunakan MVVM karena saya cukup mengerti dengan struktur MVVM daripada MVP. Di mana **view** nya MVVM adalah `Synchronization.java` yang memiliki `main` yang memanggil **viewmodel** `Game.java`. Dalam `main` ini, `Synchronization.java` hanya melakukan instansiasi `Game` sehingga memiliki struktur MVVM di mana MVVM bagian ****view**** tidak saling berhubungan dan tidak bisa mengakses ****model**** selain melalui ****viewmodel****.

## **Perbedaan Struktur LP12 dan TMD**
Berikut merupakan perbedaan struktur MVVM pada LP12 dan TMD yang saya kerjakan:

- `Display.java` yang berfungsi untuk menampilkan tampilan window game berada di **view** pada TMD saya.
- `Handler.java` yang berfungsi untuk handling GameObject berada di **viewmodel** pada TMD saya.

Sehingga, struktur yang digunakan pada LP12 ini jika mengikuti TMD yang saya buat seharusnya memiliki struktur sebagai berikut:

#### **model**

- GameInterface.java
- GameObject.java
- Player.java

#### **view**

- Display.java
- Synchronization.java

#### **viewmodel**

- Controller.java
- Game.java
- Handler.java

_Note: `GameInterface.java` tidak saya gunakan pada struktur TMD, karena `GameInterface.java` berfungsi sebagai interface yang kurang lebih memiliki fungsi yang sama seperti contract pada MVP._
