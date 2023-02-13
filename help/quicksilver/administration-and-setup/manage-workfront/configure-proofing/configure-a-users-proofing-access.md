---
user-type: administrator
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
title: 配置用户的校对访问权限
description: 作为Adobe Workfront管理员或Workfront校样管理员，您可以配置用户的访问权限，以在Workfront和Workfront校样中创建和查看校样。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 98c90139-f31a-41bc-af0b-577dd8b254e3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1244'
ht-degree: 0%

---

# 配置用户的校对访问权限

作为Adobe Workfront管理员或Workfront校样管理员，您可以配置用户的访问权限，以在Workfront和Workfront校样中创建和查看校样。

有关基本校样和集成校样可用的校样功能的信息，请参阅 [访问Workfront中的校对功能](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>您必须是Workfront管理员或Workfront校样管理员。 有关Workfront管理员的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 为用户启用和禁用校对功能（仅限旧版计划） {#enable-and-disable-proofing-for-a-user-legacy-plans-only}

如果贵组织使用旧版Select或Premium Workfront计划，则作为Workfront管理员，您可以启用和禁用用户的校对功能。

在为用户启用校样时，Workfront会启用用于自动生成用户校样的选项。

虽然您可以将某个用户启用为校样用户，但是该用户必须具有管理员权限，才能从Workfront主菜单直接导航到Workfront校样界面。 有关如何为Workfront系统中的所有校样用户启用此选项的信息，请参阅 [通过Workfront主菜单为所有用户配置Workfront校样访问权限](#configure-workfront-proof-access-via-workfront-main-menu-for-all-users).

1. 在 **主菜单**，选择 **用户**.

1. 选择一个用户，然后单击 **编辑** 图标。
1. 在 **访问** 部分，选择或取消选择 **用户可以生成校样**.

## 配置用户的校样权限配置文件

您选择的权限配置文件将授予用户，以供您组织内存在的每种校样使用。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **用户** ![](assets/users-icon-in-main-menu.png).
1. 选择一个或多个用户，然后单击 **编辑**.

1. 在 **访问** 部分中，在 **校样权限配置文件** 下拉菜单：

   >[!NOTE]
   >
   >如果您使用的是旧版Workfront计划，请确保 **用户可以生成校样** 选项，如上文 [为用户启用和禁用校对功能（仅限旧版计划）](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>监督人</strong> </td> 
      <td>用户可以管理和查看在您组织的帐户中创建的所有校样。 他们还可以编辑添加到这些校样的审阅人。 具有此权限配置文件的用户无法管理用户或编辑Workfront校样设置。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>经理</strong> </td> 
      <td> <p> 用户可以管理和查看在您组织的帐户中创建或拥有的校样。 只有作为审阅人添加时，他们才能查看其他用户的校样。 这是默认设置。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>管理员</strong> </td> 
      <td> 在Workfront校样中，为用户授予了管理员权限，并且可以编辑帐户设置。 用户可以管理和查看在您组织的帐户中创建的所有校样。 这包括添加和删除审阅人、校样和注释。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>自定义</strong> </td> 
      <td> <p>仅当您在Workfront校样中配置了自定义权限配置文件时才可用。</p> <p><b>注释</b>:  <p>确保您在此处授予的权限配置文件提供的访问权限不会高于Workfront中用户的访问级别设置(请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>)。 如果提供了更高的访问权限，则用户可以在Workfront Proof中访问验证，以确认他/她无法在Workfront中访问。</p> <p>如果您计划允许所有Workfront用户直接从Workfront访问Workfront校样，则这一点尤为重要，如 <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref">从Adobe Workfront访问Workfront校样</a>.</p> <p>默认情况下，只有Workfront管理员才能从Workfront全局导航栏访问指向Workfront校样网站的直接链接。</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   您选择的权限配置文件将授予用户，以供您组织内存在的每种校样使用。

1. 单击 **保存更改** 完成对用户设置的更新。

   >[!NOTE]
   >
   >在Workfront中创建或更新用户，且用户的Workfront电子邮件地址与授权的Workfront Proof用户的电子邮件地址相匹配时，系统会为Workfront中的用户启用校样。 有关更多信息，请参阅 [Adobe Workfront与Workfront校样之间的用户同步](../../../administration-and-setup/manage-workfront/configure-proofing/user-sync-proofing.md).

### 注意事项

设置权限时请考虑以下信息：

* 如果将用户的权限配置文件更改为权限较少的配置文件，则用户可能会无法看到Workfront中的现有校样。 当某人与Workfront中的用户共享任务，但不共享附加到该任务的校样时，可能会发生这种情况(请参阅 [在Adobe Workfront中共享验证](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [在Adobe Workfront中共享验证](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md))。
* 仅当您的Workfront环境与Workfront Proof Premium帐户集成时，才能从Workfront设置Workfront校样权限。 如果无法按此部分所述使用校对，请联系您的Workfront管理员。
* 您的Workfront环境中至少有一个用户必须具有管理员权限才能进行校样。 如果尝试从所有用户中删除校对的管理员权限，则会显示一条错误消息。
* 当您将用户的Workfront访问级别更改为除系统管理员之外的任何级别时，用户的Workfront校样权限配置文件将默认为Manager。

* 将“Workfront访问”级别更改为“系统管理员”时，“校样权限”配置文件将更改为“管理员”。

## 通过Workfront主菜单为所有用户配置Workfront校样访问权限 {#configure-workfront-proof-access-via-workfront-main-menu-for-all-users}

默认情况下，只有在Workfront中具有管理权限的用户才能访问Workfront校样，如所述  [从Adobe Workfront访问Workfront校样](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

您可以联系Workfront支持团队并提交请求，以授予所有用户访问Workfront主菜单中“Workfront校样”按钮的权限。

>[!IMPORTANT]
>
> 如果您计划允许所有Workfront用户直接从Workfront全局导航栏访问Workfront校样，请确保每个用户的权限配置文件提供的访问权限不会多于Workfront中用户的访问级别。 这会阻止用户在Workfront校样中访问无法在Workfront中访问的校样。 有关更多信息，请参阅 [为用户启用和禁用校对功能（仅限旧版计划）](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

## 配置用户对桌面校对查看器的访问权限

如果贵组织中的用户希望使用桌面校样查看器而不是Web校样查看器来查看交互式内容，则可以将桌面校样查看器配置为在用户打开交互式内容校样时自动启动。 有关桌面校对查看器以及它与Web校对查看器有何不同的信息，请参阅 [了解桌面校对查看器](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md) 和 [Web校对查看器与桌面校对查看器概述之间的差异](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

1. 在Workfront中，单击全局导航栏中的Workfront校样图标以访问Workfront校样。

   ![](assets/proof-access-proofhq-350x39.png)

1. 单击 **帐户设置** 在Workfront校样的右上角附近，单击 **设置** 选项卡。

1. 在 **校样默认值**，在 **用于交互式校样的桌面校样查看器** 行，单击 **设置**.

1. 按照 [桌面校对查看器](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#desktop-proofing-viewer) 在文章中 [为贵组织配置校样设置](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).

1. 单击&#x200B;**保存**。

## 配置用于交互校样的自定义设备

您可以向系统中添加任何自定义设备，从而允许用户查看交互式内容，并模拟内容在使用桌面校样查看器时在特定设备上的显示方式。 （在Web校样查看器中，此功能不可用，用户可以在查看交互式内容时查看交互式内容，但仅当它以各种分辨率显示时才可用，而不能在各种设备上显示。）

有关更多信息，请参阅 [在校样查看器中更改交互式校样分辨率](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

1. 从Workfront访问Workfront校样界面，如 [从Adobe Workfront访问Workfront校样](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).
1. 按照 [配置自定义设备以进行校样](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#custom-devices-for-proofs) 在文章中 [为贵组织配置校样设置](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).
