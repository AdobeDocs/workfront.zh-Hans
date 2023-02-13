---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: 创建和编辑公司
description: 您可以将公司添加到 [!DNL Workfront] 并将其用于财务规划、报告、定义对象相关权限和保密信息。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: bb597032-3395-4c9a-b622-5c920ba55131
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '1440'
ht-degree: 0%

---

# 创建和编辑公司

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

公司是 [!DNL Adobe Workfront] 代表您的组织、组织内的部门或您与之合作的客户。 您可以将公司添加到 [!DNL Workfront] 并将其用于财务规划、报告、定义对象相关权限和保密信息。

## 访问要求

要在 [!DNL Workfront]:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] 计划*</p> </td> 
   <td>[!UICONTROL Team]或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] 许可证*</p> </td> 
   <td>[!UICONTROL计划]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>以下任一项：</p> 
    <ul> 
     <li> <p>[!UICONTROL系统管理员]访问级别，允许您编辑系统中的任何公司。 有关更多信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>. </p> </li> 
     <li> <p>对管理公司的管理访问权限，用于编辑系统中的任何公司。 有关更多信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用户对特定区域的管理访问权限</a>.</p> </li> 
    </ul> <p><b>注释</b>:  
     <ul> 
      <li> <p>您还可以管理与任何分配为群组管理员的群组关联的公司。</p> </li> 
      <li> <p>要在 [!DNL Workfront] 系统时，您必须具有以下一项：</p> 
       <ul> 
        <li> <p>[!UICONTROL系统管理员]访问级别。 有关更多信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>. </p> </li> 
        <li> <p>在访问级别中，必须为[!UICONTROL Users]设置选择[!UICONTROL Edit]。 此外，对于[!UICONTROL用户]设置，在[!UICONTROL微调您的设置]下 <img src="assets/gear-icon-in-access-levels.png"> ，则必须启用[!UICONTROL创建]选项和两个[!UICONTROL用户管理员]选项中的至少一个选项。 </p> <p> <img src="assets/access-req-users.png"> </p> <p>如果您使用[!UICONTROL用户管理员（群组用户）]选项，则您必须是用户所属群组的群组管理员。</p> </li> 
       </ul> <p>有关访问级别中“用户”设置的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问级别配置，请联系您的 [!DNL Workfront] 管理员。

## 将用户添加到公司的好处 {#benefits-of-adding-users-to-a-company}

