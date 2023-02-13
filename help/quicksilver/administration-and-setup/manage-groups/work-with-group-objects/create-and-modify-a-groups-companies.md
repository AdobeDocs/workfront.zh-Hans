---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 创建和修改群组的公司
description: 在“组”区域中查看由您管理的组时，可以查看与该组及其任何子组关联的公司并与之合作。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 407f6631-ecc1-4ed8-bfec-6d726ae87a3d
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 0%

---

# 创建和修改群组的公司

在“组”区域中查看由您管理的组时，可以查看与该组及其任何子组关联的公司并与之合作。

如果您的组上有任何组，则其管理员也可以为您的组执行这些操作。 Workfront管理员（对于任何组）也是如此。

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront计划*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> <p>您必须是组的组管理员或Workfront管理员。 有关更多信息，请参阅 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref" data-mc-variable-override="">组管理员</a> 和 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">授予用户完全管理访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要了解您拥有的计划或许可证类型，请联系您的Workfront管理员。

## 从“组”区域查看、处理和创建组的公司

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **群组** ![](assets/groups-icon.png).

1. 单击要为其创建或修改公司的组名称。
1. 在左侧面板中，单击 **公司** 列出与组关联的公司以及它可能拥有的任何子组。
1. （可选）要添加公司，请单击 **添加公司**，然后使用下面列出的选项配置公司。 完成后，单击 **创建公司**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">基本信息部分</td> 
      <td> 
       <ul> 
        <li> <p><b>公司名称</b>:键入公司名称。</p> </li> 
        <li> <p><b>处于活动状态</b>:启用此选项后，用户可以找到公司并将其附加到他们创建和编辑的项目。 不活动的公司不能附加到项目。 默认情况下，此选项处于启用状态。</p> </li> 
        <li> <p><b>这是主要公司</b>:将公司分配为贵组织的主公司。 主公司通常表示大多数用户所在的Workfront帐户。</p> <p>通过修改其访问级别，您可以限制用户查看其他用户：</p> 
         <ul> 
          <li>仅在主公司</li> 
          <li> <p>在其关联公司和主公司中</p> <p>有关用户访问级别中主要公司功能的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">创建或修改自定义访问级别</a>.</p> <p>您只能将一个或没有公司指定为主公司，但不能将多个公司指定为主公司。 有关更多信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">创建或修改自定义访问级别</a>.</p> </li> 
         </ul> </li> 
        <li> <p><b>组</b>:如果有与公司有业务往来的组，您可以在此处添加该组的名称。 这对于需要报告和管理其组与之开展业务的所有公司的组管理员非常有用。</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">系统将填充 <strong>组</strong> 字段。</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">如果您在访问级别拥有对公司的管理访问权限，则可以从公司中删除该组并分配其他组，或将公司保留为没有组。</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">如果您没有对公司的管理访问权限，则 <strong>组</strong> 字段，您只能选择您管理的组或这些组下的任何子组。</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">有关对公司的管理访问权限的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">授予用户对特定区域的管理访问权限</a>.</p> </li> 
        <li> <p><b>公司成员</b>:将现有用户添加到公司。 通过执行此操作，您会将这些用户与此公司关联。</p> <p>您与一个公司关联的用户数量没有限制，但一个用户不能与多个公司关联。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">帐单费率部分</td> 
      <td> <p>您可以改写与公司层职务职责关联的开单费率。 有关创建职务角色并将其与开单费率关联的信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref" data-mc-variable-override="">创建和管理作业角色</a>.</p> <p>有关公司级别覆盖账单费率的详细信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md" class="MCXref xref" data-mc-variable-override="">在公司层改写职务职责开单费率</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">自定义Forms部分</td> 
      <td> <p>如果您要向公司添加的字段在Workfront中不可用，则可以构建自定义表单并将其与您的公司关联。 您可以从下拉菜单中选择此表单，以将其附加到您的公司。 下拉菜单中只列出活动公司。 有关创建自定义Forms的信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" data-mc-variable-override="">创建或编辑自定义表单</a>. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >如果您对访问级别中的公司具有管理访问权限，则还可以单击列表底部的添加更多公司。 这会添加一行，您可以在该行中快速配置新公司。

1. （可选）要编辑或删除公司，请至少选择一个公司，然后使用工具栏按钮进行编辑 ![](assets/edit-icon.png) 或删除 ![](assets/delete.png) 它。

   有关编辑公司的信息，请参阅 [在Workfront中创建或编辑公司](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md#adding-a-company-to-workfront) 在文章中 [创建和编辑公司](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

1. （可选）要导出公司列表，请单击导出图标 ![](assets/export.png)，然后为导出列表选择所需的文件格式。
