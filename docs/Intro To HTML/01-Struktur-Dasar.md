---
title: 01 - HTML Intro
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

## Elemen Utama dalam Struktur HTML
Dalam pembuatan susunan web biasanya terdapat elemen struktur untuk memudahkan pembacaan kode website, seperti untuk menandakan bagian kepala konten website, hingga bagian bawah pada halaman web.

```html
<body>
    <header>
        <nav></nav>
    </header>
    <main></main>
    <footer></footer>
</body>
```

1. `<header></header>` tag header digunakan representasi dari bagian atas pada sebuah website, biasanya berisi link, elemen heading `<h1> - <h6>`.
2. `<nav></nav>` tag nav berfungsi untuk membungkus tag link atau anchor `<a>`.
3. `<main></main>` tag unik yang menjadi bagian utama dari sebuah website.Hampir sebagian besar isi website berada pada tag ini.
**Note** : Konten di dalam elemen `<main>` harus unik, tidak dianjurkan untuk menempatkan tag atau elemen yang berulang seperti sidebar, navbar atau form pencarian.
4. `<footer></footer>` tag yang mempresentasikan bagian akhir dari sebuah website, biasanya berisi : *informasi kontak*, *informasi copyright*, *sitemap* dan informasi yang berikaitan dengan website.
   
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

## Image
```html
<img src='logo.png' alt='Tag ini akan menghasilkan gambar' />
```