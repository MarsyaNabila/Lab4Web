# Lab4Web - Membuat Layout Sederhana

Nama: Marsya Nabila Putri

NIM: 312410338

Kelas: TI.24.A4

# Langkah-langkah Pratikum
Membuat dokumen HTML dengan nama file ```lab4_box.html```

Kode di atas merupakan struktur dasar dari sebuah halaman web HTML5. Baris `<!DOCTYPE html>` berfungsi untuk memberitahu browser bahwa dokumen ini menggunakan HTML5. Tag `<html lang="en">` adalah elemen utama yang membungkus seluruh isi halaman dan memiliki atribut `lang="en"` yang menandakan bahwa bahasa yang digunakan adalah bahasa Inggris. Bagian `<head>` berisi informasi tentang dokumen seperti `<meta charset="UTF-8">` untuk mengatur karakter agar semua huruf dan simbol dapat ditampilkan dengan benar, `<meta name="viewport" content="width=device-width, initial-scale=1.0">` agar tampilan halaman dapat menyesuaikan dengan ukuran layar perangkat, dan `<title>Box Element</title>` untuk menentukan judul halaman yang muncul di tab browser. Sementara itu, bagian `<body>` berisi konten utama yang terlihat di halaman web. Di dalamnya terdapat tag `<header>` yang digunakan sebagai bagian kepala halaman dan berisi elemen `<h1>Box Element</h1>` yang menampilkan judul utama halaman dengan teks “Box Element”. Jadi, secara keseluruhan kode ini menampilkan halaman web sederhana dengan judul besar “Box Element” di bagian atas dan sudah memiliki struktur HTML yang lengkap dan responsif.


````html
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
````

<img width="838" height="500" alt="gambar 1" src="https://github.com/user-attachments/assets/07cfc94d-d373-416e-a2a7-37921287f902" />

<img width="1914" height="616" alt="gambar 2" src="https://github.com/user-attachments/assets/e315101f-7da9-4a44-8061-d15066eadde7" />



