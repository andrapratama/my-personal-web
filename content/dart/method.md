---
title: "Method"
date: 2022-09-01T00:09:22+07:00
draft: false
tags:
- dart
- oop
---

Method merupakan fungsi yang dimiliki oleh sebuah Class. Dalam Class Appbar yang sudah dibuat sebelumnya kita punya method dengan nama create().
{{< highlight dart >}}
class AppBar {
  // property
  String nama;
  int tinggi;
  String warna;

  AppBar(this.nama, this.tinggi, this.warna);

  // method
  void create() {
    print(
        'Aplikasi $nama ini memiliki Appbar ini tingginya $tinggi dan warnanya $warna');
  }
}
{{< /highlight >}}
