---
title: 06 - Tabel
---

Pada HTML kita juga dapat membuat tabel dengan elemen `<table></table>`.

```html

<table border="1">
    <tr>
        <th>Nama</th>
        <th>Divisi</th>
    </tr>
    <tr>
        <td>Megumin</td>
        <td>Web Development</td>
    </tr>
    <tr>
        <td>Geeks</td>
        <td>Backend Development</td>
    </tr>
</table>
```

Contoh output :

| Nama        | Divisi                  |
| ----------- | -----------             |
| Megumin     | Web Development         |
| Geeks       | Backend Development     |

Sintaks `<table></table>` merupakan deklrasi bahwa kita akan membuat suatu table, dan atribut `border` adalah untuh
menambah garis pada setiap table. Selanjutnya `<tr></tr>` adalah singkatan dari _table row_ yang berfungsi untuk membuat
suatu baris pada tabel. Terakhir ada `<td></td>` atau `<th></th>` yang menandakan kita akan membuat kolom.

## Merge Tabel

Kita dapat melakukan merge antar baris, kolom, ataupun keduanya pada HTML dengan menggunakan colspan dan rowspan.

### Colspan

Jika kita membutuhkan tabel dimana dapat melakukan penggabungan antara kolom satu dengan kolom lainya, kita dapat
menggunakan atribut `colspan`, yang dimana akan melakukan penggabungan antar kolom (horizontal).

```html

<table border="1">
    <tr>
        <th colspan="2">Name</th>
        <th>Age</th>
    </tr>
    <tr>
        <td>Jill</td>
        <td>Smith</td>
        <td>43</td>
    </tr>
    <tr>
        <td>Eve</td>
        <td>Jackson</td>
        <td>57</td>
    </tr>
</table>
```

## Rowspan

Adapun kika ingin melakukan penggabungan antara baris satu dengan baris lainya, kita dapat menggunakan atribut `rowspan`
, yang dimana akan melakukan penggabungan antar baris (vertikal).

```html

<table border="1">
    <tr>
        <th>Name</th>
        <td>Jill</td>
    </tr>
    <tr>
        <th rowspan="2">Phone</th>
        <td>555-1234</td>
    </tr>
    <tr>
        <td>555-8745</td>
    </tr>
</table>
```