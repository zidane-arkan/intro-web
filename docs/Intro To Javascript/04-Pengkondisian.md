---
title: 04 - Kondisi dan Perulangan
---

# Penggunaan Pengkondisian
Ada kalanya kita butuh suatu cara untuk mengendalikan alur aplikasi kita, untuk itu kita dapat menggunakan *pengkondisian* agar hal tersebut dapat tercapai sesuai dengan kondisi yang diberikan.
## Jika Maka
jika-maka atau *if-else* adalah salah satu cara pengkondisian yang dapat digunakan, berikut cara penggunaan-nya dalam javascript :
```javascript
let angka = 10
if (angka > 0) {
  console.log("Angka positif");
} else if (angka < 0) {
  console.log("Angka negatif");
} else {
  console.log("Angka nol");
}
```
## Switch Case
`Switch case` untuk mengevaluasi nilai yang berbeda dan mengeksekusi kode berdasarkan nilai yang cocok.
```javascript
let hari = "Rabu";

switch (hari) {
  case "Senin":
    console.log("Hari ini saya membuat header");
    break;
  case "Selasa":
    console.log("Hari ini saya membuat main");
    break;
  case "Rabu":
    console.log("Hari ini saya membuat footer");
    break;
  case "Kamis":
    console.log("Hari ini saya melakukan hoisting");
    break;
  case "Jumat":
    console.log("Hari ini saya tidur");
    break;
  default:
    console.log("Hari tidak valid");
    break;
}
```
Penting untuk diingat bahwa setiap blok case harus diakhiri dengan pernyataan break untuk mencegah eksekusi kode berlanjut ke kasus berikutnya. Jika pernyataan break dihilangkan, maka eksekusi akan dilanjutkan ke kasus berikutnya, terlepas dari apakah kondisinya cocok atau tidak.

# Penggunaan Perulangan
### For
  Perulangan for digunakan untuk melakukan iterasi sejumlah kali dengan mengatur kondisi awal, kondisi berhenti, dan langkah perubahan pada setiap iterasi.
  ```javascript
  let arr = [1,2,3,4,5]
  for (i = 0; i < arr.length; i++){
    console.log(arr[i])
  }
  ```

### For-of
  Perulangan for...of digunakan untuk mengulang melalui elemen-elemen dari objek yang dapat diiterasi seperti array atau string.
  ```javascript
  let arr = [1, 2, 3];
  for (let e of arr) {
    console.log(e);
  }
  ```
### For-in
  Perulangan for...in digunakan untuk mengulang melalui properti-properti dari sebuah objek.
  ```javascript
  let obj = { a: 'hai', b: 2, c: true };
  for (let prop in obj) {
    console.log(`${prop} : ${obj[prop]}`);
  }
  ```
### While and Do-While
Dalam jenis perulangan `while` terdapat dua cara yang dapat dipakai untuk mencapai kondisi yang kita inginkan:
- While

  ```javascript
  let number = 2
  while(number < 10){
      console.log(number)
      number *= 2
  }
  ```
  Perulangan while akan menjalankan serangkaian pernyataan selama kondisi yang diberikan benar (true). Pertama, kondisi diuji, dan jika kondisinya benar, blok kode di dalam pernyataan while akan dijalankan.

- Do-while
  ```javascript
  let number = 2
  do {
    console.log(number);
    number *= 2;
  } while (number < 10);
  ```
  Perulangan do-while hampir mirip dengan perulangan while, tetapi blok kode di dalamnya dijalankan terlebih dahulu, kemudian kondisinya diperiksa. Jika kondisi benar, perulangan akan berlanjut. Perulangan do-while akan memastikan bahwa blok kode dijalankan setidaknya sekali.