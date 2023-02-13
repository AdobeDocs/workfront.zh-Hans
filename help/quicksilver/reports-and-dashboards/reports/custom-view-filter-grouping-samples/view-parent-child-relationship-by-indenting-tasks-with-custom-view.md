---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: “查看：通过缩进任务来显示任务中的父子关系
description: 通过向任务列表添加自定义视图并确保在导出列表之前选择此视图，可以在导出的任务列表中保持父 — 子关系的区别。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 1%

---

# 查看：通过缩进任务来显示任务中的父子关系

通过向任务列表添加自定义视图并确保在导出列表之前选择此视图，可以在导出的任务列表中保持父 — 子关系的区别。  

![](assets/parent-child-indented-custom-view-350x94.png)

1. 转到包含要导出的任务列表的项目。
1. 单击 **查看** 下拉菜单，然后选择 **新建视图**.

1. 在屏幕的左上角命名过滤器。
1. 单击 **任务名称** 列标题。

1. 选择 **切换到文本模式** 中。
1. 单击文本框中的任意位置可编辑文本，并删除所有现有文本。
1. 粘贴以下文本：

   ```
   displayname=<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br>valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(" - ",{name}),IF({indent}<3,CONCAT(" - - ",{name}),IF({indent}<4,CONCAT(" - - - ",{name}),CONCAT(" - - - - ",{name})))))<br>valueformat=HTML
   ```

1. 单击&#x200B;**保存**。
1. 单击 **保存视图**.
