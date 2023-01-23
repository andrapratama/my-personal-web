---
title: "Yii2 Notes"
date: 2023-01-23T13:20:59+07:00
draft: false
tags:
- yii2
---

I tried to summarize some of the techniques that I use in my development of systems that I do in my work. Some of them may be repetitive work, so I don't forget to write them down


## **Add hasOne Condition inside Model**
{{< highlight php >}}
// kd_jenis_daerah: provinsi = 1, kabkota = 2
return $this->hasOne(RefUrusan::className(), ['kd_urusan' => 'kd_urusan1'])
        ->andOnCondition(['kd_jenis_daerah' => 1]);
{{< /highlight >}}