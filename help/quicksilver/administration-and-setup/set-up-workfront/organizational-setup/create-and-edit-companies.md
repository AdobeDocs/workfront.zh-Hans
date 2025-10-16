---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: 创建和编辑公司
description: 您可以将公司添加到 [!DNL Adobe Workfront] 中，并将它们用于财务规划、报告、定义对象权限以及保密信息。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bb597032-3395-4c9a-b622-5c920ba55131
source-git-commit: 30b61b32add4c6d062b5b524773d309008c9563d
workflow-type: tm+mt
source-wordcount: '1399'
ht-degree: 0%

---

# 创建和编辑公司

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment, and is being released in a phased rollout to Production.</span>-->

公司是[!DNL Adobe Workfront]中的组织单位，可以代表您的组织、组织内的部门或与您合作的客户。 您可以将公司添加到[!DNL Workfront]中，并将它们用于财务规划、报告、定义对象权限以及保密信息。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Workfront] 包</p> </td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 许可证</p> </td> 
   <td><p>[！UICONTROL计划]</p>
   <p>[！UICONTROL标准版]</p>
   </td> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td> <p>您必须具备以下任一项：</p> 
    <ul> 
     <li> <p>[！UICONTROL系统管理员]访问级别，允许您编辑系统中的任何公司。</p> </li> 
     <li> <p>管理公司的管理权限，允许您编辑系统中的任何公司。</p> </li> 
    </ul> <p><b>注释</b>：  
     <ul> 
      <li> <p>您还可以管理与您被分配为组管理员的任何组关联的公司。</p> </li> 
      <li> <p>若要在[!DNL Workfront]系统中添加和删除用户，您必须具备以下任一项：</p> 
       <ul> 
        <li> <p>[！UICONTROL系统管理员]访问级别。 </p> </li> 
        <li> <p>您的访问级别中的<b>[！UICONTROL用户]</b>设置配置为<b>[！UICONTROL编辑]</b>访问权限，且<b>[！UICONTROL创建]</b>和在<b>[！UICONTROL微调您的设置]</b> <b>下启用的两个</b>[！UICONTROL用户管理]<img src="assets/gear-icon-in-access-levels.png">选项中的至少一个选项。 </p> <p> <img src="assets/access-req-users.png"> </p> <p>在这两个选项中，如果启用了<b>[！UICONTROL用户管理员（组用户）]</b>，您必须是该用户所属组的组管理员。</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 将用户添加到公司的好处 {#benefits-of-adding-users-to-a-company}

* 通过将用户与直接报告相关联，您可以构建公司的组织结构图。 只有来自同一公司的用户才能添加为该公司其他用户的直接报告。
* 作为项目经理，您可以确定同一公司内的可用资源。
* 通过选择下列一项或全部设置，您可以在公司之间保持信息的私密性：

   * 来自同一公司的用户可以看到彼此的请求。

     有关[!DNL Workfront]管理员如何根据用户的公司授予请求类似访问权限的更多信息，请参阅[配置系统范围的任务和问题偏好设置 [!DNL Workfront]](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#changing-task-and-issue-preferences)文章中的[为](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)中的每个人配置任务和问题偏好设置部分。

     有关组管理员如何根据用户的公司授予请求类似访问权限的详细信息，请参阅[配置组的任务和问题首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)。

   * 用户只能看到与其公司关联的请求队列。 有关限制请求队列可见性的详细信息，请参阅[提供对请求队列的访问权限](../../../manage-work/requests/create-and-manage-request-queues/provide-access-to-request-queues.md)。
   * 您可以将用户限制为仅可查看其公司中的用户，或公司中的用户以及主公司的用户。 有关用户隐私的主要公司功能的信息，请参阅[创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。
   * 用户可以限制仅由公司用户查看他们对项目所做的更新。 有关将更新设为公司私有的详细信息，请参阅[更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。

## 在[!DNL Workfront]中创建或编辑公司 {#create-or-edit-a-company-in-workfront}

您可以添加的公司数量没有限制。 但是，我们建议限制您使用的公司数量，因为对象权限可能会出现问题 — 碎片过多可能会影响用户对工作项的可见性。

默认情况下，与您的[!DNL Workfront]实例关联的公司已在您的[!DNL Workfront]系统中创建，并且是您组织的主要公司。 其名称与您的客户名称相同。 有关[!DNL Workfront]中客户信息的详细信息，请参阅[配置系统的基本信息](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md)。

添加或编辑公司：

{{step-1-to-setup}}

1. 单击&#x200B;**[!UICONTROL 公司]**。

   此时将显示公司列表。

1. 如果要添加公司，请单击&#x200B;**[!UICONTROL 新建公司]**。

   或

   如果您正在编辑现有公司，请选择该公司，然后单击公司列表顶部的&#x200B;**[!UICONTROL 编辑]**&#x200B;图标![编辑图标](assets/edit-icon.png)。

1. 更新&#x200B;**基本信息**&#x200B;部分中的以下信息：

   * **公司名称**<!--<span class="preview">or **Name**</span>-->：键入公司的名称。
   * **处于活动状态**：启用此选项后，用户可以找到该公司并将其附加到他们创建和编辑的项目。 无法将非活动的公司附加到项目。 此选项默认处于启用状态。
   * **这是主要公司**<!--<span class="preview">or **Is Primary**</span>-->：将公司指定为组织的主要公司。 主要公司通常表示您的大多数用户工作的Workfront帐户。

     您可以将一家公司指定为主要公司，也可以不指定任何公司，但不得将多家公司指定为主要公司。 有关详细信息，请参阅[创建和修改自定义访问级别](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

     >[!NOTE]
     >
     >通过修改用户的访问级别，您可以限制用户查看其他用户：仅查看其主公司中的用户，或查看其关联公司和主公司中的用户。 有关主公司如何与用户的访问级别配合使用的信息，请参阅[创建和修改自定义访问级别](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

   * **组**：如果有一个组与公司开展业务，您可以在此处添加该组的名称。 这对于需要报告和管理其组与其开展业务的所有公司的组管理员非常有用。

     如果您不关联将与此公司合作的组，则该组的管理员无法访问该公司，除非他们对具有访问级别的公司具有管理访问权限。 有关如何授予此访问权限的信息，请参阅[授予用户对特定区域的管理访问权限](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

     开始键入组的名称，然后在该组出现时将其选定。

     将组分配给公司时，该组的组管理员将获得对该公司的管理访问权限。 有关详细信息，请参阅本文中的[组管理员和公司](#group-administrators-and-companies)。

   * **公司成员**：将现有用户添加到公司。 这样，您就可以将这些用户与此公司相关联。

     开始键入用户的名称，然后在该用户出现时将其选定。

     您与一个公司关联的用户的数量没有限制，但一个用户不能与多个公司关联。

1. 在&#x200B;**自定义Forms**&#x200B;分区中添加或更新自定义表单。

   如果有一些要添加到公司的字段在Workfront中不可用，则可以构建自定义表单并将其与公司关联。

   您可以从下拉菜单中选择此表单，以将其附加到您的公司。 菜单中仅列出活动的自定义表单。

   >[!NOTE]
   >
   >高级自定义表单功能(如外部查找字段和Workfront本地字段)仅在您于详细信息页面（而非编辑公司对话框）中打开公司记录时可用。 （在公司列表中，单击公司名称以打开详细信息。）

   有关创建自定义表单的信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

1. （视情况而定）如果您正在创建公司，请单击&#x200B;**[!UICONTROL 创建公司]**<!--<span class="preview">or **Save**</span>-->。

   或

   如果您正在编辑现有公司，请单击&#x200B;**[!UICONTROL 保存更改]**<!--<span class="preview">or **Save**</span>-->。

## 管理公司成员资格

有关管理现有公司成员资格的信息，请参阅[管理公司成员资格](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md)。

## 管理记帐费率

有关在公司级别覆盖计费率的信息，请参阅[在公司级别覆盖工作角色计费率](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md)。

## 与公司共享对象概述

某些权限适用于与公司关联的用户，如[将用户添加到公司的好处](#benefits-of-adding-users-to-a-company)部分中所述。 除了这些权限之外，您还可以允许用户通过与其公司共享对象来查看、贡献或编辑[!DNL Workfront]中的对象。

您无需一次与单个用户共享对象，而是可以与其整个公司共享该对象。 公司中的每个用户对该对象具有相同的权限。

有关共享对象的详细信息，请参阅[共享对象权限概述](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

## 组管理员和公司 {#group-administrators-and-companies}

当[!DNL Workfront]管理员将组分配给公司时，该组的组管理员将在[!UICONTROL 设置]中获得[!UICONTROL 管理]对公司的访问权限。 这包括访问[!UICONTROL 设置]中的[!UICONTROL 公司]页面，他们可以在该页面查看和管理与其组关联的公司。

通过访问[!UICONTROL 公司]页面，组管理员可以将组分配给公司，但该公司必须是组管理员创建的公司。 如果组管理员的访问级别未配置为对公司的管理访问权限，则当组管理员创建公司时，需要[!UICONTROL 组]字段，其粗体标题指示如下：

![编辑公司](assets/group-admin-add-company.png)

有关用户如何获得其访问级别的公司管理访问权限的信息，请参阅[授予用户对特定区域的管理访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

有关在[!UICONTROL 设置]区域管理公司的信息，请参阅本文中的[在 [!DNL Workfront]](#create-or-edit-a-company-in-workfront)中创建或编辑公司。

<!-- OLD HTML TABLE
<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic Info] section</td> 
      <td> 
       <ul> 
        <li> <p><b>[!UICONTROL Company Name]</b>: Type a name for the company.</p> </li> 
        <li> <p><b>[!UICONTROL Is Active]</b>: When this option is enabled, users can find the company and attach it to projects that they create and edit. An inactive company cannot be attached to projects. This option is enabled by default.</p> </li> 
        <li> <p><b>[!UICONTROL This is the Primary Company]</b>: Assigns the company as your organization's primary company. The primary company typically represents your [!DNL Workfront] account where most of your users work.</p> <p>You can have one company or no company designated as a primary company, but you cannot have multiple companies designated as primary companies. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> <p><b>NOTE</b>: By modifying their access levels, you can restrict users to see other users: only in their primary company, or in their associated company and the primary company. For information about how the primary company works with users' access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </li> 
        <li> <p><b>[!UICONTROL Group]</b>: If there is a group that conducts business with the company, you can add the name of the group here. This is useful for group administrators who need to report on and manage all the companies that their groups do business with.</p> <p><b>IMPORTANT</b>: If you don't associate the group that will be working with this company, administrators for the group can't access the company unless they have administrative access to companies in their access level. For information about how this access is granted, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Start typing the name of the group, then press <strong>[!UICONTROL Enter]</strong> when it appears.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">When you assign a group to a company, the group administrators for the group gain [!UICONTROL Manage] access to the company. For more information, see <a href="#group-administrators-and-companies" class="MCXref xref">Group administrators and companies</a> in this article.</p> </li> 
        <li> <p><b>[!UICONTROL Company Members]</b>: Add existing users to the company. By doing this, you are associating these users with this company.</p> <p>There is no limit to how many users you associate with one company, but a user cannot be associated with more than one company.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Custom Forms] section</td> 
      <td> <p>If there are fields that you want to add to your company that are not available in [!DNL Workfront], you can build a custom form and associate it with your company. </p> <p>You can attach this form to your company by selecting it from the drop-down menu. Only active custom forms are listed in the menu.</p> <p><strong>Note:</strong> Advanced custom form features such as External lookup fields and Workfront native fields are only available when you open the company record on the details page, not on the Edit Company dialog. (From the list of companies, click the company name to open the details.)</p> <p> For information about creating custom forms, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Create a custom form</a>. </p> </td>
     </tr> 
    </tbody> 
   </table>
   -->
