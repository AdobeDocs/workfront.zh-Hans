---
product-area: portfolios;projects
navigation-topic: create-and-manage-portfolios
title: 审核请求的项目
description: 在Adobe Workfront中，项目请求显示为状态为[!UICONTROL 已请求]的项目。 本文介绍了如何审查项目请求。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1acfb885-0da3-495d-ba66-e80e339e90de
source-git-commit: 7fef704355fad677f2bdf40e630ea0146a9e1d58
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# 审核请求的项目

<!--Audited: 10/2025-->

当有多个项目请求被提交审查时，项目管理办公室或项目组合委员会可以开会审查提交的请求，确定项目请求的批准。 项目请求在[!UICONTROL 中显示为状态为]已请求[!DNL Adobe Workfront]的项目。

您可以通过执行以下操作之一来提交项目请求以供审阅：

* 将项目状态更改为&#x200B;**[!UICONTROL 已请求]**。
* 完成项目的[!UICONTROL 业务案例]并提交以进行审批。\
   有关完成项目的业务案例的详细信息，请参阅[为项目创建业务案例](../../../manage-work/projects/define-a-business-case/create-business-case.md)。

您可以在[!DNL Adobe Workfront]的以下区域中查看请求的项目：

* 在项目报告中
* 在项目组合内

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 包</td> 
   <td><p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td> <p>[!UICONTROL 标准版] </p> 
   <p>[!UICONTROL 计划]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>对项目组合的[!UICONTROL 视图]或更高访问权限</p> <p>[!UICONTROL Edit]对项目的访问权限</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>项目组合上的[!UICONTROL View]权限或更高版本</p> <p>[!UICONTROL Manage]对项目的权限以更新其状态</p>  </td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td><p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL View] access or higher to Portfolios</p> <p>[!UICONTROL Edit] access to Projects</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL View] permissions or higher on the portfolio</p> <p>[!UICONTROL Manage] permissions on the projects to update their status</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## 在项目报告中查看请求的项目

您可以生成项目报告，以查看哪些项目的状态为[!UICONTROL 已请求]。

有关通过生成项目报告来批准项目请求的更多信息，请参阅[[!UICONTROL 批准业务案例]](../../../manage-work/projects/define-a-business-case/approve-business-case.md#build-a-report)中的[通过生成项目报告来批准业务案例](../../../manage-work/projects/define-a-business-case/approve-business-case.md)部分。

## 查看项目组合中请求的项目

1. 转到所请求要审阅项目的项目组合。
1. 单击左侧面板中的&#x200B;**[!UICONTROL 项目]**
1. 从&#x200B;**[!UICONTROL 筛选器]**&#x200B;下拉菜单中，选择&#x200B;**[!UICONTROL 请求的]**。

   列表中仅显示状态为&#x200B;**[!UICONTROL 已请求]**&#x200B;的项目。

   >[!TIP]
   >
   > 除了具有&#x200B;**[!UICONTROL 已请求]**&#x200B;的状态外，项目还必须与选定的Portfolio关联才能显示在此列表中。

1. 单击列表中的项目名称以将其打开。
1. 单击左侧面板中的&#x200B;**[!UICONTROL 项目详细信息]**。
1. 执行以下任一操作：

   * 单击&#x200B;**[!UICONTROL 业务案例]**，然后单击&#x200B;**[!UICONTROL 业务案例摘要]**&#x200B;区域中的&#x200B;**[!UICONTROL 批准]**&#x200B;或[!UICONTROL 拒绝]以批准或拒绝业务案例。

     ![approve_or_reject_business_case.png](assets/approve-or-reject-business-case-350x563.png)

     如果业务案例获得批准，项目状态将更改为&#x200B;**[!UICONTROL 已批准]**。

     如果业务案例被拒绝，项目状态将更改为&#x200B;**[!UICONTROL 已拒绝]**。

     >[!NOTE]
     >
     >没有通知可提醒提交业务案例批准的用户其项目请求是否被批准或拒绝。

     或

   * 在&#x200B;**[!UICONTROL 状态]**&#x200B;下拉菜单中，将项目的状态更改为任何其他状态。

     ![从下拉列表中更改项目状态](assets/project-status-change-from-drop-down-in-header-nwe-350x294.png)



