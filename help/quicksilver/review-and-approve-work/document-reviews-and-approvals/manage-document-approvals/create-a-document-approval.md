---
product-area: documents
navigation-topic: approvals
title: 创建文档审阅或审批请求
description: 您可以在Adobe Workfront中请求其他用户批准文档。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: a02699e1-3557-47f0-89b7-dbecb507a174
source-git-commit: b615236d2666ebcc6db0d1f796fb0baaf362e0f2
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---

# 创建文档审阅或审批请求

您可以在Adobe Workfront中请求其他用户或团队批准文档，或请求他们审核文档而无需批准。

>[!IMPORTANT]
>
>本文内容介绍更新的文档审批功能，该功能仅适用于特定帐户。 有关标准审批流程的信息，请参阅[工作审批](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md)中列出的文章。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
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
   <td> <p>管理与请求访问或审批关联的对象的访问权限 </p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 从文档页面创建文档审阅或审批请求

1. 将鼠标悬停在文档上，然后单击“文档详细信息”。
   ![文档详细信息](assets/doc-details.png)

1. 在文档名称附近，在版本下拉菜单中选择要创建批准的文档版本。 默认情况下将选择最新版本。

1. 在左窗格中单击&#x200B;**审批**。

1. （可选）设置审批的截止日期。 用户和团队将在指定截止日期前72小时（即24小时）通过电子邮件接收通知。

1. 要添加审批者，请单击&#x200B;**审批者**&#x200B;并开始键入用户或团队名称。

1. 要添加审阅者，请单击&#x200B;**审阅者**&#x200B;复选框，然后开始键入用户或团队名称。

   ![添加审批者和截止日期](assets/add-approver-and-deadline.png)

1. 重复上一步骤以添加其他批准者或审阅者。

## 从文档摘要面板创建文档审阅或审批请求

1. 转到包含文档的项目、任务或问题，然后选择&#x200B;**文档**。

1. 单击所需的文档，该文档的“文档摘要”窗格将打开。

1. 在版本下拉列表中选择要创建批准的文档版本。 默认情况下将选择最新版本。

1. 向下滚动到“文档摘要”窗格中的&#x200B;**审批**&#x200B;部分，然后单击&#x200B;**添加**。

![在文档摘要中添加批准者](assets/doc-summary-add-approvers.png)

1. （可选）设置审批的截止日期。 用户和团队将在指定截止日期前72小时（即24小时）通过电子邮件接收通知。

1. 要添加审批者，请单击&#x200B;**审批者**&#x200B;并开始键入用户或团队名称。

1. 要添加审阅者，请单击&#x200B;**审阅者**&#x200B;复选框，然后开始键入用户或团队名称。

   ![添加审批者和截止日期](assets/add-approver-and-deadline.png)

1. 重复上一步骤以添加其他批准者或审阅者。





<!--
## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![Resubmit approval](assets/nwe-resubmit-approval-350x149.png)
-->
