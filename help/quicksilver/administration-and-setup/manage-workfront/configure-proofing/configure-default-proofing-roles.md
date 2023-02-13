---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: 配置默认校对角色
description: 作为Adobe Workfront管理员，您可以为访问在Workfront中创建校样的用户和来宾用户配置默认校样角色。 将用户添加到校样的任何人员都可以为他们调整这些角色。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: d64213bf-f270-404f-a45a-6f94c7b7cb91
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 1%

---

# 配置默认校对角色

作为Adobe Workfront管理员，您可以为访问在Workfront中创建校样的用户和来宾用户配置默认校样角色。 将用户添加到校样的任何人员都可以为他们调整这些角色。

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
   <td> <p>您必须是Workfront管理员。 有关Workfront管理员的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 配置默认校对角色

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

   <!--
   <li In the left panel, click Proofs Proof roles.
   -->

1. 单击 **审核和批准** 在左侧列表底部附近。
1. 在 **文档校样的指定收件人的角色** 部分，为添加到校样工作流的用户和来宾用户选择默认角色。

   请参阅 [与校对角色关联的权限](#rights-associated-with-proofing-roles) 下方提供了每个校对角色及其关联权限的列表。

   >[!NOTE]
   >
   >* 此设置仅适用于在设置角色后在Workfront系统中创建的用户；不会发送给现有用户。
   >* 将用户添加到校样的人员可以调整此角色，如 [将用户添加到校样](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) in [在Adobe Workfront中共享验证](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).


1. 在 **打开文档校样的非收件人的角色** 部分，为可访问校样但未添加到校样工作流的用户和来宾用户选择默认角色。

   当用户和来宾有权访问已为其创建校样的文档时，会出现这种情况：即使尚未将它们添加到校样的工作流，它们也可以打开校样。

   **示例：** 以下是如何使用此设置的示例：

   * 您选择 **只读** 以限制所有验证活动，例如，向被请求进行该活动的用户添加评论并做出决策。
   * 您选择 **审阅人** 因为您希望团队的任何成员都能够在校样中添加标记和注释。

1. 单击&#x200B;**保存**。

## 与校对角色关联的权限 {#rights-associated-with-proofing-roles}

下表显示了每个角色以及与其关联的权限：

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>查看校样</strong> </p> </th> 
   <th> <p><strong>添加标记</strong> </p> </th> 
   <th> <p><strong>添加注释</strong> </p> </th> 
   <th> <p><strong>如果没有回复，则编辑自己的评论</strong> </p> </th> 
   <th> <p><strong>做出决定</strong> </p> </th> 
   <th> <p><strong>删除他人的评论</strong> </p> </th> 
   <th>解决注释</th> 
   <th>将操作应用到注释</th> 
   <th> <p><strong>编辑校样</strong> </p> </th> 
   <th>与他人共享证据</th> 
   <th>创建新版本</th> 
   <th> <p><strong>在“主页”区域中查看批准请求</strong> </p> </th> 
   <th>添加新审阅人</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>只读</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>查看者</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>审批者</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>审核人和批准者</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>作者</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p><strong>审阅人</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p><strong>✓</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> <p> </p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>新Workfront计划的用户可以向系统中的任何用户授予作者或审核者角色。 旧版计划中的用户可以向系统中具有校样许可证的任何用户授予作者或审核者角色。
