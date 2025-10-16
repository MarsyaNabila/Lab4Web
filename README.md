# Lab4Web - Membuat Layout Sederhana

Nama: Marsya Nabila Putri

NIM: 312410338

Kelas: TI.24.A4

# Langkah-langkah Pratikum
Membuat dokumen HTML dengan nama file ```lab4_box.html```


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
        .div4 {
            background: blue;
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
