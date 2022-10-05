---
title: "Enumerate Types"
date: 2022-01-01T00:03:22+07:00
draft: false
tags:
- dart
- oop
---

Di bahasa pemrograman dart kita bisa menyimpan konstan di satu tempat dan ditangani bersamaan yang disebut Enumerated Type. Sering disebut juga Enumerations atau Enums yang mewakili kumpulan konstan sehinga kode lebih jelas dan mudah dibaca.

{{< highlight dart >}}
void main(List<String> arguments) {
  // cara penggunaannya

  // memanggil semua nilai
  print(Widget.values);

  // memanggil nilai text
  print(Widget.text);

  // hanya memanggil nama text
  print(Widget.text.name);

  // memanggil nilai index
  print(Widget.button.index);

  // mengimplementasikannya di switch statements
  var menu = Menu.profile;

  switch (menu) {
    case Menu.home:
      print("Home Page");
      break;
    case Menu.profile:
      print("Profile Page");
      break;
    case Menu.settings:
      print("Settings Page");
      break;
    case Menu.about:
      print("About Page");
      break;
  }

  // membuat seperti class
  print(SubMenu.B.value);
  print(SubMenu.B);
  print(SubMenu.A.toString());
}

enum Widget { text, button, image, appbar }

enum Menu {
  home,
  profile,
  settings,
  about;
}

// membuat seperti class
enum SubMenu {
  A(100),
  B(80),
  C(60);

  // property
  final int value;

  // constructor
  const SubMenu(this.value);

  @override
  String toString() => "Hasil yang Anda dapat $name dengan nilai $value";
}
{{< /highlight >}}

hasilnya

    [Widget.text, Widget.button, Widget.image, Widget.appbar]
    Widget.text
    text
    1
    Profile Page
    80
    Hasil yang Anda dapat B dengan nilai 80
    Hasil yang Anda dapat A dengan nilai 100