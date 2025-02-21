---
product-area: documents
navigation-topic: approvals
title: 上传新文档版本并请求审批
description: 您可以在Adobe Workfront中上传新文档版本并请求其他用户审批。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
source-git-commit: 8270a107ba2501eddbb27f52c843c337aa1f8a99
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 0%

---

# 上传新文档版本并请求审批

如果标记为的文档需要在以前的审阅中工作，则可以将新版本上载到原始文档并开始另一轮审批。 上传文档的新版本后，先前版本将被锁定。

如果新版本的文件名与先前版本的文件名不同，则Workfront显示具有新文件名的文档。

当向具有未完成审批的文档中添加新版本时，先前版本的审批显示为“已撤回”。 先前的批准流程将关闭，即使一些参与者尚未做出决定。

如果删除了最新的文档版本，则以前的版本仍保持锁定状态。 如果需要编辑以前的版本，则必须手动解锁该版本。


## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p> 任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>当前：请求或更高版本</p>
   或
   <p>新文档：参与者或更高版本</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">对象权限</td> 
   <td> <p>编辑对与文档关联的对象的访问权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/grant-and-request-access-to-objects.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

+++

## 使用拖放操作添加新版本

>[!NOTE]
>
>Internet Explorer无法执行拖放操作。

1. 转到文档上传所在的文档区域。
1. 从桌面或单独的浏览器选项卡中，将文档的新版本拖动到Workfront中现有版本的上方。

   拖动新版本时，您可以将鼠标悬停在Workfront文档文件夹上以将其打开。 然后，可以通过将文件拖动到屏幕的顶部或底部来上下滚动。

1. 将新版本拖放到&#x200B;**文档**&#x200B;选项卡上的现有文件上。

1. 上传文档后，单击该文档并打开文档摘要面板。

1. 向下滚动到“文档摘要”窗格中的&#x200B;**审批**&#x200B;部分，然后单击&#x200B;**添加**。

![在文档摘要中添加批准者](assets/doc-summary-add-approvers.png)

1. （可选）设置审批的截止日期。 用户和团队将在指定截止日期前72小时（即24小时）通过电子邮件接收通知。

1. 要从以前的版本快速添加审阅人和批准者，请单击下面列出的审阅人和批准者名称旁边的添加按钮。
   <!--need screenshot when working-->

1. （可选）从审批者/审阅者更改角色。

1. 要添加新的批准者和审阅者，请单击&#x200B;**审阅者**&#x200B;或&#x200B;**批准者**，然后开始键入用户或团队。

   ![添加审批者和截止日期](assets/add-approver-and-deadline.png)
