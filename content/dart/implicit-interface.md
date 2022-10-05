---
title: "Implicit Interface"
date: 2022-01-01T00:04:22+07:00
draft: false
tags:
- dart
- oop
---

Setiap class di dalam bahasa pemrograman Dart bisa bertindak sebagai Interface. Maka dari itu disebutlah sebagai Implicit Interface. Contoh penerapannya

{{< highlight dart >}}
void main(List<String> arguments) {
  var appBarHome = AppBarHome('Instagram', 20, 'putih', 'klik profil');
  appBarHome.create();
  appBarHome.build();
}

// class yang fungsinya dibiarkan tetap kosong karena akan diimplementasi di class yang mengimplementasikannya
class Widget {
  void build() {}
}

// class AppBar yang memiliki karakteristik umum
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

// class yang AppBar yang lebih spesifik
class AppBarHome extends AppBar implements Widget {
  late String aksi;
  AppBarHome(String nama, int tinggi, String warna, this.aksi)
      : super(nama, tinggi, warna);

  // mengimplementasikan fungsi dari kelas Widget
  @override
  void build() {
    createAction();
  }

  void createAction() {
    print('Aksi menunya adalah $aksi');
  }
}
{{< /highlight >}}

hasilnya

    Aplikasi Instagram ini memiliki Appbar ini tingginya 20 dan warnanya putih
    Aksi menunya adalah klik profil