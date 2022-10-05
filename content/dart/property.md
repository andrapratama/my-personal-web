---
title: "Property"
date: 2022-01-01T00:10:22+07:00
draft: false
tags:
- dart
- oop
---


Property merupakan variabel yang dimiliki oleh sebuah Class. Dalam Class Appbar yang sudah dibuat sebelumnya kita punya property nama, tinggi dan warna.
{{< highlight dart >}}
class AppBar {
  // property
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
