---
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: 在Adobe Workfront Fusion中将用户添加到组织
description: 您可以在Adobe Workfront Fusion中将用户添加到组织。
author: Becky
feature: Workfront Fusion
exl-id: 98248cca-98f5-4eb5-b203-67e261df33f1
source-git-commit: 1b4a6d2b2ad57ddf1afd5dadf8b1fed358f95b61
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 0%

---

# 在Adobe Workfront Fusion中将用户添加到组织或团队

>[!IMPORTANT]
>
>此页面上描述的过程仅适用于尚未载入[!DNL Adobe Admin Console]的组织。 如果您的组织已登记到[!DNL Adobe Admin Console]，则必须通过[!DNL Adobe Admin Console]执行此操作。
>
>有关将您的组织移至[!DNL  Adobe Admin Console]和AdobeUnified Experience后添加用户的说明，请参阅[通过 [!DNL Adobe Admin Console]](/help/quicksilver/workfront-fusion/fusion-in-admin-console/add-fusion-users-admin-console.md)将用户添加到 [!DNL Adobe Workfront Fusion] 。
>
>有关因您的组织是否已登记到Adobe Admin Console而不同的过程列表，请参阅[基于平台的管理差异(Adobe Workfront Fusion/Adobe业务平台)](../../../quicksilver/workfront-fusion/fusion-in-admin-console/fusion-in-admin-console.md)。

## 访问要求

您必须具有以下权限才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
   <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
    <td> <p>[！UICONTROL计划]，[！UICONTROL工作]</p> </td> 
   </tr>
   <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]许可证**</td> 
   <td>
   <p>当前许可证要求：无[!DNL Workfront Fusion]许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]，[！UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]计划，则贵组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]才能使用本文中描述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]计划中。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]，才能使用本文中介绍的功能。</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">访问级别配置*</td> 
   <td> 
     <p>您必须是组织的[!DNL Workfront Fusion]管理员。</p>
     <p>您必须是团队的[!DNL Workfront Fusion]管理员。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 将用户添加到组织


<!--
<p>The procedure to add a user to your Fusion organization differs based on whether your organization has been onboarded to the Adobe Business Platform. </p>
<ul>
<li> <p><a href="#add-a-user-to-an-organization-that-has-been-onboarded-to-the-adobe-business-platform" class="MCXref xref">Add a user to an organization that has been onboarded to the Adobe Business Platform</a> </p> </li>
<li> <p><a href="#add-a-user-to-an-organization-that-has-not-been-onboarded-to-the-adobe-business-console" class="MCXref xref">Add a user to an organization that has not been onboarded to the Adobe Business Console</a> </p> </li>
</ul>
<div>
<p><strong>Add a user to an organization that has been onboarded to the Adobe Business Platform</strong></p>
<p>If your organization has been onboarded to the Adobe Business Platform, you must perform this action through the Adobe Admin Console.</p>
<p>For instructions on adding a user in the Adobe Admin Console:</p>
<ul>
<li> <p>See <a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create" class="MCXref xref">Create users in Workfront with the Adobe Admin Console</a></p> </li>
<li> <p>See the section "Add users" in the article <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li>
<li> <p>Contact your Adobe Admin Console Administrator.</p> </li>
</ul>
<p>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Business Platform, see <a href="../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md" class="MCXref xref">Platform-based administration differences (Adobe Workfront/Adobe Business Platform)</a>.</p>
</div>
<p><strong>Add a user to an organization that has not been onboarded to the Adobe Business Console</strong></p>

-->

要将用户添加到组织，您必须是要向其添加用户的组织的管理员。 有关角色的信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/organizations/organization-roles.md)中的[组织角色。

要将用户添加到组织，请执行以下操作：

1. 导航到菜单中的&#x200B;**[!UICONTROL 组织]**，然后选择要将用户添加到的组织。
1. 在仪表板中打开&#x200B;**[!UICONTROL 用户]**&#x200B;选项卡。
1. 单击&#x200B;**[!UICONTROL 邀请新用户]**，然后单击&#x200B;**[!UICONTROL 发送]**&#x200B;发送邀请。

   >[!NOTE]
   >
   >   
   >如果您看不到[!UICONTROL 邀请新用户]按钮，则表示您的组织已载入[!DNL Adobe Business Platform.]
   >
   >  有关将用户添加到已登记到[!DNL Adobe Business Platform]的组织中的说明，请参阅[通过 [!DNL Adobe Admin Console]](/help/quicksilver/workfront-fusion/fusion-in-admin-console/add-fusion-users-admin-console.md)将用户添加到 [!DNL Adobe Workfront Fusion] 

1. 填写表单。

   <table style="table-layout:auto">
<col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL电子邮件地址]</td>
      <td>
        输入用户的电子邮件地址
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL名称]</td>
      <td>
        <p>输入用户的全名</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL角色] </td>
      <td>选择用户的角色。 有关角色的解释，请参阅<a href="/help/quicksilver/workfront-fusion/organizations/organization-roles.md">组织和团队角色。</a></p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">团队</td>
      <td>选择您希望用户成为其成员的所有团队。</td>
    </tr>
    <tr>
      <td role="rowheader">注释</td>
      <td>输入用户的注释。 此注释将显示在用户邀请电子邮件中。</td>
    </tr>
  </tbody>
</table>

用户会收到一封邀请电子邮件，以便接受邀请。

## 将用户添加到团队

创建团队时，会将您的用户分配给团队。 如果需要将现有用户添加到团队，则可以在团队的“用户”页面上添加这些用户。

将用户添加到团队的处理从该团队的页面中进行。

1. 转到要将用户添加到的团队，方法是：选择左侧面板中的&#x200B;**组织**，单击组织页面上的&#x200B;**团队**&#x200B;选项卡，然后选择团队。

   或

   如果您在另一个团队的页面上，请单击页面顶部的团队下拉列表。

1. 在团队页面（页面顶部显示团队名称）上，选择&#x200B;**用户**&#x200B;选项卡。
1. 在页面上找到用户。 您组织中的用户即使不是团队成员，也会显示在此页面上。
1. 单击用户名右侧的&#x200B;**无**，然后选择您希望他们在团队中的角色。

用户即添加到团队。