---
title: "Inheritance"
date: 2022-09-01T00:06:22+07:00
draft: false
tags:
- dart
- oop
---

Inheritance adalah cara dari suatu class agar bisa mewarisi sifat dari class lain. Class yang mewarisi sifat seperti property dan methodnya adalah SuperClass atau Parent Class, sedangkan Class yang diwarisi adalah Subclass atau Child Class. Contohnya seperti dibawah ini
menginstansi objeknya. Contohnya sebagai berikut
{{< highlight dart >}}
void main(List<String> arguments) {
  var appBarHome = AppBarHome('Instagram', 20, 'putih', 'klik profil');
  // memanggil fungsi dari class AppBar
  appBarHome.create();
  // memanggil fungsi dari class AppBarHome itu sendiri
  appBarHome.createAction();
}

// parent class
class AppBar {
  final String _nama;
  final int _tinggi;
  final String _warna;

  AppBar(this._nama, this._tinggi, this._warna);

  String get nama => _nama;
  int get tinggi => _tinggi;
  String get warna => _warna;

  void create() {
    print(
        'Aplikasi $nama ini memiliki Appbar ini tingginya $tinggi dan warnanya $warna');
  }
}

//child class
class AppBarHome extends AppBar {
  late String aksi;

  AppBarHome(String nama, int tinggi, String warna, this.aksi)
      : super(nama, tinggi, warna);

  void createAction() {
    print('Aksi menunya adalah $aksi');
  }
}
{{< /highlight >}}
hasilnya

    Aplikasi Instagram ini memiliki Appbar ini tingginya 20 dan warnanya putih
    Aksi menunya adalah klik profil