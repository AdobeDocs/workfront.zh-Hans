---
content-type: api
navigation-topic: general-api
title: 使用API资源管理器
description: 使用API资源管理器
author: Becky
feature: Workfront API
role: Developer
exl-id: dcb7dadb-4dd8-48da-a559-cbe8ad99ff9e
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---


# 使用API资源管理器

使用Adobe Workfront核心API时，API Explorer是一种旧版参考工具，它对支持的资源、参数和变量之间的关系进行编录。

## 访问API Explorer：

1. 使用Web浏览器导航到 [API资源管理器](https://developer.adobe.com/workfront/api-explorer/)\
   ![](assets/mceclip1-350x149.png)

1. 在API Explorer的右上角，选择所需的Workfront **API版本**，默认情况下会自动选择最新版本
1. 此 **筛选** 字段，可用于筛选按名称列出的对象，并将截断相应显示的对象列表：

   ![](assets/mceclip2-350x147.png)

   * **字段**：指定对象中的可用字段。
   * **引用**：指定对象的可用参考变量。 引用是变量的别名。 初始化后，引用可以与变量名称互换使用。 引用使用初始化的内存。
   * **收藏集**：对象的可用集合。 集合是表示对象和资源之间一对多关系的变量。
   * **Search**：对象的可用搜索资源。 搜索结果基于API请求中搜索资源指定的查询参数。
   * **操作**：对象支持的操作。 操作可以是针对某个资源或一组资源执行的简单或复杂的过程。 给定的操作也可能影响相关资源。

1. 打开选项卡，然后单击对象ID以查看适用的变量。\
   ![](assets/approval-350x89.png)\
   根据所选对象，可能应用以下变量：

   | 变量 | 定义 |
   |---|---|
   | 字段名称 | Workfront API内操作中使用的字段的名称。 |
   | 字段类型 | 可输入数据表中特定字段中的值的类型。 可能的字段类型值包括string、double、int、dateTime。 |
   | 枚举类型 | 可用于标识数据类型的值的类型。 |
   | 可能值 | 对象的可接受值。 |
   | 属性类型对象代码 | 可用于修改对象类的属性。 |
   | URL | 允许应用程序与Workfront API通信的条目路径。 |
   | 参数 | 可在应用程序和Workfront之间传递的对象变量。 |
   | 结果类型 | 可从方法返回的可允许的数据类型。 |
