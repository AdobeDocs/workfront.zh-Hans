---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: 在Workfront中预算资源所需的访问权限
description: 当您具有工作项、用户、工作角色和团队的特定访问级别设置和权限时，您可以查看和管理有关您有权查看的项目资源规划的信息。
author: Lisa
feature: Resource Management
exl-id: d2bfc411-188a-4f8b-8180-0e984f01b5ab
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# 在Workfront中预算资源所需的访问权限

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><b>(LINKED TO PRODUCT</b>: This is also linked to the product, in two different tooltips in the RP:</p>
<p>- the tooltip for the View-only mode of the Budgeted Hours boxes. You gave this link to Vazgen and the team for the tooltip and documented this in this sheet:https://docs.google.com/spreadsheets/d/1zKjNVw_TyfQ474jbY7JorSWTkptMNb5RFCck2IficYs/edit#gid=0</p>
<p>- Also in the tooltip from this issue: https://hub.workfront.com/issue/view?ID=5ca708d00024a39e58b5dbeaceb00939)</p>
<p>This might need to be moved to Resource Management overview and title needs to be changed to "Acces needed to manage resources" when the res manager prerequisite will drop for resource scheduling and the field goes away.</p>
<p>This should be linked from Planning in the Resource Planner - in the Budgeting Resources in the RP area)</p>
</div>
-->

当您的公司购买包含资源规划的Adobe Workfront许可证后，您可以查看您有权查看的项目的资源预算信息。 您可以在资源规划程序中查看预算信息。

有关在Workfront中使用预算编制工具的先决条件的更多信息，请参阅[资源规划入门](../../resource-mgmt/resource-planning/get-started-resource-planning.md)。

要预算资源、管理资源池并查看资源计划工具中的成本信息，您的公司和您必须具有以下访问权限：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p>
       <p>规划</p></td>
  </tr>  
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> 
    <ul> 
     <li> <p>编辑访问级别中资源管理的访问权限，包括：</p> 
      <ul> 
       <li> <p>有权编辑项目优先级和预算小时数。 </p> </li> 
       <li> <p>管理资源池的权限（如果需要管理资源池）。</p> </li> 
      </ul> <p>有关资源管理访问级别的信息，请参阅文章<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">授予对资源管理的访问权限</a>。</p> </li> 
     <li> <p>编辑对项目和用户的访问权限。 </p> </li> 
     <li> <p> 如果需要按“成本”查看或管理信息，请在访问级别编辑对财务数据的访问。</p> <p>有关财务数据访问级别的更多信息，请参阅文章<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">授予对财务数据的访问权限</a>。</p> </li> 
    </ul> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目权限，包括管理财务权限。</p> <p>有关项目权限的信息，请参阅文章<a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">在Adobe Workfront中共享项目</a>。</p> <p>有关项目的财务权限的信息，请参阅文章<a href="../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md"><a href="../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">共享对象的财务权限</a></a>。</p>

<p><b>注意：</b>在“角色”视图中预算资源时，如果角色下列出的至少一个项目的管理权限不足，则无法为该角色预算小时数、FTE或成本。 您只能为拥有管理权限的项目编制预算。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。
