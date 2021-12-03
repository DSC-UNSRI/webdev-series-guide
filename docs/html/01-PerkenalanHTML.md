---
sidebar_position: 1
title: 01 - Perkenalan HTML
---

# Apa itu HTML

HTML (**H**yper**T**ext **M**arkup **L**anguage) adalah sebuah bahasa _markup_ yang digunakan developer web untuk
membuat struktur dan mendeskripiskan konten dari sebuah halaman website. HTML terdiri dari elemen yang menjelaskan
berbagai jenis konten: paragraf, tautan, judul, gambar, video, dll.

Dalam HTML semua sintaks tidak _case-sensitive_ (tidak peduli huruf besar atau kecil).

## Struktur Dasar HTML
HTML memiliki struktur dasar yang digunakan yaitu sebagai berikut :
```html
<!DOCTYPE html>
<html>
<head>
    <title>WebDev Series</title>
</head>
<body>
    <p>Halo GDSC UNSRI !</p>
</body>
</html>
```

1. `<!DOCTYPE html>` mewakili jenis dokumen, dan membantu browser untuk menampilkan halaman web dengan benar.
Tag tersebut hanya boleh muncul sekali, di bagian atas halaman (sebelum tag HTML apa pun).
2. `<html></html>` merupakan tag pembungkus konten pada web browser.
3. `<head></head>` merupakan tag pembungkus semua konten yang terdapat pada tab browser, seperti judul halaman.
4. `<body></body>` merupakan tag yang dimana semua konten seperti tulisan, gambar diletakkan.

## Elemen HTML
HTML terdiri dari kumpulan-kumpulan elemen. Contoh elemen :
```html
<h1>Halo Dunia!</h1>
```

Elemen pada html terdiri dari beberapa tag
1. `<h1>` Tag pembuka, merupakan nama dari suatu elemen, dibungkus oleh < dan >
2. `Halo Dunia!` Konten, merupakan isi konten dari suatu elemen, contohnya bisa seperti teks, ataupun elemen lagi (bersarang)
3. `</h1>` Tag penutup, sama seperti tag pembuka, tapi dengan tambahan /(slash).