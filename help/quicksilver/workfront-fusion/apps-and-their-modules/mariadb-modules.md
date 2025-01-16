---
title: MariaDB模块
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 45d4d7fe-a70c-4906-adb4-f913a870fe47
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# [!DNL MariaDB]模块

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* [MariaDB模块](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/mariadb-modules.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

在[!DNL Adobe Workfront Fusion]方案中，您可以自动使用[!DNL MariaDB]的工作流，并将其连接到多个第三方应用程序和服务。

如果需要有关创建方案的说明，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)中创建方案。

有关模块的信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)中的[模块。

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
   <p>当前许可证要求：无[!DNL Workfront Fusion]许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]计划，则贵组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]才能使用本文中描述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]计划中。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]，才能使用本文中介绍的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 先决条件

要使用[!DNL MariaDB]模块，您必须具有[!DNL MariaDB]帐户。

## 将[!DNL MariaDB]连接到[!DNL Workfront Fusion]

您可以在[!DNL MariaDB]模块内直接创建与[!DNL MariaDB]帐户的连接。

1. 在任意[!DNL MariaDB]模块中，单击[!UICONTROL 连接]字段旁边的&#x200B;**[!UICONTROL 添加]**。
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
      <td> <p>输入数据库实例的IP地址或主机名。 此主机必须可从网络外部访问。</p> <p>示例： <code>[!DNL mariadb.hwoh2j5h.us-east-1.rds.amazon.com]</code></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL端口]</td> 
      <td>默认端口为3306。 如果您使用的是非标准端口，请将此号码设置为您的端口。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL数据库名称]</td> 
      <td>输入要与之交互的数据库名称。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL用户名]</td> 
      <td>输入您的用户名。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL密码]</td> 
      <td>输入密码。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**[!UICONTROL 继续]**&#x200B;以创建连接并返回模块。

## [!DNL MariaDB]模块及其字段

配置[!DNL MariaDB]模块时，[!DNL Workfront Fusion]显示下面列出的字段。 除此以外，可能还会显示其他[!DNL MariaDB]字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关详细信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中将信息从一个模块映射到另一个模块。

![](assets/map-toggle-350x74.png)

### 执行查询（高级）

此操作模块根据您提供的查询从数据库中检索信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>有关将[!DNL MariaDB]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">将[!DNL MariaDB]连接到[!DNL Workfront Fusion]</a>。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Query]</td> 
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
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>有关将[!DNL MariaDB]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">将[!DNL MariaDB]连接到[!DNL Workfront Fusion]</a>。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL表]</td> 
   <td> <p>选择包含要读取的记录的表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL筛选器]</td> 
   <td> <p>设置要按其选择行的筛选器</p> 
    <ul> 
     <li> <p>选择要作为搜索依据的字段</p> </li> 
     <li> <p>选择要用于搜索的运算符</p> </li> 
     <li> <p>输入或映射要搜索的值。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL排序] </td> 
   <td> <p>对于要作为结果排序依据的每个级别，单击<strong>[！UICONTROL添加项]</strong>，然后选择要作为结果排序依据的字段以及要按升序还是降序排序</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>
