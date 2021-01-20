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
  - [Break and Continue](#break-and-continue)
  - [Conditional if](#conditional-if)
    - [Kondisi if](#kondisi-if)
    - [Kondisi if .. else](#kondisi-if--else)
    - [Kondisi if .. else if](#kondisi-if--else-if)
  - [Conditional switch](#conditional-switch)
  - [Array](#array)
- [Pengolahan Multimedia Interaktif Menggunakan Kode Program](#pengolahan-multimedia-interaktif-menggunakan-kode-program)
  - [Properti Movie Clip](#properti-movie-clip)
  - [Menambah Objek dengan AddChild dan RemoveChild (AS3)](#menambah-objek-dengan-addchild-dan-removechild-as3)
  

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

### Break and Continue
Break dan continue digunakan untuk menginterupsi sebuah operasi berulang (loops). Break digunakan untuk menghentikan operasi berulang ketika suatu kondisi dalam blok terpenuhi.

1. Penerapan break dapat dilihat pada kode program berikut
```as3
for (var i:int=1; i<20; i+=3){
    if(i==10){
        break;
        }

    trace(i);

}

//output 1 4 7
```

Berdasarkan contoh di atas, operasi for seharusnya menaikkan nilai variabel i sebanyak 3 poin untuk setiap langkah, sehingga menghasilkan angka 1,4,7,10,13,16 dan 19. Tetapi karena adanya kondisi (i==10) terpenuhi, hasilnya adalah kode break dijalankan dan operasi berulang dihentikan sehingga menghasilkan angka 1, 4, dan 7.

2. Penerapan continue dapat dilihat pada kode program berikut

```as3
for(var i:=1; i<20; i+=3){
     if(i==10){
        continue; 
        }
    trace(i);
}

//output 1 4 7 13 16 19
```
Pada dasarnya kode continue akan melewatkan satu langkah jika kondisi terpenuhi, sehingga pada kode di atas dengan kondisi (i == 10) terpenuhi maka perulangan hanya dilewati satu langkah, sehingga angka 10 tidak muncul.

### Conditional if
Logika dasar di sebagian besar bahasa pemrograman menggunakan kondisi if. Dengan kode if sebuah kondisi dapat diketahui kebenarannya dan blok kode akan dieksekusi berdasarkan kondisi tersebut.

#### Kondisi if
Perhatikan kode program sebagai berikut.
```as3
function bilGanjil(angka:int):void{
    if (angka%2 == 1){
        trace(angka+” adalah bilangan ganjil”);
    }
}

bilGanjil(7);
```
Jika pada baris 2 terdapat sebuah kondisi dengan sebuah nilai mengalami operasi modulus (%) dengan angka 2. Jika angka yang dimaksud dibagi dengan bilangan 2 dan ternyata menyisakan bilangan 1 (disimbolkan dengan operator ==), maka angka tersebut dipastikan sebagai bilangan ganjil.

#### Kondisi if .. else
Perhatikan kode program sebagai berikut.

```as3
function bilGanjil(angka:int):void{
    if(angka%2 == 1){
        trace(angka+”adalah bilangan ganjil”);
    } else {
        trace(angka+” adalah bilangan genap”);
    }
}

bilGanjil(7); // 7 adalah bilangan ganjil

bilGenap(4); // 4 adalah bilangan genap
```
Pada kondisi tersebut di atas, jika kondisi bernilai salah maka kode pada blok else akan dijalankan. Secara umum, kondisi if .. else dapat dilakukan beberapa kali dengan kondisi yang berbeda-beda.

#### Kondisi if .. else if
Perhatikan kode program sebagai berikut.
```as3
function cekNil(nilai:int):void{
    if(nilai<6){
        trace(“Anda tidak lulus”);
    } else if (nilai<8) {
        trace(“Cukup bagus, Anda mendapatkan nilai C”);
    } else if (nilai<10) {
        trace(“Bagus, Anda mendapatkan nilai B”);
    } else {
        trace(“Nilai Sempurna”);
    }

}

cekNil(9); // Nilai sempurna
```

Berdasarkan kondisi di atas maka prosedur pengecekan logika diawali dari kondisi teratas dan jika terpenuhi akan dilanjutkan ke logika berikutnya. Dengan demikian ketika kode cekNil(9); dijalankan maka kondisi (nilai < 6) tidak terpenuhi, kondisi (nilai < 8) tidak terpenuhi, sedangkan kondisi (nilai < 10) terpenuhi. Oleh karena itu ditampilkan hasil kondisi terakhir yang terpenuhi yaitu (nilai < 10).

### Conditional switch
Kondisi switch digunakan ketika terdapat beberapa kondisi yang berbeda-beda. Pada kode tersebut beberapa kondisi telah ditentukan, dan ketika kondisi yang tersebut terpenuhi di salah satu kode case maka kode dijalankan sampai terjadinya eksekusi kode break. Jika tidak ada kondisi yang terpenuhi maka blok kode default yang akan dijalankan. Perhatikan contoh kode berikut ini.
```as3
function cekNil(Nil:String):void{
    Switch(Nil){
        case “A”: {
            trace(“Nilai Anda : Sangat baik”);
            break;
        }
        case”B”: {
            trace(“Nilai Anda : Baik “);
            break;
        }
        case “C”: {
            trace(“Nilai Anda : Cukup baik “);
            break;
        }
        case “D”: {
            trace(“Nilai Anda : Kurang”);
            break;
        }
        case “E”: {
            trace(“Anda gagal “);
            break;
        }
        default: {
            trace(“input data salah”);
            break;
        }
    }
}

cekNil(“C”);
```

### Array
Array sebagai sebuah struktur data yang bisa digunakan untuk menyimpan beberapa variabel dengan nama yang sama. Misalnya data nama siswa kelas 1, data soal kuis, data nama hari, data nama bulan, dan sebagainya. Perhatikan penerapan berikut.

```as3
var nmHari:Array = [“Senin”, “Selasa”, “Rabu”, “Kamis”,”Jumat”, “Sabtu”, “Minggu”];

trace(nmHari[1]); //Selasa

trace(nmHari[4]); //Jumat
```

Berdasarkan kode program di atas, terlihat bahwa variabel nmHari yang memiliki nilai yaitu “Senin” sampai “Minggu” dideklarasikan dengan tipe array. Untuk menggunakan data yang berada di dalam Array, dapat digunakan nama variabel diikuti tanda [nomor_data]. Misalnya variabel nmHari[0] yang ternyata bernilai “Senin”, karena berada di urutan pertama (nomor data dimulai dari angka 0), dan seterusnya.

## Pengolahan Multimedia Interaktif Menggunakan Kode Program
Keunggulan multimedia di dalam interaktivitas adalah media tersebut mampu memaksa user untuk berinteraksi dengan materi secara fisik dan mental. Interaktivitas sebagai derajat partisipan dalam proses komunikasi memiliki kontrol dan kemampuan bertukar peran dalam mutual discourse. Dengan menggunakan konsep tersebut bisa dibedakan tiga level interaktivitas yaitu:

1. Percakapan tatap muka dengan derajat interaktivitas tertinggi, 
2. Interaktivitas antara orang dengan medium, atau orang dengan sistem di mana isi dapat dimanipulasikan, serta 
3. Interaktivitas yang diperoleh dalam sistem informasi tanpa adanya intervensi dari user untuk mengubah konten. 

Oleh sebab itu, guna memahami proses pengembangan interaktifitas dalam media yang akan dibuat, perlu memahami terlebih dahulu dasar-dasar dalam memanipulasi objek.

### Properti Movie Clip
Movie clip sebagai salah satu bentuk objek sering diaplikasikan dalam multimedia interaktif, sehingga seorang programmer harus mampu memanipulasi Movie clip. Setiap objek dalam Adobe Flash memiliki parameter-parameter yang disebut sebagai properties, misalnya Movie clip tersebut memiliki posisi dengan bentuk kordinat x dan y (z jika menggunakan metode 3D), rotasi, timeline, skala, warna, dan sebagainya.

Langkah-langkah dalam membuat tombol Movie clip menggunakan Adobe Flash CS6 adalah sebagai berikut.

1. Mengaktifkan program Adobe Flash, dan selanjutnya klik pada ActionScript 3 (AS3). Setelah itu membuat sebuah lingkaran menggunakan Oval Tool (atau menekan tombol O) dengan warna kuning atau sesuai dengan kebutuhan.

2. Selanjutnya melakukan Selection Tool (atau menekan tombol V), setelah itu melakukan seleksi lingkaran dengan cara klik satu kali.

3. Berikutnya melakukan convert menjadi Movie Clip dengan cara menekan tombol F8 sehingga muncul kotak dialog Convert to Symbol dan diberi nama tmb_kuning dan pada Type pilih opsi Movie clip dan diakhiri dengan menekan tombol OK.

4. Double klik pada “tmb_kuning” sehingga masuk ke Movie clip tmb_kuning. Pada tahap tersebut dapat membuat animasi sederhana berupa Motion Tween dan memberi sedikit efek menggunakan fitur Filter.

5. Selanjutnya melakukan Convert to Movie clip pada lingkaran kuning yang berada dalam Movie clip tersebut dengan menekan tombol F8 dan memberi nama tmb_kuning2. Adapun pada Type opsi Movie clip.

6. Berikutnya klik kanan pada frame 10 dan klik pada Insert Keyframe (atau menekan tombol F6). Kilik kanan kembali pada frame 20 dan klik pada Insert Keyframe. Setelah itu, klik kanan pada antara frame 1 sampai 10 dan klik pada Create Motion Tween. Ulangi langkah-langkah tersebut untuk frame 11 sampai 20.

7. Klik pada lingkaran kuning yang ada di frame 10. Selanjutnya di panel Properties klik pada pilih Filter→Add Filter (simbol +)→klik Glow. Selanjutnya mengatur visual efek sesuai kebutuhan, misalnya menggunakan warna hijau, blur X : 55 dan blur Y : 55. Centang pada Inner Glow dengan tujuan efek Glow berada di dalam objek lingkaran.

8. Setelah itu, klik kanan pada frame 1 dan pilih Actions (atau menekan tombol F9), lalu klik kode : stop(); dengan tujuan agar animasi Button yang dibuat dapat berhenti. Ulangi langkah yang sama untuk frame ke-10 dan frame ke-20. Setelah itu memberi nama : Home di dalam Movie clip tmb_kuning2.

9. Selanjutnya masuk ke dalam Scene 1 dengan cara klik pada Scene 1. Klik tombol tersebut diikuti dengan menekan tombol F9 sehingga muncul kotak dialog ActionScript dan masukkan kode program sebagai berikut.
```as3
On (release, rollover) {
    gotoAndPlay(2);
}

On (release, rollout) {
    gotoAndPlay(11);
}
```
10. Untuk menjalankan movie clip dilakukan dengan menekan tombol kombinasi Ctrl+ Enter. Diikuti dengan mengarahkan pointer pada tombol tersebut. Jika berubah menjadi glow hijau, berarti Movie clip yang dibuat sudah berhasil.

### Menambah Objek dengan AddChild dan RemoveChild (AS3)
Salah satu metode yang paling sering digunakan oleh programmer dalam membuat aplikasi adalah menambahkan objek ke layar dengan menggunakan kode dengan memanfaatkan fasilitas AddChild dan RemoveChild. Script AddChild dan RemoveChild digunakan untuk memasukkan dan menghapus objek pada sebuah stage. Script tersebut berguna bagi programmer yang menginginkan objek-objek di stage dapat dimasukkan dan dihapus. Prosedur pelaksanaannya diawali dengan membuat objek dan memberi linkage pada objek tersebut. Setelah itu baru memberikan script.

1. Membuat sebuah dokumen Flash dengan ukuran 400 x 400 pixel dan sebuah lingkaran berukuran 100 x 100 pixel. Seleksi lingkaran tersebut dan tekan F8. Pada panel yang muncul identitas sebagai berikut.

    - Pada kotak isian name, masukkan : LingkarClip.
    - Pada option type pilih pada Movie clip.
    - Klik atau contreng pada Export for ActionScript.
    - Pada kotak isian class, masukkan : LingkarClip.
    - Akhiri dengan menekan tombol OK.

2. Selanjutnya Movie clip yang ada di stage harus dihapus.

3. Klik pada frame 1 diikuti dengan menekan tombol F9 untuk mengaktifkan panel Action dan diisi dengan kode script sebagai berikut.
```as3
var LingkarClip:LingkarClip=new LingkarClip();

//perintah membuat variable bernama LingkarClip dan diisi movie clip yang berlinkage LingkarClip

addChild(LingkarClip);

// perintah memasukkan LingkarClip ke dalam stage.
```
4. Guna melakukan tes (ujicoba) dilakukan dengan menekan tombol kombinasi Ctrl+Enter. Hasilnya adalah terlihat sebuah lingkaran di stage (sebelumnya tidak ada).

5. Guna mengubah posisi Movie clip dapat diatur pada komposisi koordinat sumbu x dan y. Langkahnya adalah klik pada frame 1 diikuti dengan menekan tombol F9 untuk mengaktifkan panel Action dan menambahkan script sebagai berikut.
```as3
var LingkarClip:LingkarClip=new LingkarClip();

//prosedur mengatur posisi LingkarClip
    LingkarClip.x=250;
    LingkarClip.y=250;
    addChild(LingkarClip);
```
Setelah menekan tombol kombinasi Ctrl+Enter, maka posisi lingkaran tepat berada di tengah-tengah stage.

6. Berikutnya adalah prosedur menghapus Movie clip dengan cara klik pada frame 1 diikuti dengan menekan tombol F9 untuk mengaktifkan panel Action dan menambahkan script sebagai berikut.
```as3
var LingkarClip:LingkarClip=new LingkarClip();

LingkarClip.x=250;

LingkarClip.y=250;

addChild(LingkarClip);

removeChild(LingkarClip); //menghapus LingkarClip
```
Setelah menekan tombol kombinasi Ctrl+Enter, maka lingkaran akan terhapus dengan sendirinya.