---
title: "Form Html Dengan Bootstrap"
date: 2022-09-22T09:55:48+07:00
draft: false
tags:
- html
- css
- bootstrap
---


Ada framework CSS yang cukup populer, yang dapat memudahkan kita dalam melakukan styling CSS. Dan kali ini kita akan menggunakan Bootstrap.

```html
<!DOCTYPE html>
<html>

<head>
    <title>Form HTML Bootstrap</title>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.1/dist/css/bootstrap.min.css" rel="stylesheet"
        integrity="sha384-iYQeCzEYFbKjA/T2uDLTpkwGzCiq6soy8tYaI1GyVh/UjpbCx/TYkiZhlZB6+fzT" crossorigin="anonymous">
</head>

<body>

    <div class="container">
        <h2 class="text-center">Data Diri</h2>
        <div class="row">
            <div class="col-4">

            </div>
            <div class="col-4">
                <form action="#">
                    <div class="mb-3">
                        <label for="foto" class="form-label">Foto</label>
                        <input type="file" id="foto" class="form-control" name="foto">
                    </div>
                    <div class="mb-3">
                        <label for="nama_lengkap" class="form-label">Nama Lengkap</label>
                        <input type="text" id="nama_lengkap" class="form-control" name="nama_lengkap">
                    </div>
                    <div class="mb-3">
                        <label for="nama_lengkap" class="form-label">Nama Panggilan</label>
                        <input type="text" id="nama_panggilan" class="form-control" name="nama_panggilan">
                    </div>
                    <div class="mb-3">
                        <label for="tanggal_lahir" class="form-label">Tanggal Lahir</label>
                        <input type="date" id="tanggal_lahir" class="form-control" name="tanggal_lahir">
                    </div>
                    <div class="mb-3">
                        <label for="alamat" class="form-label">Alamat</label>
                        <textarea id="alamat" class="form-control" name="alamat" cols="20" rows="3"></textarea>
                    </div>
                    <div class="mb-3">
                        <label for="email" class="form-label">Email</label>
                        <input type="email" id="email" class="form-control" name="email">
                    </div>
                    <div class="mb-3">
                        <label for="alamat" class="form-label">Telepon</label>
                        <input type="number" id="telepon" class="form-control" name="telepon">
                    </div>
                    <div class="mb-3">
                        <label for="jenis_kelamin" class="form-label">Jenis Kelamin</label>&nbsp;&nbsp;
                        <input type="radio" id="laki_laki" class="form-check-input" name="jenis_kelamin" value="1">
                        <label for="laki_laki" class="form-check-label">Laki-Laki</label>
                        <input type="radio" id="perempuan" class="form-check-input" name="jenis_kelamin" value="2">
                        <label for="perempuan" class="form-check-label">Perempuan</label>
                    </div>
                    <div class="mb-3">
                        <label for="warga_negara" class="form-label">Warga Negara</label>
                        <select id="warga_negara" class="form-control" name="warga_negara">
                            <option value="wni">WNI</option>
                            <option value="wna">WNA</option>
                        </select>
                    </div>
                    <div class="mb-3">
                        <label for="hobi" class="form-label">Hobi</label>
                        <div class="form-check">
                            <input type="checkbox" id="membaca" class="form-check-input" name="hobi" value="1">
                            <label for="membaca" class="form-check-label"> Membaca</label><br>
                            <input type="checkbox" id="menonton" class="form-check-input" name="hobi" value="2">
                            <label for="menonton" class="form-check-label"> Menonton</label><br>
                            <input type="checkbox" id="olahraga" class="form-check-input" name="hobi" value="3">
                            <label for="olahraga" class="form-check-label"> Olahraga</label>
                        </div>
                    </div>
                    <div class="mb-3 text-center">
                        <input type="submit" value="Simpan" class="btn btn-primary">
                    </div>
                </form>
            </div>
            <div class="col-4">

            </div>
        </div>
    </div>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.1/dist/js/bootstrap.bundle.min.js"
        integrity="sha384-u1OknCvxWvY5kfmNBILK2hRnQC3Pr17a+RTT6rIHI7NnikvbZlHgTPOOmMi466C8" crossorigin="anonymous">
    </script>
</body>

</html>
```

Hasilnya
![image](/assets/images/form-html-bootstrap.png)