---
title: 14 - Flex
---

# Flex

Bertujuan untuk untuk pengaturan layout, posisi dan tampilan dari suatu elemen yang ukurannya belum diketahui atau bernilai dinamis, baik itu merubah tinggi dan lebar, urutan posisi elemen, dan spasi (jarak) diantara elemen tersebut.

Secara garis besar `flex` dibagi menjadi dua :

## 1. Flex Container

Pada bagian ini, `flex container` bertindak sebagai parent.

Contoh implementasi flex container dengan 3 flex items :

```html
<div class="flex-container">
  <div>box 1</div>
  <div>box 2</div>
  <div>box 3</div>
</div>
```

### Jenis- jenis Properti Flex Container

### A. Display

Menentukkan container untuk flex apakah `inline-flex` (inline) atau `flex` (block). Inilah yang mendasari sebuah elemen akan memiliki sifat flex atau tidak.

```css
.flex-container {
  display: flex; /* atau inline-flex*/
}
```

### B. Flex-direction

Digunakan untuk mengatur arah alur dari items yang ada di dalam container. Terdapat 4 jenis value dari properti ini, yaitu :

- `column` : secara vertikal (dari atas ke bawah)
- `column-reverse` : secara vertikal (tetapi dari bawah ke atas)
- `row` : secara horizontal (dari kiri ke kanan)
- `row-reverse` : secara horizontal (tetapi dari kanan ke kiri)

Contoh pengaplikasian :

```css
.flex-container {
  display: flex;
  flex-direction: column;
}
```

### C. Flex-wrap

`flex-wrap` digunakan untuk mendefinisikan bahwa elemen item di dalam container flexbox tidak harus disejajarkan dalam satu baris. Artinya, elemen item tersebut dibungkus (dipindahkan) ke baris baru bila sudah memenuhi lebar container-nya. Terdapat 3 jenis value dari properti ini, yaitu :

- `wrap` : item flex akan dibungkus jika perlu
- `nowrap` : item flex tidak akan dibungkus (default)
- `wrap-reverse` : item flex akan dibungkus jika perlu, dalam urutan terbalik

Contoh Pengaplikasian :

```css
.flex-container {
  display: flex;
  flex-wrap: wrap;
}
```

### D. Flex-flow

`flex-flow` merupakan singkatan dari properti `flex-direction` dan `flex-wrap`.

Contoh Pengaplikasian :

```css
.flex-container {
  display: flex;
  flex-flow: row wrap;
}
```

### E. Justify-content

Properti ini digunakan untuk menyelaraskan setiap item flex yang berada di dalam container, agar container tersebut bisa mendistribusikan ruang kosong yang tersisa ketika item flex dalam satu baris tersebut tidak flexsibel atau meskipun flexsibel tapi sudah mencapai batas ukuran maksimum. Terdapat 5 jenis value dari properti ini, yaitu :

- `flex-start` : item flex diselaraskan di awal container (default)
- `center` : item flex diselaraskan di tengah container
- `flex-end` : item flex diselaraskan di akhir container
- `space-around` : item flex didistribusikan secara merata di dalam container dengan space/ruang yang sama diantara item
- `space-between` : item flex didistribusikan secara merata di dalam container, item pertama ada di garis awal dan item terakhir di garis akhir

Contoh Pengaplikasian :

```css
.flex-container {
  display: flex;
  justify-content: flex-start;
}
```

### F. Align-items

`Align-items` hampir sama dengan konsep `justify-content` hanya saja pada align-items, item-item flex diatur secara vertikal. Terdapat 5 jenis value dari properti ini, yaitu :

- `flex-start` : menyelaraskan item di bagian atas container
- `center` : menyelaraskan item di tengah container
- `flex-end` : menyelaraskan item di bagian bawah container
- `baseline` : menyelaraskan item seperti garis dasar mereka sejajar
- `stretch` : meregangkan item untuk mengisi container (default)

Contoh pengaplikasian :

