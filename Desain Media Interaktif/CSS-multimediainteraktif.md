# Style pada Multimedia Interaktif (CSS) <!-- omit in toc --> 


Informasi memegang peranan penting dalam berbagai bidang kehidupan manusia, sehingga dunia teknologi informasi dapat berkembang dengan pesat. Informasi tersebut tidak terlepas dari perkembangan teknologi yang membuat segalanya lebih dinamis dan efisien. Salah satunya pada penggunaan bidang multimedia interaktif berupa gambar, teks, video, audio, dan animasi.

Bidang tersebut banyak digunakan dalam desain majalah, iklan televisi, presentasi, seminar, maupun membuat film animasi sebagai langkah alternatif dalam menyampaikan informasi agar lebih menarik. Pada umumnya, untuk membuat multimedia interaktif dengan tampilan menarik beserta kemudahan dalam mengubah tampilan layar berkaitan erat dengan kinerja style **CSS (Cascading Style Sheet)**. Cascading style sheet juga dapat diterapkan pada elemen-elemen HTML multimedia di antaranya gambar, video, dan audio

- [Pengaturan Style pada Teks](#pengaturan-style-pada-teks)
  - [Pengaturan warna pada teks (color)](#pengaturan-warna-pada-teks-color)
  - [Pengaturan spasi antarkarakter (word letter spacing)](#pengaturan-spasi-antarkarakter-word-letter-spacing)
  - [Pengaturan bentuk dalam teks dekorasi (decoration)](#pengaturan-bentuk-dalam-teks-dekorasi-decoration)
  - [Pengaturan antarkata (spaci word spacing)](#pengaturan-antarkata-spaci-word-spacing)
  - [Pengaturan jarak indentasi paragraph (text indent)](#pengaturan-jarak-indentasi-paragraph-text-indent)
  - [Pengaturan dari huruf besar dan kecil dalam sebuah teks (text transform)](#pengaturan-dari-huruf-besar-dan-kecil-dalam-sebuah-teks-text-transform)
  - [Pengaturan efek beyangan (shadow effect) dalam teks bayangan (shadow text)](#pengaturan-efek-beyangan-shadow-effect-dalam-teks-bayangan-shadow-text)
  - [Pengaturan teks rata (text alignment)](#pengaturan-teks-rata-text-alignment)
- [Pengaturan style pada tampilan gambar](#pengaturan-style-pada-tampilan-gambar)
- [Pengaturan style pada latar belakang (Background)](#pengaturan-style-pada-latar-belakang-background)


## Pengaturan Style pada Teks

Dalam pengaturan style teks meliputi beberapa jenis rangkaian properti di antaranya pewarnaan, spasi, jenis font, style font, color font, dan sebagainya yang dapat dikondisikan dalam kemasan CSS. Beberapa properti dari CSS antara lain sebagai berikut.

| No | Properti           | Keterangan                                                                    |
|----|--------------------|-------------------------------------------------------------------------------|
| 1  | *color*            | Mengatur warna pada teks/script yang hendak dituju.                           |
| 2  | *direction*        | Menentukan arah tulisan atau teks pada script terkait.                        |
| 3  | *letter-spacing*   | Menambah atau mengurangi properti dari spasi antarkarakter dalam suatu teks.  |
| 4  | *line-height*      | Mengatur tinggi barisnya suatu teks.                                          |
| 5  | *text-align*       | Bertugas memberi rata atau batas teks secara horizontal.                      |
| 6  | *text-decoration*  | Menentukan hiasan/decorasi pada teks.                                         |
| 7  | *text-indent*      | Bertugas mengatur jarak inden dalam baris pertama dalam teks blok.            |
| 8  | *text-shadow*      | Bertugas menentukan efek dari bayangan pada suatu teks.                       |
| 9  | *text-transform*   | Bertugas mengatur dari teks kecil hingga besar.                               |
| 10 | *unicode-bidi*     | Bertugas mengeset Unicode.                                                    |
| 11 | *vertical-align*   | Mengatur dari batas teks secara vertikal.                                     |
| 12 | *white-space*      | Mengatur dari penulisan white-space pada suatu elemen.                        |
| 13 | *word-spacing*     | Menambahkan atau mengurangi spasi antarkata dalam suatu teks.                 |

Bentuk-bentuk pengaturan style pada teks adalah sebagai berikut.

### Pengaturan warna pada teks (color)

Penggunaan style pada pengaturan warna (color) dapat diimplementasikan dalam sebuah teks/script. Pengaturan warna dalam teks tersebut menggunakan 3 nilai jenis warna yang terdiri atas nilai HEX, nilai RGB, dan nilai warna live (langsung) misalnya blue, red, black, pink, brown, atau white. Bentuk format penulisan untuk pemberian warna pada teks adalah sebagai berikut.

`Selector {color:’nilai warna’}`

Sedangkan bentuk implementasikan adalah sebagai berikut.

1. `.kotak {color:”#30cc91”}`
2. `.kotak {color:”rgb(249,54)”}`
3. `.kotak {color:”brown”}`

### Pengaturan spasi antarkarakter (word letter spacing)

Komponen letter-spacing berfungsi sebagai sarana atau alat yang digunakan untuk memberikan jarak (spasi) dalam karakter atau hutuf terkait. Bentuk format penulisan untuk pengaturan spasi antarkarakter (word letter spacing) adalah

`selector:{letter-spacing: nilai spasi;}`

Bentuk implementasikannya adalah sebagai berikut.

`Selector: {letter-spacing: 14px;}`

### Pengaturan bentuk dalam teks dekorasi (decoration)

Pengaturan teks menggunakan properti teks dekorasi bertujuan untuk membantu dalam mengatur atau menghapus suatu dekorasi dalam suatu teks. Bentuk format penulisan untuk pengaturan bentuk dalam teks dekorasi (decoration) adalah selector {text-decoration: nilai text-decoration}. Bentuk penerapannya sebagai berikut.

`.kotak {text-decoration: 20px text-decoration}`

### Pengaturan antarkata (spaci word spacing)

Word spacing sebagai salah satu style pada CSS dipergunakan untuk memberikan spasi (jarak) pada beberapa kata-kata atau huruf. Bentuk format penulisan untuk pngaturan antarkata (spassi word spacing) adalah sebagai berikut.

`Selector: {word-spacing: nilai spasi;}`

Bentuk penerapannya sebagai berikut.

`Selector: {word-spacing: 24px;}`

### Pengaturan jarak indentasi paragraph (text indent)

Secara mendasar, text indent bertugas sebagai alat untuk mengatur jarak indent dari baris awal dalam suatu teks blok, sehingga teks pada beris-baris awal terlihat lebih menjorok ke dalam dibandingkan teks baris lainnya. Bentuk format penulisan untuk pengaturan jarak indentasi paragraf (text indent) adalah sebagai berikut.

`Selector: {text-indent: nilai indent}`

Bentuk penerapannya sebagai berikut

`.kotak {text-indent: 16px indent}`

### Pengaturan dari huruf besar dan kecil dalam sebuah teks (text transform)

Text transform dipergunakan untuk menentukan ukuran huruf besar/kecil dalam suatu teks. Bentuk format penulisan untuk hutuf besar dan kecil dalam sebuah teks (text transform) adalah sebagai berikut.

`Selector: {text-transform: nilai text-transform}`

Bentuk penerapannya sebagai berikut.

`Selector: {text-transform: 22px text-transform}`

### Pengaturan efek beyangan (shadow effect) dalam teks bayangan (shadow text)

Shadow teks berfungsi sebagai alat yang dipergunakan untuk memberikan suatu bayangan pada sebuah teks. Bentuk format penulisan untuk pengaturan efek bayangan (shadow effect) dalam text bayangan (shadow text) adalah sebagia berikut.

`Selector {text-shadow: koordinatx koordinatY nilai warna teks;}`

Bentuk penerapannya sebgai berikut.

`Selector {text-shadow: koordinatx koordinatY #30cc90;}`

### Pengaturan teks rata (text alignment)

Properti dari text-alignment berfungsi sebagai alat yang mengatur dari jenis rata pada suatu teks bertipe horinzontal. Teks rata dapat ditulis dalam bentuk rata kanan, rata kiri, rata tengah, rata sejajar, maupun rata kanan kiri. Bentuk format penulisan untuk pengaturan teks rata (text alignment) adalah sebagi berikut.

`Selector: {text-align: jumlah nilai text-align;}`

Bentuk penerapannya sebagai berikut.

`.kotak {text-align: 18px text-align;}`

## Pengaturan style pada tampilan gambar

Style sangat berperan dalam menyajikan suatu informasis visual agar terlihat lebih baik serta lebih optimal jika dilihat dari sisi nonpenulisan, sehingga lebih disukai oleh mesin pencari (search engine). Dalam hal ini, penggunaan cascading style sheet (CSS) dapat diterapkan pada semua objek yang ingin disisipkan dalam bentuk tag tag tertentu, misalnya bentuk tulisan, table, gambar, maupun objek lainnya. Guna memberi pengaturan dalam penggunaan gambar pada umumnya dapat diterapkan secara inline, misalnya dengan format pemanggilan berikut.

```html
<imgsrc=’nm-filebr’width=’lebargbr’height=’tinggigbr’alt=’kata-kuncigbr’title=’judulgbr’ border=’garistebal’ />
```

Selain dengan metode inline, penambahan CSS dapat diterapkan dengan metode embed (diluar/eksternal) dalam CSS. Misalnya, apabila terdapat 4 gambar yang ingin diberi style, di mana ke 4 gambar tersebut berukuran sama, yaitu 150px x 150px dengan jarak margin atas dari gambar tersebut adalah 15px. Dalam hal ini, penulisan yang berhubungan dengan tayangan yang akan ditampilkan dalam bentuk kode program berikut.

```HTML
<!DOCTYPE HTML>
<html>
<head>
    <Tampilan 4 gambar CSS </title>
    <style>
        Img {
            Margin-top: 15px;
            Float: left;
            Clear: both;
            Width: 150px;
            Height: 150px;
        }

    </style>
</head>

<body>
    Tampilan 4 image (gambar) CSS </br>
    <img src=’meja.jpg’>
    <img src=’kursi.jpg’>
    <img src=’gelas.jpg’>
    <img src=’kipas.jpg’>
</body>

</html>
```

## Pengaturan style pada latar belakang (Background)

Pada dasarnya, penambahan gambar pada latar belakang (background) menggunakan dua jenis property, yaitu latar belakang (background) dan gambar latar belakang (background-image). Nilai yang diinputkan untuk property tersebut adalah URL gambar yang adakalanya berjumlah lebih dari satu dalam sebuah file CSS, termasuk didalamnya penambahan dalam satu font. Perhatikan contoh script berikut!

```css
div {
    background: url(latbcgl.png’);
    background-image: url(latbcgl.png’);
}
```

Jika menggunakan kode script di atas, dapat menimbulkan masalah ketika ukuran gambar yang digunakan tidak sesuai dengan ukuran-ukuran elemen. Misalnya, gambar akan ditampilkan berulang-ulang secara horizontal maupun vertical jika ukuran elemen tersebut lebih besar dari ukuran gambar. Oleh sebab itu, jika ingin menerapkan gambar dalam bentuk kode program maka penulisan script-nya adalah sebagai berikut.

```html
<html>

<head>
    <title>Latar Belakang Gambar </title>
    <style type=’text/css’>
        #awal1 {
            background-image: url(komp_mm.jpg);
            height: 400px; 
            width: 600px;
        }
    </style>

</head>

<body>
    <div id=’awal1’>
    </div>
</body>

</html>
```
Berdasarkan kode tersebut di atas, jika gambar aslinya berukuran 60px x 60px dan ukuran background yang digunakan adalah 400px x 600px, maka hasilnya adalah gambar tersebut ditampilkan berulang-ulang dalam bidang latar belakang berukuran 400px x 600px. Agar terlihat rapi, dapat menggunakan property background repeat guna mengatur perulangan kode. Dalam hal ini, terdapat 4 nilai yang dapat dimasukkan dalam property background-repeat, yaitu no-repeat, repeat, repeat-y, dan repeat-x.

1) No-repeat yang berarti menghilangkan perulangan.

2) Repeat adalah memberikan perulangan.

3) Repeat-x yaitu memberikan perulangan pada sumbu x (horizontal).

4) Repeat-y adalah atribut yang memberikan perulangan pada sumbu y (vertical). Adapun listing dalam kode CSS  digunakan untuk menghilangkan perulangan pada sumbu x dan sumbu y, sehingga atribut nama (komp_mm.jpg) hanya ditampilkan satu kali saja, maka penerapannya sebagai berikut.

 ```css
#awal {
    background-image: url(komp_mm.jpg);
    background-repeat: no-repeat;
    Height: 400px;
    width: 600px;
}
```