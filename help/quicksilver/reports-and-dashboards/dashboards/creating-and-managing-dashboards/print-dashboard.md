---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: 打印功能板
description: 可以将仪表板打印或导出到。PDF文件。 要打印仪表板，您必须具有查看仪表板的权限。
author: Nolan
feature: Reports and Dashboards
exl-id: 30f3481b-23b6-4dc9-be0d-9cffd5d4dfed
source-git-commit: a9abbeaa9abd0e905c60000a218eddb85d0389b9
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# 打印功能板

<!-- Audited: 1/2025 -->

可以将仪表板打印或导出到。PDF文件。 要打印仪表板，您必须具有查看仪表板的权限。

>[!NOTE]
>
>此功能仅用于标准“仪表板”视图。 它不适用于嵌入到项目区域或设置为自定义选项卡的仪表板。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront计划</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront许可证</strong></td> 
      <td> 
      <p>新增：</p>
         <ul>
         <li><p>标准</p></li>
         </ul>
      <p>当前：</p>
         <ul>
         <li><p>工作或更高</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置</strong></td> 
   <td> <p>查看对报告、功能板和日历的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong>/td&gt; 
   <td> <p>查看仪表板的权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

必须先创建仪表板，然后才能打印它。

有关创建功能板的信息，请参阅[创建功能板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md)。

## 了解打印仪表板时打印的信息

当打印仪表板或将其另存为。PDF文件时，仪表板的某些信息(如Adobe Workfront Web应用程序中的信息)可能不会显示在打印或导出的文件中。

* [显示什么？](#what-is-displayed)
* [哪些内容未显示？](#what-is-not-displayed)

### 将显示什么？ {#what-is-displayed}

以下信息包含在打印或导出的仪表板文件中：

* 仪表板标题
* 报告标题
* 上次生成报告的时间戳
* 仪表板上的所有对象，包括列表视图、外部网页、报告和日历
* 贵公司的徽标(如果Workfront管理员已在全局导航栏中对其进行自定义)。 有关将Workfront网站品牌化的详细信息，请参阅[将Adobe Workfront实例品牌化](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md)。

### 哪些内容未显示？ {#what-is-not-displayed}

以下信息不包括在打印或导出的仪表板文件中：

* Workfront导航栏
* 特定于Workfront的任何其他格式
* 根据报表的大小以及单个列的数量和宽度，导出和打印仪表板可能会导致某些列被截断。

## 打印功能板

1. 转到要打印的仪表板。
1. 执行以下任一操作：

   * 单击&#x200B;**仪表板操作** > **打印预览**

   * 按&#x200B;**Ctrl+P**（在Windows上）或&#x200B;**Command+P**(在Mac上)

     >[!IMPORTANT]
     >
     >* 当仪表板嵌入到自定义选项卡中时，这两个选项均不可用。 有关创建自定义选项卡的信息，请参阅[创建自定义选项卡或分区](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md)。
     >* 使用Internet Explorer浏览器时，键盘快捷键选项不可用。

1. 在&#x200B;**目标**&#x200B;字段中，从各种可用的打印选项中进行选择。\
   根据您使用的浏览器和浏览器版本，打印选项会有所不同。

1. （可选）将仪表板另存为。PDF文件，然后单击&#x200B;**保存**&#x200B;以保存。PDF。\
   要了解如何将仪表板另存为。PDF文件，请参阅[导出仪表板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md)。

1. 单击&#x200B;**打印**。
