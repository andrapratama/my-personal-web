---
title: "Form Html Lengkap"
date: 2022-09-20T11:17:16+07:00
draft: false
tags:
- html
---

Mari kita buat sebuah halaman HTML dengan form yang lengkap

```html
<!DOCTYPE html>
<html>
<head>
    <title>Form HTML</title>
</head>
<body>
    <h2>Data Diri</h2>

    <form action="#">
        <label for="foto">Foto</label><br>
        <input type="file" id="foto" name="foto"><br><br>

        <label for="nama_lengkap">Nama Lengkap</label><br>
        <input type="text" id="nama_lengkap" name="nama_lengkap"><br><br>

        <label for="nama_lengkap">Nama Panggilan</label><br>
        <input type="text" id="nama_panggilan" name="nama_panggilan"><br><br>

        <label for="tanggal_lahir">Tanggal Lahir</label><br>
        <input type="date" id="tanggal_lahir" name="tanggal_lahir"><br><br>

        <label for="alamat">Alamat</label><br>
        <textarea id="alamat" name="alamat" cols="20" rows="3"></textarea><br><br>

        <label for="alamat">Telepon</label><br>
        <input type="number" id="telepon" name="telepon"><br><br>

        <label for="jenis_kelamin">Jenis Kelamin</label><br>
          <input type="radio" id="laki_laki" name="jenis_kelamin" value="1">
          <label for="laki_laki">Laki-Laki</label><br>
          <input type="radio" id="perempuan" name="jenis_kelamin" value="2">
          <label for="perempuan">Perempuan</label><br>
        <br>

        <label for="warga_negara">Warga Negara</label><br>
        <select id="warga_negara" name="warga_negara">
            <option value="wni">WNI</option>
            <option value="wna">WNA</option>
        </select><br><br>

        <label for="hobi">Hobi</label><br>
        <input type="checkbox" id="membaca" name="hobi" value="1">
        <label for="membaca"> Membaca</label><br>
        <input type="checkbox" id="menonton" name="hobi" value="2">
        <label for="menonton"> Menonton</label><br>
        <input type="checkbox" id="olahraga" name="hobi" value="3">
        <label for="olahraga"> Olahraga</label>

        <br>
        <br>
        <input type="submit" value="Simpan">
    </form>
</body>
</html>
```