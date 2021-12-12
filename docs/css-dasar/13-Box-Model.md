---
title : 13 - Box Model 
---

# Box Model

*Box model itu apaan sih? Bukan maksudnya model di dalam box ya!*

## Apa itu Box Model? 
Box model adalah elemen yang membungkus konten HTML yang kita buat. Elemen ini terdiri dari beberapa bagian yaitu `margin`, `padding`, `border`, dan `content`.

*Mengapa harus dibungkus?*

Mari kita lihat ilustrasi berikut!

Ini tampilan HTML yang belum diberi Box Model:

![Tampilan sebelum di Box Model](/img/css/Sebelumboxmodel.png)

Lalu, jika sudah diberi Box Model, kira-kira akan menjadi seperti ini:

![Setelah diberi Box Model](/img/css/after.png)

*Terlihat perbedaannya ya, kan?*

## Struktur dan Pengertian Properti Box Model

### 1. Gambar Struktur Box Model

![Struktur](/img/css/Boxmodel.png)

### 2. Pengertian Setiap Properti Box Model

**Content** merupakan gambar atau tulisan yang dibuat untuk ditampilkan. Biasa dibuat di halaman HTML. Content yang akan dibungkus dalam Box Model biasa akan diberi tag `<div></div>`.

```html
<html>
    <head> 
    <title>
    Let's Practise!
    </title>
    </head>
    <body>
        // Di bawah ini adalah content
        <div> <h1>  Hello World! </h1> </div>
    </body>
</html>
```

**Margin** merupakan ruang atau spasi antara satu elemen dengan elemen lainnya. Margin bersifat transparan sehingga antar elemen tidak saling menempel.
```css
div {
    margin: 20px;
}
```
Kita juga bisa memilih margin mana yang mau kita atur dengan menambahkan `-top`, `-bottom`, `-left`, atau `-right`.
```css
div {
    margin-top: 20px;
    margin-left: 10px;
}
```

**Border** merupakan garis tepi atau garis pembatas yang memisahkan elemen kita dengan sekelilingnya. Kita bisa mengatur warna, ketebalan, dan jenis garis yang digunakan. Strukturnya `border: ketebalanpx warna jenis;`

```css
div {
    border: 5px red solid;
}
```

**Padding** merupakan ruang kosong transparan yang berada di sekeliling konten. Hal ini membuat konten tampak lebih rapi dan tidak menempel dengan bordernya.

```css
div {
    padding: 20px;
}
```
Sama seperti margin, kita juga bisa memilih padding mana yang mau diatur dengan menambahkan `-top `, `-bottom`, `-left`, atau `-right`.

```css
div {
    padding-top: 20px;
    padding-bottom: 5px;
}
```



## Mengatur Ukuran Box Model

Mengatur ukuran Box Model bisa banget dilakukan dengan menggunakan properti `width` dan `height`

```css
div {
    width: 50px;
    height: 35px;
}
```

## Contoh Kode Lengkap

Kita beri contoh kode untuk menampilkan tampilan yang ada di atas tadi ya..

```html
<html>
    <head>
        <title> Test </title>
        <link rel = "stylesheet" href = "style.css">
    </head>
    <body>
        
        <div>
            <h1> Hi, Folks! </h1>
            <h3> Welcome to GDSC Sriwijaya University </h3>
        </div>

    </body>
</html>
```

```css
div {
    background-color: antiquewhite;
    width: fit-content;
    padding: 30px;
    margin: 50px;
    border: red solid;
}
```


