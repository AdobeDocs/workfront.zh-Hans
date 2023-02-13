---
product-area: projects
navigation-topic: manage-tasks
title: 在“任务详细信息”部分中管理任务财务
description: 在“任务详细信息”部分中管理任务财务
author: Alina
feature: Work Management
exl-id: 54ae48e5-bc8c-4e90-8fa1-0015523df4e6
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 5%

---

# 在“任务详细信息”部分中管理任务财务

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some of the information (fields) in this article is also in the Edit tasks article; if you need to update one field, to it in both articles)</p>
-->

您可以通过访问“任务详细信息”部分的“概述”区域来查看或编辑任务的财务信息。 在此区域中，可以查看或编辑的字段数量有限。 有关编辑任务的所有财务信息的信息，请参阅 [编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目和任务的访问权限</p> <p>查看对金融数据或更高版本的访问权限</p> <p>您必须拥有对财务数据的编辑访问权限才能编辑有关任务的财务信息</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看包含View Finance或更高版本的任务权限</p> <p>您必须对包含“编辑财务”的任务具有“管理”权限，才能编辑有关任务的财务信息</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 在“任务详细信息”部分中编辑任务财务

1. 转到要查看任务的项目。

   >[!NOTE]
   >
   >要查找任务，您还可以搜索该任务，然后单击名称以访问该任务。 有关在Workfront中搜索对象的更多信息，请参阅 [搜索Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

1. 单击 **任务** 中。
1. 单击要查看的任务的名称。
1. 单击 **任务详细信息**.
1. （可选）单击 **全部折叠** 图标。

   ![](assets/collapse-all-icon-on-details-page.png)

   >[!NOTE]
   >
   >根据Workfront管理员或组管理员设置布局模板的方式，任务详细信息部分中的字段可能会重新排列或不显示。 有关信息，请参阅 [使用布局模板自定义详细信息视图](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. 单击 **金融** 以展开和查看任务的财务信息。

   单击 **编辑** 图标 ![](assets/edit-icon.png) 在“详细信息”部分的右上角，单击 **金融**.

1. 通过单击字段或单击，编辑任何可编辑的字段 **+添加** 向空字段添加信息。
1. 在 **金融** 区域：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">成本类型</td> 
      <td> <p>指定任务的成本类型。 这将根据任务的小时数确定如何计算任务的成本。 </p> <p>从以下选项中进行选择： </p> 
       <ul> 
        <li> <p>无成本</p> </li> 
        <li> <p>固定小时 </p> </li> 
        <li> <p> 用户小时 </p> </li> 
        <li> <p> 角色小时</p> </li> 
       </ul> <p>有关跟踪成本的更多信息，请参阅 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">跟踪成本</a> . 您的Workfront管理员或组管理员为系统或组中的任务选择默认的成本类型设置。 有关设置项目默认值的信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系统范围的项目首选项</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">收入类型</td> 
      <td> <p>为任务指定收入类型。 这将根据任务上的小时数确定如何计算任务的收入。 </p> <p>从以下选项中进行选择： </p> 
       <ul> 
        <li> <p> 不可记帐 </p> </li> 
        <li> <p>用户小时 </p> </li> 
        <li> <p>角色小时 </p> </li> 
        <li> <p>固定小时 </p> </li> 
        <li> <p>受限用户小时 </p> </li> 
        <li> <p>受限角色小时 </p> </li> 
        <li> <p>用户小时加固定 </p> </li> 
        <li> <p>角色小时加固定 </p> </li> 
        <li> <p>固定收入 </p> </li> 
       </ul> <p>有关跟踪收入的更多信息，请参阅<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">账单和收入概述</a> . </p> <p>您的Workfront管理员或组管理员为系统或组中的任务选择默认的收入类型设置。 有关设置项目默认值的信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系统范围的项目首选项</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">计划成本</td> 
      <td> <p>这是一种计算，它根据计划小时数、成本类型以及用户或任务角色的小时费率来显示任务的成本。 有关跟踪成本的更多信息，请参阅 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">跟踪成本</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">实际成本</td> 
      <td> <p> 这是一种计算，它根据实际工时、成本类型以及用户或任务角色的小时费率来显示任务的成本。 有关跟踪成本的更多信息，请参阅 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">跟踪成本</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">计划收入</td> 
      <td> <p>这是一种计算，它根据计划小时数、收入类型以及用户或职务角色的小时费率显示与任务关联的收入。 有关跟踪成本的更多信息，请参阅 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">跟踪成本</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">实际收入</td> 
      <td> <p>这是一种计算方式，它根据实际小时数、收入类型以及用户或职务角色的小时费率显示与任务关联的收入。 有关跟踪成本的更多信息，请参阅 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">跟踪成本</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>CPI / SPI / CSI</strong> </td> 
      <td> <p>这些是任务性能量度，用于显示任务在给定时间的执行情况。 这些值是根据项目的性能指数方法计算的。<br>有关更多信息，请参阅以下文章：</p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">计算成本绩效指数(CPI)</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">计算计划性能索引(SPI) </a> </p> </li> 
        <li> <p> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">计算成本计划绩效指数(CSI)</a> </p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">完成时估计(EAC)</td> 
      <td> <p>此计算显示完成时任务的总成本。 有关完成时估计的详细信息，请参阅 <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">完成时计算估计(EAC)</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （视情况而定）如果您正在编辑财务部分中的字段，请单击 **保存****更改**.
