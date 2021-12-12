---
title: 10 - Position
---

# Position

Terdapat beberapa cara untuk memanipulasi posisi suatu elemen dalam CSS.

## Static

Position `static` adalah posisi default dari suatu elemen yang tidak dipengaruhi oleh atribut `top`, `left`, `right`, dan `bottom`.
Posisi ini tidak menempatkan elemen dengan cara yang spesial. Posisinya pun mengikuti alur halaman.

Contoh implementasi :

```css
div.static {
  position: static;
  border: 3px solid #73AD21;
}
```

## Relative

Position `relative` adalah posisi dimana elemen diposisikan relatif dari posisi normalnya.
Atribut `top`, `left`, `right`, dan `bottom` akan memengaruhi elemen yang mempunyai atribut posisi ini dan akan diatur menjauhi posisi normalnya.

Contoh implementasi :

```css
div.relative {
  position: relative;
  left: 30px;
  border: 3px solid #73AD21;
}
```

## Fixed

Position `fixed` adalah posisi dimana elemen diposisikan relatif dari viewport yang berarti elemen yang berada dalam posisi ini tidak akan bergerak bahkan jika halaman discroll.
Posisi ini tidak akan meninggalkan bidang kosong pada posisi normalnya dimana elemen diletakkan sesuai dengan tempatnya di alur halaman.
Atribut `top`, `left`, `right`, dan `bottom` akan memengaruhi elemen yang mempunyai atribut posisi ini.

Contoh implementasi :

```css
div.fixed {
  position: fixed;
  bottom: 0;
  right: 0;
  width: 300px;
  border: 3px solid #73AD21;
}
```

## Absolute

Position `absolute` adalah posisi dimana elemen diposisikan relatif dari parent elementnya.
Jika elemen tersebut tidak mempunyai parent element, maka element body akan dijadikan patokan relatif dari pemposisiannya.
Posisi ini tidak mengikuti alur normal pada halaman dan dapat menutupi elemen lain.

Contoh implementasi :

```css
div.absolute {
  position: absolute;
  top: 80px;
  right: 0;
  width: 200px;
  height: 100px;
  border: 3px solid #73AD21;
}
```

## Sticky

Position `sticky` adalah posisi dimana elemen diposisikan sesuai dengan posisi scroll dari user.
Elemen dengan posisi ini akan bertukar atribut antara `relative` dan `fixed` tergantung dari posisi scroll yang ditentukan.
Posisi ini akan menjadi `relative` jika posisi scroll tidak memenuhi dan akan berganti ke `fixed` jika posisi scroll telah memenuhi.

> Internet Explorer tidak mendukung posisi ini. Safari memerlukan prefix `-webkit-` agar posisi ini bekerja. Anda juga harus mengatur setidaknya satu dari atribut `top`, `left`, `right`, atau `bottom` agar posisi ini bekerja.

Contoh implementasi :

```css
div.sticky {
  position: -webkit-sticky; /* Safari */
  position: sticky;
  top: 0;
  background-color: green;
  border: 2px solid #4CAF50;
}
```
