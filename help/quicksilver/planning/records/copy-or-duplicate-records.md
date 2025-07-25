---
title: 重复记录
description: 您可以在表视图中复制现有记录。 现有记录的相同副本将添加到记录类型页面。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2fed8c96-0c9c-4662-a9c4-66dae507ff2a
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 2%

---

# 重复记录

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

在Adobe Workfront Planning中，记录是记录类型的实例。

您可以在表视图中复制现有记录。 现有记录的相同副本将添加到记录类型页面。

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
<p>贵组织的Workfront实例必须载入Adobe Unified Experience才能访问Workfront Planning。</p> 
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">适用于Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td> 
   <td><p> 标准</p>
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
   <td>   <p>为工作区和记录类型贡献或更高权限</a> </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p> </td> 
  </tr> 
</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


## 复制记录<!--in a record type table (I don't think you can create them elsewhere right now)-->

通过复制现有记录，可以在记录类型页面的表视图中创建记录。 在原始记录下创建并添加与现有记录相同的记录。


{{step1-to-planning}}

1. 单击要在其中添加记录的工作区。

   工作区将打开，记录类型显示为卡片。

1. 单击记录类型卡片。 有关创建记录类型的信息，请参阅[创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)。

   记录类型页面将在您上次访问的视图中打开。 默认情况下，将在表格视图中打开记录类型页面。
所选类型的所有记录都将显示在视图中。

1. （视情况而定）选择表视图。

1. 执行下列操作之一：

   * 将鼠标悬停在记录名称上，然后单击与记录名称内联的&#x200B;**更多**&#x200B;菜单，然后单击&#x200B;**复制**&#x200B;图标![灰色复制图标](assets/duplicate-icon-gray.png) 。

     表格视图中记录的![更多菜单](assets/more-menu-from-record-in-table-view.png)

   * 选择记录，然后单击页面底部工具栏中的&#x200B;**复制**&#x200B;图标![白色和蓝色复制图标](assets/duplicate-icon-white-and-blue.png)。

     ![表格视图中工具栏中的图标重复](assets/duplicate-icon-in-toolbar-in-table-view.png)

   在原始记录下创建具有相同名称的相同记录。 新记录的所有字段均填充有与原始记录相同的信息。

1. （可选）在表格视图中的可用字段中开始更新有关新记录的信息，或在记录预览或页面中单击该记录和更新信息。

   >[!NOTE]
   >
   >  * 记录没有必填字段。 但是，我们建议您为记录的主要字段添加信息，因为在将记录相互链接时，识别记录会很有帮助。 有关主字段的详细信息，请参阅[管理表视图](/help/quicksilver/planning/views/manage-the-table-view.md)和[主字段概述](/help/quicksilver/planning/fields/primary-field-overview.md)。
   >
   >  * 引用其他记录类型或计算字段的字段为只读字段。

   有关编辑记录的详细信息，请参阅[编辑记录](/help/quicksilver/planning/records/edit-records.md)。

1. （可选）在将新记录或其信息添加到表视图时，使用以下键盘快捷键可撤消或重做添加新记录或其信息：

   * 按CTRL + Z (⌘ + Z表示Mac)可撤消更改
   * 按CTRL + Shift + Z (⌘ + Shift + Z用于Mac)以重做更改。
