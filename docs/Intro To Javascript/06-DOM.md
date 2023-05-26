---
title : 06 - DOM
---

# Apa itu DOM ?
Dapat dikatakan bahwa DOM merupakan representasi objek dalam sebuah website, dan objek tersebut dapat diakses,diubah atau dimanipulasi sesuai kemauan kita.
Saat website selesai dimuat, web tersebut akan membuat sebuah *Tree of Objects* : 

![Box Model](/img/treedom.png)
## DOM dan HTML
DOM atau **Document Object Model** memiliki kemampuan untuk mengakses element HTML. Berikut beberapa cara untuk melakukannya :
1. Menggunakan `document.getElementById`

    Berfungsi dalam JavaScript yang digunakan untuk mendapatkan referensi elemen HTML dalam dokumen berdasarkan ID elemen tersebut. 
    ```javascript
    let elementHero = document.getElementById('hero')
    console.log(elementHero)
    ```

2. Menggunakan `document.getElementsByClassName`

    Metode ini digunakan untuk mendapatkan `class` yang sama pada html, mengembalikan objek HTMLCollection.
    ```javascript
    let red = document.getElementsByClassName('red')
    console.log(red)
    ```
    Perlu diingat bahwa `document.getElementsByClassName()` mengembalikan sebuah objek HTMLCollection, yang mirip dengan array tetapi sebenarnya bukan array. Metode array seperti `push()`,`pop()` atau `join()` tidak dapat digunakan.

3. Menggunakan `document.querySelector`

    Cara kerja metode ini hampir sama dengan `document.getElementById()` namun elemen yang bisa diambil bukan hanya berupa `id` namun `class juga` dengan catatan bahwa hanya elemen pertama yang dikembalikan.
    ```javascript
    let judul = document.getElementByClassName('#judul')
    console.log(judul)
    let list = document.getElementByClassName('.list')
    console.log(list)
    ```

4. Menggunakan `document.querySelectorAll`

    Mirip dengan `document.getElementsByClassName`, namun data yang dikembalikan berupa nodeList.
    ```javascript
    let tebal = document.querySelectorAll('.tebal');
    for(let i = 0; i < tebal.length; j+=){
        tebal[i].style.backgroundColor = 'blue'
    }
    ```

## Manipulasi elemen
Selain mengakses, kita juga dapat memanipulasi elemen yang telah kita akses. Caranya adalah sebagai berikut :
1. Ubah isi kontent melalui `.innerHTML`
```javascript
let judul = document.getElementByClassName('#judul')
judul[0].innerHTML = 'Teks yang dibuat query'
```
2. Mengubah atribut elemen  `.setAttribute`
```javascript
let judul = document.getElementById('#gambar')
judul.setAttribute('src','info.png')
```
3. Manipulasi style elemen dengan `.style.property`
```javascript
let tab = document.getElementById('tab');
tab.style.backgroundColor = 'blue';
tab.style.padding = '32px';
```

## *Event Handlers* Javascript
Kita juga dapat menangkap *event* yang dilakukan user kita pada suatu elemen dan memberikan reaksi terhadap *event* tersebut.
- `onClick`
    ```javascript
    let element = document.getElementById('hero')
    element.onClick = function(){
        alert('Hello World')
    }
    ```
- `window.innerWidth dan innerHeight`

    Properti innerWidth dan innerHeight untuk mendapatkan ukuran layar (viewport) dalam JavaScript. Properti innerWidth memberikan lebar viewport sedangkan properti innerHeight memberikan tinggi viewport.
    ```javascript
    let width = window.innerWidth;
    let height = window.innerHeight;
    ```
## Lebih banyak tentang DOM dan Events
Untuk materi lebih lanjut mengenai DOM, kalian dapat mengakses web berikut :
- [JavaScript HTML DOM Document](https://www.w3schools.com/js/js_htmldom_document.asp)
- [HTML Events](https://www.w3schools.com/js/js_events.asp)