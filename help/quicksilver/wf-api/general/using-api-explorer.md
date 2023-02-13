---
content-type: api
navigation-topic: general-api
title: 使用API资源管理器
description: 使用API资源管理器
author: John
feature: Workfront API
exl-id: dcb7dadb-4dd8-48da-a559-cbe8ad99ff9e
source-git-commit: 40698643b0fa530b38da465f3bc1e4d841fcc190
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---


# 使用API资源管理器

使用Adobe Workfront核心API时，API资源管理器是一个旧版引用工具，可对支持的资源、参数和变量之间的关系进行编录。

## 访问API资源管理器：

1. 使用Web浏览器导航到 [API Explorer](https://one.workfront.com/s/api-explorer)\
   ![](assets/mceclip1-350x149.png)

1. 在API资源管理器的右上角，选择所需的Workfront **API版本**，默认情况下会自动选择最新版本
1. 的 **过滤器** 字段，可用于筛选按名称列出的对象，并将相应地截断显示的对象列表：

   ![](assets/mceclip2-350x147.png)

   * **字段**:指定对象中的可用字段。
   * **引用**:指定对象的可用引用变量。 引用是变量的别名。 初始化后，引用可与变量名称交替使用。 引用使用初始化的内存。
   * **收藏集**:对象的可用集合。 集合是表示对象和资源之间一对多关系的变量。
   * **搜索**:对象的可用搜索资源。 搜索结果基于搜索资源在API请求中指定的查询参数。
   * **操作**:对象支持的操作。 操作可以是针对资源或一组资源执行的简单或复杂的过程。 给定的操作也可能影响相关资源。

1. 打开一个选项卡，然后单击对象ID以查看适用的变量。\
   ![](assets/approval-350x89.png)\
   根据所选对象，可能会应用以下变量：

   | 变量 | 定义 |
   |---|---|
   | 字段名称 | 在Workfront API中的操作中使用的字段名称。 |
   | 字段类型 | 可输入到数据表中特定字段的值类型。 可能的字段类型值包括字符串、双精度、整数、dateTime。 |
   | 枚举类型 | 可用于标识数据类型的值类型。 |
   | 可能值 | 对象的可接受值。 |
   | 属性类型ObjCode | 可用于修改对象类的属性。 |
   | URL | 允许应用程序与Workfront API通信的登入路径。 |
   | 参数 | 可在应用程序和Workfront之间传递的对象变量。 |
   | 结果类型 | 允许从方法返回的数据类型。 |
