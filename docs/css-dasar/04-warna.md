---
title : 04 - Warna
---

# Warna

Pada css kita bisa mengubah warna pada teks, shape, ataupun background. Terdapat beragam cara untuk mendifinisikan warna
pada css, bisa dengan nama warna, kode RGB, dan lain-lainya.

## Nama Warna

Ini merupakan cara yang biasa kita pakai, hanya perlu menuliskan nama warna yang kita inginkan. Terdapat banyak warna
yang didukung oleh CSS, kamu bisa melihat warna-warna tersebut pada situs
berikut : [https://www.w3schools.com/colors/colors_names.asp](https://www.w3schools.com/colors/colors_names.asp).

```css
h3 {
    color: green;
}
```

## RGB (Red Green Blue)

Jenis nilai ini menggunakan angka mulai dari 0-255 atau persen 0%-100% untuk menentukan hasil warna yang ingin kita
dapatkan. Nilai 0 atau 0% berarti tidak ada warna yang digunakan dan Nilai 255 atau 100% berarti seluruh warna
digunakan. Warna disini hanya Merah, Hijau dan Biru, warna lain dihasilkan dari penggabungan ketiga warna ini.

```css
h3 {
    color: rgb(255, 0, 0); /*Warna Merah*/
}

h4 {
    color: rgb(0, 255, 0); /*Warna hijau*/
}

h5 {
    color: rgb(0, 0, 255); /*Warna Biru*/
}
```

## RGBA (Red Green Blue Alpha)

Hampir sama seperti jenis nilai *RGB*, namun nilai ini memiliki tambahan satu nilai lagi yaitu nilai ***alpha channel***
. Nilai alpha ini mendefinisikan transparansi dari nilai *RGB* yang telah kita masukkan. Dengan jangkuan nilai 0-1 atau
0%-100%. Semakin besar nilai, semakin jelas warna tersebut dan *vice versa*.

```css
h3 {
    color: rgba(0, 255, 0, 0.5); /*Warna Hijau Pudar*/
}

h4 {
    color: rgba(0, 255, 0, 1); /*Warna hijau Cerah*/
}
```

## Hexadecimal

Jenis nilai yang paling sering digunakan dalam menentukan warna di CSS, *Hexadecimal* menggunakan enam nilai untuk
menampilkan warna yang kita inginkan. Ke-enam nilai ini mempresentasikan warna Merah,Hijau dan Biru masing-masing warna
mewakili dua nilai.

```css
h3 {
    color: #00ff00; /*Warna Hijau*/
}

h4 {
    color: #df0090; /*Warna Pink*/
}
```

## HSL (Hue Saturation Lightness)

Nilai ini jarang digunakan namun penting untuk kalian yang ingin bereksperimen dengan penyesuaian warna atau gradasi.
Nilai *Hue* digunakan untuk menentukan warna dan didefinisikan menggunakan derajat, lalu untuk nilai *Saturation* kita
pakai untuk mengatur Intensitas warna,serta *Lightness* yang berguna untuk menentukan tingkat kecerahan warna, kedua
nilai ini ditentukan dalam persen.

```css
h3 {
    color: hsl(240, 100%, 50%); /*Warna Biru*/
}

h4 {
    color: hsl(270, 100%, 50%); /*Warna Ungu*/
}
```

## HSLA (Hue Saturation Lightness Alpha)

Untuk nilai ini cara kerjanya sama seperti *RGBA* terhadap *RGB* yaitu untuk menentukan transparansi sebuah warna,
apakah jelas atau samar. Jangkauan nilainya pun sama yaitu 0-1 atau 0%-100%.

```css
h3 {
    color: hsla(270, 100%, 50%, 1); /*Warna Ungu Jelas*/
}

h4 {
    color: hsla(270, 100%, 50%, 0.3); /*Warna Ungu Samar*/
}
```