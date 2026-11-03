---
user-type: administrator
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
title: 配置用户的验证访问权限
description: 作为Adobe Workfront管理员或Workfront Proof管理员，您可以配置用户在Workfront和Workfront Proof中创建和查看验证的访问权限。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 98c90139-f31a-41bc-af0b-577dd8b254e3
TQID: 'https://experienceleague.adobe.com/L-AMDvQYgtXJwxmtwekimbEA9OQQN72QHIcoQ2iKzGU'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4ea8bc003ce17978be5e5a6fd838012dfcfeae78
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 3%
---
# 配置用户的验证访问权限

作为Adobe Workfront管理员或Workfront Proof管理员，您可以配置用户在Workfront和Workfront Proof中创建和查看验证的访问权限。

有关可用于基本和集成校对的校对功能的信息，请参阅[访问Workfront中的校对功能](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td>“任一”</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td>规划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>您必须是Workfront管理员或Workfront Proof管理员。 有关Workfront管理员的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

+++

<!--

## Configure a user's proof permission profile

The permission profile you select is granted to the users for each proof that exists within your organization.

{{step-1-to-users}}
 
1. Select one or more users, then click **Edit**.  

1. In the **Access** section, click one of the following Workfront Proof permission options in the **Proof Permission Profile** drop-down menu:

   >[!NOTE]
   >
   >If you are on a legacy Workfront plan, make sure the **User can generate proofs** option is enabled, as explained above in the section [Enable and disable proofing for a user (legacy plans only)](#enable-and-disable-proofing-for-a-user-legacy-plans-only). 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Supervisor</strong> </td> 
      <td>Users can manage and view all proofs created on your organization's account. They can also edit reviewers added to these proofs. Users with this permission profile can't manage users or edit Workfront Proof settings.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Manager</strong> </td> 
      <td> <p> Users can manage and view proofs created or owned on your organization's account. They can view other users' proofs only when added as a reviewer. This is a default setting. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administrator</strong> </td> 
      <td> Users are given Administrator permissions in Workfront Proof and can edit account settings. Users can manage and view all proofs created on your organization's account. This includes adding and removing reviewers, proofs, and comments.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Custom</strong> </td> 
      <td> <p>Available only if you have configured a custom permission profile within Workfront Proof.</p> <p><b>NOTE</b>:  <p>Ensure that the permission profile you grant here does not provide higher access than the user's Access Level setting in Workfront (see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>). If it does provide higher access, the user can access proofs within Workfront Proof that he or she cannot access within Workfront.</p> <p>This is especially important if you plan to allow all Workfront users to access Workfront Proof directly from the Workfront as described in <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref">Access Workfront Proof from Adobe Workfront</a>.</p> <p>By default, only Workfront administrators have access to a direct link to the Workfront Proof site from the Workfront Global Navigation Bar.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   The permission profile you select is granted to the users for each proof that exists within your organization.

1. Click **Save Changes** to complete the update to the user settings.

   >[!NOTE]
   >
   >When you create or update a user in Workfront and the user's Workfront email address matches that of a licensed Workfront Proof user, the system enables proofing for the user within Workfront. For more information, see [User synchronization between Adobe Workfront and Workfront Proof](../../../administration-and-setup/manage-workfront/configure-proofing/user-sync-proofing.md).

### Considerations

Consider the following information when setting permissions:

* If you change a user's permission profile to a profile with fewer permissions, the user might lose visibility to existing proofs within Workfront. This can occur when someone shares a task with a user within Workfront, but doesn't share the proof attached to the task (see [Share a proof within Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [Share a proof within Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)).
* You can set Workfront Proof permissions from Workfront only if your Workfront environment is integrated with a Workfront Proof Premium account. If you cannot use proofing as discussed in this section, contact your Workfront administrator.
* At least one user in your Workfront environment must have Administrator permissions for proofing. An error message appears if you try to attempt to remove Administrator permissions for proofing from all users.
* When you change a user's Workfront Access level to any level other than System Administrator, the user's Workfront Proof permission profile defaults to Manager.   

* When you change the Workfront Access level to System Administrator, the Proof Permission profile changes to Administrator.

-->

## 通过Workfront主菜单为所有用户配置Workfront Proof访问权限 {#configure-workfront-proof-access-via-workfront-main-menu-for-all-users}

默认情况下，只有在Workfront中拥有管理权限的用户才能访问Workfront Proof，如[从Adobe Workfront访问Workfront Proof](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md)所述。

您可以通过联系Workfront Proof支持部门并提交请求，向所有用户授予对Workfront主菜单中Workfront按钮的访问权限。

>[!IMPORTANT]
>
> 如果您计划允许所有Workfront用户直接从Workfront全局导航栏访问Workfront Proof，请确保每个用户的权限配置文件不会提供比该用户在Workfront中的访问级别更多的访问权限。 这会阻止用户在Workfront Proof中访问他们无法在Workfront中访问的校样。 有关详细信息，请参阅[为用户启用和禁用校对（仅限旧版计划）](#enable-and-disable-proofing-for-a-user-legacy-plans-only)。

## 配置用户对桌面验证查看器的访问权限

如果贵组织中的用户希望使用桌面验证查看器而不是Web验证查看器来查看交互式内容，您可以将桌面验证查看器配置为在用户打开交互式内容验证时自动启动。 有关该桌面校对查看器的信息以及它与Web校对查看器的不同之处，请参阅[了解桌面校对查看器](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md)和[Web校对查看器和桌面校对查看器之间的区别](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md)。

1. 在Workfront中，单击全局导航栏中的Workfront Proof图标以访问Workfront Proof。

   ![校对图标](assets/proof-access-proofhq-350x39.png)

1. 单击Workfront Proof右上角附近的&#x200B;**帐户设置**，然后单击&#x200B;**设置**&#x200B;选项卡。

1. 在&#x200B;**验证默认值**&#x200B;下，在&#x200B;**交互式验证的桌面验证查看器**&#x200B;行的末尾，单击&#x200B;**设置**。

1. 按照[为组织配置校对设置](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md)一文中[桌面校对查看器](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#desktop-proofing-viewer)的说明，修改桌面校对查看器设置。

1. 单击&#x200B;**保存**。

## 为交互式验证配置自定义设备

您可以将任何自定义设备添加到系统中，从而使用户能够查看交互式内容，并在使用Desktop Proofing Viewer时模拟内容在特定设备上的显示方式。 （此功能在Web校对查看器中不可用，用户可以在其中查看交互式内容，但只能查看以各种分辨率显示的内容，不能查看各种设备上的内容。）

有关详细信息，请参阅[在验证查看器中更改交互式验证分辨率](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md)。

1. 从Workfront访问Workfront Proof界面，如[从Adobe Workfront访问Workfront Proof](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md)中所述。
1. 修改桌面验证查看器设置，如[为组织配置验证设置](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md)中的[为验证配置自定义设备](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#custom-devices-for-proofs)中所述。
