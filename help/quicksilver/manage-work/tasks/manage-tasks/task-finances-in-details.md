---
product-area: projects
navigation-topic: manage-tasks
title: 在“任务详细信息”部分管理任务财务
description: 在“任务详细信息”部分管理任务财务
author: Alina
feature: Work Management
exl-id: 54ae48e5-bc8c-4e90-8fa1-0015523df4e6
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 4%

---

# 在“任务详细信息”部分管理任务财务

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some of the information (fields) in this article is also in the Edit tasks article; if you need to update one field, to it in both articles)</p>
-->

您可以通过访问任务详细信息部分的概述区域来查看或编辑任务的财务信息。 您可以在此区域中查看或编辑的字段数量有限。 有关编辑任务的所有财务信息的信息，请参阅[编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md)。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目和任务的访问权限</p> <p>查看对财务数据或更高版本的访问权限</p> <p>您必须具有财务数据的编辑权限才能编辑任务的财务信息</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看包含View Finance或更高版本的任务的权限</p> <p>您必须对包含“编辑财务”的任务具有“管理”权限，才能编辑任务的财务信息</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 在“任务详细信息”部分中编辑任务财务

1. 转到要查看任务的项目。

   >[!NOTE]
   >
   >要查找任务，您还可以搜索该任务，然后单击名称以访问该任务。 有关在Workfront中搜索对象的详细信息，请参阅[搜索Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md)。

1. 单击左侧面板中的&#x200B;**任务**。
1. 单击要查看的任务的名称。
1. 单击&#x200B;**任务详细信息**。
1. （可选）单击“任务详细信息”页面右上角的&#x200B;**全部折叠**&#x200B;图标。

   ![](assets/collapse-all-icon-on-details-page.png)

   >[!NOTE]
   >
   >根据Workfront管理员或组管理员如何设置布局模板，任务详细信息部分中的字段可能会重新排列或不显示。 有关信息，请参阅[使用布局模板自定义详细信息视图](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)。

1. 单击&#x200B;**财务**&#x200B;展开并查看任务的财务信息。

   单击“详细信息”部分右上角的&#x200B;**编辑**&#x200B;图标![](assets/edit-icon.png)，然后单击&#x200B;**财务**。

1. 编辑任何可编辑的字段，方法是单击该字段或单击&#x200B;**+添加**&#x200B;将信息添加到空字段。
1. 在&#x200B;**财务**&#x200B;区域查看或编辑以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">成本类型</td> 
      <td> <p>指定任务的成本类型。 这将根据任务的小时数确定如何计算任务成本。 </p> <p>从以下选项中选择： </p> 
       <ul> 
        <li> <p>无成本</p> </li> 
        <li> <p>固定每小时 </p> </li> 
        <li> <p> 用户每小时 </p> </li> 
        <li> <p> 角色每小时</p> </li> 
       </ul> <p>有关跟踪成本的更多信息，请参阅<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">跟踪成本</a> 。 您的Workfront管理员或组管理员为您的系统或组中的任务选择默认成本类型设置。 有关设置项目默认设置的信息，请参阅<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系统范围的项目首选项</a> 。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">收入类型</td> 
      <td> <p>指定任务的收入类型。 这将根据任务的小时数确定如何计算任务收入。 </p> <p>从以下选项中选择： </p> 
       <ul> 
        <li> <p> 不可计费 </p> </li> 
        <li> <p>用户每小时 </p> </li> 
        <li> <p>角色每小时 </p> </li> 
        <li> <p>固定每小时 </p> </li> 
        <li> <p>受限用户小时 </p> </li> 
        <li> <p>受限角色小时 </p> </li> 
        <li> <p>用户小时加固定 </p> </li> 
        <li> <p>角色小时加固定 </p> </li> 
        <li> <p>固定收入 </p> </li> 
       </ul> <p>有关跟踪收入的更多信息，请参阅<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">账单和收入概述</a> 。 </p> <p>您的Workfront管理员或组管理员为您的系统或组中的任务选择默认收入类型设置。 有关设置项目默认设置的信息，请参阅<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系统范围的项目首选项</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">规划成本</td> 
      <td> <p>此计算基于计划小时数、成本类型和用户或工作角色的小时费率显示任务成本。 有关跟踪成本的更多信息，请参阅<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">跟踪成本</a>。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">实际成本</td> 
      <td> <p> 此计算基于用户或工作角色的实际小时数、成本类型和小时费率显示任务成本。 有关跟踪成本的更多信息，请参阅<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">跟踪成本</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">规划收入</td> 
      <td> <p>此计算基于计划小时数、收入类型和用户或工作角色的小时费率显示与任务关联的收入。 有关跟踪成本的更多信息，请参阅<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">跟踪成本</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">实际收入</td> 
      <td> <p>此计算基于用户或工作角色的实际小时数、收入类型和小时费率显示与任务关联的收入。 有关跟踪成本的更多信息，请参阅<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">跟踪成本</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>CPI/SPI/CSI</strong> </td> 
      <td> <p>这些是显示任务在给定时间的执行情况的任务绩效指标。 其值根据项目的绩效指标方法计算。<br>有关详细信息，请参阅以下文章：</p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">计算成本绩效指数(CPI)</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">计算计划绩效指数(SPI) </a> </p> </li> 
        <li> <p> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">计算成本计划绩效指数(CSI)</a> </p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">完工估算(EAC)</td> 
      <td> <p>这是一个计算，显示任务完成时的总成本。 有关完工估算的详细信息，请参阅<a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">计算完工估算(EAC)</a>。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （视情况而定）如果您正在编辑“财务”部分中的字段，请单击&#x200B;**保存**&#x200B;**更改**。
