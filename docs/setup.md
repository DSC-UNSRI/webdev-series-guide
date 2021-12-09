---
sidebar_position: 2
id: setup
title: Instalasi Editor
---

# Instalasi Editor

Proses pembuatan website akan lebih maksimal jika didukung oleh editor atau IDE yang pas. Ada cukup banyak pilihan bagus
yang bisa dipertimbangkan, diantaranya: Visual Studio Code, JetBrains WebStorm, Atom, Sublime Text, dan lainnya.

Kami sarankan untuk memilih editor yang paling nyaman digunakan, preferensi masing-masing pastinya berbeda. Kami sendiri
lebih sering menggunakan Visual Studio Code. Editor ini sangat ringan, mudah didapat, dan memiliki ekstensi yang bagus
untuk mendukung pembuatan website. Jika pembaca ingin menggunakan editor yang sama, maka silakan melanjutkan panduan
berikut.

## Instalasi Editor Visual Studio Code

1. Download Visual Studio Code di [https://code.visualstudio.com/download](https://code.visualstudio.com/download),
   pilih sesuai dengan sistem operasi yang digunakan.
2. Jalankan _installer_.
3. Setelah selesai jalankan editornya.

![Visual Studio Code](/img/instalasi/instalasi-vscode.png)

## Settings

Ada beberapa konfigurasi yang dibutuhkan pada Visual Studio Code agar kita lebih merasa nyaman saat menuliskan kode,
untuk membuka setting kita bisa membuka pada tab atas bagian file lalu preferences (atau bisa langsung
menekan `ctrl + comma`) pada keyboard.

### 1. Word Wrap

![Word-Wrap](/img/instalasi/word-wrap-min.png)

Buka settings, lalu cari word wrap dan ubah word wrap menjadi `on`, artinya visual studio code akan otomatis memformat
lebar kode kita sesuai dengan lebar layar kita, sehingga kita tidak perlu scroll kesamping lagi apabila kode terlalu
panjang.

### 2. Format on Save

Buka settings, lalu cari format on save dan ubah menjadi true atau centang. Konfigurasi ini berguna pada saat kita
melakukan save, kode kita akan otomatis diformat.

![Format on Save](/img/instalasi/format-on-save-min.png)

### 3. Tab Size

Buka settings, lalu cari Tab Size dan ubah menjadi angka 2.

## Ekstensi

Visual Studio Code memiliki sangat banyak ekstensi yang bisa di unduh, ekstensi akan memudahkan kita dalam proses coding
nantinya. Kamu bisa mengunduh ekstensi-ekstensi pada navigasi sebelah kiri bagian **Exstension**.Berikut
ekstensi-ekstensi yang sering digunakan pada pembuatan website :

### 1. Prettier

![Prettier](/img/instalasi/Prettier-min.png)

Ekstensi prettier akan membantu kita dalam memformat atau merapihkan kodingan kita. Setelah melakukan penginstallan,
selanjutnya ada beberapa pengaturan yang harus diterapkan

![Prettier](/img/instalasi/prettier-setting-min.png)

Buka settings pada tab atas bagian file lalu preferences (atau bisa langsung menakan `ctrl + comma`) lalu
ketikkan `Default Formatter` dan pilih `prettier`.

### 2. Live Server

Ekstensi ini berfungsi sebagai auto-refresh website kita setiap kita melakukan perubahan pada kode.