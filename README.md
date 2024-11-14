# Praktikum 10 Dasar State Management 
### Brilyan Satria Wahyuda
### TI-3H
### 2241720019
## Praktikum 1

1. Selesaikan langkah-langkah praktikum tersebut, lalu dokumentasikan berupa GIF hasil akhir praktikum beserta penjelasannya di file README.md! Jika Anda menemukan ada yang error atau tidak berjalan dengan baik, silakan diperbaiki.
   
2. Jelaskan maksud dari langkah 4 pada praktikum tersebut! Mengapa dilakukan demikian?

    <p>Dibuat data_layer.dart yang bertujuan untuk export dua model plan.dart dan task.dart, hal ini agar tidak terlalu banyak import pada file lain. Cukup impor data_layer saja</p>
3. Mengapa perlu variabel plan di langkah 6 pada praktikum tersebut? Mengapa dibuat konstanta ?
    <p>Variabel plan digunakan untuk menyimpan daftar task yang akan dikelola. Sebagai instance dari Plan, variabel ini bisa memungkinkan kita mengakses dan mengubah daftar tugas. </p>

4. Lakukan capture hasil dari Langkah 9 berupa GIF, kemudian jelaskan apa yang telah Anda buat!
![Praktikum 1](praktikum1.gif)

    <p>Aplikasi menampilkan daftar tugas atau sebuah to-do list dengan masing-masing item berupa Checkbox dan TextFormField. Checkbox yang berfungsi untuk penanda apakah tugas sudah selesai, sedangkan TextFormField memungkinkan pengguna untuk mengubah deskripsi tugas.</p>

5. Apa kegunaan method pada Langkah 11 dan 13 dalam lifecyle state ?
    <p>
- initState(): Menginisialisasi state saat widget pertama kali dibuat. initState digunakan untuk membuat ScrollController dan menambahkan listener yang akan menutup keyboard ketika pengguna melakukan scroll.
- dispose(): Membersihkan resource ketika widget tidak lagi digunakan. dispose akan membuang ScrollController saat widget PlanScreen dihancurkan, sehingga mencegah memory leak.
</p>