---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: 数据存储模块
description: An [!DNL Adobe Workfront Fusion] 数据存储（与数据库或简单表类似）可以存储场景中的数据，因此可以在各个场景或场景运行之间传输数据。 在同步过程中，您可以使用数据存储来存储来自不同系统的新数据。
author: Becky
feature: Workfront Fusion
exl-id: 1dc9cb88-d1b9-4a67-91fb-be980cc1ccd1
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '1164'
ht-degree: 0%

---

# [!UICONTROL 数据存储] 模块

An [!DNL Adobe Workfront Fusion] 数据存储（与数据库或简单表类似）可以存储场景中的数据，因此可以在各个场景或场景运行之间传输数据。 在同步过程中，您可以使用数据存储来存储来自不同系统的新数据。

通过数据存储模块，您可以添加、替换、更新、检索、删除、搜索或计数您的记录。 [!DNL Adobe Workfront Fusion] 数据存储。

有关创建、编辑数据存储以及对其进行故障诊断的信息，请参阅 [数据存储位置 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

有关Workfront Fusion中数据存储的视频介绍，请参阅：

* [数据存储](https://video.tv.adobe.com/v/3427029/){target=_blank}

## 访问要求

您必须具有以下权限才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td>
  <td> <p>[！UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td>
   <td> <p>[！UICONTROL计划]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td> 
   <td>
   <p>当前许可证要求：否 [!DNL Workfront Fusion] 许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] 对于工作自动化和集成]，[！UICONTROL [!DNL Workfront Fusion] 工作自动化]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 计划，您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 计划。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关的信息 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 先决条件

使用 [!UICONTROL 数据存储] 模块，必须先创建数据存储。

有关创建数据存储的信息，请参阅 [数据存储位置 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

## [!UICONTROL 数据存储] 模块及其字段

配置数据存储模块时， [!DNL Workfront Fusion] 显示下面列出的字段。 除此之外，还可能会显示其他数据存储字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

全部 [!UICONTROL 数据存储] 模块是操作类型模块。

* [添加/替换记录](#addreplace-a-record)
* [更新记录](#update-a-record)
* [获取记录](#get-a-record)
* [检查记录是否存在](#check-the-existence-of-a-record)
* [删除记录](#delete-a-record)
* [删除所有记录](#delete-all-records)
* [搜索记录](#search-records)
* [对记录计数](#count-records)

### [!UICONTROL 添加/替换记录]

此操作模块添加或替换记录。

指定数据存储和记录的键。

该模块返回记录ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

>[!NOTE]
>
>当您尝试添加已存在于数据存储中的记录时，模块会引发错误，该记录以相同的名称和 [!UICONTROL 覆盖现有记录] 选项已禁用。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL数据存储]</td> 
   <td> <p> 选择或添加要在其中创建记录的数据存储。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Key] </td> 
   <td> <p>输入您希望模块添加或替换的记录的唯一键。 该键以后可用于检索记录。 如果将此字段留空，则会自动生成键。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL覆盖现有记录] </td> 
   <td> <p>启用此选项以覆盖记录。 要覆盖的记录必须在上面的“键”字段中指定。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL记录] </td> 
   <td> <p>在记录的字段中输入所需的值。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 更新记录]

此操作模块更新记录。

指定数据存储和记录的键。

该模块返回记录ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL数据存储]</td> 
   <td> <p> 选择或添加要在其中创建记录的数据存储。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Key] </td> 
   <td> <p>输入您希望模块更新的记录的唯一键。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Insert missing record] </td> 
   <td> <p>启用此选项以在具有指定键的记录不存在时创建新记录。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL记录]</td> 
   <td> <p> 在要更新的记录字段中输入所需的值。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 获取记录]

此操作模块可检索记录。

指定数据存储和记录的键。

该模块返回记录ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL数据存储]</td> 
   <td> <p> 选择要从中检索记录的数据存储</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Key] </td> 
   <td> <p>输入您希望模块检索的记录的唯一键值。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 检查记录是否存在]

此操作模块指定特定记录是否存在。

指定数据存储和记录的键。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL数据存储] </td> 
   <td> <p>选择要检查记录是否存在的数据存储。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Key] </td> 
   <td> <p>输入您希望模块检查是否存在记录的唯一键。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 删除记录]

此操作模块删除记录。

指定数据存储和记录的键。

该模块返回记录ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL数据存储] </td> 
   <td> <p>选择要检查记录是否存在的数据存储。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Key] </td> 
   <td> <p>输入您希望模块删除的记录的唯一键值。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 删除所有记录]

此操作模块会从特定数据存储中删除所有记录。

您指定数据存储。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL数据存储] </td> 
   <td> <p>选择要从中删除所有记录的数据存储。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 搜索记录]

此搜索模块在数据存储区中查找与您指定的搜索查询匹配的对象中的记录。

您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL数据存储]</td> 
   <td> <p> 选择要搜索的数据存储。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL筛选器]</p> </td> 
   <td> <p>为搜索设置过滤器。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL排序]</p> </td> 
   <td> <p style="font-weight: normal;">对于要作为排序依据的每个字段，请填写以下字段：</p> <p style="font-weight: bold;">[！UICONTROL Key]</p> <p>选择要作为结果排序依据的列名。</p> <p style="font-weight: bold;">[！UICONTROL顺序]</p> <p>选择是否要以升序或降序对结果进行排序。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL限制]</td> 
   <td> <p> 设置搜索结果的最大数量 [!DNL Workfront Fusion] 在一个执行周期内返回。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL即使模块未返回任何结果，仍继续执行路由]</td> 
   <td> <p> 如果启用，则此模块所属的路由将继续处理，即使此模块未返回任何结果。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 对记录计数]

此操作模块对数据存储中的记录进行编号。

您指定数据存储。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL数据存储] </td> 
   <td> <p>选择包含要计数的记录的数据存储。</p> </td> 
  </tr> 
 </tbody> 
</table>
