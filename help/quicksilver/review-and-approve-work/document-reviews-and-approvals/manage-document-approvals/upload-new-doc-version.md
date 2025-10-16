---
product-area: documents
navigation-topic: approvals
title: 上传新文档版本并请求审批
description: 您可以在Adobe Workfront中上传新文档版本并请求其他用户审批。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
source-git-commit: b615236d2666ebcc6db0d1f796fb0baaf362e0f2
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 0%

---

# 上传新文档版本并请求审批

如果标记为的文档需要在以前的审阅中工作，则可以将新版本上载到原始文档并开始另一轮审批。 上传文档的新版本后，先前版本将被锁定。

如果新版本的文件名与先前版本的文件名不同，则Workfront显示具有新文件名的文档。

当向具有未完成审批的文档中添加新版本时，先前版本的审批显示为“已撤回”。 先前的批准流程将关闭，即使一些参与者尚未做出决定。

如果删除了最新的文档版本，则以前的版本仍保持锁定状态。 如果需要编辑以前的版本，则必须手动解锁该版本。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p> 任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>请求或更高版本</p>
   <p>参与者或更高版本</p>
   <p>如果您使用的是Frame.io集成，则必须具有Standard许可证才能创建批准工作流。</p>
    </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对文档的访问权限</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">对象权限</td> 
   <td> <p>编辑对与文档关联的对象的访问权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 使用拖放操作添加新版本

>[!NOTE]
>
>Internet Explorer无法执行拖放操作。


如果您需要对文档进行另一轮审核和批准，则可以在Workfront中创建新文档版本。

可添加先前的参与者、新参与者或两者的组合。 您可以在“文档详细信息”页面上查看有关先前版本和参与者的信息。

要添加新版本：

1. 导航到Workfront中的文档。
1. 将新文件拖放到上一个文档上。 这会自动创建新版本。

1. 文档上传完成后，选择文档，然后单击&#x200B;**文档详细信息**。
   ![打开文档详细信息页面](assets/open-doc-details.png)


1. 在左侧面板中，单击&#x200B;**审批**，然后单击&#x200B;**添加**。

1. 若要添加所有以前的参与者，请单击&#x200B;**添加所有**。 您也可以根据需要添加新参与者或删除以前的参与者。


1. 要添加现有的审批模板，请单击“模板”按钮并开始键入模板名称。

   >[!TIP]
   >
   >   具有Standard许可证的用户可以从设置区域创建可重复使用的审批模板。 有关详细信息，请参阅[为资源和文档创建批准模板](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)。


1. （可选）设置审批的截止日期。 用户和团队将在指定截止日期前72小时（即24小时）通过电子邮件接收通知。

1. 添加所有审阅人和批准者后，单击&#x200B;**提交请求**。 将通过电子邮件通知参与者。

   ![提交新版本以供审批](assets/add-previous-participants.png)


