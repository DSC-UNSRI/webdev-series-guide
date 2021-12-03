---
title: 02 - Text
---

## Heading

HTML headings adalah sebuah tag yang digunakan untuk mendefinisikan judul, atau sub-judul yang ingin ditampilkan pada
sebuah halaman website.

Contoh Heading :
# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6

Terdapat berbagai varian heading yaitu dari `<h1>` sampai `<h6>`.
`<h1>` mendefinisikan hal yang paling penting pertama. `<h6>` mendefiniskan hal yang terpenting terakhir.

```html
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>
```

## Paragraf

```html
<p>Ini adalah paragraf</p>
```

## Format Teks

### Bold

Elemen `<b>` dan `<strong>` pada HTML dapat digunakan untuk menebalkan teks.

```html
<b>Ini adalah teks tebal</b>
<strong>Ini juga teks tebal</strong>
```

### Italic

Elemen `<i>` dan `<em>` pada HTML dapat digunakan untuk memiringkan teks.

```html
<i>Ini adalah teks miring</i>
<em>Ini juga teks miring</em>
```

### Small

Elemen `<small>` pada HTML dapat digunakan untuk mendefinisikan teks yang kecil.

```html
<small>Ini adalah teks kecil</small>
```

### Mark/Highlight

Elemen `<mark>` pada HTML dapat digunakan untuk menghighlight suatu teks.

```html
<p>Kusuka susu, <mark>susu yang murni</mark></p>
```

### Strikethrough

Elemen `<s>` dan `<del>` pada HTML dapat digunakan untuk mencoret suatu teks.

```html
<p>Saya <s>suka menonton anime</s> selalu mengumpul tugas tepat waktu</p>
<p>Saya <del>suka tidur dan malas-malasan</del> rajin membaca dan belajar</p>
```

### Garis Bawah

Elemen `<ins>` dan `<u>` pada HTML dapat digunakan untuk menggarisbawahi suatu teks.

```html
<ins>Ini teks yang digarisbawahi</ins>
<u>Ini juga teks yang digarisbawahi</u>
```

### Subscript dan Superscript

Superscript atau subscript adalah angka, simbol atau indikator yang berukuran lebih kecil dibandingkan dengan teks normal lainnya. Superscript diletakkan sedikit lebih tinggi, sedangkan subscript diletakkan sedikit lebih rendah dari teks normal. HTML menyediakan `<sub>` dan `<sup>` sebagai tag formatting untuk fungsi ini.

```html
<p>H<sub>2</sub>O</p>
<p>x<sup>2</sup> + x + C</p>
```