---
title : 02 - Selektor
---

# Selector

Selector pada CSS berfungsi untuk menunjuk ke elemen HTML yang ingin diberi style.

Terdapat 5 macam selector yaitu :

## Element Selector

Jenis selector ini memungkinkan kita untuk menunjuk elemen HTML berdasarkan nama elemennya.

Contoh pengaplikasian :

```css
p {
  text-align: center;
  color: red;
}
```

## ID Selector

Jenis selector ini memungkinkan kita untuk menunjuk elemen HTML yang spesifik mempunyai attribut `id` dengan value yang sama dengan nama selector.
Jenis selector ini dimulai dengan simbol pagar (#) dan hanya dapat menunjuk tepat 1 elemen saja.

Contoh pengaplikasian :

#### CSS

```css
#paraf {
  text-align: center;
  color: red;
}
```

#### HTML

```html
<p id="paraf">Paraf</p>
```

## Class Selector

Jenis selector ini memungkinkan kita untuk menunjuk elemen HTML yang mempunyai attribut `class` dengan value yang sama dengan nama selector.
Jenis selector ini dimulai dengan simbol titik (.).

Contoh pengaplikasian :

#### CSS

```css
.center {
  text-align: center;
  color: red;
}

.dark {
  background-color: green;
}
```

#### HTML

```html
<p class="dark center">Hitam</p>
```

## Universal Selector

Jenis selector ini menunjuk ke seluruh elemen HTML.

Contoh pengaplikasian :

```css
* {
  text-align: center;
  color: blue;
}
```

## Grouping Selector

Jenis selector ini berfungsi untuk mengelompokan beberapa elemen dengan atribut-atribut yang sama.

Contoh pengaplikasian :

```css
h1, h2, h3 {
  text-align: center;
  color: red;
}
```