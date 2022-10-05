---
title: "Extension Method"
date: 2022-01-01T00:01:22+07:00
draft: false
tags:
- dart
- oop
---

Extension Method bertujuan agar kita bisa membuat fungsionalitas tambahan dari library yang sudah ada. Bisa dari library bawaan Dart itu sendiri atau pun library orang lain.

{{< highlight dart >}}
void main() {
  var angkaAcak = [120, 500, 90, 189];
  print(angkaAcak);

  // fungsi sortAsc
  var angkaBerurut = angkaAcak.sortAsc();
  print(angkaBerurut);
}

// extension tambahan
extension Sorting on List<int> {
  List<int> sortAsc() {
    var list = this;
    var length = this.length;

    for (int i = 0; i < length - 1; i++) {
      int min = i;
      for (int j = i + 1; j < length; j++) {
        if (list[j] < list[min]) {
          min = j;
        }
      }

      int tmp = list[min];
      list[min] = list[i];
      list[i] = tmp;
    }

    return list;
  }
}

{{< /highlight >}}