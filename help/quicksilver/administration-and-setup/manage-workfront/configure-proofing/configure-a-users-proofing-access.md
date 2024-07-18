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
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1244'
ht-degree: 0%

---

# 配置用户的验证访问权限

作为Adobe Workfront管理员或Workfront Proof管理员，您可以配置用户在Workfront和Workfront Proof中创建和查看验证的访问权限。

有关可用于基本和集成校对的校对功能的信息，请参阅[访问Workfront中的校对功能](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md)。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>您必须是Workfront管理员或Workfront Proof管理员。 有关Workfront管理员的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 为用户启用和禁用验证（仅限旧版计划） {#enable-and-disable-proofing-for-a-user-legacy-plans-only}

如果您的组织使用的是旧版Select或Premium Workfront计划，则作为Workfront管理员，您可以为用户启用和禁用验证功能。

为用户启用验证时，Workfront为用户启用选项以自动生成验证。

尽管您可以将用户启用为验证用户，但是该用户必须具有管理员权限，才能直接从Workfront主菜单导航到Workfront Proof界面。 有关如何为Workfront系统中的所有验证用户启用此选项的信息，请参阅[通过Workfront主菜单为所有用户配置Workfront Proof访问权限](#configure-workfront-proof-access-via-workfront-main-menu-for-all-users)。

1. 在&#x200B;**主菜单**&#x200B;中，选择&#x200B;**用户**。

1. 选择一个用户，然后单击&#x200B;**编辑**&#x200B;图标。
1. 在&#x200B;**访问**&#x200B;部分中，选择或取消选择&#x200B;**用户可以生成验证**。

## 配置用户的校对权限配置文件

您选择的权限配置文件将授予用户用于您组织内存在的每个证明。

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)，然后单击&#x200B;**用户** ![](assets/users-icon-in-main-menu.png)。
1. 选择一个或多个用户，然后单击&#x200B;**编辑**。

1. 在&#x200B;**访问**&#x200B;部分中，单击&#x200B;**校对权限配置文件**&#x200B;下拉菜单中的以下Workfront Proof权限选项之一：

   >[!NOTE]
   >
   >如果您使用的是旧版Workfront计划，请确保已启用&#x200B;**用户可生成验证**&#x200B;选项，如上文[为用户启用和禁用验证（仅限旧版计划）](#enable-and-disable-proofing-for-a-user-legacy-plans-only)部分中所述。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>主管</strong> </td> 
      <td>用户可以管理和查看在您组织的帐户中创建的所有验证。 他们还可以编辑添加到这些校样的审阅人。 具有此权限配置文件的用户无法管理用户或编辑Workfront Proof设置。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>经理</strong> </td> 
      <td> <p> 用户可以管理和查看在您组织的帐户中创建或拥有的验证。 他们只能在添加为审阅者时查看其他用户的验证。 这是默认设置。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>管理员</strong> </td> 
      <td> 用户在Workfront Proof中拥有管理员权限，可以编辑帐户设置。 用户可以管理和查看在您组织的帐户中创建的所有验证。 这包括添加和删除审阅人、验证和注释。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>自定义</strong> </td> 
      <td> <p>仅当您在Workfront Proof中配置了自定义权限配置文件时可用。</p> <p><b>注释</b>：  <p>请确保您在此处授予的权限配置文件所提供的访问权限不会高于Workfront中用户的访问级别设置（请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>）。 如果它提供了更高的访问权限，则用户可以访问Workfront Proof中他或她无法在Workfront中访问的验证。</p> <p>如果您计划允许所有Workfront用户直接从Workfront访问Workfront Proof，这一点尤其重要，如<a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref">从Adobe Workfront访问Workfront Proof</a>中所述。</p> <p>默认情况下，只有Workfront管理员有权从Workfront全局导航栏访问指向Workfront Proof站点的直接链接。</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   您选择的权限配置文件将授予用户用于您组织内存在的每个证明。

1. 单击&#x200B;**保存更改**&#x200B;以完成用户设置的更新。

   >[!NOTE]
   >
   >当您在Workfront中创建或更新用户，并且该用户的Workfront电子邮件地址与许可的Workfront Proof用户的电子邮件地址匹配时，系统会在Workfront中为用户启用验证。 有关详细信息，请参阅[Adobe Workfront与Workfront Proof之间的用户同步](../../../administration-and-setup/manage-workfront/configure-proofing/user-sync-proofing.md)。

### 注意事项

设置权限时，请考虑以下信息：

* 如果将用户的权限配置文件更改为权限较少的配置文件，则该用户可能会失去对Workfront中现有验证的可见性。 当有人在Workfront中与用户共享任务，但未共享附加到任务的验证时，可能会发生这种情况(请参阅[在Adobe Workfront中共享验证](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)，在Adobe Workfront中共享验证[)。](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
* 仅当您的Workfront Proof环境与Workfront Premium帐户集成时，才能从Workfront Proof设置Workfront权限。 如果您无法使用本节中讨论的验证，请与Workfront管理员联系。
* Workfront环境中必须至少有一位用户具有验证的“管理员”权限。 如果您尝试从所有用户中删除校对的管理员权限，则会显示一条错误消息。
* 当您将用户的Workfront访问级别更改为系统管理员以外的任何级别时，用户的Workfront Proof权限配置文件默认为经理。

* 当您将Workfront访问级别更改为系统管理员时，验证权限配置文件更改为管理员。

## 通过Workfront主菜单为所有用户配置Workfront Proof访问权限 {#configure-workfront-proof-access-via-workfront-main-menu-for-all-users}

默认情况下，只有在Workfront中拥有管理权限的用户才能访问Workfront Proof，如[从Adobe Workfront访问Workfront Proof](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md)所述。

您可以通过联系Workfront Proof支持部门并提交请求，向所有用户授予对Workfront主菜单中Workfront按钮的访问权限。

>[!IMPORTANT]
>
> 如果您计划允许所有Workfront用户直接从Workfront全局导航栏访问Workfront Proof，请确保每个用户的权限配置文件不会提供比该用户在Workfront中的访问级别更多的访问权限。 这会阻止用户在Workfront Proof中访问他们无法在Workfront中访问的校样。 有关详细信息，请参阅[为用户启用和禁用校对（仅限旧版计划）](#enable-and-disable-proofing-for-a-user-legacy-plans-only)。

## 配置用户对桌面验证查看器的访问权限

如果贵组织中的用户希望使用桌面验证查看器而不是Web验证查看器来查看交互式内容，您可以将桌面验证查看器配置为在用户打开交互式内容验证时自动启动。 有关该桌面校对查看器的信息以及它与Web校对查看器的不同之处，请参阅[了解桌面校对查看器](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md)和[Web校对查看器和桌面校对查看器之间的区别](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md)。

1. 在Workfront中，单击全局导航栏中的Workfront Proof图标以访问Workfront Proof。

   ![](assets/proof-access-proofhq-350x39.png)

1. 单击Workfront Proof右上角附近的&#x200B;**帐户设置**，然后单击&#x200B;**设置**&#x200B;选项卡。

1. 在&#x200B;**验证默认值**&#x200B;下，在&#x200B;**交互式验证的桌面验证查看器**&#x200B;行的末尾，单击&#x200B;**设置**。

1. 按照[为组织配置校对设置](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md)一文中[桌面校对查看器](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#desktop-proofing-viewer)的说明，修改桌面校对查看器设置。

1. 单击&#x200B;**保存**。

## 为交互式验证配置自定义设备

您可以将任何自定义设备添加到系统中，从而使用户能够查看交互式内容，并在使用Desktop Proofing Viewer时模拟内容在特定设备上的显示方式。 （此功能在Web校对查看器中不可用，用户可以在其中查看交互式内容，但只能查看以各种分辨率显示的内容，不能查看各种设备上的内容。）

有关详细信息，请参阅[在验证查看器中更改交互式验证分辨率](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md)。

1. 从Workfront访问Workfront Proof界面，如[从Adobe Workfront访问Workfront Proof](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md)中所述。
1. 修改桌面验证查看器设置，如[为组织配置验证设置](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md)中的[为验证配置自定义设备](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#custom-devices-for-proofs)中所述。
