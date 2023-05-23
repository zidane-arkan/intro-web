---
title: 01 - CSS Intro
---

# Perkenalan CSS

## Apa itu CSS ?

Cascading Style Sheets (CSS) adalah bahasa yang digunakan untuk melakukan _styling_ pada dokumen HTML. CSS
mendeskripsikan gaya visual dan memperindah konten yang ditulis pada HTML. CSS terdiri dari banyak properti yang
digunakan pengembang untuk memformat konten seperti properti tentang font, teks, spasi, tata letak, dll.

Contoh Penggunaan CSS :
```css
div {
    background-image: url("image.jpg");
    color : black;
}
```

### Deskripsi
1. `div`, disebut sebagai selector, yang berfungsi sebagai memilih elemen apa yang ingin diubah.
2. `color: black;` merupakan cara penulisan style.
3. `color` dan `background-image` disebut sebagai properti, atau bagian apa yang ingin diubah dari suatu elemen.
4. `black` dan `url("image.jpg")` merupakan value, atau nilai yang diberikan.


## Penempatan CSS

Terdapat berbagai cara untuk meletakkan atau menghubungkan css pada dokumen HTML.

### Inline CSS

Kita dapat meletakkan kode css langsung pada elemen html dengan menggunakan atribut `style`. Akan tetapi cara ini **
tidak**
disarankan, karena apabila semakin banyak html dan css kita, maka akan semakin sulit untuk membaca kode nanti.

```html
<h1 style="color: blue">Halo GDSC Universitas Sriwijaya!</h1>
```

### Internal CSS

Selain inline css, kita juga dapat memisahkan antara elemen dan kode css akan tetapi masih pada satu dokumen HTML. Cara
ini juga **tidak** disarankan karena apabila kita ingin menggunakan ulang `style` yang kita buat, maka kita harus
menuliskannya kembali, sehingga kode tersebut diulang-ulang padahal memiliki fungsi yang sama.

```html
<!doctype html>
<html>
<head>
    <title>Belajar Internal CSS</title>
    <style>
        h1 {
            color: blue;
        }
    </style>
</head>
<body>
<h1>Halo GDSC Universitas Sriwijaya!</h1>
</body>
</html>
```

### Eksternal CSS

Metode terakhir adalah Eksternal CSS, dan kami menyarankan untuk menggunakan metode tersebut karena selain _reusabilty_,
kode kita juga lebih bersih dan modular. Dengan metode ini, kita memisahkan file antara html dan css.

Buatlah sebuah file dengan struktur sebagai berikut :

```
project-folder
|
└───css-dasar
│   │   02-penempatan-css.html
│   │
│   └───css
|       |   02-penempatan-css.css
```

```html
<!doctype html>
<html>
<head>
    <title>Belajar Eksternal CSS</title>
    <link rel="stylesheet" href="css/02-penempatan-css.css">
</head>
<body>
<h1>Halo GDSC Universitas Sriwijaya!</h1>
</body>
</html>
```

```css
h1 {
    color: blue;
}
```