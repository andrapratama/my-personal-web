---
title: "Flutter Lifecycle"
date: 2023-01-17T22:06:55+07:00
draft: false
tags:
- flutter
---

Sebelum mengetahui bagaimana *lifcycle* di **Flutter**, mari kita lihat di masing-masing *native* **Android** dan **iOS**

## Android

* onCreate
* onStart
* onResume
* — — — — — — — — —
* onPause
* onStop
* (forever alone onRestart)
* onDestroy

Sebagian besar *login* berakhir di dalam metode **onCreate**: Init Views, Database, Listeners, dll. *Lifecycle* seperti **onResume** dan **onPause** sangat bermanfaat untuk mengetahui apakah pengguna meninggalkan layar atau kembali ke layar.

## iOS

* viewDidLoad
* viewWillAppear
* viewDidAppear
* — — — — — — — — —
* viewWillDisappear
* viewDidDisappear
* viewDidUnload

Kedua platform menggunakan langkah yang (hampir) sama untuk membuat dan menghancurkan layar. **viewDidLoad()** menampung banyak logika bisnis dan **Will/Did Appear/Disappear** yang bagus untuk menyimpan informasi, tahu kapan pengguna meninggalkan layar, dll.


## Flutter

Sekarang kita perlu tahu persamaannya untuk Flutter. Ada 2 Widget utama:  **StatelessWidget** dan  **StatefulWidget**. StatefulWidget akan jadi fokusnya karena memiliki logika yang sama seperti Android dan iOS.

## StatefulWidget
Ini adalah salah satu Widget terpenting karena memiliki **state** Widget, yang ini tahu kapan sesuatu berubah dan menggambar ulang apa pun yang diperlukan di layar kita. Siklus hidup yang satu ini adalah sebagai berikut:





### Tabel Persamaan

| Android   | iOS      | Flutter   |
| --------  | -------- | ------ |
| onCreate | viewDidLoad | initState |