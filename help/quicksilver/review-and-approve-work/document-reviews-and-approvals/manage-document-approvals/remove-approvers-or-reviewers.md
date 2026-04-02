---
product-area: documents
navigation-topic: approvals
title: 从文档审批工作流中删除审批人或审阅人
description: 您可以从文档中删除单个批准者或审阅者。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6877ee90-9a70-4616-98f4-4b0ff932d79a
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 2%

---

# 从文档审批工作流中删除审批人或审阅人

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览Sandbox”环境中可用。</span>

分配资产或文档后，您可以从资产或文档中删除单个批准者或审阅者。

>[!IMPORTANT]
>
>本文内容介绍更新的文档审批功能，该功能仅适用于特定帐户。 有关标准审批流程的信息，请参阅[工作审批](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md)中列出的文章。

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
   <td> 
   <p>参与者或更高版本</p>
   <p>审核或更高</p>
   <p>如果您使用的是Frame.io集成，则必须具有Standard许可证才能创建批准工作流。</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>查看或更高权限的项目、任务、问题、模板、项目组合、程序、报告、功能板和日历、文档</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理与请求访问或审批关联的对象的访问权限 </p>  </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


## 从生产环境中的“文档详细信息”页面中删除审批者或审阅者

1. 通过单击文档名称转到文档页面，然后在版本下拉菜单中选择要移除审批的文档版本。 默认情况下会选择最新版本。

1. 在左侧面板中选择&#x200B;**审批**。

1. 将鼠标悬停在要删除的批准者或审阅者的名称上，然后单击其名称后面显示的&#x200B;**删除**&#x200B;图标![删除图标](../assets/delete.png)。

   审批或审阅请求将被删除，审批者会收到通知，告知不再需要其审批。 与审批相关的共享访问权限也会被删除。

1. （可选）要将审批者降级为审核者而不是完全删除他们，请取消选中与其名称一致的&#x200B;**审批者**&#x200B;复选框。

1. 重复上一步骤以移除任何其他批准者或审阅者。

## 从生产环境中的“文档摘要”中删除批准者或审阅者

1. 转到包含文档的项目、任务或问题，然后选择&#x200B;**文档**。

1. 单击所需的文档，该文档的“文档摘要”面板将打开。

1. 在版本下拉菜单中选择您要为其删除审批者或审阅者的文档版本。 默认情况下会选择最新版本。

1. 向下滚动到“文档摘要”面板中的&#x200B;**审批**&#x200B;部分。 将鼠标悬停在要删除的批准者或审阅者的名称上，然后单击其名称后面显示的&#x200B;**删除**&#x200B;图标![删除图标](../assets/delete.png)。

   审批或审阅请求将被删除，审批者会收到通知，告知不再需要其审批。 与审批相关的共享访问权限也会被删除。

1. （可选）要将审批者降级为审核者而不是完全删除他们，请取消选中与其名称一致的&#x200B;**审批者**&#x200B;复选框。

1. 重复上一步骤以移除任何其他批准者或审阅者。


<div class="preview">

## 在旧文档区域的预览环境中，从审批工作流中删除审批人或审阅人

如果您的组织位于Workfront存储中，则当您访问Workfront中的文档时，将会看到旧版文档区域。 有关Workfront存储的详细信息，请参阅[Workfront存储与Adobe企业存储](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage)。

要从批准工作流中删除批准者或审阅者，请执行以下操作：

1. 转到包含文档的项目、任务或问题，然后在左侧面板中选择&#x200B;**文档**。

1. 单击所需的文档，该文档的“文档摘要”面板将打开。

1. 向下滚动到“文档摘要”面板中的&#x200B;**审批**&#x200B;部分。

1. 单击&#x200B;**编辑工作流**。

1. 找到要删除的参与者，然后单击其名称旁边的&#x200B;**删除**&#x200B;图标。

   审批或审阅请求将被删除，审批者会收到通知，告知不再需要其审批。 与审批相关的共享访问权限也会被删除。

   ![编辑审批工作流](assets/edit-approval-in-legacy.png)

1. （可选）要将审批者的角色更改为审阅者（反之亦然），请单击用户名旁边的下拉菜单，然后选择新角色。

1. 重复上一步骤以移除任何其他批准者或审阅者。

</div>


## 将审批人或审阅人移至“新建文档”区域中的审批工作流

如果您的组织使用企业存储，则当您访问Workfront中的文档时，将会看到“新建文档”区域。 有关企业存储的详细信息，请参阅[企业存储概述](/help/quicksilver/review-and-approve-work/esm-overview.md)。

要创建审批工作流，请执行以下操作：

1. 转到包含文档的项目、任务或问题，然后在左侧面板中选择&#x200B;**文档**。

1. 单击文档，然后单击页面右侧的&#x200B;**审批**&#x200B;图标。

   ![在文档摘要中添加批准者](assets/approvals-icon-new.png)


1. 单击&#x200B;**编辑工作流**。

1. 找到要删除的参与者，然后单击其名称旁边的&#x200B;**删除**&#x200B;图标。

   审批或审阅请求将被删除，审批者会收到通知，告知不再需要其审批。

1. （可选）要将审批者的角色更改为审阅者（反之亦然），请单击用户名旁边的下拉菜单，然后选择新角色。

1. 重复上一步骤以移除任何其他批准者或审阅者。

   ![从阶段中删除参与者](assets/add-or-remove-participants.png)
1. 单击&#x200B;**保存**。