---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: 数据存储模块
description: 安 [!DNL Adobe Workfront Fusion] 数据存储（与数据库或简单表类似）可以存储来自场景的数据，从而可以在单个场景或场景运行之间传输数据。 您可以在同步期间使用数据存储来存储来自不同系统的新数据。
author: Becky
feature: Workfront Fusion
exl-id: 1dc9cb88-d1b9-4a67-91fb-be980cc1ccd1
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1103'
ht-degree: 0%

---

# [!UICONTROL 数据存储] 模块

安 [!DNL Adobe Workfront Fusion] 数据存储（与数据库或简单表类似）可以存储来自场景的数据，从而可以在单个场景或场景运行之间传输数据。 您可以在同步期间使用数据存储来存储来自不同系统的新数据。

数据存储模块允许您在 [!DNL Adobe Workfront Fusion] 数据存储。

有关创建、编辑数据存储以及对其进行故障诊断的信息，请参阅 [数据存储在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

## 访问要求

您必须具有以下访问权限才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td>
  <td> <p>[!UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td>
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p>  <p>[!UICONTROL [!DNL Workfront Fusion] （工作自动化）</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 先决条件

使用 [!UICONTROL 数据存储] 模块中，您必须先创建数据存储。

有关创建数据存储的信息，请参阅 [数据存储在 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

## [!UICONTROL 数据存储] 模块及其字段

配置数据存储模块时， [!DNL Workfront Fusion] 显示下面列出的字段。 除这些字段外，还可能会显示其他数据存储字段，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

全部 [!UICONTROL 数据存储] 模块是操作类型模块。

* [添加/替换记录](#addreplace-a-record)
* [更新记录](#update-a-record)
* [获取记录](#get-a-record)
* [检查记录是否存在](#check-the-existence-of-a-record)
* [删除记录](#delete-a-record)
* [删除所有记录](#delete-all-records)
* [搜索记录](#search-records)
* [计数记录](#count-records)

### [!UICONTROL 添加/替换记录]

此操作模块可添加或替换记录。

指定数据存储和记录的键。

模块会返回记录的ID和任何关联字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

>[!NOTE]
>
>当您尝试使用与 [!UICONTROL 覆盖现有记录] 选项。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL数据存储]</td> 
   <td> <p> 选择或添加要创建记录的数据存储。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL密钥] </td> 
   <td> <p>输入希望模块添加或替换的记录的唯一键。 该键稍后可用于检索记录。 如果将此字段留空，则会自动生成一个键。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL覆盖现有记录] </td> 
   <td> <p>启用此选项可覆盖记录。 要覆盖的记录必须在上面的键字段中指定。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL记录] </td> 
   <td> <p>在记录的字段中输入所需的值。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 更新记录]

此操作模块会更新记录。

指定数据存储和记录的键。

模块会返回记录的ID和任何关联字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL数据存储]</td> 
   <td> <p> 选择或添加要创建记录的数据存储。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL密钥] </td> 
   <td> <p>输入要更新模块的记录的唯一键。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL插入缺失记录] </td> 
   <td> <p>如果具有指定键的记录不存在，则启用此选项可创建新记录。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL记录]</td> 
   <td> <p> 在要更新的记录字段中输入所需的值。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 获取记录]

此操作模块检索记录。

指定数据存储和记录的键。

模块会返回记录的ID和任何关联字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL数据存储]</td> 
   <td> <p> 选择要从中检索记录的数据存储</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL密钥] </td> 
   <td> <p>输入希望模块检索的记录的唯一键值。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 检查记录是否存在]

此操作模块指定是否存在特定记录。

指定数据存储和记录的键。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL数据存储] </td> 
   <td> <p>选择要检查记录是否存在的数据存储。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL密钥] </td> 
   <td> <p>输入希望模块检查是否存在的记录的唯一键。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 删除记录]

此操作模块会删除记录。

指定数据存储和记录的键。

模块会返回记录的ID和任何关联字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL数据存储] </td> 
   <td> <p>选择要检查记录是否存在的数据存储。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL密钥] </td> 
   <td> <p>输入要删除模块的记录的唯一键。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 删除所有记录]

此操作模块会从特定数据存储中删除所有记录。

您可以指定数据存储。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL数据存储] </td> 
   <td> <p>选择要从中删除所有记录的数据存储。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 搜索记录]

此搜索模块在数据存储中查找与您指定的搜索查询匹配的对象中的记录。

您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL数据存储]</td> 
   <td> <p> 选择要搜索的数据存储。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL过滤器]</p> </td> 
   <td> <p>设置搜索的过滤器。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL排序]</p> </td> 
   <td> <p style="font-weight: normal;">对于要排序的每个字段，填写以下字段：</p> <p style="font-weight: bold;">[!UICONTROL密钥]</p> <p>选择要按对结果进行排序的列名称。</p> <p style="font-weight: bold;">[!UICONTROL顺序]</p> <p>选择是要按升序还是降序对结果进行排序。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL限制]</td> 
   <td> <p> 设置搜索结果的最大数量 [!DNL Workfront Fusion] 在一个执行周期中返回。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL即使模块未返回任何结果，仍继续执行路由]</td> 
   <td> <p> 如果启用，则此模块将继续处理的路由，即使此模块未返回任何结果也是如此。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 计数记录]

此操作模块会对数据存储中的记录进行编号。

您可以指定数据存储。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL数据存储] </td> 
   <td> <p>选择包含要计数的记录的数据存储。</p> </td> 
  </tr> 
 </tbody> 
</table>
