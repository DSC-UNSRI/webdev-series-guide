---
title : 04 - Color CSS
---

# Color CSS

Disini kita akan membahas salah satu *property* yang berada di CSS yaitu `color`.

## Mengenal Teori Warna
Sebelum menggunakan properti `color` ada baiknya kita mengenal sedikit tentang *Teori Warna*. Teori ini merupakan pedoman yang kita pakai untuk menyampaikan pesan kepada *user*. Teori ini mengajarkan bahwa dalam memilih warna, kita harus selektif terhadap kebutuhan *user* kita. Misalkan *user* kita ingin membangun sebuah website untuk kedai kopinya tentu kita perlu menggunakan warna gelap atau *monokrom* agar menggambarkan filosofi kopi yang terkandung didalam-nya. Jadi selalu cari tahu ya, apa warna yang cocok untuk web yang akan kita buat.

## Menuliskan Properti Color
Sama seperti properti lain kita dapat menggunakan properti `color` dengan Metode *Inline*,*Internal* atau *Eksternal* CSS.

### 1. Metode Inline
Memasukkan-nya secara langsung kedalam `tag` HTML.
```html
    <p style = "color : red">Selamat Datang di Event ini</p>
```
### 2. Metode Internal
Bisa juga kita masukkan dibagian `head` HTML.
```html
    <head>
        <style>
            h3 {
                color: black;
            }
        </style>
    </head>
```
### 3. Metode Eksternal
Terakhir dengan menghubungkan file CSS dan HTML.
```css
    /*Ini Berada di file berbeda*/
    h3 {
        color : green;
    }
```

## Mendefinisikan Jenis Nilai Color
Banyak cara untuk menentukan nilai *property* `color` didalam CSS. Tidak hanya dengan menggunakan nama warna yang ingin kita gunakan.Berikut jenis nilai yang bisa kita gunakan. *Jangan lupa dicoba ya!*

### 1. Color Keywords
Ini merupakan cara yang biasa kita pakai, hanya perlu menuliskan nama warna yang kita inginkan.
```css
    h3 {
        color : green;
    }
```

### 2. RGB (Red Green Blue)
Jenis nilai ini menggunakan angka mulai dari 0-255 atau persen 0%-100% untuk menentukan hasil warna yang ingin kita dapatkan. Nilai 0 atau 0% berarti tidak ada warna yang digunakan dan Nilai 255 atau 100% berarti seluruh warna digunakan. Warna disini hanya Merah, Hijau dan Biru, warna lain dihasilkan dari penggabungan ketiga warna ini.
```css
    h3 {
        color : rgb(255,0,0); /*Warna Merah*/
    }
    h4{
        color: rgb(0,255,0);  /*Warna hijau*/
    }
    h5{
        color : rgb(0,0,255); /*Warna Biru*/
    }
```

### 3. RGBA (Red Green Blue Alpha)
Hampir sama seperti jenis nilai *RGB*, namun nilai ini memiliki tambahan satu nilai lagi yaitu nilai ***alpha channel***. Nilai alpha ini mendefinisikan transparansi dari nilai *RGB* yang telah kita masukkan. Dengan jangkuan nilai 0-1 atau 0%-100%. Semakin besar nilai, semakin jelas warna tersebut dan *vice versa*.
```css
    h3 {
        color :  rgba(0,255,0,0.5); /*Warna Hijau Pudar*/
    }
    h4{
        color : rgba(0,255,0,1);    /*Warna hijau Cerah*/
    }
```

### 4. HSL (Hue Saturation Lightness)
Nilai ini jarang digunakan namun penting untuk kalian yang ingin bereksperimen dengan penyesuaian warna atau gradasi. Nilai *Hue* digunakan untuk menentukan warna dan didefinisikan menggunakan derajat, lalu untuk nilai *Saturation* kita pakai untuk mengatur Intensitas warna,serta *Lightness* yang berguna untuk menentukan tingkat kecerahan warna, kedua nilai ini ditentukan dalam persen.
```css
    h3 {
        color :  hsl(240, 100%, 50%); /*Warna Biru*/
    }
    h4{
        color :  hsl(270,100%,50%);   /*Warna Ungu*/
    }
```

### 5. HSLA (Hue Saturation Lightness Alpha)
Untuk nilai ini cara kerjanya sama seperti *RGBA* terhadap *RGB* yaitu untuk menentukan transparansi sebuah warna, apakah jelas atau samar. Jangkauan nilainya pun sama yaitu 0-1 atau 0%-100%.
```css
    h3 {
        color :  hsla(270, 100%, 50%,1); /*Warna Ungu Jelas*/
    }
    h4{
        color :  hsla(270,100%,50%,0.3);  /*Warna Ungu Samar*/
    }
```

### 6. Hexadecimal Color Values
Jenis nilai yang paling sering digunakan dalam menentukan warna di CSS, *Hexadecimal* menggunakan enam nilai untuk menampilkan warna yang kita inginkan. Ke-enam nilai ini mempresentasikan warna Merah,Hijau dan Biru masing-masing warna mewakili dua nilai.
```css
    h3 {
        color : #00ff00; /*Warna Hijau*/
    }
    h4{
        color : #df0090;  /*Warna Pink*/
    }
```

## Memilih Nilai Color
Nah setelah mencoba nilai-nilai color yang ada, kalian jangan pusing memikirkan jenis nilai color mana yang seharusnya kita pakai.  Jenis-jenis ini ditunjukkan, hanya agar kalian dapat mengetahui dan memahami jenis nilai color ini. Cukup gunakan jenis nilai color yang sering dipakai seperti* Color Keywords*, *RGB* atau *Hexadecimal Color Values*.