---
title: 授予对筛选器、视图和分组的访问权限
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: 作为Adobe Workfront管理员，您可以使用访问级别定义用户对列表和报告筛选器、视图和分组控件的访问权限。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4fb6eefd-74dd-4941-91d4-0e5f637febf3
source-git-commit: d0ab54670d1767e2fa2a9cdf2e7eda1ce8940c7f
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 1%

---

# 授予对筛选器、视图和分组的访问权限

作为Adobe Workfront管理员，您可以使用访问级别来定义用户对列表和报告筛选器、视图和分组控件的访问权限，如[访问级别概述](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)中所述。

有关筛选器、视图和分组控件的信息，请参阅[报告元素：筛选器、视图和分组](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 使用自定义访问级别配置用户对筛选器、视图和分组的访问权限

1. 开始创建或编辑访问级别，如[创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)中所述。
1. 单击筛选器右侧&#x200B;**查看**&#x200B;或&#x200B;**编辑**&#x200B;按钮上的齿轮图标![](assets/gear-icon-settings.png)，然后在&#x200B;**微调设置**&#x200B;下选择要授予的功能。

   ![](assets/gear-icon-filters-dashboards-groupings.jpg)

   默认情况下，拥有“计划”、“工作”、“审阅者”或“请求”许可证的用户具有完整的“查看”和“编辑”功能。 拥有外部用户许可证的用户无法访问筛选器、视图和分组。

   <!--If this changes, undraft section with table below
   -->

1. （可选）要为您正在处理的访问级别中的其他对象和区域配置访问设置，请继续执行[配置对Adobe Workfront的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)中列出的文章之一，如[授予对任务的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)和[授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。
1. 完成后，单击&#x200B;**保存**。

   创建访问级别后，可将其分配给用户。 有关详细信息，请参阅[编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

<!--## Access to filters, views, and groupings by license type

Drafting out this section for now because the table is redundant since all four license types can do everything.</span>-->

此表列出了Workfront管理员可以允许每种许可证类型的用户使用过滤器、视图和分组执行的操作。 有关Workfront许可证类型的信息，请参阅[Adobe Workfront许可证概述](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md)。

<table style="table-layout:auto">
<col>
<col>
<col>
<col>
<col>
<thead>
<tr>
<th> 操作 </th>
<th> 规划器 </th>
<th> 员工 </th>
<th> 查看者 </th>
<th> 请求者 </th>
</tr>
</thead>
<tbody>
<tr>
<td>编辑筛选器、视图和分组</td>
<td>✓ {\f13 }</td>
<td>✓ {\f13 }</td>
<td>✓ {\f13 }</td>
<td>✓ {\f13 }</td>
</tr>
<tr>
<td>创建过滤器、视图和分组</td>
<td>✓ {\f13 }</td>
<td>✓ {\f13 }</td>
<td>✓ {\f13 }</td>
<td>✓ {\f13 }</td>
</tr>
<tr>
<td>查看筛选器、视图和分组</td>
<td>✓ {\f13 }</td>
<td>✓ {\f13 }</td>
<td>✓ {\f13 }</td>
<td>✓ {\f13 }</td>
</tr>
<tr>
<td>删除筛选器、视图和分组</td>
<td>✓ {\f13 }</td>
<td>✓ {\f13 }</td>
<td>✓ {\f13 }</td>
<td>✓ {\f13 }</td>
</tr>
<tr>
<td>共享筛选器、视图和分组</td>
<td>✓ {\f13 }</td>
<td>✓ {\f13 }</td>
<td>✓ {\f13 }</td>
<td>✓ {\f13 }</td>
</tr>
<tr>
<td>在系统范围内共享筛选器、视图和分组</td>
<td>✓ {\f13 }</td>
<td>✓ {\f13 }</td>
<td>✓ {\f13 }</td>
<td>✓ {\f13 }</td>
</tr>
</tbody>
</table>
