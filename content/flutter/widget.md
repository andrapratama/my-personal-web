---
title: "Widget"
date: 2022-09-01T00:05:22+07:00
draft: true
tags:
- flutter
- widget
---

Widget pada Flutter adalah komponen-komponen yang tampil di layar seperti **Text**, **Button**, **Image** dan sebagainya yang bisa dilihat, dan juga komponen-komponen yang mengatur seperti apa Widget tadi (Text, Button, Image dan sebagainya yang bisa dilihat) ditampilkan seperti **Row**, **Column**, **Stack**, **Container**.

Widget-widget tersebut bisa dikonfigurasi dan diberi status (*state*). Ketika ada perubahan konfigurasi dan status, widget akan dibuat ulang sesuai dengan konfigurasi dan statenya yang baru

Contoh Aplikasi Flutter sederhana yang memanggil funsi runApp() dengan sebuah widget:
{{< highlight dart >}}
import 'package:flutter/material.dart';

void main() {
  runApp(
    const Center(
      child: Text(
        'Hello, world!',
        textDirection: TextDirection.ltr,
      ),
    ),
  );
}
{{< /highlight >}}

# Widget Dasar

- **Text** memungkinkan untuk membuat serangkaian teks dengan gaya (*style*) yang kita inginkan.

- **Row** dan **Column** memungkinkan untuk membuat tata letak (*layout*) sesuai arah, *Row* untuk horizontal dan *Column* intuk vertikal. Desain objek ini didasarkan pada model tata letak *flexbox web*.

- **Stack** memungkinkan untuk menempatkan widget secara bertumpuk. Widget bisa menimpa satu sama lain seperti urutan cat. Kita bisa menggukanan Widget **Positioned** pada anak (*child*) Widget **Stack** untuk untuk memposisikannya relatif terhadap tepi atas, kanan, bawah, atau kiri. **Stack** didasarkan pada model tata letak pemosisian *absolut web*.

- **Container** memungkinkan untuk membuat elemen visual berbentuk persegi panjang yang bisa didekorasi dengan Widget **BoxDecoration** seperti background, border atau shadow. **Contaianer** juga punya margin, padding dan batasan yang diterapkan pada ukurannya. Selain itu, **Container** dapat ditransformasikan dalam ruang tiga dimensi menggunakan matriks.