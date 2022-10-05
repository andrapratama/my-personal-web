---
title: "Abstract Class"
date: 2022-01-01T00:05:22+07:00
draft: false
tags:
- dart
- oop
---

Abstraction (Abstraksi) erupakan cara untuk membuat class yang sifatnya private. class yang bersifat abstrak akan menjadi parent. class tersebut hanya bisa diakses oleh class child yang nantinya akan direalisasikan dalam bentuk objek. Contohnya:

{{< highlight dart >}}
abstract class Widget {
  late String nama;
 
}
{{< /highlight >}}