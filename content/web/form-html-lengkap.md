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
        <table>
            <tr>
                <td><label for="foto">Foto</label></td>
                <td><input type="file" id="foto" name="foto"></td>
            </tr>
            <tr>
                <td><label for="nama_lengkap">Nama Lengkap</label></td>
                <td><input type="text" id="nama_lengkap" name="nama_lengkap"></td>
            </tr>
            <tr>
                <td><label for="nama_lengkap">Nama Panggilan</label></td>
                <td><input type="text" id="nama_panggilan" name="nama_panggilan"></td>
            </tr>
            <tr>
                <td><label for="tanggal_lahir">Tanggal Lahir</label></td>
                <td><input type="date" id="tanggal_lahir" name="tanggal_lahir"></td>
            </tr>
            <tr>
                <td><label for="alamat">Alamat</label></td>
                <td><textarea id="alamat" name="alamat" cols="20" rows="3"></textarea></td>
            </tr>
            <tr>
                <td><label for="email">Email</label></td>
                <td><input type="email" id="email" name="email"></td>
            </tr>
            <tr>
                <td><label for="alamat">Telepon</label></td>
                <td><input type="number" id="telepon" name="telepon"></td>
            </tr>
            <tr>
                <td><label for="jenis_kelamin">Jenis Kelamin</label></td>
                <td>
                    <input type="radio" id="laki_laki" name="jenis_kelamin" value="1">
                    <label for="laki_laki">Laki-Laki</label>
                    <input type="radio" id="perempuan" name="jenis_kelamin" value="2">
                    <label for="perempuan">Perempuan</label>
                </td>
            </tr>
            <tr>
                <td><label for="warga_negara">Warga Negara</label></td>
                <td><select id="warga_negara" name="warga_negara">
                        <option value="wni">WNI</option>
                        <option value="wna">WNA</option>
                    </select></td>
            </tr>
            <tr>
                <td><label for="hobi">Hobi</label></td>
                <td><input type="checkbox" id="membaca" name="hobi" value="1">
                    <label for="membaca"> Membaca</label><br>
                    <input type="checkbox" id="menonton" name="hobi" value="2">
                    <label for="menonton"> Menonton</label><br>
                    <input type="checkbox" id="olahraga" name="hobi" value="3">
                    <label for="olahraga"> Olahraga</label></td>
            </tr>
            <tr>
                <td></td>
                <td><input type="submit" value="Simpan"></td>
            </tr>
        </table>
    </form>
</body>
</html>
```

Hasilnya
![image](/assets/images/form-html.png)