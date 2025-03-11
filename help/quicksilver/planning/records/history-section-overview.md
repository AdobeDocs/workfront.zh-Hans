---
title: “历史记录”部分概述
description: 您可以在Adobe Workfront Planning中记录的右侧面板中查看对记录所做的更改并由系统记录。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8258589f-a7c3-4d77-9abe-c99e9184bd21
source-git-commit: fd8e5d3baf6af0dbdd1275494fad54b204abd1a5
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 3%

---

# “历史记录”部分概述

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>-->

{{planning-important-intro}}

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Workfront Planning records" should be there-->

通过在记录的右侧面板中添加评论或回复，您可以对Adobe Workfront Planning记录进行协作。 您还可以在此区域查看对记录所做的其他更改以及系统记录的更改。

记录的右侧面板显示以下部分：

* **个评论**：显示评论和用户添加到记录的回复。 有关管理Workfront Planning记录中的注释的更多信息，请参阅[管理记录注释](/help/quicksilver/planning/records/manage-record-comments.md)。
* **历史记录**：显示用户对记录字段进行的系统记录更改。

## 访问要求

+++ 展开以查看访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> 产品</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront规划<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront计划*</p></td> 
   <td> 
<p>以下任意Workfront计划：</p> 
<ul><li>选择</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning不适用于旧版Workfront计划</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront规划包*</p></td> 
   <td> 
<p>任何 </p> 
<p>有关每个Workfront计划中包括的内容的更多信息，请联系您的Workfront客户经理。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>贵组织的Workfront实例必须载入Adobe Unified Experience，才能访问Workfront Planning的所有功能。</p> 
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">适用于Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td> 
   <td> <p>标准</p>
   <p>Workfront计划不适用于旧版Workfront许可证</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td> <p>Adobe Workfront Planning没有访问级别控制</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>   <p>查看工作区<!--<span class="preview">and record type</span>-->或更高权限</a> </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>布局模板</p></td> 
   <td> <p>必须为所有用户(包括Workfront管理员)分配一个布局模板，该模板应包括主菜单中的Planning区域。 </p> </td> 
  </tr> 
</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 找到记录的“历史记录”部分

{{step1-to-planning}}

1. 单击工作区的卡片。

   工作区将打开，记录类型显示在信息卡上。

1. 单击记录类型卡片。
此时将打开记录类型页面，并显示该类型的所有记录。

1. 从任何视图中，单击记录的名称。

   此时将打开记录的页面。 默认情况下，“注释”区域会在右侧面板中打开。
1. 单击&#x200B;**显示历史记录**&#x200B;图标![](assets/show-history-icon.png)。 对记录字段所做的所有更改都将显示在右侧面板中，从最近的更改开始。
1. （可选）单击&#x200B;**隐藏历史记录**&#x200B;图标![](assets/hide-history-icon.png)以关闭右侧面板。

## 有关“历史记录”部分的注意事项

您可以在记录页面的右侧面板的“历史记录”部分中查看对记录字段所做的更改。

![](assets/history-area-in-comments.png)

* Workfront Planning会在“历史记录”部分中记录以下信息：

   * 任何字段更改

   * 字段的旧值和新值（当值更改时）。 旧值以删除线格式显示。

   * 进行更改的用户的全名

   * 更改发生的日期和时间戳。

* 以下类型的字段始终显示旧值（以删除线格式）和新值：

   * 文本
   * 段落
   * 货币
   * 日期
   * 数字
   * 百分比
   * 单选

* 仅当删除了多个值中的至少一个值时，以下类型的字段才会以删除线格式显示旧值：

   * 多选
   * 链接的记录字段
   * 人员

  如果更改仅向字段添加了值，则旧值不会显示，而仅显示新字段值。

* 复选框类型的字段从不以删除线格式显示旧值。 如果字段已编辑，则仅显示进行更改时的当前状态。

  有关Workfront Planning字段的更多信息，请参阅[创建字段](/help/quicksilver/planning/fields/create-fields.md)。

* 对以下类型的字段所做的更改不会显示在“历史记录”部分中：

   * 链接（查找）字段
   * 公式
   * 创建者
   * 创建日期
   * 上次修改者
   * 上次修改日期

* 如果从系统中删除某个字段，则对该字段所做的更新将保留在“历史记录”部分中。 没有迹象表明记录的History部分中已移除该字段。