```css
.flex-container {
  display: flex;
  height: 200px;
  align-items: stretch;
}
```

### G. Align-content

Algin-content memadukan konsep `align-items` dan `justify-content` dimana antar items menggunakan konsep `align items` dan antar line menerapkan konsep `justify-content`. Property `align-content` tidak dapat diterapkan jika item-item flex hanya terdiri dari satu line saja. Terdapat 6 jenis value dari properti ini, yaitu :

- `flex-start` : baris dimulai dari awal container
- `center` : baris yang diletakkan pada tengah container
- `flex-end` : baris dimulai dari akhir container
- `space-around` : baris merata didistribusikan dengan ruang yang sama di sekitar setiap baris
- `space-between` : baris terdistribusi merata, baris pertama ada di awal container sementara yang terakhir ada di akhir container
- `stretch` : baris peregangan untuk mengambil ruang yang tersisa

Contoh pengaplikasian :

```css
.flex-container {
  display: flex;
  height: 600px;
  flex-wrap: wrap;
  align-content: space-between;
}
```

## 2. Flex Items

Merupakan item atau content yang ada dalam sebuah flex container maka dinamakan sebagai flex item.

### Jenis- jenis Properti Flex Item

### A. Order

Properti `order` digunakan untuk mengatur urutan dari item flex, secara default nilai order adalah 1. Namun kita dapat menyesuaikan nilai tersebut sesuai dengan kebutuhan kita..

Contoh implementasi :

```html
<div class="flex-container">
  <div style="order: 2">box 1</div>
  <div style="order: 4">box 2</div>
  <div style="order: 3">box 3</div>
  <div style="order: 1">box 4</div>
</div>
```

### B. Flex-grow

`Flex-grow` mendefinisikan kemampuan item flex untuk bertambah ukurannya jika memungkinkan ukuran pada container yang tersedia.

Contoh implementasi :

```html
<div class="flex-container">
  <div style="flex-grow: 0">box 1</div>
  <div style="flex-grow: 1">box 2</div>
  <div style="flex-grow: 2">box 3</div>
  <div style="flex-grow: 3">box 4</div>
</div>
```

**Note :** flex-grow hanya berlaku pada container flex dan tidak dapat digunakan pada nilai inline-flex.

### C. Flex-shrink

Kebalikan dari `flex-grow`, `flex-shrink` memiliki kemampuan untuk melakukan penyusutan/pengurangan ukuran item flex jika ukuran container flex tidak mencukupi.

Contoh implementasi :

```html
<div class="flex-container">
  <div>box 1</div>
  <div style="flex-shrink: 2">box 2</div>
  <div style="flex-shrink: 4">box 3</div>
  <div>box 4</div>
  <div>box 5</div>
</div>
```

### D. Flex-basis

`Flex-basis` digunakan untuk mengatur ukuran lebar dari item flex atau sama dengan properti `width`.

Contoh implementasi :

```html
<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div style="flex-basis: 200px">3</div>
  <div>4</div>
</div>
```

### E. Flex

Properti ini merupakan shorthand atau singkatan untuk properti `flex-grow`, `flex-shrink` dan `flex-basis`.

Contoh implementasi :

```html
<div class="flex-container">
  <div>1</div>
  <div style="flex: 0 1 200px">2</div>
  <div>3</div>
  <div>4</div>
</div>
```

### F. Align-self

Align-self berfungsi untuk menentukan perataan untuk item yang dipilih di dalam container flex. Value pada `align-self` sama dengan yang ada pada `align-items`. Namun ini akan lebih spesifik berakibat pada item flex tertentu saja.

Contoh implementasi :

```html
<div class="flex-container">
  <div style="align-self: flex-start">1</div>
  <div style="align-self: center">2</div>
  <div style="align-self: flex-end">3</div>
  <div>4</div>
</div>
```

**Note :** Penggunaan float, clear dan vertical-align tidak berlaku pada flex item.
