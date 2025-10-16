# Lab4Web - Membuat Layout Sederhana

Nama: Marsya Nabila Putri

NIM: 312410338

Kelas: TI.24.A4

# Langkah-langkah Pratikum
Membuat dokumen HTML dengan nama file ```lab4_box.html```

Kode di tersebut merupakan contoh penggunaan elemen box dengan CSS float. Pada bagian `<head>` terdapat pengaturan seperti `<meta charset="UTF-8">` untuk menentukan karakter, `<meta name="viewport">` agar tampilan responsif, dan `<title>Box Element Float</title>` sebagai judul halaman. Bagian `<style>` digunakan untuk mengatur tampilan kotak. Semua elemen `<div>` diberi properti `float: left` agar sejajar ke kiri, `padding: 10px` untuk memberi jarak dalam kotak, `color: white` untuk warna teks, `text-align: center` agar teks berada di tengah, dan `width: 100px` untuk menentukan lebar. Empat kotak dibuat dengan kelas berbeda: `.div1` berwarna merah, `.div2` kuning dengan teks hitam, `.div3` hijau, dan `.div4` biru. Khusus `.div4` ditambahkan `clear: left` dan `float: none` supaya posisinya berada di bawah tiga kotak sebelumnya. Di dalam `<body>` terdapat empat `<div>` dengan teks “Div 1” sampai “Div 4” yang menampilkan hasil pengaturan tersebut. Jadi, tampilan akhirnya menampilkan tiga kotak berwarna sejajar ke kiri dan satu kotak biru di baris bawah.

```css
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

Kode CSS di atas digunakan untuk mengatur tampilan halaman web **Layout Sederhana** agar terlihat rapi dan seimbang. Pada bagian awal dilakukan **import font** dari Google Fonts (*Open Sans*) dan **reset CSS** untuk menghapus margin serta padding default semua elemen. Bagian **body** mengatur jenis huruf, ukuran, dan warna teks utama, sedangkan **#container** berfungsi sebagai wadah utama dengan lebar 980px dan bayangan lembut di sekelilingnya. Bagian **header** menampilkan judul dengan warna abu-abu, sementara **nav** digunakan sebagai menu navigasi berwarna biru dengan teks putih dan efek hover agar berubah warna menjadi lebih terang. Panel **#hero** berfungsi sebagai area pembuka atau banner dengan latar abu-abu muda, teks besar, dan tombol di bawahnya.
Selanjutnya, **#wrapper** membungkus dua bagian utama, yaitu **#main** untuk konten utama dan **#sidebar** untuk area samping. Sidebar berisi **widget-box** yang menampilkan daftar link dan teks tambahan dengan desain sederhana dan warna biru pada judulnya. Kelas **.box** digunakan untuk membuat tiga kotak sejajar dengan gambar, teks, dan tombol, sedangkan **.image-circle** membuat gambar tampil bulat. Elemen **.entry** mengatur tampilan artikel yang berisi gambar di sisi kiri atau kanan dengan teks di sampingnya, dan **.divider** berfungsi sebagai garis pemisah antar bagian. Terakhir, **footer** diberi latar hitam dengan teks putih sebagai penutup halaman. Secara keseluruhan, CSS ini mengatur layout halaman agar tampil bersih, teratur, dan mudah dibaca.

```html
/* import google font */ 
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&display=swap'); 
@import url('https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:ital,wght@0,300;0,700;1,300&display=swap'); 

/* Reset CSS */ 
* { 
    margin: 0; 
    padding: 0; 
} 

body { 
    line-height:1; 
    font-size:100%; 
    font-family:'Open Sans', sans-serif; 
    color:#5a5a5a; 
} 

#container { 
    width: 980px; 
    margin: 0 auto; 
    box-shadow: 0 0 1em #cccccc; 
} 

/* header */ 
header { 
    padding: 20px; 
} 

header h1 { 
    margin: 20px 10px; 
    color: #b5b5b5; 
} 

/* navigasi */ 
nav { 
    display: block; 
    background-color: #1f5faa; 
} 

nav a { 
    padding: 15px 30px; 
    display: inline-block; 
    color: #ffffff; 
    font-size: 14px; 
    text-decoration: none; 
    font-weight: bold; 
} 

nav a.active, 
nav a:hover { 
    background-color: #2b83ea; 
} 

/* Hero Panel */ 
#hero { 
    background-color: #e4e4e5; 
    padding: 50px 20px; 
    margin-bottom: 20px; 
} 

#hero h1 { 
    margin-bottom: 20px; 
    font-size: 35px; 
} 

#hero p { 
    margin-bottom: 20px; 
    font-size: 18px; 
    line-height: 25px; 
} 

/* main content */ 
#wrapper { 
    margin: 0; 
} 

#main { 
    float: left; 
    width: 640px; 
    padding: 20px; 
} 

/* sidebar area */ 
#sidebar { 
    float: left; 
    width: 260px; 
    padding: 20px; 
} 

/* widget */ 
.widget-box { 
    border:1px solid #eee; 
    margin-bottom:20px; 
} 

.widget-box  .title { 
    padding:10px 16px; 
    background-color:#428bca; 
    color:#fff; 
} 

.widget-box ul { 
    list-style-type:none; 
} 

.widget-box li { 
    border-bottom:1px solid #eee; 
} 

.widget-box li a { 
    padding:10px 16px; 
    color:#333; 
    display:block; 
    text-decoration:none; 
} 

.widget-box li:hover a { 
    background-color:#eee; 
} 

.widget-box p { 
    padding:15px; 
    line-height:25px; 
} 

/* footer */ 
footer { 
    clear:both; 
    background-color:#1d1d1d; 
    padding:20px; 
    color:#eee; 
} 

/* box */ 
.box { 
    display:block; 
    float:left; 
    width:33.333333%; 
    box-sizing:border-box; 
    -moz-box-sizing:border-box; 
    -webkit-box-sizing:border-box; 
    padding:0 10px; 
    text-align:center; 
} 

.box h3 { 
    margin: 15px 0; 
} 

.box p { 
    line-height: 20px; 
    font-size: 14px; 
    margin-bottom: 15px; 
} 

box img { 
    border: 0; 
    vertical-align: middle; 
} 

.image-circle { 
    border-radius: 50%; 
} 

.row { 
    margin: 0 -10px; 
    box-sizing: border-box; 
    -moz-box-sizing: border-box; 
    -webkit-box-sizing: border-box; 
} 

.row:after, .row:before, 
.entry:after, .entry:before { 
    content:''; 
    display:table; 
} 

.row:after, 
.entry:after { 
    clear:both; 
} 

.divider { 
    border:0; 
    border-top:1px solid #eeeeee; 
    margin:40px 0; 
} 

/* entry */ 
.entry { 
    margin: 15px 0; 
} 

.entry h2 { 
    margin-bottom: 20px; 
} 

.entry p { 
    line-height: 25px; 
} 

.entry img { 
    float: left; 
    border-radius: 5px; 
    margin-right: 15px; 
} 

.entry .right-img { 
    float: right; 
}
```









