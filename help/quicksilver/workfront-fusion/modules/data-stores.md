---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: 数据存储位置 [!DNL Adobe Workfront Fusion]
description: 数据存储类似于数据库或简单表，可以存储场景中的数据，从而可以在单独的场景或场景运行之间传输数据。 在同步过程中，您可以使用数据存储来存储来自不同系统的新数据。
author: Becky
feature: Workfront Fusion
exl-id: 2a665a71-b819-4861-b119-f5c28b87e9c5
source-git-commit: 85e5483b7ee1433d0b1efbaa37c6d55c7c1d5bf7
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 1%

---

# 数据存储位置 [!DNL Adobe Workfront Fusion]

数据存储类似于数据库或简单表，可以存储场景中的数据，从而可以在单独的场景或场景运行之间传输数据。 在同步过程中，您可以使用数据存储来存储来自不同系统的新数据。

通过数据存储模块，您可以对中的记录执行以下操作 [!DNL Adobe Workfront Fusion] 数据存储：

* 添加
* 替换
* 更新
* Retrieve
* 删除
* 搜索
* 计数

有关使用数据存储模块的信息，请参阅 [[!UICONTROL 数据存储] 模块](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

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
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[！UICONTROL计划]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]许可证**</td> 
   <td>
   <p>当前许可证要求：否 [!DNL Workfront Fusion] 许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] 用于工作自动化和集成] </p>
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

## 在中创建数据存储 [!DNL Workfront Fusion]

