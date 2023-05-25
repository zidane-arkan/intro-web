---
title: 01 - Javascript Intro
---

# Apa itu Javascript ? 
Javascript adalalah salah satu bahasa populer di dunia *programming* khusunya di dunia pemrograman web, karena mudah dipelajari dan tidak memiliki spesifikasi khusus untuk dijalankan, cukup browser.

## Contoh Syntax Javascript

```javascript
function getNama(nama){
    let salam = 'Hello'
    console.log(salam + ' ' + nama)
}
getNama('Henry')
```

## Peran JavaScript dalam Website
Jika dianggap sebagai manusia, javascript dapat dianggap sebagai otak yang berperan untuk mengendalikan dan memastikan tubuh *dalam hal ini website* berjalan atau berubah sesuai kemauan kita.

## Cara memanggil Javascript di halaman HTML
Ada dua cara umum yang dapat dilakukan untuk menggunakan javascript di halaman html kita : 
1. Menggunakan langsung javascript didalam halaman HTML
   - Didalam tag `<head>`
    ```html
    <head>
        <script>
            let nama = 'Human'
            console.log(nama)
        </script>
    </head>
    ```
   - Didalam tag `<footer>`
    ```html
    <body>
        <header></header>
        <main></main>
        <footer>
            <script>
                let nama = 'Human'
                console.log(nama)
            </script>
        </footer>
    </body>
    ```
2. Memanggil Javascript secara external
   Penggunaan javascript secara external merupakan cara yang sering digunakan karena memudahkan developer membaca dan mengedit file Javascript serta html.
   Contoh pemanggilan Javascript :
   ```html
   <body>
        <header></header>
        <main></main>
        <footer>
            <script src='./script.js'></script>
        </footer>
    </body>
   ```