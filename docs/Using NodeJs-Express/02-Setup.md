---
title: 02 - Intro Project
---

# Apa Yang Akan Kita Buat ?
Kita akan membuat sebuah API sederhana untuk aplikasi Kontak menggunakan Node Js + Express.

## Mengenal Node Js
Dalam hal tumpukan aplikasi, Node.js menghadirkan persilangan yang menarik antara teknologi frontend dan backend. Dibangun di atas JavaScript, yang secara tradisional merupakan bahasa skrip web sisi-klien frontend, Node.js memperluas kemampuan JavaScript untuk berjalan di backend, bagian sisi-server dari arsitektur aplikasi web, serta untuk arsitektur tanpa server.

Meskipun Node.js sendiri adalah platform yang kuat dan serbaguna, ada kerangka kerja/pendekatan yang dibangun di atas Node.js untuk meningkatkannya lebih jauh seperti : Nest Js, Deno dan Electron.

![NodeJs System](./image/nodejsystem.jpg)

Manajer paket untuk Node.js disebut npm. Tujuannya adalah untuk melayani sebagai indeks perpustakaan yang dibangun oleh komunitas pengembang Node.js yang mudah dibagikan dan diimpor oleh proyek lain. Paket-paket ini memberikan solusi bermanfaat untuk fungsi dan kode umum yang menyederhanakan perancah proyek baru dan meningkatkan yang lama.

## Lalu apa itu Express ?
Express.js adalah framework web app untuk Node.js yang ditulis dengan bahasa pemrograman JavaScript. Framework open source ini dibuat oleh TJ Holowaychuk pada tahun 2010 lalu.Framework yang satu ini punya arsitektur MVC (Model View Controller). Dengan begitu, setiap data diolah pada Model, dihubungkan melalui Controller, lalu ditampilkan menjadi informasi melalui View.

Express.js di JavaScript adalah framework yang menggunakan pendekatan *Unopinionated* dalam proses pengembangan. Artinya, pengguna punya kebebasan dalam menentukan metode yang akan digunakan untuk mengeksekusi suatu perintah.Nah, *Unopinionated* ini punya beberapa kelebihan. Misalnya Anda bisa menentukan sendiri arsitektur yang akan dikembangkan. Di samping itu, ukuran framework juga cenderung lebih kecil, sehingga performanya jauh lebih cepat.

## Persiapan Project
Sebelum kita mulai untuk membuat Arsitektur Back-End Pertama kita, ada beberapa hal yang harus dipersiapkan terlebih dahulu : 
1. Install [Node Js](https://nodejs.org/en/download)
 - Pastikan node js telah terinstall dengan memasukkan Perintah pada cmd : 
  
    ```javascript
    npm -v
    node -v
    ```

2. Install Extension Thunder Client
3. Install Express js