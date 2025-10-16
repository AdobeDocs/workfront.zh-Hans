---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 在Adobe Workfront中共享验证
description: 您可以通过共享文档或将用户添加到校样来在Adobe Workfront中共享校样文档。
author: Courtney
feature: Digital Content and Documents
exl-id: a5438db3-6507-4ebc-a27c-65f02c45783e
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '1157'
ht-degree: 0%

---

# 在Adobe Workfront中共享验证

您可以通过共享文档或将用户添加到校样来在Adobe Workfront中共享校样文档。

如果您按本文所述共享验证，则收件人将具有相同权限访问文档和验证。 此外，您还可以请求收件人审批证明。

>[!TIP]
>
>您还可以在验证查看器中共享验证。 有关说明，请参阅[从验证查看者共享验证](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md)。

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
   <p>标准</p>
   <p>工作或计划</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校样权限配置文件 </td> 
   <td>经理或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader">校样角色</td> 
   <td>作者或审查方</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对文档的访问权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 共享验证链接

共享验证链接可授予Workfront用户查看访问权限。 用户可以使用其Workfront登录凭据评论验证并订阅验证的电子邮件通知。 非验证用户可以使用电子邮件地址和显示名称进行评论和订阅。

>[!IMPORTANT]
>
>必须启用允许通过公共URL或嵌入代码共享验证设置。

1. 选择包含要与用户共享的验证的文档。

   您只能选择一个文档。 您无法同时共享多个文档的链接。

1. 单击&#x200B;**共享** > **校对链接**。
1. 在出现的&#x200B;**校对链接**&#x200B;框中，执行以下任一操作：

   * 要将链接复制到剪贴板，请单击&#x200B;**复制链接**。

     您现在可以通过第三方工具（如聊天或电子邮件应用程序）分发链接。

   * 要通过电子邮件直接从Adobe Workfront发送链接，请执行以下操作：

      1. 在&#x200B;**或指向**&#x200B;的电子邮件链接字段中，开始键入并选择收件人的姓名。 或者指定要与之共享的外部用户的电子邮件地址。

         >[!NOTE]
         >
         >如果在共享验证时看到别名电子邮件，则在存在相应的别名电子邮件时，不要通过输入原始电子邮件来创建新的访客用户。

      1. 从以下选项中选择：

         <table style="table-layout:auto">
          <col>
          <col>
          <tbody>
           <tr>
            <td role="rowheader">发送公共链接</td>
            <td><p>电子邮件通知中包含一个按钮，可将用户定向到他们正在使用的验证查看者中的验证，并授予查看权限。</p><p>如果<strong>通过公共URL或嵌入代码订阅验证</strong>对验证关闭，则用户可以使用其Workfront登录凭据登录以向验证添加评论。 如果启用，则提供其电子邮件地址和名称（无需密码）的任何人都可以签名并向验证中添加注释。</p></td>
           </tr>
           <tr>
            <td role="rowheader">发送下载链接</td>
            <td>电子邮件通知中包含一个按钮，可将用户定向到下载页面，其中提供文件详细信息、文件名和文件大小，并内联显示文件。 用户可以单击下载页面中的下载链接以下载文件。</td>
           </tr>
           <tr>
            <td role="rowheader">添加自定义消息</td>
            <td>允许您为电子邮件通知指定自定义主题和正文。</td>
           </tr>
          </tbody>
         </table>

      1. 单击&#x200B;**发送**。

         收件人会收到电子邮件通知，其中包含有关验证和您选择包含的按钮的信息。

         ![](assets/proof-share-email-350x87.png)

## 将用户添加到验证

如果您拥有验证的“编辑”权限，则可以向验证添加任何Workfront用户。 如果验证具有多个阶段，则将用户添加到单个阶段

>[!WARNING]
>
>除了本文中所列的方法之外，还可以在现有验证的更新选项卡的评论中通过标记用户来将用户添加到验证。 但是，以这种方式添加到验证的用户将不会收到电子邮件通知，除非在将他们添加到验证的工作流后再次对其进行标记。
>
>因此，我们建议通过以下列出的方法之一将用户添加到验证，而不是在评论中标记用户。
>

>[!NOTE]
>
>如果您使用的是旧版Workfront计划，其中可以为用户启用和禁用验证，请记住以下事项：
>
>* 收件人无需启用验证即可查看验证。
>* 如果启用了自动工作流，并且您向验证中添加了未在Workfront中启用验证的用户，则会在自动工作流中创建一个新阶段。 首次查看验证时，您添加的用户会自动添加到此新阶段。 （有关详细信息，请参阅[自动化工作流概述](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)。）
>

### 从文档选项卡将用户添加到现有验证

1. 选择包含要添加用户的验证的文档。
1. 如果验证没有自动工作流（阶段），请单击“阶段1”部分右上角的&#x200B;**更多**&#x200B;图标，然后在下拉菜单中单击&#x200B;**共享**。

   或

   如果验证确实具有自动工作流，请单击阶段右上角要添加审阅者的&#x200B;**更多**&#x200B;图标，然后在下拉菜单中单击&#x200B;**共享**。

1. 在显示的&#x200B;**共享此版本**&#x200B;框中（位于&#x200B;**共享**&#x200B;下），开始键入要与其共享校对的用户的名称或电子邮件地址，然后在该名称出现在下拉列表中时单击该名称。

1. （可选）重复此步骤以将多个用户添加到验证中。
1. （可选）设置审阅人的截止日期。
1. （可选）如果您希望让审阅人知道您已将他们添加到验证中，请确保选中&#x200B;**通过电子邮件通知联系人**。
1. （可选）**向电子邮件添加自定义消息**。
1. 添加所有审阅人后，单击&#x200B;**共享**。

### 将用户从验证查看者添加到现有验证

您可以在Web验证查看器和桌面验证查看器中查看验证时，将用户添加到验证。

有关详细信息，请参阅[从验证查看者共享验证](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users)一文中的[通过将用户添加到验证来共享验证](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md)

## 验证审批报表

您可以创建一个报告Workfront中已共享的验证审批的报告。 此报表在您的系统中提供以下验证审批信息：

* 已提交供审批的文档
* 审批者的姓名
* 校对版本
* 校样 ID
* 校对创建日期

在基于对象创建报告时，您可以访问此审批，如[创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)中所述。

有关验证审批对象报告的详细信息，请参阅[了解Adobe Workfront中的对象](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects)中的[对象报告](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)部分

## 批准共享验证

当用户将您添加到验证并使用自动工作流授予审批者角色或查看者和审批者角色时，审批请求显示在主页区域的“我的审批”小部件中。 然后，您可以直接从Workfront查看验证并做出批准决定。

有关如何通过“我的审批”构件做出审批决策的信息，请参阅[从主页区域审批工作](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-home-area)或[在](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-my-work-area)审批工作[中审批工作](../../../review-and-approve-work/manage-approvals/approving-work.md)。
