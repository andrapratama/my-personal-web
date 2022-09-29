---
title: "Constructor"
date: 2022-09-01T00:08:22+07:00
draft: false
tags:
- dart
- oop
---

Constructor merupakan fungsi yang pertama kali dipanggil ketika sebuah objek dibuat. Dalam Class Appbar yang sudah dibuat sebelumnya kita punya Constructor yang namanya sama persis dengan nama Classnya.
{{< highlight dart >}}
class AppBar {
  // property
  String nama;
  int tinggi;
  String warna;

  // constructor
  AppBar(this.nama, this.tinggi, this.warna);

  // method
  void create() {
    print(
        'Aplikasi $nama ini memiliki Appbar ini tingginya $tinggi dan warnanya $warna');
  }
}
{{< /highlight >}}