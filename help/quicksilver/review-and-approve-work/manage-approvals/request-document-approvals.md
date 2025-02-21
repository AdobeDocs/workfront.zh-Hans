---
product-area: documents
navigation-topic: approvals
title: 请求文件审批
description: 您可以在Adobe Workfront中请求经理或其他用户批准文档。 如果您的Workfront管理员启用了此功能，您还可以向没有Workfront帐户的人员请求文档审批，如配置系统安全首选项中所述。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f54a221b-4bf0-414e-b2f3-ace861d85496
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 1%

---

# 请求文件审批

您可以在Adobe Workfront中请求经理或其他用户批准文档。 如果您的Workfront管理员启用了此功能，您还可以向没有Workfront帐户的人员请求文档审批，如[配置系统安全首选项](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)中所述。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>审核或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看或更高权限的项目、任务、问题、模板、项目组合、程序、报告、功能板和日历、文档</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理与请求访问或审批关联的对象的访问权限 </p> <p>有关请求其他访问权限的信息，请参阅<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

+++

## 请求文档审批

1. 转到包含文档的项目、任务或问题，然后选择&#x200B;**文档**。
1. 查找所需的文档。

1. 向下滚动到“摘要”中的&#x200B;**审批**&#x200B;部分，然后开始在&#x200B;**添加审批者**&#x200B;文本框中键入。 您可以按姓名添加Workfront用户，或通过电子邮件添加外部用户。

1. 如果Adobe Workfront管理员启用了与不使用Workfront的用户进行协作的功能（如[配置系统安全首选项](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)中所述），则可以键入其电子邮件地址以包含这些用户。

   您不能请求团队或组的批准。

1. 重复上一步添加其他批准者。

## 在新版本上重新提交审批

上传新版本时，文档审批决策不会自动重置。 例如，如果文档被批准存在更改，则决策会将“更改”显示为决策，即使您上传具有指定更改的新版本也是如此。 如果您手动重新提交审批，则可以清除新版本上的决策。

1. 转到包含文档的项目、任务或问题，然后选择&#x200B;**文档**。
1. 查找所需的文档。

1. 向下滚动到“摘要”中的&#x200B;**Approvals**&#x200B;部分，单击“更多”图标，然后单击“重新提交”。

   ![重新提交审批](assets/nwe-resubmit-approval-350x149.png)

## 删除文档审批请求

1. 转到包含文档的项目、任务或问题，然后选择&#x200B;**文档**。
1. 查找所需的文档。

1. 向下滚动到“摘要”中的&#x200B;**审批**&#x200B;部分，然后单击内联审批者姓名的&#x200B;**更多**&#x200B;菜单并选择&#x200B;**删除**。

   审批请求将被删除，审批者会收到通知，告知不再需要其审批。 与审批相关的共享访问权限也会被删除。

## 向审批者发送提醒

您可以发送消息以提醒文档审批者您正在等待他们的反馈。

1. 转到包含文档的项目、任务或问题，然后选择&#x200B;**文档**。
1. 查找所需的文档。

1. 向下滚动到“摘要”中的&#x200B;**审批**&#x200B;部分，然后单击内联审批者姓名的&#x200B;**更多**&#x200B;菜单并选择&#x200B;**提醒**。

   审批者会收到通知，通知他们审批仍待处理。 如果已启用，他们也会收到电子邮件提醒。
