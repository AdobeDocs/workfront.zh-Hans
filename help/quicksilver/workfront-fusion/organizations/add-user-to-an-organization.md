---
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: 在Adobe Workfront Fusion中将用户添加到组织
description: 您可以在Adobe Workfront Fusion中将用户添加到组织。
author: Becky
feature: Workfront Fusion
exl-id: 98248cca-98f5-4eb5-b203-67e261df33f1
source-git-commit: 5d4434d090c4b6cdefc9c313fecccf6d6e9a510b
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 0%

---

# 在Adobe Workfront Fusion中将用户添加到组织

>[!IMPORTANT]
>
>本页中介绍的过程仅适用于尚未载入的组织 [!DNL Adobe Admin Console]. 如果您的组织已载入 [!DNL Adobe Admin Console]，您必须通过 [!DNL Adobe Admin Console].
>
>有关在中添加用户的说明[!DNL  Adobe Admin Console]，请参阅文章中的“编辑用户详细信息”部分 [单独管理用户](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) 或联系 [!UICONTROL Adobe Admin Console] 管理员。
>
>有关因您的组织是否已登记到Adobe Admin Console而不同的过程列表，请参阅 [基于平台的管理差异(Adobe Workfront Fusion/Adobe业务平台)](../../../quicksilver/workfront-fusion/fusion-in-admin-console/fusion-in-admin-console.md).

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
   <p>当前许可证要求：否 [!DNL Workfront Fusion] 许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] 对于工作自动化和集成]，[！UICONTROL [!DNL Workfront Fusion] 工作自动化]</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 计划，您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 计划。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">访问级别配置*</td> 
   <td> 
     <p>您必须是 [!DNL Workfront Fusion] 组织管理员。</p>
     <p>您必须是 [!DNL Workfront Fusion] 您的团队的管理员。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关的信息 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

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

要将用户添加到组织，您必须是要向其添加用户的组织的管理员。 有关角色的信息，请参见 [中的组织角色 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/organizations/organization-roles.md).

要将用户添加到组织，请执行以下操作：

1. 导航到 **[!UICONTROL 组织]** 在菜单中，选择要将用户添加到的组织。
1. 打开 **[!UICONTROL 用户]** 选项卡。
1. 单击 **[!UICONTROL 邀请新用户]**，填写表单（电子邮件、消息、角色），然后单击以发送邀请 **[!UICONTROL 发送]**.

>[!NOTE]
>
>   
><p>如果您看不到[！UICONTROL邀请新用户]按钮，则表示您的组织已载入到 [!DNL Adobe Business Platform.] </p>
>
>   <p>有关将用户添加到已载入的组织的说明 [!DNL Adobe Business Platform]，请参见 <a href="#add-a-user-to-an-organization-that-has-been-onboarded-to-the-adobe-business-platform" class="MCXref xref">将用户添加到已载入的组织 [!DNL Adobe Business Platform]</a></p>

用户会收到一封邀请电子邮件，以便接受邀请。
