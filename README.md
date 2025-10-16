# Lab4Web - Membuat Layout Sederhana

Nama: Marsya Nabila Putri

NIM: 312410338

Kelas: TI.24.A4

# Langkah-langkah Pratikum
Membuat dokumen HTML dengan nama file ```lab4_box.html```

Kode di tersebut merupakan contoh penggunaan elemen box dengan CSS float. Pada bagian `<head>` terdapat pengaturan seperti `<meta charset="UTF-8">` untuk menentukan karakter, `<meta name="viewport">` agar tampilan responsif, dan `<title>Box Element Float</title>` sebagai judul halaman. Bagian `<style>` digunakan untuk mengatur tampilan kotak. Semua elemen `<div>` diberi properti `float: left` agar sejajar ke kiri, `padding: 10px` untuk memberi jarak dalam kotak, `color: white` untuk warna teks, `text-align: center` agar teks berada di tengah, dan `width: 100px` untuk menentukan lebar. Empat kotak dibuat dengan kelas berbeda: `.div1` berwarna merah, `.div2` kuning dengan teks hitam, `.div3` hijau, dan `.div4` biru. Khusus `.div4` ditambahkan `clear: left` dan `float: none` supaya posisinya berada di bawah tiga kotak sebelumnya. Di dalam `<body>` terdapat empat `<div>` dengan teks “Div 1” sampai “Div 4” yang menampilkan hasil pengaturan tersebut. Jadi, tampilan akhirnya menampilkan tiga kotak berwarna sejajar ke kiri dan satu kotak biru di baris bawah.

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

# Membuat Layout Sederhana





