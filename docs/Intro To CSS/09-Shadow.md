---
title : 09 - Shadow
---

# Apa itu shadow dalam CSS ?

Shadow seperti namanya merupakan properti yang berfungsi untuk menambahkan efek bayangan baik dalam elemen yang berupa text, kotak atau gambar.

## Jenis Shadow Effect

Pada CSS terdapat tipe shadow, yang masing-masing memiliki kegunaanya masing-masing : 
1. `text-shadow`
2. `box-shadow`
Kedua properti tersebut memiliki kegunaan masing-masing, mari kita bahas bersama-sama.

## Text Shadow

Digunakan untuk menambahkan bayangan pada teks di halaman web.Memberikan efek visual yang menarik dan memungkinkan untuk mengubah penampilan teks dengan memberikan bayangan pada elemen teks tersebut.

Contoh penggunaan `text-shadow` : 
```css
p {
  text-shadow: 3px 2px 4px #ddffdd;
}
```
:::tip Deskripsi
Dibaca dari paling kiri `3px` melambangkan offset secara horizontal, kemudian `2px` dibaca sebagai offset secara vertikal, `4px` merupakan besar efek blur yang akan diberikan dan `#ddffdd` merupakan warna yang dipakai.
:::

Juga memungkinkan untuk menggunakan lebih dari 1 shadow :
```css
h1 {
  color: white;
  text-shadow: 1px 1px 2px #fffffff, 0 0 25px #dfdfdf, 0 0 5px #bbddff;
}
```

## Box Shadow

Jika `text-shadow` digunakan secara spesifik untuk text, maka `box-shadow` digunakan untuk elemen-elemen lain. Mulai dari div,span,section dan sebagainya.

Contoh penggunaan `box-shadow` :
```css
div {
  box-shadow: 10px 10px 5px 12px lightblue;
}
```
:::tip Deskripsi++
Untuk nilai tambahan yang berada di urutan ke-4, menentukan nilai *spread* dari suatu bayangan.
:::