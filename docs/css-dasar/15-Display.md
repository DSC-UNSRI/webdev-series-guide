---
title : 15 - Display
---

# Display

Properti `display` menentukan perilaku tampilan dari suatu elemen.
Dalam HTML, nilai properti tampilan default diambil dari spesifikasi HTML *default* browser pengguna. Nilai *default* dalam XML adalah inline, termasuk elemen SVG.

## Jenis Display

Untuk `display` sendiri terdiri dari beragam *value*, berikut beberapa *value* dari *property* ini yang akan kita bahas : 

- **block**
- **inline**
- **inline-block**

Selanjutnya, mari kita bahas satu persatu ketiga jenis display ini agar lebih paham terkait penggunaan-nya.

### Block

Elemen yang menggunakan nilai ***block*** akan dimulai pada baris baru dan menggunakan lebar layar yang tersedia. Anda dapat menentukan properti lebar dan tinggi untuk elemen tersebut. Contoh elemen yang berada di level *block* secara *default* adalah `<div>`, `<section>`, `<p>`, dan banyak lagi. Kita dapat memberikan nilai *block* kepada element yang tidak menggunakan-nya, seperti element `span` yang secara *default* menggunakan nilai ***inline***;

```css
span {
    display : block; 
}
```

### Inline

Berbeda dengan nilai **block** yang mengambil seluruh lebar layar, nilai ***inline*** tidak akan dimulai pada baris baru dan akan mengambil lebar layar yang tersisa/tersedia. nilai ini hanya mengambil ruang secukupnya saja. Sama seperti sebelum-nya kita dapat mendefinisikan nilai ini ke element lain-nya.

```css
div{
    display:inline;
}
.header{
    display:inline;
}
```
Namun perlu diingat bahwa nilai *inline* ini tidak dapat diatur lebar (*width*) dan tinggi-nya (*height*).

### Inline-block

Tipe nilai ini bisa dibilang sebagai penyempurnaan tipe nilai `display` ***inline*** sebelumnya, Mengapa ? Karena nilai ini dapat mengatasi kelemahan yang ada pada tipe ***inline***, nilai ***inline-block*** ini dapat diatur lebar dan tinggi-nya, yang tidak dapat kita lakukan ketika elemen diberi tampilan ***inline***.

```css
div{
    display:inline-block;
}
.main{
    display:inline-block;
}
```
Jadi, Anda bisa melihat tampilan ***inline-block*** sebagai gabungan nilai ***inline*** dan nilai ***blok*** dalam satu paket.



