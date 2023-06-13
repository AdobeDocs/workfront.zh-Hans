---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 在Adobe Workfront中共享验证
description: 您可以通过共享文档或将用户添加到校样来在Adobe Workfront中共享校样文档。
author: Courtney
feature: Digital Content and Documents
exl-id: a5438db3-6507-4ebc-a27c-65f02c45783e
source-git-commit: 5c0cd18074cffdf0a4fe15affaf61add7314a83a
workflow-type: tm+mt
source-wordcount: '1221'
ht-degree: 0%

---

# 在Adobe Workfront中共享验证

您可以通过共享文档或将用户添加到校样来在Adobe Workfront中共享校样文档。

如果您共享验证（如本文所述），则收件人将具有相同权限访问文档和验证。 此外，您还可以请求收件人审批证明。

>[!TIP]
>
>您还可以在验证查看器中共享验证。 有关说明，请参阅 [从验证查看器共享验证](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>当前计划：Pro或更高版本</p> <p>或</p> <p>旧版计划：选择或Premium</p> <p>有关验证不同计划的访问权限的更多信息，请参阅 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的验证功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>当前计划：工作或计划</p> <p>旧版计划：任意（您必须为用户启用验证）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校对权限配置文件 </td> 
   <td>经理或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader">验证角色</td> 
   <td>作者或审查方</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、角色或验证权限配置文件，请联系您的Workfront或Workfront Proof管理员。

## 共享校对链接

共享验证链接可授予Workfront用户查看访问权限。 用户可以使用其Workfront登录凭据对验证进行评论并订阅验证的电子邮件通知。 非验证用户可以使用电子邮件地址和显示名称进行评论和订阅。

>[!IMPORTANT]
>
>必须启用“允许通过公共URL或嵌入代码共享验证”设置。

1. 选择包含要与用户共享的验证的文档。

   您只能选择一个文档。 您无法同时共享多个文档的链接。

1. 单击 **共享** > **校对链接**.
1. 在 **校对链接** 框中，执行以下任一操作：

   * 要将链接复制到剪贴板，请单击 **复制链接**.

     您现在可以通过第三方工具（如聊天或电子邮件应用程序）分发链接。

   * 要通过电子邮件直接从Adobe Workfront发送链接，请执行以下操作：

      1. 在 **或通过电子邮件将链接发送至** 字段中，开始键入并选择收件人的名称。 或指定要与之共享的外部用户的电子邮件地址。

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
            <td><p>电子邮件通知中包含一个按钮，可将用户定向到他们正在使用的验证查看者中的验证，并授予查看权限。</p><p>如果 <strong>通过公共URL或嵌入代码订阅验证</strong> 已针对验证关闭，用户可以使用其Workfront登录凭据登录以向验证添加评论。 如果启用，则提供其电子邮件地址和名称（无需密码）的任何人都可以签名并向验证中添加注释。</p></td>
           </tr>
           <tr>
            <td role="rowheader">发送下载链接</td>
            <td>电子邮件通知中包含一个按钮，可将用户定向到下载页面，其中提供文件详细信息、文件名和文件大小，并内联显示文件。 用户可以单击下载页面中的下载链接以下载该文件。</td>
           </tr>
           <tr>
            <td role="rowheader">添加自定义消息</td>
            <td>允许您为电子邮件通知指定自定义主题和正文。</td>
           </tr>
          </tbody>
         </table>

      1. 单击 **发送**.

         收件人将收到电子邮件通知，其中包含有关验证和您选择包含的按钮的信息。

         ![](assets/proof-share-email-350x87.png)

## 将用户添加到验证

如果您拥有验证的“编辑”权限，则可以向验证添加任何Workfront用户。 如果验证有多个阶段，则需将用户添加到单个阶段

>[!WARNING]
>
>除了本文中所列的方法外，还可通过在现有验证的更新选项卡的评论中标记用户来将用户添加到验证中。 但是，以这种方式添加到验证的用户将不会收到电子邮件通知，除非他们在添加到验证的工作流后再次被标记。
>
>因此，我们建议通过以下列出的方法之一将用户添加到验证，而不是在评论中标记他们。
>

>[!NOTE]
>
>如果您使用的是旧版Workfront计划，其中可以为用户启用和禁用验证，请记住以下事项：
>
>* 您的收件人无需启用验证即可查看验证。
>* 启用自动工作流后，如果您将用户添加到验证中，而此验证未在Workfront中启用，则会在自动工作流中创建一个新阶段。 首次查看验证时，您添加的用户会自动添加到此新阶段。 (有关更多信息，请参阅 [自动化工作流概述](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).)
>

### 从文档选项卡将用户添加到现有验证

1. 选择包含要添加用户的验证的文档。
1. 如果验证没有自动工作流（暂存），请单击 **更多** 图标，然后单击 **共享** （在下拉菜单中）。

   或

   如果验证确实具有自动化工作流，请单击 **更多** 图标（位于要添加审阅人的舞台的右上角），然后单击 **共享** （在下拉菜单中）。

1. 在 **共享此版本** 框，位于下 **共享**，开始键入要与其共享验证的用户姓名或电子邮件地址，然后在验证出现在下拉列表中时单击该名称。

1. （可选）重复此步骤以将多个用户添加到验证中。
1. （可选）设置审阅人的截止日期。
1. （可选）确保 **通过电子邮件通知联系人** 如果要让审阅人知道您已将其添加到校样中，请选择。
1. （可选） **添加自定义消息** 至电子邮件。
1. 添加所有审阅人后，单击 **共享**.

### 从验证查看者将用户添加到现有验证

在Web验证查看器和桌面验证查看器中查看验证时，您可以将用户添加到验证中。

有关更多信息，请参阅 [通过添加用户来共享验证](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users) 在文章中 [从验证查看器共享验证](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md)

## 验证审批报告

您可以创建一个报告Workfront中已共享的验证审批的报告。 此报表在您的系统中提供以下验证审批信息：

* 已提交供审批的文档
* 审批者的姓名
* 校对版本
* 校对 ID
* 校对创建日期

在基于对象创建报告时，您可以访问此审批，如中所述 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

有关验证审批对象报告的详细信息，请参阅 [对象报告](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) 中的部分 [了解Adobe Workfront中的对象](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)

## 批准共享验证

当用户将您添加到验证并使用“自动工作流”授予“审批者”角色或“查看者和审批者”角色时，审批请求将显示在“主页”或“我的工作”区域的审批选项卡上。 然后，您可以直接从Workfront查看验证并做出批准决定。

有关如何从“我的工作”区域作出批准决策的信息，请参阅 [批准主页区域中的工作](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-home-area) 或 [审批工作](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-my-work-area) 在 [审批工作](../../../review-and-approve-work/manage-approvals/approving-work.md).
