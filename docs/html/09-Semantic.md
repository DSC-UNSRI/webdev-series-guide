---
title: 09 - Semantic
---

# Semantic Tag

Tag semantik adalah tag yang berfungsi seperti `<div>` dan `<span>` namun lebih mendefinisikan
kegunaannya. Berikut adalah beberapa tag-tag semantik :

## Tag `<nav>`

Tag `<nav>` biasanya digunakan sebagai pembungkus bar navigasi atau set navigasi.

Ingat bahwa tidak seluruh set/link navigasi harus berada pada tag ini, hanya beberapa yang penting saja seperti
halnya yang ada pada navbar suatu website.

```html
<nav>
    <a href="/html/">HTML</a> |
    <a href="/css/">CSS</a> |
    <a href="/js/">JavaScript</a> |
    <a href="/jquery/">jQuery</a>
</nav>
```

## Tag `<header>`

Tag `<header>` biasanya digunakan sebagai pembungkus yang mendefinisikan konten berupa pengenalan atau set navigasi.

Tag ini biasa digunakan untuk menaruh tag heading (`<h1>` sampai `<h6>`), logo/gambar yang berkaitan dengan website,
atau informasi yang berkaitan dengan kepemilikan website. 

> `<header>` dapat diletakkan berulang kali, namun tidak dapat diletakkan didalam tag `<footer>`, `<address>`, atau tag `<header>` itu sendiri

Contoh penggunaan :

```html
<header>
    <h1>What Does WWF Do?</h1>
    <p>WWF's mission:</p>
</header>
```

## Tag `<main>`

Tag `<main>` digunakan sebagai pembungkus dari konten utama suatu website.

Contoh penggunaan :

```html
<main>
    Your entire main content here.
</main>
```

## Tag `<section>`

Tag `<section>` biasanya digunakan sebagai pembungkus yang mendefinisikan suatu bagian website.

Tag ini biasa digunakan untuk bagian intro dari suatu website, chapter-chapter suatu post, informasi kontak, dan lain-lain.

Contoh penggunaan :

```html
<section>
    <h1>WWF</h1>
    <p>The World Wide Fund for Nature (WWF) is an international organization working on issues regarding the conservation, research and restoration of the environment, formerly named the World Wildlife Fund. WWF was founded in 1961.</p>
</section>

<section>
    <h1>WWF's Panda symbol</h1>
    <p>The Panda has become the symbol of WWF. The well-known panda logo of WWF originated from a panda named Chi Chi that was transferred from the Beijing Zoo to the London Zoo in the same year of the establishment of WWF.</p>
</section>
```

## Tag `<article>`

Tag `<article>` digunakan sebagai pembungkus suatu artikel yang berupa konten yang independen dan berdiri sendiri.

Penggunaan tag ini haruslah masuk akal, dan haruslah mungkin agar tag ini dapat disebarkan secara independen dari seisi website.

Tag ini biasa digunakan untuk menandai post forum, post suatu blog, komen dari user, artikel koran online, dan sebagainya.

Contoh penggunaan :

```html
<article>
    <h2>Google Chrome</h2>
    <p>Google Chrome is a web browser developed by Google, released in 2008. Chrome is the world's most popular web browser today!</p>
</article>

<article>
    <h2>Mozilla Firefox</h2>
    <p>Mozilla Firefox is an open-source web browser developed by Mozilla. Firefox has been the second most popular web browser since January, 2018.</p>
</article>

<article>
    <h2>Microsoft Edge</h2>
    <p>Microsoft Edge is a web browser developed by Microsoft, released in 2015. Microsoft Edge replaced Internet Explorer.</p>
</article>
```

## Tag `<aside>`

Tag `<aside>` digunakan untuk menandai elemen yang ada disamping konten dimana ia diletakkan (biasanya berguna untuk mendefinisikan sidebar).

Tag ini haruslah secara tidak langsung berhubungan dengan konten yang dimaksud.

Contoh penggunaan :

```html
<p>My family and I visited The Epcot center this summer. The weather was nice, and Epcot was amazing! I had a great summer together with my family!</p>

<aside>
    <h4>Epcot Center</h4>
    <p>Epcot is a theme park at Walt Disney World Resort featuring exciting attractions, international pavilions, award-winning fireworks and seasonal special events.</p>
</aside>
```

## Tag `<figure>` dan `<figcaption>`

Tag `<figure>` berfungsi sebagai penanda untuk konten yang berdiri sendiri seperti gambar, diagram, foto, dan lain sebagainya. Tag
ini memiliki pasangan berupa `<figcaption>` yang digunakan untuk memberikan suatu caption ke konten yang dibungkus oleh tag `<figure>`.

Contoh penggunaan :

```html
<figure>
    <img src="pic_trulli.jpg" alt="Trulli">
    <figcaption>Fig1. - Trulli, Puglia, Italy.</figcaption>
</figure>
```

## Tag `<footer>`

Tag `<footer>` berfungsi sebagai penanda bagian akhir suatu website yang biasanya berada di posisi paling bawah dari suatu website.

Tag ini dapat digunakan untuk menampung informasi kepemilikan, informasi copyright, informasi kontak, sitemap, tombol *kembali ke atas*,
dokumen terkait, dan sebagainya.

Contoh penggunaan :

```html
<footer>
    <p>Author: Hege Refsnes</p>
    <p><a href="mailto:hege@example.com">hege@example.com</a></p>
</footer>
```