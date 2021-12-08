---
title : 06 - Pseudo Class
---

# Pseudo Class

PseudoClass digunakan untuk mendefinisikan keadaan khusus suatu elemen, seperti elemen ketika di arahkan mouse, diklik,
dll.

Sintaks PseudoClass :

```css
selector:pseudo-class {
    property: value;
}
```

## Pseudo Class `first-child`

```html

<ul>
    <li>Megumin</li>
    <li>Geeks</li>
    <li>Nolep</li>
</ul>
```

Misalkan kita ingin mengubah warna li yang pertama saja :

```css
ul li:first-child {
    color: #00a4db;
}
```

## Pseudo Class `hover`

```html
<a href="#">Hover Aku!</a>
```

```css
a:hover {
    color: #1a8870;
}
```

## Pseudo Class `active`

```html
<a href="#">Tekan dan Tahan Aku!</a>
```

```css
a:active {
    color: #4b1113;
}
```

## Pseudo Class `visitied`

```html
<a href="instagram.com/gdscunsri">Tekan Aku dan Kembali Lagi!</a>
```

```css
a:visited {
    color: red;
}
```