* [设置数据存储](#set-up-the-data-store)
* [设置数据结构](#set-up-the-data-structure)

### 设置数据存储

在模块中使用数据存储之前，必须先在中创建数据存储 [!DNL Workfront Fusion].

>[!NOTE]
>
>您的组织的可用数据存储数量有限。 如果您尝试创建的数据存储区多于可用的数据存储区， [!DNL Workfront] 返回 [!UICONTROL 已达到最大商店数] 错误。
>
>有关更多信息，请参阅 [已达到最大存储数错误](#maximum-stores-reached-error) 本文章中。

1. 登录 [!DNL Workfront Fusion] 帐户。
1. 单击 **[!UICONTROL 数据存储]** （在左侧导航面板中）。
1. 单击 **[!UICONTROL 添加数据存储]** 屏幕右上角的。
1. 输入新数据存储的设置。

   中的字段上的粗体标题 [!DNL Workfront Fusion] 模块指示所需的设置。

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[！UICONTROL数据存储名称] </td> 
      <td> <p>输入数据存储的名称。 </p> </td> 
     </tr> 
     <tr> 
      <td> <p>[！UICONTROL Data Structure]</p> </td> 
      <td> <p>数据结构是表的列的列表。 此列表指示列名和数据类型。</p> <p>执行下列操作之一：</p> 
       <ul> 
        <li style="font-weight: bold;">选择已创建的数据结构</li> 
        <li> <p style="font-weight: bold;">添加新数据结构</p> <p>单击 <strong>[！UICONTROL添加]</strong> 以创建新数据结构。</p> <p>欲了解更多信息，请参见 <a href="#set-up-the-data-structure" class="MCXref xref">设置数据结构</a> 部分。</p> </li> 
        <li style="font-weight: bold;"> <p>将此字段留空</p> <p style="font-weight: normal;">如果不选择或添加数据结构，则数据库将仅包含主键。 如果您只想保存密钥，并且只想知道数据库中是否存在特定密钥，则此类数据库类型很有用。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td> <p>[！UICONTROL数据存储大小(MB)</p> </td> 
      <td> <p>从内部数据存储总量中分配数据存储的大小。</p> <p> 默认值为10 MB。 如果您未分配的数据存储空间少于10 MB（分配给95 MB的空间），则默认大小为未分配的存储量。  <p>注：保留金额可以随时更改。</p>  </td> 
     </tr> 
    </tbody> 
   </table>

### 设置数据结构

1. 创建或编辑数据存储时，单击 **[!UICONTROL 添加]**.
1. 在 **[!UICONTROL 添加数据结构]** 框中，配置以下字段：

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[！UICONTROL数据结构名称]</td> 
      <td> <p> 输入新数据结构的名称。</p> </td> 
     </tr> 
     <tr> 
      <td> <p>[！UICONTROL规范]</p> </td> 
      <td> <p>执行以下操作之一来设置数据存储列。</p> 
       <ul> 
        <li> <p>单击 <strong>[！UICONTROL添加项]</strong> 以手动指定一列的属性。</p> <p>输入 <strong>[！UICONTROL名称]</strong> 和 <strong>[！UICONTROL类型]</strong> 数据存储列并定义相应的属性。</p> </li> 
        <li> <p>单击 <strong>[！UICONTROL Generator]</strong> 以确定来自您提供的示例数据的列。</p> 
         <div class="example" data-mc-autonum="<b>Example: </b>">
          <span class="autonumber"><span><b>示例： </b></span></span> 
          <p>例如，以下JSON示例数据创建三列：姓名、年龄和电话号码。 电话号码是手机和固定电话号码的集合。</p> 
          <p><code>&lbrace;</code> </p> 
          <p><code>"name":"John",</code> </p> 
          <p><code>"age":30,</code> </p> 
          <p><code>"phone number": &lbrace;</code> </p> 
          <p><code>"mobile":"987654321",</code> </p> 
          <p><code>"landline":"123456789"</code> </p> 
          <p><code>&rbrace;</code> </p> 
          <p><code>&rbrace;</code> </p> 
          <p>数据存储视图中的空列：</p> 
          <p> <img src="assets/empty-columns-350x132.png" style="width: 350;height: 132;"> </p> 
          <p>然后，您可以手动或使用向数据存储添加值 [!DNL Workfront Fusion] 数据存储模块。</p> 
         </div> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL严格] </td> 
      <td> <p>启用此选项以确保有效负载与数据结构匹配。 包含未在数据结构中指定的额外项的有效负载将被拒绝。</p> </td> 
     </tr> 
    </tbody> 
   </table>

## 编辑现有数据存储

您可以在中编辑现有数据存储的属性和内容 [!UICONTROL 数据存储] 面积 [!DNL Workfront Fusion].

* [编辑数据存储的属性](#edit-the-properties-of-a-data-store)
* [编辑数据存储的内容](#edit-the-contents-of-a-data-store)

### 编辑数据存储的属性

数据存储的属性包括数据存储使用的数据结构以及数据存储的大小。

1. 单击 **[!UICONTROL 数据存储]** ![](assets/data-store-icon.png) 在左侧导航面板中打开 [!UICONTROL 数据存储] 区域。
1. 单击 **[!UICONTROL 编辑]** ![](assets/data-store-edit.png) ，位于要编辑的数据存储区旁边。
1. （可选）如果要将此数据存储使用的数据结构更改为其他现有数据结构，请从 **[!UICONTROL 数据结构]** 下拉菜单。

   或

   （可选）如果要将此数据存储使用的数据结构更改为全新的数据结构，请参阅 [设置数据结构](#set-up-the-data-structure) 本文章中。

1. （可选）通过将新大小输入到 **[!UICONTROL 数据存储大小(MB)]** 字段。
1. 单击&#x200B;**[!UICONTROL 保存]**。

### 编辑数据存储的内容

1. 单击 **[!UICONTROL 数据存储]** 图标 ![](assets/data-store-icon.png) 在左侧导航面板中打开 [!UICONTROL 数据存储] 区域。
1. 单击 **[!UICONTROL 浏览]**  ，位于要编辑的数据存储区旁边。
1. （可选）通过将列拖动到所需位置来重新排列列。
1. （可选） [!UICONTROL 编辑] 通过单击 **[!UICONTROL 编辑]** 图标，然后输入所需的值。
1. （可选）通过单击向数据存储添加新项 **[!UICONTROL 添加]**，然后输入新项目的信息。
1. 单击&#x200B;**[!UICONTROL 保存]**。

## 故障排除

* [从数据存储中恢复丢失的数据](#restoring-lost-data-from-a-data-store)
* [空间不足错误](#out-of-space-error)
* [已达到最大存储数错误](#maximum-stores-reached-error)

### 从数据存储中恢复丢失的数据

目前没有可以自动恢复丢失数据的工具。

#### 解决方法

1. 检查将项目插入数据存储的所有方案的执行日志。

   有关检查执行日志的详细信息，请参见 [在中查看方案的执行历史记录 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-scenario-execution-history.md).

1. 复制数据。
1. 再次将数据插入数据存储。

   有关将数据插入数据存储的信息，请参阅 [编辑数据存储的内容](#edit-the-contents-of-a-data-store) 本文章中。

### [!UICONTROL 空间不足] 错误

An [!UICONTROL 空间不足] 发生此错误，因为之前创建的数据存储已分配给您分配的数据存储存储。

#### 解决方法

1. 编辑任何现有数据存储以使用更少的空间。 这样可释放空间给您的新数据存储。

   有关更多信息，请参阅 [编辑数据存储的属性](#edit-the-properties-of-a-data-store) 本文章中。

>[!NOTE]
>
>我们建议您不要将所有空间分配给单个数据存储，除非您确定不需要更多数据存储。

### [!UICONTROL 已达到最大商店数] 错误

A [!UICONTROL 已达到最大商店数] 发生此错误是因为您的组织已使用其所有可用的数据存储。 组织有许多可用数据存储，其数量相当于可用场景数量的两倍。 因此，可用数据存储的总数取决于您购买的计划。

例如，如果贵组织购买了包含15种方案的计划，则最多可以拥有30个数据存储。

#### 解决方法

要减少现有数据存储的数量，请考虑执行以下操作之一：

* 合并现有数据存储
* 删除未使用的数据存储
