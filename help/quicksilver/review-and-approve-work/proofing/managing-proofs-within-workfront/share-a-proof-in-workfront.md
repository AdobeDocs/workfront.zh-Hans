---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 在Adobe Workfront中共享验证
description: 您可以在Adobe Workfront内通过共享文档或将用户添加到校样来共享已验证文档。
author: Courtney
feature: Digital Content and Documents
exl-id: a5438db3-6507-4ebc-a27c-65f02c45783e
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1137'
ht-degree: 0%

---

# 在Adobe Workfront中共享验证

您可以在Adobe Workfront内通过共享文档或将用户添加到校样来共享已验证文档。

如果您共享校样（如本文所述），则收件人对文档和校样具有相同的访问权限。 此外，您还可以向收件人请求校样的批准。

>[!TIP]
>
>您还可以从校样查看器中共享校样。 有关说明，请参阅 [从校对查看器共享校样](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>当前计划：Pro或更高版本</p> <p>或</p> <p>旧版计划：选择或Premium</p> <p>有关使用不同计划校对访问权限的更多信息，请参阅 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的校对功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>当前计划：工作或计划</p> <p>旧版计划：任意（必须为用户启用校样）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校对权限配置文件 </td> 
   <td>经理或更高级别</td> 
  </tr> 
  <tr> 
   <td role="rowheader">校样角色</td> 
   <td>作者或审核者</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、角色或校样权限配置文件，请联系您的Workfront或Workfront校样管理员。

## 共享校样链接

共享校样链接可授予Workfront用户查看访问权限。 用户可以使用其Workfront登录凭据对校样进行评论，并订阅校样的电子邮件通知。 非校样用户可以使用电子邮件地址和显示名称进行评论和订阅。

>[!IMPORTANT]
>
>必须启用允许通过公共URL或嵌入代码共享校样设置。

1. 选择包含要与用户共享的校样的文档。

   只能选择一个文档。 您无法同时共享多个文档的链接。

1. 单击 **共享** > **校样链接**.
1. 在 **校样链接** 框中，执行以下任一操作：

   * 要将链接复制到剪贴板，请单击 **复制链接**.

      您现在可以通过第三方工具（如聊天或电子邮件应用程序）分发链接。

   * 要直接从Adobe Workfront通过电子邮件发送链接，请执行以下操作：

      1. 在 **或通过电子邮件链接至** 字段，开始键入并选择收件人的名称。 或指定要与之共享的外部用户的电子邮件地址。

         >[!NOTE]
         >
         >如果在共享校样时看到别名电子邮件，则如果存在相应的别名电子邮件，则不要通过输入原始电子邮件来创建新的来宾用户。

      1. 从以下选项中进行选择：

         <table style="table-layout:auto">
          <col>
          <col>
          <tbody>
           <tr>
            <td role="rowheader">发送公共链接</td>
            <td><p>在电子邮件通知中包含一个按钮，用于将用户引导至其所使用的校对查看器中的校样，并授予“查看”访问权限。</p><p>如果 <strong>通过公共URL或嵌入代码订阅校样</strong> 为校样关闭时，用户可以使用其Workfront登录凭据登录，以向校样添加注释。 如果启用了该设置，则提供其电子邮件地址和名称（无需密码）的任何人都可以签名并向校样添加注释。</p></td>
           </tr>
           <tr>
            <td role="rowheader">发送下载链接</td>
            <td>在电子邮件通知中包含一个按钮，可将用户引导至下载页面，该页面提供文件详细信息、文件名和文件大小，并且文件显示为内嵌。 用户可以单击下载页面中的下载链接以下载文件。</td>
           </tr>
           <tr>
            <td role="rowheader">添加自定义消息</td>
            <td>用于指定电子邮件通知的自定义主题和正文。</td>
           </tr>
          </tbody>
         </table>

      1. 单击 **发送**.

         收件人会收到一封电子邮件通知，其中包含有关您选择包含的校样和按钮的信息。

         ![](assets/proof-share-email-350x87.png)

## 将用户添加到校样

如果您对校样具有编辑权限，则可以将任何Workfront用户添加到校样中。 如果校样具有多个阶段，则将用户添加到单个阶段

>[!NOTE]
>
>如果您使用的是旧版Workfront计划，可以在该计划中为用户启用和禁用校对，请记住以下事项：
>
>* 要查看校样，收件人无需启用校样。
>* 启用自动工作流后，如果向校样中添加了未在Workfront中启用校样的用户，则会在自动工作流中创建一个新阶段。 您添加的用户在首次查看校样时会自动添加到此新阶段。 (有关详细信息，请参阅 [自动化工作流概述](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).)
>


### 从“文档”选项卡将用户添加到现有校样

1. 选择包含要将用户添加到的校样的文档。
1. 如果校样没有自动工作流（阶段），请单击 **更多** 图标，然后单击 **共享** 中。

   或

   如果校样确实具有自动工作流，请单击 **更多** 图标，然后单击 **共享** 中。

1. 在 **共享此版本** 框，位于 **共享**，开始键入要与其共享校样的用户的名称或电子邮件地址，然后在下拉列表中显示该名称时单击该名称。

1. （可选）重复此步骤以向校样添加多个用户。
1. （可选）为审阅人设置截止时间。
1. （可选）确保 **通过电子邮件通知用户** 选中。
1. （可选） **添加自定义消息** 收件人。
1. 添加所有审阅人后，单击 **共享**.

### 从校样查看器将用户添加到现有校样

您可以在Web校样查看器和桌面校样查看器中查看校样时，将用户添加到校样中。

有关更多信息，请参阅 [通过向校样添加用户来共享校样](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users) 在文章中 [从校对查看器共享校样](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md)

## 报告校对批准

您可以创建报告在Workfront中共享的校样批准情况的报表。 此报表在您的系统中提供了以下验证批准信息：

* 已提交以供审批的文件
* 审批者的姓名
* 校样版本
* 校对 ID
* 校样创建日期

在基于对象创建报告时，您可以访问此批准，如 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

有关校样批准对象报表的更多信息，请参阅 [对象报告](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) 部分 [了解Adobe Workfront中的对象](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)

## 批准共享校样

当用户将您添加到校样并使用自动工作流授予“审批者”角色或“审批者和审批者”角色时，批准请求会显示在“主页”或“我的工作”区域的“批准”选项卡中。 然后，您可以直接从Workfront查看校样并对校样做出批准决策。

有关如何从“我的工作”区域做出批准决策的信息，请参阅 [从主页区域批准工作](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-home-area) 或 [批准工作](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-my-work-area) in [批准工作](../../../review-and-approve-work/manage-approvals/approving-work.md).
