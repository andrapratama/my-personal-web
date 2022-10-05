---
title: "Mixins"
date: 2022-01-01T00:02:22+07:00
draft: false
tags:
- dart
- oop
---

Karena bahasa pemrograman Dart tidak mendukung multiple inheritance, Mixin memungkinkan untuk kita bisa mengimpelentasikan beberapa class ke dalam suatu kelas turunan. 

{{< highlight dart >}}
void main(List<String> arguments) {
  var appBarHome = AppBarHome();
  appBarHome.create();
}

abstract class Widget {
  void build();
}

mixin Text implements Widget {
  @override
  void build() {
    print('Tampilkan Text');
  }
}

mixin Button implements Widget {
  @override
  void build() {
    print('Tampilkan Tombol');
  }
}

class AppBar implements Widget {
  @override
  void build() {
    print('Tampilkan AppBar');
  }
}

class AppBarHome extends Widget with Text, Button, AppBar {
  void create() {
    build();
  }
}
{{< /highlight >}}

hasilnya

    Tampilkan AppBar

Fungsi yang ditampilkan adalah yang berasal dari class terakhir, dalam contoh ini class AppBar. Fungsi dari class Text ditimpa oleh class Button, kemudian class Button ditimpa oleh class AppBar.
Kenapa kita menimplementasikan mixin? Dalam contoh kita ini, AppBarHome yang kita buat memiliki Text, Button dan AppBar itu sendiri untuk ditampilkan. Jika ada AppBar lain, misal AppBarAbout yang tidak memiliki Button maka cukup kita buat seperti ini.

{{< highlight dart >}}
class AppBarAbout extends Widget with Text, AppBar {
  void create() {
    build();
  }
}
{{< /highlight >}}

Jadi beberapa AppBar punya perilaku yang sama, seperti menampilkan Text dan AppBar.