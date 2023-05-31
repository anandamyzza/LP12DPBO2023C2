# Deskripsi Tugas Latihan 12 DPBO 2023
* Ubahlah hasil dari Latihan Praktikum 7 menjadi MVP atau MVVM dan berikan alasannya.

## Penjelasan Kenapa Menggunakan MVVM
Alasan utama mengapa menggunakan MVVM karena saya cukup mengerti dengan struktur MVVM daripada MVP. Di mana **view**nya MVVM adalah `Synchronization.java` yang memiliki `main` yang memanggil **viewmodel** `Game.java`. Dalam `main` ini, `Synchronization.java` hanya melakukan instansiasi `Game` sehingga memiliki struktur MVVM di mana MVVM bagian **view** tidak saling berhubungan dan tidak bisa mengakses **model** selain melalui **viewmodel**.
