# Lab4Web - Membuat Layout Sederhana

Nama: Marsya Nabila Putri

NIM: 312410338

Kelas: TI.24.A4

# Langkah-langkah Pratikum
Membuat dokumen HTML dengan nama file ```lab4_box.html```

Kode di tersebut merupakan contoh penggunaan elemen box dengan CSS float. Pada bagian `<head>` terdapat pengaturan seperti `<meta charset="UTF-8">` untuk menentukan karakter, `<meta name="viewport">` agar tampilan responsif, dan `<title>Box Element Float</title>` sebagai judul halaman. Bagian `<style>` digunakan untuk mengatur tampilan kotak. Semua elemen `<div>` diberi properti `float: left` agar sejajar ke kiri, `padding: 10px` untuk memberi jarak dalam kotak, `color: white` untuk warna teks, `text-align: center` agar teks berada di tengah, dan `width: 100px` untuk menentukan lebar. Empat kotak dibuat dengan kelas berbeda: `.div1` berwarna merah, `.div2` kuning dengan teks hitam, `.div3` hijau, dan `.div4` biru. Khusus `.div4` ditambahkan `clear: left` dan `float: none` supaya posisinya berada di bawah tiga kotak sebelumnya. Di dalam `<body>` terdapat empat `<div>` dengan teks “Div 1” sampai “Div 4” yang menampilkan hasil pengaturan tersebut. Jadi, tampilan akhirnya menampilkan tiga kotak berwarna sejajar ke kiri dan satu kotak biru di baris bawah.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Box Element Float</title>
    <style>
        div {
            float: left;
            padding: 10px;
            color: white;
            text-align: center;
            width: 100px;
        }
        .div1 { background: red; }
        .div2 { background: yellow; color: black; }
        .div3 { background: green; }
        .div4 { background: blue;
        clear: left;
        float: none;
        }
    </style>
</head>
<body>
    <section>
        <div class="div1">Div 1</div>
        <div class="div2">Div 2</div>
        <div class="div3">Div 3</div>
        <div class="div4">Div 4</div>
    </section>
</body>
</html>
```

<img width="838" height="500" alt="gambar 1" src="https://github.com/user-attachments/assets/07cfc94d-d373-416e-a2a7-37921287f902" />

<img width="1914" height="616" alt="gambar 2" src="https://github.com/user-attachments/assets/e315101f-7da9-4a44-8061-d15066eadde7" />

# Membuat Layout Sederhana

Kode di atas merupakan struktur dasar halaman web dengan layout sederhana menggunakan HTML dan CSS eksternal bernama **style.css**. Pada bagian `<head>` terdapat pengaturan meta, judul halaman, serta link ke file CSS agar tampilan lebih rapi. Di dalam `<body>` terdapat elemen utama `<div id="container">` yang membungkus seluruh isi halaman. Bagian `<header>` menampilkan judul “Layout Sederhana”, sedangkan `<nav>` berisi menu navigasi seperti Home, Artikel, About, dan Kontak. Bagian `<section id="hero">` menampilkan teks sambutan “Hello World!” dengan deskripsi singkat dan tombol “Learn more”. Selanjutnya, bagian `<section id="wrapper">` berisi dua bagian yaitu `<section id="main">` untuk konten utama dan `<aside id="sidebar">` untuk sidebar. Dalam main terdapat tiga kotak berisi gambar, judul, teks, dan tombol, lalu dua artikel dengan gambar dan teks. Sidebar berisi dua widget, satu berisi daftar link dan satu lagi berisi teks pendek. Bagian terakhir adalah `<footer>` yang menampilkan hak cipta “© 2021 - Universitas Pelita Bangsa”. Secara keseluruhan, kode ini membuat layout web lengkap dengan header, navigasi, konten utama, sidebar, dan footer yang tampil rapi dengan bantuan CSS.


```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Layout Sederhana</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div id="container">
        <header>
            <h1>Layout Sederhana</h1>
        </header>

        <nav>
            <a href="home.html" class="active">Home</a>
            <a href="artikel.html">Artikel</a>
            <a href="about.html">About</a>
            <a href="kontak.html">Kontak</a>
        </nav>

        <section id="hero">
            <h1>Hello World!</h1>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis.</p>
            <a href="home.html" class="btn btn-large">Learn more &raquo;</a>
        </section>

        <section id="wrapper">
            <section id="main">
                <div class="row">
                    <div class="box">
                        <img src="https://dummyimage.com/120/db7d25/fff.png" alt="" class="image-circle">
                        <h3>Heading</h3>
                        <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod.</p>
                        <a href="#" class="btn btn-default">View detail</a>
                    </div>
                    <div class="box">
                        <img src="https://dummyimage.com/120/3e73e6/fff.png" alt="" class="image-circle">
                        <h3>Heading</h3>
                        <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod.</p>
                        <a href="#" class="btn btn-default">View detail</a>
                    </div>
                    <div class="box">
                        <img src="https://dummyimage.com/120/71e6d4/fff.png" alt="" class="image-circle">
                        <h3>Heading</h3>
                        <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod.</p>
                        <a href="#" class="btn btn-default">View detail</a>
                    </div>
                </div>

                <hr class="divider">

                <article class="entry">
                    <h2>First featurette heading.</h2>
                    <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="">
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla.</p>
                </article>

                <hr class="divider">

                <article class="entry">
                    <h2>Second featurette heading.</h2>
                    <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="" class="right-img">
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu.</p>
                </article>
            </section>

            <aside id="sidebar">
                <div class="widget-box">
                    <h3 class="title">Widget Header</h3>
                    <ul>
                        <li><a href="#">Widget Link</a></li>
                        <li><a href="#">Widget Link</a></li>
                        <li><a href="#">Widget Link</a></li>
                        <li><a href="#">Widget Link</a></li>
                        <li><a href="#">Widget Link</a></li>
                    </ul>
                </div>

                <div class="widget-box">
                    <h3 class="title">Widget Text</h3>
                    <p>Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla.</p>
                </div>
            </aside>
        </section>

        <footer>
            <p>&copy; 2021 - Universitas Pelita Bangsa</p>
        </footer>
    </div>
</body>
</html>
```

<img width="1063" height="531" alt="gambar 3" src="https://github.com/user-attachments/assets/de651fe2-252d-4819-93bb-1b617e9ffbc7" />

# CSS Style








