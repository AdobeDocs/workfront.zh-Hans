---
title: 在Adobe Workfront Planning中为申请表单添加批准
description: 您可以在Adobe Workfront Planning请求表单中添加批准流程，以在创建记录之前为每个提交的请求启动批准。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 453dbf1c7598858e99d963f7a3806355a8cc80a9
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 1%

---

# 在Adobe Workfront Planning中为申请表单添加批准

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

您可以在Adobe Workfront Planning请求表单中添加批准流程，以在创建记录之前为每个提交的请求启动批准。

本文介绍了工作区经理如何向与记录类型关联的请求表单添加批准。

有关在Workfront Planning中创建申请表单的信息，请参阅[在Adobe Workfront Planning中创建和管理申请表单](/help/quicksilver/planning/requests/create-request-form.md)。

有关向记录类型提交请求以创建记录的信息，请参阅[提交Adobe Workfront Planning请求以创建记录](/help/quicksilver/planning/requests/submit-requests.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront包</p></td> 
   <td> 
<p>任何Workfront包和任何Planning包</p>
或
<p>Any Workflow package and any Planning package</p>

<p>有关每个Workfront Planning包中所包含内容的更多信息，请联系您的Workfront客户代表。</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p>标准</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>   <p>管理对工作区的权限并记录类型</a> </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>  </td> 
  </tr>  
</tbody> 
</table>

有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 有关将审批添加到请求表单的注意事项

* 您可以向请求表单添加一个或多个批准者。 您可以将用户和团队添加为批准者。
* 对于通过提交请求表单而创建的记录，您可以在“批准者”和“批准日期”字段中显示批准信息。 有关信息，请参阅[创建字段](/help/quicksilver/planning/fields/create-fields.md)。
* 向请求表单添加多个批准者时，所有批准者都必须接受请求，然后才能在Workfront Planning中创建记录。
* 如果所有批准者都批准了该请求，则将为与请求表单关联的记录类型创建记录。
* 如果至少有一个批准者拒绝了请求，并且所有其他批准者都批准了该请求，则会在Workfront中为请求区域创建一个请求，但不会为与请求表单关联的记录类型创建记录。
* 向请求表单添加审批是可选的。 如果申请表单与批准无关，Workfront Planning会在提交申请后立即创建记录。

<!--

## Add an approval to a request form in the Production environment

1. Start creating a request form for a record type, as described in [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. Click **Configuration**.

    The **Configuration** area displays.

    ![Configuration tab](assets/configuration-tab.png)
1. In the **Approvers** field, start typing the name of a user or team that you want to set as an approver, then select it when it displays in the list. 
1. (Optional and conditional) If you have set more than one approver, and only need one approver to make a decision, enable the **Only one decision is required** option.

    (****most of the Note below is duplicated in the Create a request form article***)

      >[!NOTE]
      >
      >
      >* You can add one or several approvers to a request form.
      >
      >* If you add more than one approver, and the Only one decision is required option is not enabled, all approvers must approve the request before Workfront Planning creates a record.
      >
      >* If at least one approver rejects the request, the request is rejected and the record is not created. The request remains in the Requests area of Workfront.
      >
      >* If you add more than one approver, and the Only one decision is required option is not enabled, all approvers must make a decision before a request is either approved or rejected.
      >
      >* If a team is set as an approver, only one decision is required from the team.


1. (Optional) Click **Publish** if you have never shared the request form before.

    Or

    Click **Share** to share the form, then **Copy link**. 
1. (Optional) After a user uses the link you share and submits a request, Workfront Planning sends an approval in-app notification and an email to the approvers.

   For information about approving requests, see [Approve a request](/help/quicksilver/planning/requests/approve-request.md).

-->

## 将审批规则添加到请求表单

审批规则根据已提交请求中的字段值定义审批流程。

例如，如果请求表单具有“Campaign type”字段，则可以创建一个规则，在字段的值为“Digital”时将请求发送给一个人，在字段的值为“Print”时将请求发送给另一个人。

添加审批规则时，请考虑以下事项：

* 您可以将一个或多个批准者添加到批准规则。
* 如果至少有一位审批者拒绝了请求，则该请求会被拒绝，并且不会创建记录。 The request remains in the Requests area of Workfront.
* If you add more than one approver, and the Only one decision is required option is not enabled, all approvers must make a decision before a request is either approved or rejected.
* If a team is set as an approver, only one decision is required from one member of the team.

To set approval rules for a request form:

1. 开始为记录类型创建请求表单，如[在Adobe Workfront Planning中创建和管理请求表单](/help/quicksilver/planning/requests/create-request-form.md)一文中所述。
1. 打开请求表单时，单击&#x200B;**设置**。

   **设置**&#x200B;选项卡打开。

1. 要开始配置审批规则，请单击左侧面板中的&#x200B;**审批** ![审批图标](assets/approvals-icon-on-form.png)。

1. （可选）如果要设置默认审批流程，请至少向&#x200B;**默认审批规则**&#x200B;区域的&#x200B;**审批者**&#x200B;字段添加一个用户或团队，然后单击&#x200B;**仅需要一个决策**&#x200B;复选框（如果要在任何默认审批者批准记录后创建记录）。

   ![默认审批规则区域](assets/default-approvers.png)

1. （可选）开始添加审批规则。 对于每个自定义批准规则，请执行以下操作：

   1. 单击&#x200B;**添加批准规则**
   1. 单击占位符标题&#x200B;**无标题的批准规则**，然后输入批准规则的名称。
   1. 单击&#x200B;**选择字段**&#x200B;并选择激活规则的字段。
   1. 选择规则的运算符。 运算符因字段类型而异。
   1. If the selected operator requires a value, click the plus icon and add one or more values.
   1. (Optional) Click **Add condition** to add more conditions and connect them by **And** or **Or** statements by configuring the additional conditions as in steps C-E.
   1. In the **Actions** area of the approval rule, in the **Approvers** field, add at least one user or team to be set at the approver when the condition is met.
   1. (Conditional and optional) If you want the record to be created after any one of the approvers has approved it, check the **Only one decision is required** checkbox. Otherwise, all approvers must decide on the approval before the request is accepted or rejected.

   >[!NOTE]
   >
   >   添加审批规则时，请考虑以下事项：
   >
   >   * 如果仅设置了默认规则，则它会应用于提交的每个请求。
   >   * 如果满足自定义规则，则默认不会应用于请求审批工作流。 只有匹配的自定义规则才适用于审批，默认规则将被忽略。
   >   * 如果满足多个自定义规则，则应用顺序中的第一个规则。 在这种情况下，默认审批不适用（如果有）。

1. 单击&#x200B;**保存**&#x200B;以保存审批规则。
1. （可选）如果您以前从未共享过该请求表单，请单击&#x200B;**发布**。
