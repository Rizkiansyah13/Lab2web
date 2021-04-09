# Praktikum 2
# Pemrograman Web 

```
Nama : Muhammad Rizkiansyah
NIM : 311910071
KELAS : TI.19.C1
```
## 1. Membuat dokumen HTML
Buatlah dokumen HTML seperti berikut
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Dasar</title>
</head>
<body>
    <header>
      <h1>CSS Internal dan <i>Inline CSS</i></h1>
    </header>
    <nav>
      <a href="lab2_css_dasar.html">CSS Dasar</a>
      <a href="lab2_css_eksternal.html">CSS Eksternal</a>
      <a href="lab1_tag_dasar.html">HTML Dasar</a>
    </nav>
    <!-- CSS ID Selector -->
    <div id="intro">
      <h1>Hello World</h1>
      <p>Kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemrograman Web</b> di <i>Universitas Pelita Bangsa</i>. Pelajaran pertama yang kami dapat adalah membuat tampilan web sederhana dalam rangka mengenal tag-tag dasar HTML dan CSS.</p>
      <!-- CSS Class Selector -->
      <a class="button btn-primary" href="#intro">Informasi selengkapnya.</a>
    </div>
</body>
</html>
```
![langkah 1](https://user-images.githubusercontent.com/81818687/114202393-558bfa80-9981-11eb-8685-c73cf71e8ace.png)
## 2. Mendeklarasikan CSS Internal
Kemudian tambahkan deklarasi CSS internal seperti berikut pada bagian head dokumen.
```
<head>
    <title>CSS Dasar</title>
    <style>
        body {
            font-family:'Open Sans', sans-serif;
        }
        header {
            min-height: 80px;
            border-bottom:1px solid #77CCEF;
        }
        h1 {
            font-size: 24px;
            color: #0F189F;
            text-align: center;
            padding: 20px 10px;
        }
        h1 i {
            color:#6d6a6b;
        }
    </style>
</head>
```
![Langkah 2](https://user-images.githubusercontent.com/81818687/114202780-bca9af00-9981-11eb-966a-af751c33655a.png)
## 3. Menambahkan Inline CSS
Kemudian tambahkan deklarasi inline CSS pada tag

seperti berikut.
``` 
<p style="text-align: center; color: #0d0275;">
```
![langkah 3](https://user-images.githubusercontent.com/81818687/114203074-04c8d180-9982-11eb-842a-b60fddf667cd.png)
## 4. Membuat CSS Eksternal
Buatlah file baru dengan nama style_eksternal.css kemudian buatlah deklarasi CSS seperti berikut.
```
nav {
    background: #20A759;
    color:#fff;
    padding: 10px;
}
nav a {
    color: #fff;
    text-decoration: none;
    padding:10px 20px;
}
nav .active,
nav a:hover {
    background: #0B6B3A;
}
```
![4](https://user-images.githubusercontent.com/81818687/114203321-3f326e80-9982-11eb-828c-13d56c1d4fa5.png)
Kemudian tambahkan tag untuk merujuk file css yang sudah dibuat pada bagian
```
<head>
    <!-- menyisipkan css eksternal -->
    <link rel="stylesheet" href="style_eksternal.css" type="text/css">
</head>
```
![5](https://user-images.githubusercontent.com/81818687/114203482-6b4def80-9982-11eb-905e-3ba84f274d71.png)\
## 5. Menambahkan CSS Selector
Selanjutnya menambahkan CSS Selector menggunakan ID dan Class Selector. Pada file style_eksternal.css, tambahkan kode berikut.
```
/* ID Selector */
#intro {
    background: #418fb1;
    border: 1px solid #099249;
    min-height: 100px;
    padding: 10px;
}
#intro h1 {
    text-align: left;
    border: 0;
    color: #fff;
}
/* Class Selector */
.button {
    padding: 15px 20px;
    background: #bebcbd;
    color: #fff;
    display: inline-block;
    margin: 10px;
    text-decoration: none;
}
.btn-primary {
    background: #E42A42;
}
```
![6](https://user-images.githubusercontent.com/81818687/114203647-8caedb80-9982-11eb-994b-ee066fdd97bc.png)
## Pertanyaan dan Tugas
1.Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini.
```
saya melakukan eksperimen, merubah nilai padding pada nav a dan merubah warna.
```
![7](https://user-images.githubusercontent.com/81818687/114203963-db5c7580-9982-11eb-9fd3-2548f5fce49d.png)
2.Apa perbedaan pendeklarasian CSS elemen h1 {...} dengan #intro h1 {...}? berikan penjelasannya!
```
Pendeklarasian CSS elemen h1 mengubah tampilan seluruh elemen yang memiliki tag h1, sedangkan #intro h1 hanya mengubah tampilan elemen h1 yang memiliki id #intro.
```
3.Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya!
```
Kedua deklarasi tersebut akan tampil, namun selector ID yang akan tampil jika deklarasinya ada yang sama antara ID dan Class.
```
4.Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut 
terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser? 
``` dua-duanya , karena masing" selector terdapat declarasi Css ```
Berikan penjelasan dan contohnya! ( <p id="paragraf-1" class="text-paragraf"> )

``` yaitu tag yg menunjukan element paraghrap ```
contoh nya 




