---
title : 12 - Fonts CSS
---

# Fonts CSS

Berguna untuk menjelaskan bagaimana sebuah teks akan ditampilkan pada sebuah website, mari Bersama kita mempelajari *
property* `font`.

## Jenis-Jenis Property Fonts

Properti *fonts* sendiri memiliki banyak *property* yang dapat digunakan mulai dari *property* `font-family`
hingga `font`. Jadi mari kita lihat penggunaan dan penjelasan dari masing-masing property ini.

### 1. Property font-family

Properti ini berguna untuk menentukan *font* jenis apa yang ingin kita gunakan. Berikut cara menggunakan properti ini.

```css
.header {
    font-family: 'Arial';
}

.main {
    font-family: 'Open sans';
}
```

`font-family` juga memiliki sistem ***fallback***, sistem ini digunakan untuk menjamin kompabilitas browser terhadap
suatu jenis *font*, sebab terdapat jenis-jenis *font* yang tidak dapat digunakan di web tertentu. Penulisan-nya pun
sederhana cukup tambahkan *font* baru setelah *font* utama. Disarankan untuk menggunakan jenis font *default* yang
dimiliki masing-masing
browser, [Cek Font Default Browser](https://granneman.com/webdev/coding/css/fonts-and-formatting/web-browser-font-defaults)
.

```css
.header {
    font-family: 'Arial', sans-serif;
}

.main {
    font-family: 'Times New Roman', Times;
}
```

### 2. Property font-size

Selain menentukan jenis *font* apa yang ingin kita pakai, kita juga harus menentukan ukuran dari *font* tersebut
menggunakan *property* `font-size`.Properti ini menerima nilai dalam bentuk *pixels (px)*, *percentage (%)*, *vw*, *em*
hingga *rem*.

```css
h1 {
    font-size: 40px;
}

h2 {
    font-size: 10%;
}

h3 {
    font-size: 2em;
}

h4 {
    font-size: 3rem;
}

h5 {
    font-size: 5vw;
}
```

Walaupun tidak terdapat aturan dalam menentukan tipe nilai apa yang ingin kita gunakan. Namun disarankan untuk
mengurangi penggunaan tipe nilai *pixels (px)*. Hal ini dikarenakan sudah ada nilai-nilai *font* seperti *em*,*rem*
dan *vw* yang lebih fleksibel juga *responsive* dalam penggunaanya baik pada layar *desktop* maupun *mobile*.

### 3. Property font-weight

`font-weight` bertugas untuk mengatur ketebalan dari sebuah *font*. Nilai-nya dispesifikasikan dalam teks *lighter*, *
normal*, *bold*, dan *bolder* maupun angka dengan *range* 100-900.

1. *lighter*, membuat teks menjadi sangat halus.
2. *normal*, merupakan ukuran *default* dari teks.
3. *bold*, membuat teks menjadi tebal.
4. *bolder*, membuat teks sangat tebal.

Penggunaan nilai didalam *property* `font-weight` :

```css
h1 {
    font-weight: lighter;
}

h2 {
    font-weight: normal;
}

h3 {
    font-weight: bold;
}

h4 {
    font-weight: bolder;
}

h5 {
    font-weight: 600;
}
```

### 4. Property font-style

Properti `font-style` adalah properti yang kegunaan-nya lebih difokuskan untuk membuat teks menjadi miring. Terdapat 3
Nilai didalam-nya yaitu :

1. *normal*, merupakan nilai default yang akan digunakan jika kita tidak mengubah nilai *property* `font-style`.
2. *italic*, mengubah teks menjadi miring.
3. *oblique*, memiliki fungsi yang sama dengan italic namun tidak disarankan untuk digunakan karena masalah
   kompabilitas.

Pemakaian nilai diatas menggunakan *Property* `font-style` :

 ```css
h1 {
    font-style: normal;
}

h2 {
    font-style: italic;
}

h3 {
    font-style: oblique;
}
```

### 5. Property font-variant

`font-variant` merupakan *property* yang berguna untuk menciptakan efek ***small-caps***, efek ini membuat teks yang
memiliki hutuf kecil menjadi kapital dan huruf kapital menjadi lebih besar. Terdapat 2 nilai yang dapat digunakan
didalam properti ini, yaitu :

1. *normal*, menampilkan teks dalam bentuk normal.
2. *small-caps*, menampilkan teks dengan efek ***small-caps***.

```css
h1 {
    font-variant: normal;
}

h2 {
    font-variant: small-caps;
}
```

### 6. Property font

Properti ini menggunakan metode **Shorthand**. Metode ini berfungsi untuk mempersingkat penulisan dari kelima properti
yang sudah dijelaskan tadi, dengan menggabungkan-nya kedalam satu properti. Berikut cara penulisan properti ini :

```css
h1 {
    font: normal small-caps lighter 2em sans-serif, Arial;
}
```

Untuk lebih mudah dipahami *property* ini, kita baca dari kiri ke kanan secara berurutan :

1. `font-style`
2. `font-variant`
3. `font-weight`
4. `font-size`
5. `font-family`

Jika ada salah satu nilai tidak diisi, maka secara otomatis akan berisi nilai *default* masing-masing *property*.

## Mengimport Font Non-Standard

Dalam penggunaan jenis *font* kita tidak harus selalu menggunakan *font* **default** yang ada didalam browser, kita
dapat mengimport font tersebut kedalam file kita kemudian menggunakan-nya. Jadi disini kita mengimport *font* **
Non-Standard** dari website [Google Font](https://fonts.google.com/). Berikut metode untuk melakukan import *font* :

### 1. Import Metode Internal

Kita dapat menempatkan link *font* **Non-standard** yang telah kita pilih kedalam file HTML.

```html
<!DOCTYPE html>
<html>
<head>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Lato&display=swap" rel="stylesheet">
</head>
<style>
    h1 {
        font-family: 'Lato', sans-serif;
    }
</style>
</html>
```

### 2. Import Metode Eksternal

Atau memasukkan-nya kedalam file CSS kita.

```css
@import url('https://fonts.googleapis.com/css2?family=Lato&display=swap');

h1 {
    font-family: 'Lato', sans-serif;
}
```

## Menggunakan Pasangan Font

Dalam pembuatan website nanti-nya kita pasti akan memakai lebih dari 1 *font*, oleh karena itu kita harus paham mengenai
aturan ***Font Pairing***. Aturan ini memberikan bimbingan pada kita dalam memilih pasangan font yang tepat untuk kita
gunakan agar membuat teks yang ada menjadi menarik untuk dilihat dan dibaca. Mari bersama kita lihat aturan apa saja
yang ada.

### 1. Memasangkan Font Dari Keluarga Yang Sama

Untuk mempermudah kita dalam memilih *font* yang berbeda ada baiknya kita mengetahui Keluarga dari *font* tersebut,
Apakah font-font ini sejenis atau tidak ? Apakah berasal dari Keluarga *font* yang sama ?. Keluarga *font* (*font
family*) yang paling sering digunakan di antaranya :

- [*serif*](https://www.fontsquirrel.com/fonts/list/classification/serif)
- [*sans serif*](https://www.fontsquirrel.com/fonts/list/classification/sans%20serif)
- [*cursive*](https://www.cufonfonts.com/search/cursive)
- [*lucida*](https://lucidafonts.com/)

Dengan mengetahui jenis-jenis *font* yang terdapat didalam-nya, kita dapat mempersempit pilihan dari font-font yang akan
kita gunakan nanti-nya.

### 2. Gunakan Font Yang Saling Kontras

Selalu hindari untuk menggunakan *font* yang terlalu mirip karena akan menimbulkan masalah-masalah yang tidak diingikan,
mulai dari sulit membedakan antara teks yang penting dan tidak hingga membuat user kesulitan membaca pesan yang ingin
anda sampaikan. Jadi sangat disarankan menggunakan font-font yang mudah untuk dibedakan, kombinasi *font family* yang
sering dipakai adalah kombinasi antara *font serif* dan *sans serif*.

### 3. Memilih Font Yang Dominan

Setelah memilih font-font apa yang ingin kita pasangkan, selanjutnya kita akan menentukan *font* mana yang akan
digunakan sebagai *font* dominan. Nantinya Font dominan akan banyak digunakan sebagai *header* dan dibedakan dengan *
font* lainnya melalui ukuran, berat dan kontras warna.

## Memahami Font

*Font* atau huruf berguna untuk memberitahukan kepada user, tentang seberapa penting suatu teks yang ada di website
kita. Kita juga harus memperhatikan jenis *font* yang sedang dipakai, apakah *font* tersebut cocok dengan pesan yang
ingin disampaikan atau tidak. Selain itu, kita juga harus menggunakan *font* yang mudah dibaca. Font yang mudah dibaca
akan menambah nilai pada teks Anda. Penting juga untuk memilih warna dan ukuran teks yang benar pada *font*.



