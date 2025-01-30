---
title: 从Workfront Planning创建Workfront对象
description: 在从Workfront Planning中的其他记录连接对象时，您可以创建Workfront对象类型。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7c3db950-4cd9-424c-a7a7-4fa7dfa995f6
source-git-commit: 928ea5da9955b8c1c98782df81698c49987d4c18
workflow-type: tm+mt
source-wordcount: '864'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# 从Workfront Planning创建Workfront对象


<!-- remove preview and production at release time-->

<span class="preview">此页面上突出显示的信息是指尚未普遍可用的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

您可以从Workfront Planning创建以下类型的Workfront对象：

* 项目
* 项目组合

将Workfront计划记录与项目或项目组合连接时，您可以从Workfront Planning创建Workfront项目和项目组合。

>[!IMPORTANT]
>
>* 从记录中连接项目和项目组合时，只能在Workfront中创建它们。
>
>* 从Workfront Planning中的记录连接程序、组或公司时，不能创建这些程序、组或公司。
>
<!--* You cannot create a project from a template when when you create projects by connecting them from a record. You must manually add tasks and project information or a template to the new project after you add it to the record.-->

有关将Planning记录与Workfront对象连接的信息，请参阅[连接记录](/help/quicksilver/planning/records/connect-records.md)。

## 访问要求

+++ 展开以查看Workfront Planning的访问要求。

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
<p>贵组织的Workfront实例必须载入AdobeUnified Experience，才能访问Workfront Planning的所有功能。</p> 
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">AdobeWorkfront的Unified Experience</a>。 </p> 
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
   <p>在将记录连接到要创建的对象类型（项目和项目组合）时，在Workfront中编辑对这些对象的访问权限。 </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td> <p>管理要向其中添加记录的工作区的权限。 </p>  
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

* 记录类型连接到Workfront项目或项目组合。 有关信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。
* 记录。 有关信息，请参阅[创建记录](/help/quicksilver/planning/records/create-records.md)。
* Workfront Planning和Workfront中的正确访问和权限，如本文的[访问要求](#access-requirements)部分所述。

## 将项目与Workfront Planning中的记录连接时创建项目

要在从其他记录连接项目时创建项目，请执行以下操作：

1. 转到记录的详细信息页面或记录类型的表，然后开始将Workfront Planning记录与Workfront项目连接，如文章[连接记录](/help/quicksilver/planning/records/connect-records.md)中所述。

   您可以在Workfront Planning的以下区域的连接字段中连接项目：

   * 记录类型的表格视图
   * 记录的详细信息页面或预览框

1. （视情况而定）如果尝试从其他记录的已连接记录字段添加项目时找不到项目，请添加名称，然后单击“**+添加”**。 添加按钮后跟您键入的项目名称。

   <!--at production or when the permanent Add button is released to preview, take the first part of the direction above out and say "Click +Add to add a new project"; take this out too: "The Add button is followed by the project name you typed."-->

   ![](assets/add-project-when-connecting-it-from-connection-field.png)

   <span class="preview">将打开&#x200B;**创建项目**&#x200B;框。</span>

1. <span class="preview">（可选）更新&#x200B;**项目名称**。 默认情况下，从记录中连接项目时，将按照您作为搜索项添加的内容来命名项目。</span>
1. <span class="preview">（可选）选择&#x200B;**项目模板**。 如果不选择模板，Workfront将创建一个不含任务的空白项目。</span>
1. <span class="preview">单击&#x200B;**创建**。</span>
1. <span class="preview">（视情况而定）如果您选择从模板创建项目，请按照文章[使用模板创建项目](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md)中的步骤完成添加项目。</span>

   将创建新项目并将其添加到所选记录的已连接字段中。

1. （可选）在Workfront规划中单击新项目的名称，以在Workfront中打开项目页面，并对项目进行其他更新。

## 将项目组合与Workfront Planning中的记录连接时创建项目组合

要在从其他记录连接项目组合时创建项目组合，请执行以下操作：

1. 转到记录的详细信息页面或记录类型的表，然后开始将Workfront Planning记录与Workfront项目组合连接，如文章[连接记录](/help/quicksilver/planning/records/connect-records.md)中所述。

   您可以在Workfront Planning的以下区域中从连接字段连接项目组合：

   * 记录类型的表格视图
   * 记录的详细信息页面或预览框

   <!--at production or when the permanent Add button is released to preview, take the first part of the direction below out and say "Click +Add to add a new portfolio"; take this out too: "The Add button is followed by the portfolio name you typed."-->

1. （视情况而定）如果尝试从其他记录的已连接记录字段添加项目组合时找不到项目组合，请添加名称，然后单击“**+添加项目组合”**。 “添加”按钮后面还有您键入的项目组合名称。

   ![](assets/add-portfolio-when-connecting-it-from-connection-field.png)

   将创建项目组合并将其添加到所选记录的连接字段。

1. （可选）在Workfront Planning中单击新项目组合的名称，以在Workfront中打开项目组合页面，并对项目组合进行其他更新。

<!--

<div class="preview">

## Create programs when connecting them with records from Workfront Planning

To create programs as you are connecting them from other records: 

1. Go to a record's details page or to the record type's table and start connecting Workfront Planning records with Workfront portfolios, as described in the article [Connect records](/help/quicksilver/planning/records/connect-records.md). 

    You can connect programs from a connection field in following areas of Workfront Planning:

    * The table view of a record type
    * The details page or preview box of a record

    ********at production or when the permanent Add button is released to preview, take the first part of the direction below out and say "Click +Add to add a new program"; take this out too: "The Add button is followed by the program name you typed."***********
    
1. (Conditional) If you cannot find a program when trying to add it from the connected record field of another record, add a name, then click **+ Add**. The Add button is followed by the program name you typed. 

    ![](assets/add-wf-program-when-connecting-it-from-connection-field.png)

    The **Create program** box opens.

1. Update the **Program name**. This is a required field.
1. Choose a **Portfolio** from the drop-down, or start typing the name of a portfolio, then select it when it displays in the list. This is a required field. 
1. Click **Create**.

    The program is created and added to the connection field of the record you selected. 

1. (Optional) Click the name of the new program from Workfront Planning to open the program's page in Workfront and make additional updates to it. 

</div>

-->