<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>FikryHafizh | 222303022 | KA-REG-4</title>
<style>
body {
            background-image: url('bacround.jpg');
            font-family: Arial, sans-serif;
        }
        nav {
            text-align: center;
            margin: 20px 0;
        }
        nav a {
            margin: 0 15px;
            text-decoration: none;
            color: blue;
            font-size: 20px;
        }
        h1 {
            text-align: center;
        }
        .content {
            text-align: center;
        }
        .content img {
            margin: 10px;
        }
        form {
            display: inline-block;
            text-align: left;
            margin-top: 20px;
        }
        form label, form input, form button {
            display: block;
            margin: 10px 0;
        }
    </style>
</head>
<body>
</style>
<body>
    <h1>Kios Beras Iwan</h1>
    <p> Kios Beras Iwan menyediakan Pelayanan secara online melalui whatsappp berikut beberapa daftar harga yang tersedia.</p>

    <h2>Daftar Harga</h2>
    <div>
        <img src="Img/foto3.jpg" alt="Foto" height="670" width="550"></a>
        <p><b><i>Harga Mulai Dari</b> Rp 57.000,00</i></p>
        <hr><p><b><i>Isi Data Sesuai Keinginan Anda</i></p>
            <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Formulir Layanan Kios Beras Iwan</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f2f2f2;
            padding: 20px;
        }
        .container {
            background-color: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            max-width: 500px;
            margin: auto;
        }
        .form-group {
            margin-bottom: 15px;
        }
        .form-group label {
            display: block;
            margin-bottom: 5px;
        }
        .form-group input, .form-group select, .form-group textarea {
            width: 100%;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 4px;
        }
        .form-group textarea {
            resize: vertical;
        }
        .btn {
            background-color: #f0539a;
            color: white;
            padding: 10px 15px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            font-size: 16px;
        }
        .btn:hover {
            background-color: #f0539a;
        }
    </style>
</head>
<body>

<div class="container">
    <br>
    <h2>Pemesanan Via Formulir</h2>
    <form id="bookingForm">
        <div class="form-group">
            <label for="name">Nama:</label>
            <input type="text" id="name" name="name" required>
        </div>
        <div class="form-group">
            <label for="phone">Nomor Telepon:</label>
            <input type="tel" id="phone" name="phone" required>
        </div>
        <div class="form-group">
            <label for="service">Tipe Beras:</label>
            <select id="service" name="service" required>
                <option value="Belimbing 25KG">Belimbing 25KG</option>
                <option value="Super Lele 5KG">Super Lele 5KG</option>
                <option value="Si Buyung 5kg">Si Buyung 5kg</option>
                <option value="Si Buyung 10KG">Si Buyung 10KG</option>
                <option value="Pinang Mas 20KG">Pinang Mas 20KG</option>
                <option value="Super Kelapa 5KG">Super Kelapa 5KG</option>
                <option value="Super Kelapa 10KG">Super Kelapa 10KG</option>
            </select>
        </div>
        <div class="form-group">
            <label for="amount">Jumlah Pesanan:</label>
            <input type="tel" id="amount" name="amount" required>
            <div class="form-group">
                <label for="addreas">Alamat:</label>
                <input type="tel" id="addreas" name="addreas" required>
        <div class="form-group">
            <label for="notes">Catatan Tambahan:</label>
            <textarea id="notes" name="notes" rows="4"></textarea>
        </div>
        <button type="button" class="btn" onclick="sendToWhatsApp()">Kirim Pesanan</button>
    </form>
</div>

<script>
    function sendToWhatsApp() {
        var name = document.getElementById("name").value;
        var phone = document.getElementById("phone").value;
        var service = document.getElementById("service").value;
        var amount = document.getElementById("amount").value;
        var addreas = document.getElementById("addreas").value;
        var notes = document.getElementById("notes").value;

        var message = "Hallo Kios Beras Iwan, saya ingin melakukan booking dengan detail berikut:%0A" +
                      "Nama: " + name + "%0A" +
                      "Nomor Telepon: " + phone + "%0A" +
                      "Layanan: " + service + "%0A" +
                      "Jumlah: " + amount + "%0A" +
                      "Alamat: " + addreas + "%0A" +
                      "Catatan Tambahan: " + notes;

        var whatsappURL = "https://wa.me/6285846589594?text=" + message;

        window.open(whatsappURL, "_blank");
    }
</script>

</body>
</html>
