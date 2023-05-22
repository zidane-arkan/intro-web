---
title: 07 - Layout
---

# Layouting dalam HTML

Penggunaan layout mengacu pada cara sebuah elemen-elemen atau tag-tag yang ada digabungkan sehingga menjadi sebuah group yang dapat diatur secara berkelompok.

## Div

Pada elemen div secara default display bernilai block, artinya adalah ketika menggunakan elemen tersebut maka akan
membuat line baru (enter). Pengertian display sendiri nanti akan diperjelas pada materi CSS.

Contoh :

```html
<div>
    <h1>Hello World</h1>
    <p>Salam kepada seluruh dunia</p>
</div>
```

## Span

Pada elemen span memiliki nilai default bernilai inline, artinya adalah ketika menggunakan elemen tersebut maka tidak
akan membuat line baru.

```html
<p>Halo Semua!<span>Halo juga Geeks</span></p>
```

## Section

Tag `<section></section>` biasanya digunakan untuk menandakan bagian umum atau garis besar pada sebuah halaman website.

```html
<section>
    <div>
        <h2>Sejarah Dunia kita Part I</h2>
        <p></p>
    </div>
    <div>
        <h2>Sejarah Dunia kita Part II</h2>
        <p></p>
    </div>
</section>
```

## Article

Merupakan tag yang berdiri sendiri dan biasanya untuk konten yang mandiri.

:::tip Catatan
An article should make sense on its own and it should be possible to distribute it independently from the rest of the site.

Potential sources for the `<article></article>` element:

- Forum post
- Blog post
- News story
:::


```html
<article>
    <h2>Google Chrome</h2>
    <p>Google Chrome is a web browser developed by Google.</p>
</article>

<article>
    <h2>Mozilla Firefox</h2>
    <p>Mozilla Firefox is an open-source web browser developed by Mozilla.</p>
</article>

<article>
<h2>Microsoft Edge</h2>
    <p>Microsoft Edge is a web browser developed by Microsoft.</p>
</article>
```

## Aside
Tag `<aside></aside>` mendefinisikan beberapa konten selain dari konten yang ditempatkan di dalamnya. Biasanya berada di samping sebuah halaman website.

```html
<aside>
    <h4>Epcot Center</h4>
    <h4>Paint Center</h4>
    <h4>Code Center</h4>
</aside>
```