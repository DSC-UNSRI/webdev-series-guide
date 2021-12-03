---
title: 04 - Hyperlink
---

## Link

Seringkali kita saat membuat suatu dokumen memberikan sumber referensi seperti buku, jurnal, ataupun website, pada HTML
apabila kita ingin mengarahkan pengguna website pada situs yang kita inginkan, kita bisa menggunakan HyperLink.

```html
<a href="https://www.instagram.com/gdsc.unsri/" target="_blank">Lihat Instagram GDSC UNSRI</a>
```

Output :

[Lihat Instagram GDSC UNSRI](https://www.instagram.com/gdsc.unsri/)

Kode diatas merupakan contoh dari penggunaan HyperLink dengan menggunakan elemen `<a></a>`. Selanjutnya kita perlu
mendefinisikan situs yang ingin dituju dengan atribut `href`, dan selanjutnya atribut `target` digunakan sebagai aksi
saat kita menekan link tersebut apakah dibuka di tab sekarang, membuat tab baru, atau membuat tab pada window baru.

Varian nilai dari atribu `target` :

- _self, apabila kita tidak menuliskan atribut target, maka secara default akan membuka situs pada tab saat ini.
- _blank, membuka situs pada tab baru.

## Absolut URLs vs Relatif URLs

Contoh link diatas merupakan contoh dari Absolut URLs, karena merupakan **alamat lengkap** dari suatu website.
Seringkali kita ingin menampilkan halaman dari folder kita sendiri, kita bisa menggunakan Relatif URLs.

Misalkan kita memiliki struktur project seperti berikut :

```
project-folder
|   README.md
|
└───html
│   │   01-introduction.html
│   │   05-link.html
│   │
│   └───test-link
|       |   hello-world.html
```

Apabila kita berada pada file `05-link.html` dan ingin mengarahkan sebuah teks pada halaman `hello-world.html`, kita
bisa mengakses nya seperti berikut :

```html
<!--05-link.html-->
<a href="test-link/hello-world.html">Klik untuk pindah ke halaman hello-world</a>
```

dan apabila kita ingin kembali kehalaman `05-link.html`, kita bisa melakakukan seperti berikut :

```html
<!--hello-world.html-->
<a href="../html/05-Link.html">Klik untuk kembali ke halaman 05-Link</a>
```

Sintaks `../` digunakan untuk keluar dari folder atau naik satu tingkat folder.