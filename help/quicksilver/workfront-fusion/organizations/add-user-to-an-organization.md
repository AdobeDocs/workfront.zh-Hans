---
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: 在Adobe Workfront Fusion中将用户添加到组织
description: 您可以在Adobe Workfront Fusion中将用户添加到组织。
author: Becky
feature: Workfront Fusion
exl-id: 98248cca-98f5-4eb5-b203-67e261df33f1
source-git-commit: 392eee3c7b1aacf92d7877f07a8154924f3926a0
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---

# 在Adobe Workfront Fusion中将用户添加到组织

>[!IMPORTANT]
>
>本页中介绍的过程仅适用于尚未载入的组织。 [!DNL Adobe Admin Console]. 如果您的组织已载入 [!DNL Adobe Admin Console]，您必须通过 [!DNL Adobe Admin Console].
>
>有关在中添加用户的说明[!DNL  Adobe Admin Console]，请参阅文章中的“编辑用户详细信息”部分 [单独管理用户](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) 或联系 [!UICONTROL Adobe Admin Console] 管理员。
>
>有关因贵组织是否已载入Adobe Admin Console而不同的过程列表，请参阅 [基于平台的管理差异(Adobe Workfront Fusion/Adobe业务平台)](../../../quicksilver/workfront-fusion/fusion-in-admin-console/fusion-in-admin-console.md).

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
   <td> <p>Workfront Fusion for Work Automation and Integration，</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">访问级别配置*</td> 
   <td> 
     <p>您必须是 [!DNL Workfront Fusion] 组织管理员。</p>
     <p>您必须是 [!DNL Workfront Fusion] 团队管理员。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关以下项的信息 [!DNL Adobe Workfront Fusion] 许可证，请参见 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 将用户添加到组织

<p>根据您的组织是否已载入到Adobe业务平台，向Fusion组织添加用户的过程有所不同。 </p>
<ul>
<li> <p><a href="#add-a-user-to-an-organization-that-has-been-onboarded-to-the-adobe-business-platform" class="MCXref xref">将用户添加到已载入到Adobe业务平台的组织</a> </p> </li>
<li> <p><a href="#add-a-user-to-an-organization-that-has-not-been-onboarded-to-the-adobe-business-console" class="MCXref xref">将用户添加到尚未载入到Adobe业务控制台的组织</a> </p> </li>
</ul>
<div>
<p><strong>将用户添加到已载入到Adobe业务平台的组织</strong></p>
<p>如果贵组织已登记到Adobe业务平台，则必须通过Adobe Admin Console执行此操作。</p>
<p>有关在Adobe Admin Console中添加用户的说明：</p>
<ul>
<li> <p>参见 <a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create" class="MCXref xref">使用Adobe Admin Console在Workfront中创建用户</a></p> </li>
<li> <p>请参阅文章中的“添加用户”部分 <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">单独管理用户</a></p> </li>
<li> <p>联系Adobe Admin Console管理员。</p> </li>
</ul>
<p>有关因贵组织是否已载入Adobe业务平台而不同的过程列表，请参阅 <a href="../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md" class="MCXref xref">基于平台的管理差异(Adobe Workfront/Adobe业务平台)</a>.</p>
</div>
<p><strong>将用户添加到尚未载入到Adobe业务控制台的组织</strong></p>

要将用户添加到组织，您必须是要向其添加用户的组织的管理员。 有关角色的信息，请参见 [中的组织角色 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/organizations/organization-roles.md).

要将用户添加到组织，请执行以下操作：

1. 导航到 **[!UICONTROL 组织]** 在菜单中，选择要将用户添加到的组织。
1. 打开 **[!UICONTROL 用户]** 选项卡。
1. 单击 **[!UICONTROL 邀请新用户]**，填写表单（电子邮件、消息、角色），然后单击以发送邀请 **[!UICONTROL 发送]**.

>[!NOTE]
>
>   
><p>如果您没有看到[！UICONTROL邀请新用户]按钮，则表示您的组织已载入 [!DNL Adobe Business Platform.] </p>
>
>   <p>有关将用户添加到已载入的组织的说明 [!DNL Adobe Business Platform]，请参见 <a href="#add-a-user-to-an-organization-that-has-been-onboarded-to-the-adobe-business-platform" class="MCXref xref">将用户添加到已载入的组织 [!DNL Adobe Business Platform]</a></p>

用户会收到一封邀请电子邮件，用户可以通过单击 [!UICONTROL 接受角色] 按钮。