* 您可以通过将用户与直接报表关联来构建公司的组织图。 只能将同一公司的用户添加为该公司其他用户的直接报表。
* 作为项目经理，您可以确定同一公司内的可用资源。
* 您可以选择以下任一或所有设置，以在公司之间保持信息保密：

   * 来自同一公司的用户可以看到彼此的请求。

      有关如何 [!DNL Workfront] 管理员可以根据用户的公司授予对请求的类似访问权限，请参阅部分 [为 [!DNL Workfront]](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#changing-task-and-issue-preferences) 在文章中 [配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

      有关群组管理员如何根据用户的公司授予对请求的类似访问权限的详细信息，请参阅 [为组配置任务和问题首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   * 用户只能看到与其公司关联的请求队列。 有关限制请求队列可见性的更多信息，请参阅 [提供对请求队列的访问权限](../../../manage-work/requests/create-and-manage-request-queues/provide-access-to-request-queues.md).
   * 您可以限制用户仅查看其公司或公司以及主公司中的用户。 有关用户隐私的主要公司功能的信息，请参阅 [创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   * 用户可以限制他们对项目所做的更新，使其仅供公司用户查看。 有关将更新设为公司私有的详细信息，请参阅 [更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## 在中创建或编辑公司 [!DNL Workfront] {#create-or-edit-a-company-in-workfront}

您可以添加的公司数量没有限制。 但是，我们建议限制您使用的公司数量，因为对象权限可能会出现问题，太多碎片可能会干扰用户对工作项的可见性。

默认情况下，与您的实例关联的公司 [!DNL Workfront] 已在 [!DNL Workfront] 系统，并且是贵组织的主要公司。 它与您的客户名称同名。 有关客户信息的更多信息，请参阅 [!DNL Workfront]，请参阅 [配置系统的基本信息](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

添加或编辑公司：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 单击 **[!UICONTROL 公司]**.
1. 如果要添加公司，请单击 **[!UICONTROL 新公司]**.

   或

   如果您正在编辑现有公司，请选择公司，然后单击 **[!UICONTROL 编辑]**.

1. 使用显示的选项可配置以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic Info]部分</td> 
      <td> 
       <ul> 
        <li> <p><b>[!UICONTROL公司名称]</b>:键入公司名称。</p> </li> 
        <li> <p><b>[!UICONTROL处于活动状态]</b>:启用此选项后，用户可以找到公司并将其附加到他们创建和编辑的项目。 不活动的公司不能附加到项目。 默认情况下，此选项处于启用状态。</p> </li> 
        <li> <p><b>[!UICONTROL这是主要公司]</b>:将公司分配为贵组织的主公司。 主公司通常表示 [!DNL Workfront] 帐户。</p> <p>您可以有一个公司，或者没有一个公司被指定为主公司，但不能有多个公司被指定为主公司。 有关更多信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> <p><b>注意</b>:通过修改其访问级别，您可以限制用户查看其他用户：仅在其主要公司中，或在其关联公司和主要公司中。 有关主公司如何与用户的访问级别一起使用的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </li> 
        <li> <p><b>[!UICONTROL组]</b>:如果有与公司有业务往来的组，您可以在此处添加该组的名称。 这对于需要报告和管理其组与之开展业务的所有公司的组管理员非常有用。</p> <p><b>重要信息</b>:如果您未关联将与此公司合作的组，则该组的管理员将无法访问，除非他们具有其访问级别中公司的管理访问权限。 有关如何授予此访问权限的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用户对特定区域的管理访问权限</a>.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">开始键入组名称，然后按 <strong>[!UICONTROL Enter]</strong> 显示时。</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">当您将组分配给公司时，该组的组管理员将获得对公司的[!UICONTROL Manage]访问权限。 有关更多信息，请参阅 <a href="#group-administrators-and-companies" class="MCXref xref">组管理员和公司</a> 在本文中。</p> </li> 
        <li> <p><b>[!UICONTROL公司成员]</b>:将现有用户添加到公司。 通过执行此操作，您会将这些用户与此公司关联。</p> <p>您与一个公司关联的用户数量没有限制，但一个用户不能与多个公司关联。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL账单费率]部分</td> 
      <td> <p>您可以改写与公司层职务职责关联的开单费率。 有关创建职务角色并将其与开单费率关联的信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">创建和管理作业角色</a>.</p> <p>有关公司级别覆盖账单费率的详细信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md" class="MCXref xref">在公司层改写职务职责开单费率</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL自定义Forms]部分</td> 
      <td> <p>如果要添加到公司的字段在 [!DNL Workfront]，则可以构建自定义表单并将其与您的公司关联。 您可以从下拉菜单中选择此表单，以将其附加到您的公司。 下拉菜单中只列出活动公司。 有关创建自定义Forms的信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">创建或编辑自定义表单</a>. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 如果要创建新公司，请单击 **[!UICONTROL 创建公司]**.

   或

   如果您正在编辑现有公司，请单击 **[!UICONTROL 保存更改]**.

## 管理公司成员资格

有关管理现有公司成员资格的信息，请参阅 [管理公司成员资格](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## 关于与公司共享对象

某些权限可供与公司关联的用户使用，如 [将用户添加到公司的好处](#benefits-of-adding-users-to-a-company). 除了这些权限之外，您还可以允许用户在 [!DNL Workfront] 与公司共享对象。

您可以与其整个公司共享对象，而不是一次与一个单独的用户共享对象。 公司中的每个用户都对该对象具有相同的权限。

有关共享对象的更多信息，请参阅 [对象共享权限概述](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## 组管理员和公司 {#group-administrators-and-companies}

当 [!DNL Workfront] 管理员将组分配给公司，组管理员将获取组增益 [!UICONTROL 管理] 在 [!UICONTROL 设置]. 这包括对 [!UICONTROL 公司] 页面 [!UICONTROL 设置]，以便他们查看和管理与其群组关联的公司。

通过此访问 [!UICONTROL 公司] 页面，群组管理员可以将群组分配给公司，但它必须是群组管理员创建的公司。 如果组管理员的访问级别未配置公司的管理访问权限，则 [!UICONTROL 组] 群组管理员创建公司时，字段是必填字段 — 其标题为粗体，表示以下内容：

![](assets/manage-company-group-field-req.jpg)

有关用户如何在其访问级别获得对公司的管理访问权限的信息，请参阅 [授予用户对特定区域的管理访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

有关在 [!UICONTROL 设置] 区域，请参阅 [在中创建或编辑公司 [!DNL Workfront]](#create-or-edit-a-company-in-workfront) 在本文中。
