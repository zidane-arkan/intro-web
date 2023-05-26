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
2. Menggunakan `document.getElementByClassName`
3. Menggunakan `document.querySelector`
4. Menggunakan `document.querySelectorAll`
## Manipulasi elemen
Selain mengakses, kita juga dapat memanipulasi elemen yang telah kita akses. Caranya adalah sebagai berikut :
1. Ubah isi kontent melalui `.innerHTML`
2. Mengubah atribut elemen  `.attribute`
3. Manipulasi style elemen dengan `.style.property`

## *Event Handlers* Javascript
Kita juga dapat menangkap *event* yang dilakukan user kita pada suatu elemen dan memberikan reaksi terhadap *event* tersebut.
- `onClick`
```javascript
let element = document.getElementById('hero')
element.onClick = function(){
    alert('Hello World')
}
```

## Tambahan Materi
Untuk materi lebih lanjut mengenai DOM, kalian dapat mengakses web berikut :
- [JavaScript HTML DOM Document](https://www.w3schools.com/js/js_htmldom_document.asp)
- [HTML Events](https://www.w3schools.com/js/js_events.asp)