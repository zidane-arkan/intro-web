---
title : 05 - Penggunaan Fungsi
---

## Membuat dan Memanggil Fungsi
Fungsi merupakan sebuah kode blok yang dibuat dan digunakan untuk tugas tertentu. Berikut cara pembuatan fungsi dalam javascript :
```javascript
function sum(param){
 /*Statements*/
    console.log(a)
    return a+b /*Optional*/
    /*End Statements*/
}
```
:::tip Keterangan :
1. Kata kunci `function` digunakan untuk mendeklarasikan fungsi
2. *pangkat* merupakan nama fungsi yang dapat diubah, menyesuaikan kegunaan dari fungsi yang kita buat
3. `(a,b)` merupakan parameter yang menerima nilai yang akan digunakan didalam fungsi,parameter dipisahkan menggunakan koma. Parameter tidak **WAJIB** sehingga dapat dikosongkan.
4. `Statements` merupakan pernyataan dari penggunaan fungsi dapat berupa logika, perulangan atau mengembalikan nilai yang sudah diolah.
5. `jumlah(5,10)` adalah cara kita memanggil fungsi yang sudah dibuat dan dapat diisi sesuai jumlah parameter yang ada
:::
## Jenis Fungsi dalam Javascript
- Function Declaration
```javascript
function pangkat(a,b){
    return a**b
}
pangkat(2,2)
```
- Named Function
```javascript
const isEven = function (n){
    return n % 2 !== 1;
}
isEven(3)
```
- Arrow Function
```javascript
const isEven = (n) => {
    return n % 2 !== 1;
}
isEven(10)
```
## *Built in Functions* dalam Javascript
*Built in functions* merupakan jenis fungsi bawaaan javascript yang tidak perlu kita definisikan dan hanya perlu dipanggil. Contoh Penggunaan :
1. `alert`
Berfungsi untuk memberikan kotak dialog peringatan pada user
```javascript
    alert('Hello World')
```
2. `console.log`
Menampilkan pesan atau nilai ke konsol developer. Berguna untuk tujuan debugging.
 ```javascript
console.log('Tes saja')
```  
3. `prompt`
Menampilkan kotak dialog yang meminta input dari pengguna.
```javascript
let umur = prompt('Masukkan umur anda : ')
alert(umur)
```
4. `Math.random`
Menghasilkan nilai acak antara 0 dan 1
```javascript
let randomNumber = Math.random()
console.log(randomNumber)
```

## Materi lebih lanjut 
1. [JavaScript Built-in Functions](https://www.tutorialspoint.com/javascript/javascript_builtin_functions.htm)