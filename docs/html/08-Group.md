---
title: 08 - Grouping
---

# Grouping

Ketika kita menuliskan kode HTML dan kita merasa ada elemen-elemen yang saling terikat dan ingin membungkus
elemen-elemen tersebut menjadi sebuah elemen baru, kita bisa menggunakan HTML Grouping. Pada HTML untuk melakukan
grouping, kita bisa menggunakan elemen `<div></div>` atau `<span></span>`.

Contoh tanpa grouping :

```html
<h1>Anggota GDSC UNSRI</h1>
<ul>
    <li>Megumin</li>
    <li>Geeks</li>
</ul>

<p>Terima Kasih</p>
```

Dengan Grouping :

```html

<div>
    <h1>Anggota GDSC UNSRI</h1>
    <ul>
        <li>Megumin</li>
        <li>Geeks</li>
    </ul>
</div>

<p>Terima Kasih</p>
```

Walaupun secara output tidak ada perubahan, akan tetapi dengan grouping kita akan lebih mudah dalam membaca suatu kode.

## Div

Pada elemen div secara default display bernilai block, artinya adalah ketika menggunakan elemen tersebut maka akan
membuat line baru (enter). Pengertian display sendiri nanti akan diperjelas pada materi CSS.

Contoh :

```html
<p>Halo Megumin!
<div>Halo juga Geeks</div></p>
```

Output :
```
Halo Megumin! 
Halo juga Geeks
```

## Span

Pada elemen span memiliki nilai default bernilai inline, artinya adalah ketika menggunakan elemen tersebut maka tidak
akan membuat line baru.

```html
<p>Halo Megumin!<span>Halo juga Geeks</span></p>
```

Output :

```
Halo Megumin! Halo juga Geeks
```