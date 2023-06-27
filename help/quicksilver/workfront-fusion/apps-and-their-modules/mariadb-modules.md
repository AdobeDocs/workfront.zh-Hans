---
title: MariaDB模块
description: 在 [!DNL Adobe Workfront Fusion] 场景，您可以自动执行使用 [!DNL MariaDB]，并将其连接到多个第三方应用程序和服务。
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 45d4d7fe-a70c-4906-adb4-f913a870fe47
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '593'
ht-degree: 1%

---

# [!DNL MariaDB] 模块

在 [!DNL Adobe Workfront Fusion] 场景，您可以自动执行使用 [!DNL MariaDB]，并将其连接到多个第三方应用程序和服务。

如果您需要有关创建方案的说明，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

有关模块的信息，请参见 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] 用于工作自动化和集成] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 计划，您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 计划。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关以下项的信息 [!DNL Adobe Workfront Fusion] 许可证，请参见 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 先决条件

使用 [!DNL MariaDB] 模块，您必须具有 [!DNL MariaDB] 帐户。

## Connect [!DNL MariaDB] 到 [!DNL Workfront Fusion]

您可以创建与 [!DNL MariaDB] 直接从 [!DNL MariaDB] 模块。

1. 在任意 [!DNL MariaDB] 模块，单击 **[!UICONTROL 添加]** 旁边的 [!UICONTROL 连接] 字段。
1. 配置以下字段：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL连接名称]</p> </td> 
      <td> <p>输入新连接的名称。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL主机]</td> 
      <td> <p>输入数据库实例的IP地址或主机名。 此主机必须可从网络外部访问。</p> <p>示例: <code>[!DNL mariadb.hwoh2j5h.us-east-1.rds.amazon.com]</code></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL端口]</td> 
      <td>默认端口为3306。 如果您使用的是非标准端口，请将此数字设置为您的端口。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL数据库名称]</td> 
      <td>输入要与之交互的数据库名称。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL用户名]</td> 
      <td>输入您的用户名.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL密码]</td> 
      <td>输入您的密码。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **[!UICONTROL 继续]** 以创建连接并返回模块。

## [!DNL MariaDB] 模块及其字段

配置时 [!DNL MariaDB] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除此以外，还有 [!DNL MariaDB] 可能会显示字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### 执行查询（高级）

此操作模块根据您提供的查询从数据库中检索信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td>有关连接 [!DNL MariaDB] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">Connect [!DNL MariaDB] 到 [!DNL Workfront Fusion]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查询]</td> 
   <td> <p>输入您希望模块用于检索数据的SQL查询。</p> <p>重要信息：查询中使用的变量不会经过清理。 确保正确清理变量以防止SQL注入。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 从表中选择行（高级）]

此模块从数据库中读取记录。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td>有关连接 [!DNL MariaDB] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">Connect [!DNL MariaDB] 到 [!DNL Workfront Fusion]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL表]</td> 
   <td> <p>选择包含要读取的记录的表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL筛选器]</td> 
   <td> <p>设置选择行所依据的筛选器</p> 
    <ul> 
     <li> <p>选择要作为搜索依据的字段</p> </li> 
     <li> <p>选择要用于搜索的运算符</p> </li> 
     <li> <p>输入或映射要搜索的值。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL排序] </td> 
   <td> <p>对于希望按其排序结果的每个级别，单击 <strong>[！UICONTROL添加项]</strong>，然后选择要作为结果排序依据的字段以及要按升序还是按降序排序</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>
