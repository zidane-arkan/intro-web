---
title : 03 - Operator
---

## Operasi Matematik
1. Penjumlahan
```javascript
let jumlah = 10 + 20
```
2. Pengurangan
```javascript
let kurang = 5 + 100
```
3. Perkalian
```javascript
let kali = 30 * 10
```
4. Pembagian
```javascript
let bagi = 100 / 20
```
5. Modulus
```javascript
let modulus = 10 % 2
```
6. Increment
```javascript
let increase = 1
increase++
```
7. Decrement
```javascript
let decrease = 5
decrease--
```

## Operasi Perbandingan
1. Sama Dengan (Identik dan Coercion)
   - Identik
   ```javascript
   let num1 = 25
   let num2 = '25'
   console.log(num1 === num2)
   ```
   - Coercion
   ```javascript
   let num1 = 25
   let num2 = '25'
   console.log(num1 == num2)
   ```
2. Tidak sama dengan (Identik dan Coercion)
   - Identik
   ```javascript
   let num1 = 100
   let num2 = '100'
   console.log(num1 !== num2)
   ```
   - Coercion
   ```javascript
   let num1 = 100
   let num2 = '100'
   console.log(num1 != num2)
   ```
3. Lebih Besar atau Lebih besar sama dengan
    - Lebih Besar dari
    ```javascript
    const num1 = 250
    const num2 = 250
    console.log(num > num2)
    ```
    - Lebih besar sama dengan
    ```javascript
    const num1 = 250
    const num2 = 250
    console.log(num >= num2)
    ```
4. Lebih Kecil atau Lebih kecil sama dengan
   - Lebih Kecil
   ```javascript
   const num1 = 0
   const num2 = 1
   console.log(num1 < num2)
   ```
   - Lebih Kecil sama dengan
   ```javascript
   const num1 = 1
   const num2 = 1
   console.log(num1 <= num2>)
   ```
   
:::tip Perhatikan
Penting untuk diperhatikan bahwa operator perbandingan (== dan !=) dapat melakukan coercions, yaitu mengubah tipe data dari ekspresi untuk membandingkannya. Untuk perbandingan yang lebih ketat dan memperhatikan tipe data, disarankan untuk menggunakan operator perbandingan yang identik (=== dan !==)
:::

## Operasi Logika
- Operasi and `&&`
Operator and hanya akan menghasilkan nilai `true` jika kedua nilai yang dibandingkan juga bernilai `true`, dan menghasilkan nilai `false` jika salah satu atau kedua nilai yang dibandingkan adalah `false`.
```javascript
const check1 = true
const check2 = true
console.log(check1 && check2)
```
- Operasi atau `||`
Menghasilkan nilai true jika salah satu atau kedua nilai yang dibandingkan adalah true. Jika kedua nilai yang dibandingkan false, maka hasilnya adalah false.
```javascript
const check1 = true
const check2 = false
console.log(check1 || check2)
```
- Operasi negasi `!`
Digunakan untuk **membalik** nilai logika. Jika ditulis value adalah true maka !value adalah false dan begitu juga sebaliknya.
```javascript
const check1 = true
const check2 = true
console.log(!(check1 && check2))
```