---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: 配置默认验证角色
description: 作为Adobe Workfront管理员，您可以为访问在Workfront中创建的验证的用户和来宾用户配置默认验证角色。 将用户添加到验证的任何人都可以为其调整这些角色。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: d64213bf-f270-404f-a45a-6f94c7b7cb91
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 1%

---

# 配置默认验证角色

作为Adobe Workfront管理员，您可以为访问在Workfront中创建的验证的用户和来宾用户配置默认验证角色。 将用户添加到验证的任何人都可以为其调整这些角色。

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
   <td> <p>您必须是Workfront管理员。 有关Workfront管理员的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 配置默认验证角色

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)，然后单击&#x200B;**设置** ![](assets/gear-icon-settings.png)。

   <!--
   <li In the left panel, click Proofs Proof roles.
   -->

1. 在左侧显示的列表底部附近单击&#x200B;**审核和批准**。
1. 在文档验证&#x200B;**的指定收件人的**&#x200B;角色部分中，为添加到验证工作流中的用户和访客用户选择默认角色。

   有关每个验证角色及其关联权限的列表，请参阅下面的[与验证角色关联的权限](#rights-associated-with-proofing-roles)。

   >[!NOTE]
   >
   >* 此设置仅适用于设置角色后在Workfront系统中创建的用户，而不适用于现有用户。
   >* 将用户添加到验证的用户可以调整此角色，如[在Adobe Workfront中共享验证](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)中的[将用户添加到验证](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add)中所述。

1. 在打开文档校对&#x200B;**的非收件人角色分区的**&#x200B;角色中，为可以访问校对但未添加到校对工作流中的用户和访客用户选择默认角色。

   当用户和访客有权访问已为其创建验证的文档时会发生此情况：即使他们尚未添加到验证的工作流，也可以打开验证。

   **示例：**&#x200B;以下是有关如何使用此设置的示例：

   * 您选择&#x200B;**只读**&#x200B;以限制所有校对活动，例如向被要求进行该活动的用户添加评论和做出决策。
   * 您选择&#x200B;**查看者**，因为您希望团队的任何成员都能够在校对上添加标记和评论。

1. 单击&#x200B;**保存**。

## 与验证角色关联的权限 {#rights-associated-with-proofing-roles}

下表显示了每个角色及其关联的权限：

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
   <th> <p><strong>查看校对</strong> </p> </th> 
   <th> <p><strong>添加标记</strong> </p> </th> 
   <th> <p><strong>添加评论</strong> </p> </th> 
   <th> <p><strong>如果没有回复，则编辑自己的评论</strong> </p> </th> 
   <th> <p><strong>做出决定</strong> </p> </th> 
   <th> <p><strong>删除其他人的评论</strong> </p> </th> 
   <th>解决评论</th> 
   <th>将操作应用到注释</th> 
   <th> <p><strong>编辑校对</strong> </p> </th> 
   <th>与他人共享证明</th> 
   <th>创建新版本</th> 
   <th> <p><strong>在主页区域查看审批请求</strong> </p> </th> 
   <th>添加新审阅者</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>只读</strong> </p> </td> 
   <td> <p>✓ {\f13 }</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
   <td> <p> </p> </td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>查看者</strong> </p> </td> 
   <td> <p>✓ {\f13 }</p> </td> 
   <td> <p>✓ {\f13 }</p> </td> 
   <td> <p>✓ {\f13 }</p> </td> 
   <td> <p>✓ {\f13 }</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
   <td> <p> </p> </td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>审批者</strong> </p> </td> 
   <td> <p>✓ {\f13 }</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓ {\f13 }</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
   <td> <p> </p> </td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> <p>✓ {\f13 }</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>审阅者和批准者</strong> </p> </td> 
   <td> <p>✓ {\f13 }</p> </td> 
   <td> <p>✓ {\f13 }</p> </td> 
   <td> <p>✓ {\f13 }</p> </td> 
   <td> <p>✓ {\f13 }</p> </td> 
   <td> <p>✓ {\f13 }</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
   <td> <p> </p> </td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> <p>✓ {\f13 }</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>作者</strong> </p> </td> 
   <td> <p>✓ {\f13 }</p> </td> 
   <td> <p>✓ {\f13 }</p> </td> 
   <td> <p>✓ {\f13 }</p> </td> 
   <td> <p>✓ {\f13 }</p> </td> 
   <td> <p>✓ {\f13 }</p> </td> 
   <td> <p> </p> </td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> <p>✓ {\f13 }</p> </td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td> <p><strong>审阅人</strong> </p> </td> 
   <td> <p>✓ {\f13 }</p> </td> 
   <td> <p>✓ {\f13 }</p> </td> 
   <td> <p>✓ <strong></strong> </p> </td> 
   <td> <p>✓ {\f13 }</p> </td> 
   <td> <p>✓ {\f13 }</p> </td> 
   <td> <p>✓ {\f13 }</p> <p> </p> </td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> <p>✓ {\f13 }</p> </td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>新Workfront计划上的用户可以向系统中的任何用户授予创作或审查方角色。 旧版计划用户可以将作者或审查方角色授予系统中拥有验证许可证的任何用户。
