---
title: 管理Adobe Workfront对象的“计划”部分中的记录
description: 您可以在左侧面板的Workfront对象的Planning部分中显示连接到Adobe Workfront对象的Workfront Planning记录。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d86cf3f9-cacc-4457-acb3-a5122ae91be8
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '1734'
ht-degree: 1%

---


<!--add also Group and Company when they are available-->

# 管理来自Workfront对象的记录连接

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>-->

{{planning-important-intro}}

您可以在Workfront中将与它们连接的对象的以下区域显示Workfront Planning记录：

* Workfront对象的Planning部分：显示连接到对象的所有记录类型及其各自的连接记录。
* Planning连接自定义字段：显示一个记录类型、其各自的连接记录以及连接记录的最多7个查找字段。

## 访问要求

+++ 展开以查看访问要求。

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
<p>任何</p>
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
   <td>
   <p>标准</p>
   <p>Workfront计划不适用于旧版Workfront许可证</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>访问级别配置</p></td>
   <td> <p>查看或更高权限的项目、项目和项目组合</p>  
   <p>Workfront计划没有访问级别配置。 </p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>对象权限</p></td>
   <td>
   <p>在Workfront中，查看项目、项目组合或项目群的权限或更高的权限</a> </p> 
   <p>在Workfront规划中：
   <ul><li>
   查看对工作区和记录类型的权限以查看任何连接的记录 </li>
   或
   <li> 为工作区分配或更高权限以及记录类型以连接或断开记录</a></li></ul> </p>  
   <p>系统管理员有权访问所有Workfront Planning工作区，包括他们未创建的工作区</p> 
  </td>
  </tr>
 </tbody>
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


## 管理“计划”部分中的记录

您可以使用Workfront对象的Planning部分查看连接到Workfront对象的所有记录类型及其各自的记录。
“规划”部分适用于以下Workfront对象：

* 项目
* 项目组合
* 项目群
<!--* Group
* Company-->

### 关于Workfront对象Planning部分的注意事项

当您从Workfront对象的Planning部分中查看Workfront Planning记录时，请考虑以下事项：

* Workfront Planning记录类型必须首先连接到Workfront对象类型。

  有关信息，请参阅以下文章：

   * [连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)
   * [连接记录](/help/quicksilver/planning/records/connect-records.md)
* 您可以从Workfront对象查看Planning部分，即使没有与Workfront对象关联的记录也是如此。

### 从“规划”部分管理记录连接

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
   * 记录显示在各自的工作区和记录类型下。

   项目![的](assets/planning-section-on-project.png)计划部分

1. （可选）单击“显示所有连接”**&#x200B;**&#x200B;可显示所有连接的记录类型，包括未连接记录的记录类型。 默认情况下，不显示没有连接记录的记录类型。
1. 单击记录卡以显示有关记录的更多信息。 此时将显示记录预览框。
1. （可选）开始修改记录预览框中的字段。 您的更改会自动保存。
1. （可选）单击预览框右上角的&#x200B;**在新标签中打开**&#x200B;图标![在新标签中打开详细信息](assets/open-details-in-a-new-tab-icon.png)以打开记录的详细信息页面。 此时将在Workfront Planning中打开记录的详细信息页面。
1. （可选）将鼠标悬停在记录卡片上，单击断开连接记录图标&#x200B;**-**，然后单击&#x200B;**断开连接**。
出现以下情况：
   * 记录不再连接到Workfront对象。
   * Workfront对象也将从Workfront Planning中的记录的“已连接”字段中删除。
   * 连接到Planning记录的Workfront查找字段的值也会被删除。
1. 单击&#x200B;**连接**&#x200B;为连接的记录类型连接更多记录。

   有关详细信息，请参阅[连接记录](/help/quicksilver/planning/records/connect-records.md)。
1. （可选）如果找不到要连接的记录，并且要添加该记录，请单击&#x200B;**+添加**&#x200B;以添加新记录。 有关详细信息，请参阅[创建记录](/help/quicksilver/planning/records/create-records.md)一文中的“连接其他记录时创建记录”一节。

   出现以下情况：

   * 记录会立即连接到Workfront对象，并显示在Planning部分中。
   * Workfront对象将添加到Workfront Planning记录的已连接字段中。
   * 连接到Planning记录的Workfront查找字段的值会在Workfront Planning中填充。

## 管理Planning连接字段类型中的记录

您可以使用Workfront对象上的Planning连接自定义字段查看一种记录类型及其各自连接到Workfront对象的记录。

在创建Planning连接自定义字段时，您可以控制为Workfront对象显示哪些Planning记录类型。

* Planning连接字段会在建立连接后以及将该字段附加到以下Workfront对象的表单时显示Planning记录：

   * 项目
   * 项目组合
   * 项目群
   * 组
   * 公司

