---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 创建和修改组的公司
description: 查看在组区域管理的组时，可以查看与组及其任何子组关联的公司，并使用这些公司。
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 407f6631-ecc1-4ed8-bfec-6d726ae87a3d
source-git-commit: 5d7cc28ebb1c7d7401a60ef4fc383fc90ed20631
workflow-type: tm+mt
source-wordcount: '784'
ht-degree: 0%

---

# 创建和修改组的公司

查看在组区域管理的组时，可以查看与组及其任何子组关联的公司，并使用这些公司。

如果您的组之上存在任何组，则其管理员还可以为您的组执行这些操作。 Workfront管理员也是如此（适用于任何组）。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

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
   <td>访问级别配置</td> 
   <td>您必须是组的组管理员或系统管理员。</td>
  </tr>
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 从组区域查看、处理和创建您组的公司

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**组** ![组](assets/groups-icon.png)。

1. 单击要为其创建或修改公司的组的名称。
1. 在左侧面板中，单击&#x200B;**公司**&#x200B;列出与组相关联的公司及其可能具有的任何子组。
1. （可选）要添加公司，请单击&#x200B;**添加公司**，然后使用以下列出的选项配置公司。 完成后，单击&#x200B;**创建公司**。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">基本信息部分</td> 
      <td> 
       <ul> 
        <li> <p><b>公司名称</b>：键入公司的名称。</p> </li> 
        <li> <p><b>处于活动状态</b>：启用此选项后，用户可以找到该公司并将其附加到他们创建和编辑的项目。 无法将非活动的公司附加到项目。 此选项默认处于启用状态。</p> </li> 
        <li> <p><b>这是主要公司</b>：将公司指定为组织的主要公司。 主要公司通常表示您的大多数用户工作的Workfront帐户。</p> <p>通过修改其访问级别，您可以限制用户查看其他用户：</p> 
         <ul> 
          <li>仅在其主要公司中</li> 
          <li> <p>在他们的关联公司和主要公司中</p> <p>有关用户访问级别内的主要公司功能的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">创建或修改自定义访问级别</a>。</p> <p>您只能将一家公司指定为主要公司，或者不能将一家公司指定为主要公司，但不得将多家公司指定为主要公司。 有关详细信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">创建或修改自定义访问级别</a>。</p> </li> 
         </ul> </li> 
        <li> <p><b>组</b>：如果有一个组与公司开展业务，您可以在此处添加该组的名称。 这对于需要报告和管理其组与其开展业务的所有公司的组管理员非常有用。</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">系统用您正在查看的组填写新公司的<strong>组</strong>字段。</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">如果您对具有访问级别的公司具有管理访问权限，则可以从公司中删除组并分配其他组，或者将公司保留为不带组。</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">如果您没有公司的管理访问权限，则需要<strong>组</strong>字段，并且您只能选择您管理的组或这些组下的任何子组。</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">有关对公司的管理访问权限的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">授予用户对特定区域的管理访问权限</a>。</p> </li> 
        <li> <p><b>公司成员</b>：将现有用户添加到公司。 这样，您就可以将这些用户与此公司相关联。</p> <p>您与一个公司关联的用户的数量没有限制，但一个用户不能与多个公司关联。</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">自定义Forms部分</td> 
      <td> <p>如果有一些要添加到公司的字段在Workfront中不可用，则可以构建自定义表单并将其与公司关联。 您可以从下拉菜单中选择此表单，以将其附加到您的公司。 下拉菜单中仅列出活动的公司。 有关创建自定义表单的信息，请参阅<a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">创建自定义表单</a>。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >如果您对访问级别的公司具有管理访问权限，则还可以单击列表底部的“添加更多公司” 。 这会添加一行，您可以在其中快速配置新公司。

1. （可选）要编辑或删除公司，请至少选择一个公司，然后使用工具栏按钮编辑![编辑图标](assets/edit-icon.png)或删除![删除图标](assets/delete.png)。

   >[!NOTE]
   >
   >如果要删除公司，而公司被设置为主要公司或正用于其他对象，则系统会提示您选择其他公司来替换要删除的公司。 您选择的公司会成为“主要公司”，或者在公司分配到的对象上替换已删除的公司。

   有关编辑公司的信息，请参阅文章[创建和编辑公司](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md#adding-a-company-to-workfront)中的[在Workfront中创建或编辑公司](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)部分。

1. （可选）要导出公司列表，请单击“导出”图标![导出图标](assets/export.png)，然后为导出的列表选择所需的文件格式。
