# Teknik Pemrograman dan Pengolahan pada Multimedia Interaktif <!-- omit in toc --> 
- [Teknik Pemrograman (Coding)](#teknik-pemrograman-coding)
  - [Kode](#kode)
  - [Syntax](#syntax)
    - [Case Sensitive](#case-sensitive)
    - [Semicolons](#semicolons)
    - [Parentheses atau Tanda Kurung ()](#parentheses-atau-tanda-kurung-)
    - [Code Block](#code-block)
    - [Whitespace](#whitespace)
    - [Comments (komentar)](#comments-komentar)
    - [Literals](#literals)
    - [Keywords dan Reserved Words](#keywords-dan-reserved-words)
  

Guna membentuk sebuah interaktivitas dalam sebuah multimedia interaktif diperlukan berbagai tahap pemrograman. Pemrograman identik dengan suatu kegiatan menuliskan kumpulan urutan perintah ke komputer untuk mengerjakan sesuatu, di mana instruksi tersebut menggunakan bahasa yang dimengerti oleh komputer atau dikenal dengan Bahasa pemrograman. Dalam hal ini, programming termasuk jenis keahlian yang akhir-akhir ini banyak dipelajari orang, seiring berkembangnya teknologi dan meningkatnya permintaan masyarakat akan developer, belajar coding bisa menjadi aset berharga. Salah satunya adalah **ActionScript** sebagai Bahasa pemrograman yang dipakai oleh software Flash untuk mengendalikan object-object ataupun movie.

Dalam membuat sebuah media interaktif menggunakan Adobe Flash memerlukan proses yang Panjang dan terus-menerus. Ada berbagai jenis produk, konten, dan aplikasi yang ditujukan bagi user Flash. Namun demikian, adakalanya produk-produk tersebut menggabungkan support system untuk ActionScript dengan menambahkan interaktivitas dan perilaku output. Desainer professional dan Developer menggunakan ActionScipt untukmembuat konten dan aplikasi untuk Flash Player dengan memanfaatkan aplikasi Flash, The Flex, dan Flash Media Server.

## Teknik Pemrograman (Coding)

Adobe flash memiliki bahasa pemrograman yang disebut sebagai ActionScript, dan sejak tahun 2007 standar industri yang digunakan adalah ActionScript 3.0 (AS3) sebagai pengembangan bahasa pemrograman ActionScript 2.0. Salah satu kelebihan ActionScript 3.0 terletak pada file ActionScript 3.0 yang dapat dibuat terpisah saat runtime. Guna memahami dengan baik konsep dasar pemrograman ActionScript 3, maka diperlukan pemahaman secara bertahap, yang diawali dengan mempelajari sebuah kode pemrograman harus dimulai dari teknik dasar terlebih dahulu. Salah satu kegunaan ActionScript yang paling banyak digunakan adalah mengatur timeline untuk mengendalikan animasi, misalnya dalam sebuah media terdapat animasi yang pada awalnya merupakan gambar diam, tetapi setelah tombol ditekan gambar tersebut bergerak. Proses tersebut membutuhkan pengaturan yang melibatkan kode.

 
### Kode

Penulisan kode ActionScript dalam Adobe Flash dikerjakan di area panel Action. Pada saat aplikasi dijalankan, maka compiler akan mengecek kode setiap baris mulai dari posisi teratas hingga pada kode baris terakhir. Dari proses pengecekan tersebut, jika ditemukan kesalahan maka proses akan berhenti dan kesalahan akan ditampilkan. Hal ini tentu saja mempermudah seorang developer (pengembang aplikasi) guna menyempurnakan kode tersebut. Penulisan sebuah kode sangat spesifik dan mendetail, sebab sebuah kesalahan kecil bisa berakibat pada berhentinya aplikasi atau gagalnya proses compiling. Di samping itu, juga terdapat istilah-istilah pesan error seperti syntax, string, dan sebagainya.

1. Setelah mengaktifkan Adobe Flash, dilanjutkan dengan membuat sebuah file baru. Selanjutnya klik pada frame 1-layer 1 dan membuka panel Action dengan menekan klik pada menu Window à Action (F9). Hal penting yang harus dipahami adalah Flash ActionScript 3 hanya dapat diletakkan di sebuah frame atau di sebuah file yang terpisah menggunakan metode Class. Sehingga sebelum menuliskan kode, harus diawali dengan melakukan seleksi Keyframe tempat kode tersebut akan dijalankan.

2. Klik pada panel Action, dan pada editor kode ketikkan kode berikut.
    ```as3
    trace(“Latihan membuat kode ActionScript dasar”);
    ```
    Pada dasarnya, kode trace berfungsi untuk menampilkan parameter yang ada di dalam tanda (); berupa parameter tertentu yang berisi sebuah tulisan.

3. Untuk melakukan ujicoba dengan cara menjalankan aplikasi dengan menekan tombol kombinasi Ctrl + Enter. Hasilnya adalah munculnya panel Output dengan tulisan “Latihan membuat kode ActionScript dasar”.

4. Jika salah satu tanda petik di bagian awal dihilangkan/dihapus maka saat dijalankan dengan menekan tombol kombinasi Ctrl + Enter akan muncul panel Compiler Errors dengan menampilkan pesan khusus atau sintaks (Syntax Error): A String literal must be terminated before the line break. Pesan tersebut menyatakan telah terjadi kesalahan pada kode variabel berupa String harus diawali dengan tanda “.

### Syntax

Definisi sintaks (syntax) dalam pemrograman komputer identik dengan seperrangkat aturan yang harus dipenuhi dalam penulisan kode (coding). Sintaks meliputi simbol, kata, dan fungsi yang dapat digunakan serta bagaimana menggunakannya dalam sebuah struktur kode pemrograman. Jenis kesalahan yang sering dijumpai adalah syntax error yang menyebabkan aplikasi tidak bisa dijalankan dengan baik. Beberapa aturan dasar dalam penulisan AS3 adalah sebagai berikut.

#### Case Sensitive

Format sensitif case dalam penulisan kode AS3 sebagai bentuk dasar penulisan kode yang harus ditulis dengan tepat, yakni satu perbedaan karakter akan menghasilkan perbedaan yang jelas. Misalnya, `var bilGanjil:int;` hasilnya akan berbeda `var BilGanjil:int;` meskipun hanya berbeda pada huruf ‘b’ saja.

#### Semicolons

Penggunaan semicolons (;) atau titik koma dalam AS3 sebagai akhir dari sebuah baris kode. Walaupun ditulis dalam satu baris, jika ditambahkan tanda titik koma tepat di belakangnya akan dinyatakan sebagai baris perintah baru. Perhatikan kode AS3 berikut.
```
kode kotak 1;

kode kotak 2; kode kotak 3;
```
#### Parentheses atau Tanda Kurung ()

Parentheses digunakan untuk mengubah urutan dalam sebuah operasi/fungsi, di mana operasi yang berada dalam tanda kurung akan dijalankan terlebih dahulu oleh program. Perhatikan penerapan parentheses berikut.
```as3
trace(9-3*2); //akan menghasilkan nilai 3

trace((9-3)*2); //akan menghasilkan nilai 12
```
Di samping itu, parentheses dapat digunakan dengan memberikan masukan pada sebuah fungsi tertentu. Perhatikan penerapan sebagai berikut.
```as3
trace(“Latihan Koding AS3”); //Menghasilkan kata Latihan Koding AS3

trace(kuadrat(3)); //menghasilkan nilai 9 dengan menggunakan fungsi buatan, yaitu fungsi kuadrat()
```
#### Code Block

Satu blok kode dalam pemrograman AS3 bisa diterjemahkan sebagai sebuah paket yang digunakan dalam fungsi (function), class, loop, dan sebagainya. Dalam hal ini, satu baris atau lebih yang terletak di dalam kurung kurawal {} juga bisa disebut sebagai satu blok kode. Perhatikan penerapan code block sebagai berikut.
```as3
function pangkat(num:Number):Number{
    return num*num;
}

for(var i:uint=1;i<8;i++) {
    var hsl_pangkat:Number = pangkat(i);
    trace(“Hasil pangkat “+i+” = “+hsl_pangkat);
}
```
#### Whitespace

Istilah yang digunakan untuk penulisan, tab, enter dan spasi yang ditujukan untuk mempermudah penulisan kode sering disebut whitespace (ruang kosong). Karakteristik whitespace dapat dilihat pada baris yang menjorok masuk atau adanya baris yang sengaja dikosongkan agar terdapat jarak antara fungsi yang satu dengan fungsi di bawahnya. Perhatikan dua contoh berikut yang bermakna sama tetapi ditulis dengan cara yang berbeda.
```as3
for(var i:uint=0;i<7;i++) {
    trace(i);
}
```
atau

`for(var i:uint=0;i<7;i++){trace(i);}`
#### Comments (komentar)

Comments identik dengan catatan yang bisa ditambahkan pada kode dengan tujuan memudahkan dalam memberikan keterangan pada kode yang sedang ditulis. Program secara otomatis mengabaikan baris komentar tersebut, sehingga programmer tidak perlu khawatir menggunakan comments (komentar). Perhatikan penerapan sebagai berikut.

```
trace(“Komentar”); //komentar dalam 1 baris
```

Hal ini banyak dilakukan ketika menulis kode dalam jumlah banyak sehingga membutuhkan penjelasan-penjelasan pada baris kode untuk mempermudah proses pengecekan. Di samping itu, penggunaan comment juga bertujuan menonaktifkan sementara pada kode yang tidak dibutuhkan. Misalnya pada saat proses pengecekan kode yang panjang (debugging), seorang programmer sering kali membuat beberapa baris kode dinonaktifkan untuk menguji kesalahan yang ada. Jika ingin komentar lebih dari satu baris, dapat menggunakan tanda /* dan ditutup dengan tanda */.

#### Literals
Literals identik dengan nilai yang dituliskan ke kode dalam bentuk angka, string, maupun array. Misalnya 17, 64532, “kalimat Tanya”, [7, 8, 9], dan sebagainya.

#### Keywords dan Reserved Words

Secara mendasar, keywords dan reserved words termasuk jenis kata kunci dan kata khusus yang telah dipakai sebagai kode, sehingga tidak bisa digunakan sebagai identifier. AS3 memiliki beberapa keyword dan kata khusus yang pada panel ActionScript akan diberi warna yang berbeda dan akan memberikan peringatan jika memakainya. Keyword dalam pemrograman AS3 dikategorikan sebagai berikut.

| No | Jenis Keyword | Keterangan |
| -- | ------------- | ---------- |
| 1  | Lexical       | Kata-kata yang sudah digunakan dalam rangkaian kode. Misalnya as if return break super case |
| 2  | Syntactic     | Kata-kata yang dapat digunakan sebagai identifier, memiliki fungsi tertentu jika digunakan dalam konteks yang benar. Misalnya each include override get dynamic static |