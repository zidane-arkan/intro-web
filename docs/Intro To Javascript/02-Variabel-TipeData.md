---
title : 02 - Variabel dan Tipe Data
---

## Membuat Variabel
Variabel merupakan wadah/tempat untuk menampung nilai dan didalam Javascript Terdapat 3 jenis tipe variabel yang ada :
1. `var`
Merupakan jenis variabel yang dapat diedit dan dideklarasikan ulang, sangat jarang digunakan semenjak kemunculan tipe `let` disebabkan jenis variabel ini mudah untuk menimbulkan bug.
```javascript
var makan = 'ayam'
```
2. `let`
Penggunaan jenis variabel yang disarankan, sebab variabel dengan nama yang sama tidak dapat dibuat kembali.
```javascript
let nama = 'Makarov'
```
3. `const`
Dapat dikatakan jenis variabel yang absolut, karena baik nilai dan nama yang ada di variabel tersebut tidak dapat dibuat ulang dengan nama yang sama atau diubah isinya.
```javascript
const type = 'array'
```
## Jenis Tipe data dalam Javascript
- Number
```javascript
let number = 10
```
- String
```javascript
let film = 'solo'
```
- boolean
```javascript
let isOn = true
```
- array
```javascript
let saves = [1,2,3,4,5,'a','b']
```
- objek
```javascript
let mobil = {
  merk: "Honda",
  warna: "Merah",
  isGood: true,
  tahun: 2022,
  hidupkan: function() {
    console.log("Mobil dinyalakan");
  }
};
```
## Menggabungkan string
Penggabungan string dalam javascript dapat dilakukan dengan beberapa cara namun terdapat cara-cara yang umum dilakukan :
1. Method Concat
Metode ini memanfaatkan fungsi bawaan dalam javascript.
```javascript
let teks1 = 'Halo semua,'
let teks2 = 'nama saya lex'
let hasil = teks1.concat(teks2)
```
2. Operasi Konkatenasi
Teknik yang sering dipakai pada bahasa pemrograman lain dengan menggunakan operator tambah (+) untuk menyatukan string.
```javascript
let teks1 = 'Halo semua,'
let teks2 = 'nama saya lex'
let hasil = teks1 + teks2
```
3. Template Literal
Menggabungkan string dengan tanda `${}` kita menggunakan template literals dengan tanda kutip kembali **`** untuk menggabungkan string dengan variabel.Ekspresi atau nilai variabel di dalam **${}** akan diolah dan digabungkan dengan string yang ada di sekitarnya.
```javascript
let teks1 = 'Halo semua,'
let teks2 = 'nama saya lex'
let hasil = `Kesimpulan : ${teks1} dan ${teks2}`
```