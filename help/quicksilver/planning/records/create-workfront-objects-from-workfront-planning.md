---
title: 在将Workfront对象连接到记录时，从Workfront Planning创建这些对象
description: 在从Workfront Planning中的其他记录连接对象时，您可以创建Workfront对象类型。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7c3db950-4cd9-424c-a7a7-4fa7dfa995f6
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '1101'
ht-degree: 2%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# 在将Workfront对象连接到记录时，从Workfront Planning创建这些对象

<!-- update the title (and all the links to this article) at preview, to be this: Create Workfront objects from Workfront Planning as you connect them to records-->
<!-- remove preview and production at release time-->

<span class="preview">此页面上突出显示的信息是指尚未普遍可用的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

您可以通过以下方式从Workfront Planning创建Adobe Workfront对象：

* 从Planning记录连接Workfront对象时

  本文介绍了在从Planning记录连接Workfront对象时，如何从Workfront Planning创建这些对象。
* 当您从记录的页面使用自动化时。

  有关使用自动化创建Workfront对象的信息，请参阅[使用Adobe Workfront Planning记录自动化创建对象](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md)。

将Workfront记录与以下Workfront对象类型连接时，您可以从Workfront Planning创建以下Workfront对象类型：

* 项目
* 项目组合
* 项目群

>[!IMPORTANT]
>
>* 从记录中连接项目、项目组合和项目群时，只能在Workfront中创建它们。
>
>* 从Workfront Planning中的记录连接组或公司时，无法创建组或公司。
>

您可以在Workfront Planning的以下区域的连接字段中连接项目、项目组合和程序：

* 记录类型的表格视图
* 记录的详细信息页面或预览框
* 记录的“连接”选项卡

有关将Planning记录与Workfront对象连接的信息，请参阅[连接记录](/help/quicksilver/planning/records/connect-records.md)。

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
   <td> 标准
   <p>Workfront计划不适用于旧版Workfront许可证</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td> <p>Adobe Workfront Planning没有访问级别控制</p> 
   <p>编辑访问权限，访问权限：在Workfront中为要创建的对象类型（项目、项目组合、项目群）创建对象。 </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td> <p>管理工作区<span class="preview">的权限和要添加记录的记录类型</span>。 </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>
   <p>管理Workfront对象（项目组合）的权限以添加子对象（项目）。</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面模板</p></td> 
   <td> <p>在生产环境中，必须将所有用户（包括系统管理员）分配到包含Planning的布局模板。</p>
<p><span class="preview">在“预览”环境中，标准用户和系统管理员默认启用Planning。</span></p> </td> 
  </tr> 
</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 将Workfront对象与Workfront Planning中的记录连接时创建这些对象的先决条件

您必须具备以下条件，才能通过从现有记录连接项目或项目组合来添加新项目或项目组合：

* 记录连接到Workfront项目、项目组合或项目的类型。 有关信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。
* 记录。 有关信息，请参阅[创建记录](/help/quicksilver/planning/records/create-records.md)。
* Workfront Planning和Workfront中的正确访问和权限，如本文的[访问要求](#access-requirements)部分所述。

## 将项目与Workfront Planning中的记录连接时创建项目

要在从其他记录连接项目时创建项目，请执行以下操作：

1. 转到记录的详细信息页面或记录类型的表，然后开始将Workfront Planning记录与Workfront项目连接，如文章[连接记录](/help/quicksilver/planning/records/connect-records.md)中所述。

1. （视情况而定）单击&#x200B;**添加项目**
或
开始键入项目的名称，如果找不到，请单击&#x200B;**添加项目**。 添加按钮后跟您键入的项目名称。

   ![从连接字段连接项目时添加项目](assets/add-project-when-connecting-it-from-connection-field.png)

   将打开&#x200B;**创建项目**&#x200B;框。

1. （可选）更新&#x200B;**项目名称**。 默认情况下，从记录中连接项目时，将按照您作为搜索项添加的内容来命名项目。
1. （可选）选择&#x200B;**项目模板**。 如果不选择模板，Workfront将创建一个不含任务的空白项目。
1. 单击&#x200B;**创建**。
1. （视情况而定）如果您选择从模板创建项目，请按照文章[使用模板创建项目](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md)中的步骤完成添加项目。

   将创建新项目并将其添加到所选记录的已连接字段中。

1. （可选）在Workfront规划中单击新项目的名称，以在Workfront中打开项目页面，并对项目进行其他更新。

## 将项目组合与Workfront Planning中的记录连接时创建项目组合

要在从Planning记录连接项目组合时创建项目组合，请执行以下操作：

1. 转到记录的详细信息页面或记录类型的表，然后开始将Workfront Planning记录与Workfront项目组合连接，如文章[连接记录](/help/quicksilver/planning/records/connect-records.md)中所述。

1. （视情况而定）单击&#x200B;**添加项目组合**

   或

   开始键入项目组合的名称，如果找不到，请单击&#x200B;**添加项目组合**。 “添加”按钮后跟您键入的项目组合名称。

   ![从连接字段连接项目组合时添加项目组合](assets/add-portfolio-when-connecting-it-from-connection-field.png)

   将创建项目组合并将其添加到所选记录的连接字段。

1. （可选）在Workfront Planning中单击新项目组合的名称，以在Workfront中打开项目组合页面，并对项目组合进行其他更新。

## 在将程序与Workfront Planning中的记录连接时创建程序

要在从Planning记录连接程序时创建程序，请执行以下操作：

1. 转到记录的详细信息页面或记录类型的表，然后开始将Workfront Planning记录与Workfront项目组合连接，如文章[连接记录](/help/quicksilver/planning/records/connect-records.md)中所述。

1. 单击&#x200B;**添加程序**

   或

   开始键入项目的名称，如果找不到，请单击&#x200B;**添加项目**。 “添加”按钮后跟您键入的程序名。

   ![从连接字段连接Workfront程序时添加该程序](assets/add-wf-program-when-connecting-it-from-connection-field.png)

   将打开&#x200B;**创建程序**&#x200B;框。

1. 更新&#x200B;**项目名称**。 这是必填字段。
1. 从下拉列表中选择&#x200B;**Portfolio**，或者开始键入项目组合的名称，然后在此项目组合显示在列表中时将其选定。 这是必填字段。
1. 单击&#x200B;**创建**。

   将创建项目并将其添加到所选记录的连接字段中。

1. （可选）单击Workfront Planning中新项目的名称，以在Workfront中打开该项目页面，并对其做出其他更新。

