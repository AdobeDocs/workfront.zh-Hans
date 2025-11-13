---
title: 在将Workfront对象连接到记录时，从Workfront Planning创建这些对象
description: 在从Workfront Planning中的其他记录连接对象时，您可以创建Workfront对象类型。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7c3db950-4cd9-424c-a7a7-4fa7dfa995f6
source-git-commit: 1f9a0e6064f83c6f0947e3c7ef596e96c934a687
workflow-type: tm+mt
source-wordcount: '1271'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# 在将Workfront对象连接到记录时，从Workfront Planning创建这些对象

<!-- remove preview and production at release time-->

<!--<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

您可以通过以下方式从Workfront Planning创建Adobe Workfront对象：

* 从Planning记录连接Workfront对象时

  本文介绍了在从Planning记录连接Workfront对象时，如何从Workfront Planning创建这些对象。
* 当您从记录的页面使用自动化时。

  有关使用自动化创建Workfront对象的信息，请参阅[使用Adobe Workfront Planning记录自动化创建对象](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md)。

>[!IMPORTANT]
>
>将以下Workfront对象与Planning记录连接后，您可以从Workfront Planning创建这些对象：
>
>* 项目
>* 项目组合
>* 项目群
>
>您可以将以下Workfront对象与Planning记录连接，但不能在连接过程中创建它们：
>
>* 组
>* 公司
>

将和创建Workfront对象连接到Workfront Planning记录时，请考虑以下事项：

* 您可以从连接字段从Workfront Planning的以下区域连接Workfront项目、项目组合、程序、组和公司：

   * 记录类型的表格视图
   * 记录的详细信息页面或预览框
   * 记录的“连接”选项卡

* 您可以从Workfront Planning的以下区域创建项目：

   * 记录类型的表格视图
   * 连接字段中记录的详细信息区域
   * 记录的已连接记录页面，在详细信息区域

* 您可以从Workfront Planning的以下区域创建项目组合和程序：

   * 记录类型的表格视图
   * 连接字段中记录的详细信息区域

有关将Planning记录与Workfront对象连接的信息，请参阅[连接记录](/help/quicksilver/planning/records/connect-records.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront包</p></td> 
   <td> 
<p>任何Workfront和任何Planning包</p> <p>任何工作流和任何计划包</p>
<p>有关每个Workfront Planning包中所包含内容的更多信息，请联系您的Workfront客户代表。 </p> 
   </td>

<tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p>标准</p>
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
   <td> <p>为要添加记录的工作区和记录类型分配或更高权限。 </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>
   <p>管理Workfront对象（项目组合）的权限以添加子对象（项目）。</p>
   </td> 
  </tr>   
</tbody> 
</table>

有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++ 

<!--Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td> Standard
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p> 
   <p>Edit access with access to Create objects in Workfront for the object types that you want to create (projects, portfolios, programs). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Manage permissions to the workspace and record type where you want to add records. </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Manage permissions to Workfront objects (portfolios) to add children objects (projects).</p>
   </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).  -->


## 将Workfront对象与Workfront Planning中的记录连接时创建这些对象的先决条件

您必须具备以下条件，才能通过从现有记录连接项目或项目组合来添加新项目或项目组合：

* 记录连接到Workfront项目、项目组合或项目的类型。 有关信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。
* 连接到Workfront对象的记录类型的记录。 有关信息，请参阅[创建记录](/help/quicksilver/planning/records/create-records.md)。
* Workfront Planning和Workfront中的正确访问和权限，如本文的[访问要求](#access-requirements)部分所述。

## 将项目与Workfront Planning中的记录连接时创建项目

在Workfront Planning中将项目与Workfront Planning中的记录连接时，您可以在Planning的以下区域创建项目：

* 记录类型的表视图或连接字段中记录的详细信息区域
* 记录的已连接记录页面，在记录的详细信息区域

### 从记录的详细信息区域或记录类型的表视图创建项目

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

### 从记录的“连接的记录”页面创建项目

1. 在表格视图中将Project对象类型与Workfront Planning记录类型连接。

   有关信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。

1. 单击任意视图中的记录名称。 “详细信息”预览框打开。

1. 为项目添加&#x200B;**连接的记录页**。

   有关信息，请参阅文章[管理记录页布局](/help/quicksilver/planning/records/manage-the-record-page.md)中的“将连接的记录页添加到记录”部分。

   “连接的记录”页显示在表视图中。 连接的项目将显示在表中。

   ![已连接记录页中的项目表视图](assets/projects-connected-records-page-table.png)

1. 单击项目表中的&#x200B;**新行**&#x200B;以添加项目。

   只能在此区域添加空白项目。 无法使用模板添加项目。
1. （可选）单击表视图中的项目名称以在Workfront中打开该项目并添加更多信息。

## 将项目组合与Workfront Planning中的记录连接时创建项目组合

您可以从记录类型的表视图或记录的详细信息页面创建项目组合。

要在从Planning记录连接项目组合时创建项目组合，请执行以下操作：

1. 转到记录的详细信息页面或记录类型的表，然后开始将Workfront Planning记录与Workfront项目组合连接，如文章[连接记录](/help/quicksilver/planning/records/connect-records.md)中所述。

1. （视情况而定）单击&#x200B;**添加项目组合**

   或

   开始键入项目组合的名称，如果找不到，请单击&#x200B;**添加项目组合**。 “添加”按钮后跟您键入的项目组合名称。

   ![从连接字段连接项目组合时添加项目组合](assets/add-portfolio-when-connecting-it-from-connection-field.png)

   将创建项目组合并将其添加到所选记录的连接字段。

1. （可选）在Workfront Planning中单击新项目组合的名称，以在Workfront中打开项目组合页面，并对项目组合进行其他更新。

## 在将程序与Workfront Planning中的记录连接时创建程序

您可以从记录类型的表视图或记录的“详细信息”页创建程序。

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

