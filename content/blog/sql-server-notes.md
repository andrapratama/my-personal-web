---
title: "My Sql Server Notes"
date: 2022-12-10T14:05:18+07:00
draft: false
tags:
- sql server
---

I tried to summarize some of the techniques that I use in my development of systems that I do in my work. Some of them may be repetitive work, so I don't forget to write them down

## **Rename Column**
{{< highlight sql >}}
EXEC sp_rename 'dbo.table_name.old_column', 'new_colum', 'COLUMN';
{{< /highlight >}}

## **Formatting Money Value**
{{< highlight sql >}}
REPLACE(CONVERT(VARCHAR,money,0), '.',',')
{{< /highlight >}}

## **Limit and Offset**
{{< highlight sql >}}
SELECT [id]
      ,[name] FROM [log] ORDER BY 
      [id]
      ,[name]
OFFSET 0 ROWS 
FETCH NEXT 10 ROWS ONLY;
{{< /highlight >}}