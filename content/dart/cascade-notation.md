---
title: "Cascade Notation"
date: 2022-09-01T00:07:22+07:00
draft: false
tags:
- dart
- oop
---

Dengan Cascade Notation (cascade operator), kita bisa melakukan operasi pada objek secara berurutan. Kita bisa akses dan jalankan property dan methodnya bersamaan saat membuat atau menginstansi objeknya. Contohnya sebagai berikut
{{< highlight dart >}}
void main(List<String> arguments) {
  // contoh penggunaan cascade notation
  var appBar = AppBar('', 0, '')
    ..nama = 'Instagram'
    ..tinggi = 20
    ..warna = 'putih'
    ..create();
}

class AppBar {
  String nama;
  int tinggi;
  String warna;

  AppBar(this.nama, this.tinggi, this.warna);

  void create() {
    print(
        'Aplikasi $nama ini memiliki Appbar ini tingginya $tinggi dan warnanya $warna');
  }
}
{{< /highlight >}}
hasilnya

    Aplikasi Instagram ini memiliki Appbar ini tingginya 20 dan warnanya putih
