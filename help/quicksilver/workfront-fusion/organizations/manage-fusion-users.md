---
filename: manage-fusion-users
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: 管理 [!DNL Adobe Workfront Fusion] 您组织中的用户
description: 管理 [!DNL Adobe Workfront Fusion] 您组织中的用户
author: Becky
feature: Workfront Fusion
exl-id: fbb858a6-1230-41b4-892a-4ffeb2711922
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# 管理 [!DNL Adobe Workfront Fusion] 您组织中的用户

[!DNL Adobe Workfront Fusion] 管理员可以管理内的用户角色 [!DNL Workfront Fusion].

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on adding a user in the Adobe Admin Console:
>
>* See [Add a user to an organization in Adobe Workfront Fusion](../../workfront-fusion/organizations/add-user-to-an-organization.md#create)
>* See the section "Add users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html)
>* Contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront Fusion/Adobe Business Platform)](../../workfront-fusion/fusion-in-admin-console/fusion-adobe-admin-console.md).

-->

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
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] （对于工作自动化和集成），[！UICONTROL [!DNL Workfront Fusion] 工作自动化]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 计划，您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 计划。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。</p>
   </td> 
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

## 查看或编辑用户角色 {#view}

[!DNL Adobe Workfront Fusion] 管理员可以查看和更新用户角色。

1. 以身份登录时 [!DNL Workfront Fusion] 管理员，选择 **[!UICONTROL 用户]** 左侧导航栏中。
1. 单击 **[!UICONTROL 详细信息]** 在要查看的用户行中。
1. （可选）要更新用户的角色，请单击 **[!DNL Role]** 列中，选择要更改用户角色的组织行，然后选择新角色。

## 查看或编辑用户详细信息 {#view2}

[!DNL Adobe Workfront Fusion] 管理员可以查看和更新用户详细信息。

1. 以身份登录时 [!DNL Workfront Fusion] 管理员，选择 **[!UICONTROL 用户]** 左侧导航栏中。
1. 单击 **[!UICONTROL 详细信息]** 在要查看的用户行中。
1. （可选）要更新用户的详细信息，请单击 **[!UICONTROL 选项]** ，然后选择 **[!UICONTROL 更改详细信息]**.

## 删除用户 {#delete}

[!DNL Adobe Workfront Fusion] 管理员可以删除用户。

1. 以身份登录时 [!DNL Workfront Fusion] 管理员，选择 [!UICONTROL 用户] 左侧导航栏中。
1. 单击 **[!UICONTROL 详细信息]** 在要查看的用户行中。
1. （可选）要更新用户的详细信息，请单击 **[!UICONTROL 选项]** ，然后选择 **[!UICONTROL 删除]**.

### 在Workfront Fusion中删除用户时的注意事项

* 删除用户时，用户的连接、键和Webhook将被删除。 属于该用户的任何方案都将转移到组织“所有者”。 必须更新这些场景中的连接，因为属于用户的连接不再有效。
* 如果删除的用户拥有任何应用程序或公共模板，则应用程序或公共模板将被转移给组织“所有者”。 如果没有组织“所有者”，则应用程序或公共模板将转移给其他用户。
