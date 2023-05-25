---
title : 07 - Responsif (Media Quaries)
---

# Apa itu Media Query ?
Media-query merupakan suatu teknik untuk membuat elemen-elemen yang ada di halaman website berubah atau menyesuaikan bentuk sesuai dengan lebar atau tinggi halaman yang ada. 
Jika dalam desktop atau PC maka halaman akan berubah menyesuaikan bentuk PC atau Desktop tersebut, begitu juga dalam mobile.

Contoh sederhana pemakaian properti `media-query`:
```css
@media (max-width: 768px){
    div{
        background-color: #FDDFDD;
        width: 250px;
        height: 300px
    }
}
```
Dalam contoh ini, kita menggunakan media query dengan kondisi `(max-width: 768px)` yang berarti jika lebar layar tidak lebih dari 768 piksel, maka aturan CSS di dalam media query akan diterapkan.


## Prioritaskan Tampilan Mobile
Istilah **Mobile First** mengacu pada pembuatan website yang berfokus pada tampilan *mobile* terlebih dahulu. Penggunaan styling menggunakan CSS akan dibuat untuk memastikan tampilan di *mobile* dapat digunakan dengan baik oleh user.

```css
div{
    background-color: #FDDFDD;
    width: 250px;
    height: 300px
    }
@media only screen and (min-width: 800px) and (max-width: 1000px){
    div{
        background-color: #DDDFFF;
        width: 100%;
        height: 250px;
    }
}
```

## Menambahkan breakpoint
Penggunaan `@media` dapat digunakan berkali-kali untuk size yang berbeda, tidak diwajibkan untuk menggunakan hanya sekali.

```css
@media only screen and (min-width: 601px) {
  div.example {
    font-size: 80px;
  }
}

@media only screen and (max-width: 600px) {
  div.example {
    font-size: 30px;
  }
}
```

:::tip Referensi
Materi resposnif lebih dalam, melalui W3 School :

:::