有关详细信息，请参阅[创建表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

### 有关Planning连接字段类型的注意事项

当您从Workfront对象的Planning连接字段查看Workfront Planning记录时，请考虑以下事项：

* 将Planning记录连接到Workfront对象后，Planning连接字段将以下列方式显示在Workfront对象的自定义表单中：

   * 如果仅选择所连接记录的主字段，且连接允许链接多个记录，则Planning连接字段将显示为具有多个值的字段。 有关信息，请参阅[连接记录类型概述](/help/quicksilver/planning/architecture/connect-record-types-overview.md)。
   * 如果您的Workfront或组管理员从自定义表单上的连接记录中添加了其他查找字段，则Planning连接字段将显示为表格。 最多可以为Planning连接字段选择7个字段。 表格视图是只读的。

* 您只能将一个记录类型与一个Planning连接字段相关联。 表单中的Planning连接字段数量没有限制。
* 您必须对对象、记录和Workfront Planning具有正确的访问和权限，才能将带有Planning连接自定义字段的自定义表单附加到Workfront对象。
* 您必须拥有Workfront中工作区的Contribute权限，才能从Workfront对象的Planning连接字段中连接或断开记录。
* Workfront Planning记录类型必须首先连接到Workfront对象类型。 有关信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。这将使Workfront Planning记录可从Workfront访问。
* 只有可以具有Workfront Planning连接的对象，才能从Workfront对象的Planning连接字段中连接或断开记录。

  例如，您可能可以将带有Planning连接字段的自定义表单附加到任务，但无法将Workfront Planning对象连接到任务。
* 批量编辑Workfront对象时，无法编辑Planning连接字段。

### 从Planning连接字段类型管理记录连接

1. 转到以下已与Workfront Planning记录类型连接的对象类型之一：

   * 项目
   * 项目组合
   * 项目群
   * 公司
   * 组

1. 单击左侧面板中的&#x200B;**&lt;对象>详细信息**。
1. （视情况而定）为所选对象添加一个自定义表单，该表单至少包含一个Planning连接字段（如果不存在）。

   >[!NOTE]
   >
   >您的Workfront或组管理员必须先创建表单并在其上添加Planning连接字段，然后才能将其添加到对象。


1. 单击字段内部以添加连接的记录，然后单击字段内部的向下箭头，以从列表中选择记录。

   ![在记录列表打开的项目上规划连接字段](assets/planning-connection-field-on-project-with-record-list-open.png)

   >[!TIP]
   >
   >您无法将记录添加到与Workfront对象（配置该字段时选择的对象除外）关联的Planning连接字段中。
   >
   >例如，您无法从项目的自定义表单向为Portfolio连接创建的Planning连接字段添加记录。
   >
   >有迹象表明字段的对象与您选择的对象不匹配。
   >
   >![警告表单](assets/warning-unsupported-object-planning-connection-field-on-form.png)上不支持的对象Planning连接字段

1. 单击列表外部以将其关闭。

   出现以下情况：

   * 记录会立即连接到Workfront对象，并显示在Workfront对象的Planning连接字段和Planning部分中。
   * Workfront对象将添加到Workfront Planning记录的已连接字段中。
   * 连接到Planning记录的Workfront查找字段的值会在Workfront Planning中填充。
   * 如果您的Workfront或组管理员在创建自定义表单时添加了记录查找字段，则记录的查找字段会在表视图中自动填充。 Planning连接字段中的表视图为只读。

     ![项目详细信息自定义表单上具有表的Planning连接字段](assets/planning-connection-field-with-table-on-project-details-custom-form.png)

     >[!NOTE]
     >
     >只有在自定义表单的Planning连接字段中添加了查找字段后，才会显示表格视图。


1. （可选）在Planning连接字段中，单击记录名称或将鼠标悬停在表中记录名称上，然后单击Planning连接自定义表单上的&#x200B;**打开记录**&#x200B;图标![打开记录图标](assets/open-record-icon-on-planning-connection-custom-form.png)以在Workfront Planning中将其打开。
将打开Workfront Planning记录详细信息预览框。
1. 查看或编辑有关记录的信息，或单击&#x200B;**在新标签中打开**&#x200B;图标![在新标签中打开记录](assets/open-details-in-a-new-tab-icon.png)以打开记录详细信息页面。

1. （可选）从Workfront中的自定义表单中，单击记录上的&#x200B;**删除**&#x200B;图标![删除图标](assets/remove-icon.png)以将其从Planning连接字段中删除，并将其与Workfront对象断开连接。
Workfront对象与Planning记录断开连接，并且从Workfront中删除所有查找信息。

1. 单击&#x200B;**保存更改**&#x200B;以保存自定义表单以及您对Workfront对象所做的任何其他更改。
