---
title: 授予访问Brand权限的权限
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
description: 作为Adobe Workfront管理员，您可以通过在Admin Console中创建用户组并分配GenStudio系统管理员产品配置文件来配置品牌权限。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 727efbd6-79b4-42c5-bfa2-e5350f30ff23
source-git-commit: 3e76f4a798a55a674a5ada2661c4b6bbb55195f2
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 4%

---

# 授予对品牌权限的访问权限

添加到用户组时，用户将获得Adobe GenStudio系统管理员的品牌创建、编辑和发布权限。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>“任一”</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>标准</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Admin Console权限</td> 
   <td> <p>您必须是Adobe Admin Console中的系统管理员。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 要求

* 您的Workfront实例必须启用统一批准。

* 您的组织必须具有GenStudio Foundation。
   * Workfront中的内容审阅者提供了GenStudio Foundation中用于资源审阅和批准工作流的功能。 您无需直接访问GenStudio Foundation即可完成工作。 您通过Content Reviewer访问GenStudio Foundation功能是受Workfront合同条款约束的。
* Adobe必须有一个已签署的Adobe Gen AI协议文件。
有关签署协议的更多信息，请参阅[签署Adobe Gen AI协议](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)。

## 1.在Admin Console中配置品牌权限

### 第1步：创建用户组

在Admin Console中创建新用户组以管理品牌创建和编辑的权限。

### 第2步：将产品配置文件分配给用户组

与已分配配置文件关联的权利为该组的所有用户提供GenStudio Brands权限（创建、更新和删除品牌）。

要分配配置文件，请执行以下操作：

1. 导航到新创建的用户组。
1. 单击&#x200B;**已分配的产品配置文件**&#x200B;选项卡。
1. 单击&#x200B;**分配配置文件**。
1. 在弹出窗口中，从产品列表中选择&#x200B;**Adobe GenStudio**，然后单击&#x200B;**应用**。
1. 选择&#x200B;**Adobe GenStudio Foundation编辑器**&#x200B;配置文件。
1. 单击&#x200B;**应用**。
1. 单击&#x200B;**保存**。

### 第3步：将用户添加到用户组

要为用户分配创建、编辑和发布品牌的权限，请将其添加到用户组。

>[!NOTE]
>
>在将组添加到项目之前，必须至少添加一个用户，如步骤4中所述。

要添加用户，请执行以下操作：

1. 转到&#x200B;**Admin Console** > **用户** > **用户组**。
1. 选择您的用户组。
1. 按用户名或电子邮件地址添加用户。
1. 从现有用户的建议匹配项中选择。

### 步骤4：创建品牌项目

项目提供了一个存储位置，用户可在其中保存品牌资产。

要创建项目，请执行以下操作：

1. 导航到Admin Console中的&#x200B;**存储**&#x200B;选项卡。
1. 单击&#x200B;**项目**。
1. 单击&#x200B;**创建项目**。
1. 在弹出窗口中，输入项目名称： **Adobe GenStudio Brands**。

   >[!IMPORTANT]
   >
   >完全按照所示输入项目名称。 请勿添加额外的空格或更改大小写。

1. 单击&#x200B;**创建**。

### 步骤5：邀请用户组加入项目

将用户组添加到Brands项目，以便他们能够访问和管理资产。

1. 在&#x200B;**邀请加入项目**&#x200B;弹出窗口中，添加您创建的用户组。
1. 选择&#x200B;**可以编辑**&#x200B;权限。
1. 单击&#x200B;**邀请**。

### 结果

该组中的用户现在有权在Workfront中创建、编辑和发布品牌资产。

## 2.授予对Workfront访问级别中“品牌”的访问权限

在授予个人用户访问Workfront访问级别中Brands的权限之前，您必须完成上一节中的所有步骤。

>[!IMPORTANT]
>
>* 只有分配给Admin Console中具有GenStudio系统管理器产品配置文件的用户组的用户才能在Workfront中创建、编辑和发布品牌，即使其他用户有权访问其访问级别设置中启用的品牌。
>* 在Admin Console中，添加到访问级别且启用了“品牌”访问权限但未添加到“用户组”的用户只能查看品牌。


要授予对Workfront访问级别中“品牌”的访问权限，请执行以下操作：

{{step-1-to-setup}}

1. 单击左侧面板中的&#x200B;**访问级别**。
1. 查找要编辑的访问级别，然后单击编辑图标![编辑图标](assets/edit-icon.png)对其进行编辑。

   或

   单击&#x200B;**新建访问级别**&#x200B;以创建新的访问级别。 有关创建访问级别的详细信息，请参阅[创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。
1. 向下滚动至&#x200B;**设置其他限制**，然后选择&#x200B;**允许用户访问品牌**。
   ![允许访问品牌设置](assets/access-for-brands.png)
1. 单击&#x200B;**保存**。

配置Brands后，您可以创建内容审阅者，以在审阅和批准工作流程中根据品牌指南审阅资产。 有关详细信息，请参阅[配置AI协作者](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md)。
