---
title: 从Workfront Planning创建Workfront对象
description: 在从Workfront Planning中的其他记录连接对象时，您可以创建Workfront对象类型。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7c3db950-4cd9-424c-a7a7-4fa7dfa995f6
source-git-commit: fd8e5d3baf6af0dbdd1275494fad54b204abd1a5
workflow-type: tm+mt
source-wordcount: '1138'
ht-degree: 1%

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
* <span class="preview">当您从记录页面使用自动处理时。</span>

  <span class="preview">有关使用自动化创建Workfront对象的信息，请参阅[使用Adobe Workfront Planning记录自动化创建对象](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md)。</span>

将Workfront记录与以下Workfront对象类型连接时，您可以从Workfront Planning创建以下Workfront对象类型：

* 项目
* 项目组合
* <span class="preview">程序</span>

>[!IMPORTANT]
>
>* 从记录连接项目、项目组合和<span class="preview">程序</span>时，只能在Workfront中创建它们。
>
>* 从Workfront Planning中的记录连接组或公司时，无法创建组或公司。
>

您可以在Workfront Planning的以下区域的连接字段中连接项目、项目组合、<span class="preview">和程序</span>：

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
<p>贵组织的Workfront实例必须载入Adobe Unified Experience，才能访问Workfront Planning的所有功能。</p> 
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
   <p>在将记录连接到要创建的对象类型（项目、项目和项目组合）时，在Workfront中编辑对这些对象的访问权限。 </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td> <p>管理要添加记录的工作区<!--<span class="preview">and record type</span>-->的权限。 </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>
   <p>管理Workfront对象（项目组合）的权限以添加子对象（项目）。</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>布局模板</p></td> 
   <td> <p>必须为所有用户(包括Workfront管理员)分配一个布局模板，该模板应包括主菜单中的Planning区域 </p> </td> 
  </tr> 
</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 将Workfront对象与Workfront Planning中的记录连接时创建这些对象的先决条件

您必须具备以下条件，才能通过从现有记录连接项目或项目组合来添加新项目或项目组合：

* 记录类型连接到Workfront项目、项目组合或<span class="preview">项目</span>。 有关信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。
* 记录。 有关信息，请参阅[创建记录](/help/quicksilver/planning/records/create-records.md)。
* Workfront Planning和Workfront中的正确访问和权限，如本文的[访问要求](#access-requirements)部分所述。

## 将项目与Workfront Planning中的记录连接时创建项目

要在从其他记录连接项目时创建项目，请执行以下操作：

1. 转到记录的详细信息页面或记录类型的表，然后开始将Workfront Planning记录与Workfront项目连接，如文章[连接记录](/help/quicksilver/planning/records/connect-records.md)中所述。

1. （视情况而定） <span class="preview">单击&#x200B;**添加项目**</span>
或
开始键入项目的名称，如果找不到，请单击**添加项目**。

   如果尝试从其他记录的已连接记录字段添加项目时找不到该项目，请添加名称，然后单击&#x200B;**添加项目**。 添加按钮后跟您键入的项目名称。

   <!--at production or when the permanent Add button is released to preview, take the first part of the direction above out and say "Click Add to add a new project"; take this out too: "The Add button is followed by the project name you typed."-->

   ![从连接字段连接项目时添加项目](assets/add-project-when-connecting-it-from-connection-field.png)

   <span class="preview">将打开&#x200B;**创建项目**&#x200B;框。</span>

1. <span class="preview">（可选）更新&#x200B;**项目名称**。 默认情况下，从记录中连接项目时，将按照您作为搜索项添加的内容来命名项目。</span>
1. <span class="preview">（可选）选择&#x200B;**项目模板**。 如果不选择模板，Workfront将创建一个不含任务的空白项目。</span>
1. <span class="preview">单击&#x200B;**创建**。</span>
1. <span class="preview">（视情况而定）如果您选择从模板创建项目，请按照文章[使用模板创建项目](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md)中的步骤完成添加项目。</span>

   将创建新项目并将其添加到所选记录的已连接字段中。

1. （可选）在Workfront规划中单击新项目的名称，以在Workfront中打开项目页面，并对项目进行其他更新。

## 将项目组合与Workfront Planning中的记录连接时创建项目组合

要在从Planning记录连接项目组合时创建项目组合，请执行以下操作：

1. 转到记录的详细信息页面或记录类型的表，然后开始将Workfront Planning记录与Workfront项目组合连接，如文章[连接记录](/help/quicksilver/planning/records/connect-records.md)中所述。

   <!--at production or when the permanent Add button is released to preview, take the first part of the direction below out and say "Click Add to add a new portfolio"; take this out too: "The Add button is followed by the portfolio name you typed."-->

1. （视情况而定） <span class="preview">单击&#x200B;**添加项目组合**</span>

   或

   开始键入项目组合的名称，如果找不到，请单击&#x200B;**添加项目组合**。—>如果尝试从其他记录的已连接记录字段添加项目组合时找不到项目组合，请添加名称，然后单击&#x200B;**添加项目组合**。 “添加”按钮后面还有您键入的项目组合名称。

   ![从连接字段连接项目组合时添加项目组合](assets/add-portfolio-when-connecting-it-from-connection-field.png)

   将创建项目组合并将其添加到所选记录的连接字段。

1. （可选）在Workfront Planning中单击新项目组合的名称，以在Workfront中打开项目组合页面，并对项目组合进行其他更新。

<div class="preview">

## 在将程序与Workfront Planning中的记录连接时创建程序

要在从Planning记录连接程序时创建程序，请执行以下操作：

1. 转到记录的详细信息页面或记录类型的表，然后开始将Workfront Planning记录与Workfront项目组合连接，如文章[连接记录](/help/quicksilver/planning/records/connect-records.md)中所述。

   <!--at production or when the permanent Add button is released to preview, take the first part of the direction below out and say "Click Add to add a new program"; take this out too: "The Add button is followed by the program name you typed."-->

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

</div>

