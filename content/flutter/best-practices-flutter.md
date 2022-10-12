---
title: "Best Practices Flutter"
date: 2022-09-01T00:05:23+07:00
draft: false
tags:
- flutter
---

1. ## **SizedBox Placeholder**
    
    Gunakan `Sizebox` daripada `Container` sebagai placehoder widget

{{< highlight dart >}}
Widget showUI(){
  return Column(
    children: [
      _loaded ? const ActualUi() : const SizedBox.shrink();
    ],
  );
}
{{< /highlight >}}

Keuntungan:
- `SizedBox` punya *constructor* yang kodenya lebih efisien dibanding `Container`.
- `SizedBox` adalah objek yang lebih ringan dibandingkan  `Container` untuk dipakai.
- `SizedBox.shrink()` mengatur *width* dan *height* menjadi 0 yang secara *default* diinisialisasi null.
Kita bisa menggunakan `SizedBox` juga daripada `SizedBox.shrink()`, tapi menggunakan kata *shrink* memberikan indikasi yang jelas bahwa widget akan menempati ruang paling sedikit (atau nol) di layar.
- Pada `Container` jika widget tidak memiliki *child*, *height*, *width*, *constraints* dan *alignment*, tapi *parent* memberikan kendala batasan, kemudian `Container` meluas sesuai batasan yang disediakan *parent*nya.
2. ## **If operator**


3. ## **Const Widgets**


4. ## **Naming conventions**


5. ## **Themes**



