---
title: "Paradigma OOP Pada Dart"
date: 2022-09-25T00:12:22+07:00
draft: false
tags:
- dart
- oop
---

## Encapsulation
<strong>Encapsulation</strong> (Enkapsulasi) merupakan cara untuk mengatur <strong>Property</strong> (variabel) dan <strong>Method</strong> (fungsi) dengan menyembunyikan alur kerja atau membatasi aksesnya di dalam `class`. Sederhanya, kita bisa menentukan Property atau Method mana yang bisa diakses langsung atau tidak. Di dalam bahasa pemrograman Dart ada 2 jenisnya yaitu, `private` dan `public`. `private` berati hanya bisa diakses di dalam `class`nya, sedangkan `public` bisa diakses di luar `class`nya.

## Abstraction
<strong>Abstraction</strong> (Abstraksi) erupakan cara untuk membuat `class` yang sifatnya `private`.  `class` yang bersifat abstrak akan menjadi <i>parent</i>. `class` tersebut hanya bisa diakses oleh `class` <i>child</i> yang nantinya akan direalisasikan dalam bentuk objek.

## Inheritance
<strong>Inheritance</strong> (Pewarisan) merupakan cara untuk menurunkan <strong>Property</strong> dan <strong>Method</strong> yang dimiliki sebuah `class` <i>parent</i> (<i>superclass</i>, <i>base class</i>) ke `class` <i>child</i> (<i>subclass</i>, <i>derived class</i> atau <i>heir class</i>).

## Polymorphism
<strong>Polymorphism</strong> (Banyak bentuk) merupakan cara untuk `class` memungkinkan punya banyak pewarisan.

Referensi:
* https://www.dicoding.com/blog/pengertian-polimorfisme-dalam-pemrograman-java/
* https://blog.sanbercode.com/docs/kurikulum-flutter-mobile-apps/materi-week-2/hari-7-oop-1/
* https://blog.sanbercode.com/docs/kurikulum-flutter-mobile-apps/materi-week-2/hari-9-class/8
* https://geekasmedia.blogspot.com/2022/07/empat-pilar-oop-di-bahasa-pemrograman-dart.html