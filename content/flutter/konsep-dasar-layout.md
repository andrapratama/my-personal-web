---
title: "Konsep Dasar Layout"
date: 2022-09-01T00:05:23+07:00
draft: false
tags:
- flutter
- widget
---

UI pada Flutter dibangun dalam kode, bukan file XML atau sejenisnya. UI-nya disusun sebagai blok bangunan dasar yang disebut Widget (ada widget Text, Gambar, Baris, Kolom, Container dan sebagainya). Widget adalah objek yang tidak dapat diubah yang menjelaskan bagian tertentu dari UI. Kita bisa enggabungkan widget yang ada untuk membuat widget yang lebih canggih.
## Row dan Column 
Row dan Column adalah kelas yang memuat dan menata widget. Widget di dalam Row atau Column disebut child, dan Row dan Column disebut sebagai parent. Row menata widgetnya secara horizontal, dan Column menata widgetnya secara vertikal.

Referensi:
* https://docs.flutter.dev/codelabs/layout-basics