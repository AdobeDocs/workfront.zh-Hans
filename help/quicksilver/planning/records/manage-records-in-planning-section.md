---
title: 管理Adobe Workfront对象的“计划”部分中的记录
description: 您可以在左侧面板的Workfront对象的Planning部分中显示连接到Adobe Workfront对象的Workfront Planning记录。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d86cf3f9-cacc-4457-acb3-a5122ae91be8
source-git-commit: 64a8d2ff8546874cf829738dcea03b2946c360cb
workflow-type: tm+mt
source-wordcount: '797'
ht-degree: 1%

---


<!--add also Group and Company when they are available-->

# 管理Adobe Workfront对象“计划”部分中的记录

{{planning-important-intro}}

您可以在左侧面板的Workfront对象的Planning部分中显示连接到Adobe Workfront对象的Workfront Planning记录。

“规划”部分适用于以下Workfront对象：

* 项目
* 项目组合
* 项目群
<!--* Group
* Company-->

## 访问要求

+++ 展开以查看Workfront Planning的访问要求。

您必须具备以下条件才能访问Workfront Planning：

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
   <td role="rowheader"><p>Adobe Workfront规划计划*</p></td>
   <td>
<p>任何</p>
<p>有关每个Workfront计划中包括的内容的更多信息，请联系您的Workfront客户经理。 </p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront平台</p></td>
   <td>
<p>贵组织的Workfront实例必须载入AdobeUnified Experience，才能访问Workfront Planning的所有功能。</p>
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">AdobeWorkfront的Unified Experience</a>。 </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td>
   <td>
   <p>标准</p>
   <p>Workfront计划不适用于旧版Workfront许可证</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>访问级别配置</p></td>
   <td> <p>查看或更高权限的项目、项目群和Portfolio</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>对象权限</p></td>
   <td>
   <p>在Workfront中，查看项目、项目组合或项目群的权限或更高的权限</a> </p> 
   <p>在Workfront Planning、Contribute或更高的工作区权限中</a> </p>  
   <p>系统管理员有权访问所有Workfront Planning工作区，包括他们未创建的工作区</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>必须为包括Workfront管理员在内的所有用户分配一个布局模板，该布局模板包括主菜单的“规划”区域以及项目、项目组合和项目群的“规划”区域。 </p> 有关详细信息，请参阅<a href="/help/quicksilver/planning/access/access-overview.md">访问概述</a>。 </p>  </p>  
</td>
  </tr>
 </tbody>
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 关于Workfront对象Planning部分的注意事项

当您从Workfront对象的Planning部分中查看Workfront Planning记录时，请考虑以下事项：

* Workfront Planning记录类型必须首先连接到Workfront对象类型。

  有关信息，请参阅以下文章：

   * [连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)
   * [连接记录](/help/quicksilver/planning/records/connect-records.md)
* 您可以从Workfront对象查看Planning部分，即使没有与Workfront对象关联的记录也是如此。
* 除了从Workfront的Planning区域连接Workfront对象之外，您还可以从Planning部分将Planning记录与Workfront的Workfront对象连接。

## 管理“计划”部分中的记录

{{step1-to-planning}}

1. 单击工作区的卡片。

   工作区将打开，记录类型显示为卡片。

1. 单击连接到Workfront项目、项目组合或项目群的记录类型的卡。
1. 在表格视图或记录的详细信息页面中，转到与Workfront对象有连接的已连接记录字段。 有关信息，请参阅[连接记录](/help/quicksilver/planning/records/connect-records.md)。
1. 在连接的记录字段中单击Workfront对象的名称。
对象的页面将在Workfront中打开。

   >[!NOTE]
   >
   >  如果您知道Workfront对象已连接到Planning记录，则可以从Workfront对象导航到Planning部分。

1. 单击左侧面板中的&#x200B;**Planning**。

   >[!NOTE]
   >
   >   您的Workfront或组管理员必须先将“规划”部分添加到您的布局模板中，然后才能为Workfront项目、项目组合或项目群显示规划部分。

   此时将显示Planning部分，其中包含下列信息：

   * 连接的记录显示在包含以下信息的各个卡片上：
      * 记录名称
      * 记录缩略图
      * 在Workfront Planning中显示的已连接记录字段的名称。
   * 记录会显示在各自的工作区中。

   ![](assets/planning-section-on-project.png)

1. （可选）单击“显示所有连接”****&#x200B;可显示所有连接的记录类型，包括未连接记录的记录类型。 默认情况下，不显示没有连接记录的记录类型。
1. 单击记录卡以显示有关记录的更多信息。 此时将显示记录预览框。
1. （可选）开始修改记录预览框中的字段。 您的更改会自动保存。
1. （可选）单击预览框右上角的&#x200B;**在新标签中打开**&#x200B;图标![](assets/open-details-in-a-new-tab-icon.png)以打开记录的详细信息页面。 此时将在Workfront Planning中打开记录的详细信息页面。
1. （可选）将鼠标悬停在记录卡片上，单击断开连接记录图标&#x200B;**-**，然后单击&#x200B;**断开连接**。
出现以下情况：
   * 记录不再连接到Workfront对象。
   * Workfront对象也将从Workfront Planning中的记录的“已连接”字段中删除。
   * 连接到Planning记录的Workfront查找字段的值也会被删除。
1. 单击&#x200B;**连接**&#x200B;为连接的记录类型连接更多记录。 有关详细信息，请参阅[连接记录](/help/quicksilver/planning/records/connect-records.md)。

   出现以下情况：

   * 记录会立即连接到Workfront对象，并显示在Planning部分中。
   * Workfront对象将添加到Workfront Planning记录的已连接字段中。
   * 连接到Planning记录的Workfront查找字段的值会在Workfront Planning中填充。


