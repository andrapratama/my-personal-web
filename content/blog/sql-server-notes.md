---
title: "My Sql Server Notes"
date: 2022-12-10T14:05:18+07:00
draft: false
tags:
- sql server
---

## **Rename Column**
{{< highlight sql >}}
EXEC sp_rename 'dbo.table_name.old_column', 'new_colum', 'COLUMN';
{{< /highlight >}}

## **Formatting Money Valueq**
{{< highlight sql >}}
REPLACE(CONVERT(VARCHAR,money,0), '.',',')
{{< /highlight >}}