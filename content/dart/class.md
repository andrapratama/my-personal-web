---
title: "2. Class"
date: 2022-09-01T00:11:22+07:00
draft: false
tags:
- dart
- oop
---


Class merupakan blueprint atau cetak biru untuk membuat suatu objek. Misalkan kita mau membuat sebuah Application Bar atau Appbar pada sebuah aplikasi mobile. Kita bisa membuatnya seperti ini
{{< highlight dart >}}
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

kemudian kita coba gunakan class tersebut dan jalankan
{{< highlight dart >}}
void main(List<String> arguments) {
  var appBar = AppBar('Instagram', 20, 'green');
  appBar.create();
}
{{< /highlight >}}

hasilnya

    Aplikasi Instagram ini memiliki Appbar ini tingginya 20 dan warnanya green