---
title: 07 - Form
---

# Form

Selain konten seperti teks, gambar, atau video, kita juga dapat menerima input dari pengguna melalui formulir. HTML
menyediakan elemen `<form></form>` untuk menerima input dari user seperti text, file, button, dll. Form dikirim ke
alamat yang ditentukan oleh atribut `action`.

## Input

Elemen `<input>` pada HTML adalah elemen yang menjadi rangka untuk form yang ingin dibuat pada HTML. Elemen ini dapat direpresentasikan dengan beberapa cara tergantung dari atribut `type` yang diberikan.

### Penamaan

Setiap elemen input harus dinamai agar dapat dikirim. Penamaan dilakukan dengan atribut `name`. Jika penamaan tidak dilakukan, maka isi dari input tersebut tidak akan dikirim. 

### Label

Elemen `<label>` merepresentasikan label pada suatu input.

> Perlu diingat bahwa elemen ini memerlukan atribut `for` yang berisi sama dengan atribut `id` pada elemen input yang ditunjuk.

### Input Teks

Untuk menginput teks kita menggunakan tipe `text`.

```html
<form>
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname">
</form>
```

### Tombol Radio

Tipe `radio` digunakan untuk merepresentasikan beberapa pilihan dan hanya 1 pilihan yang dapat dipilih.

```html
<form>
  <input type="radio" id="html" name="fav_language" value="HTML">
  <label for="html">HTML</label><br>
  <input type="radio" id="css" name="fav_language" value="CSS">
  <label for="css">CSS</label><br>
  <input type="radio" id="javascript" name="fav_language" value="JavaScript">
  <label for="javascript">JavaScript</label>
</form>
```

### Checkbox

Tipe `checkbox` digunakan untuk merepresentasikan pilihan dan dapat memilih lebih dari 1 pilihan.

```html
<form>
  <input type="checkbox" id="html" name="fav_language" value="HTML">
  <label for="html">HTML</label><br>
  <input type="checkbox" id="css" name="fav_language" value="CSS">
  <label for="css">CSS</label><br>
  <input type="checkbox" id="javascript" name="fav_language" value="JavaScript">
  <label for="javascript">JavaScript</label>
</form>
```

### Password

Tipe `password` digunakan untuk merepresentasikan input yang berupa password. Seluruh teks yang diketikkan pada tipe ini akan disembunyikan.

```html
<form>
  <label for="uname">Username:</label><br>
  <input type="text" id="uname" name="uname"><br>
  <label for="pass">Password:</label><br>
  <input type="password" id="pass" name="pass">
</form>
```

### Tombol Submit

Tipe `submit` biasanya digunakan untuk merepresentasikan tombol submit pada suatu form. Biasanya dilakukan pada elemen `<button>` namun disini kita lakukan dengan elemen `<input>`.

```html
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form>
```