---
product-area: documents
navigation-topic: approvals
title: 创建分组审批
description: 您可以将多个文档捆绑到单个审批工作流中，以便它们一起在相同的阶段中移动。
author: Courtney
feature: Work Management, Digital Content and Documents
source-git-commit: 31bba5df6f491bfd048c1005ecd5330d3321e748
workflow-type: tm+mt
source-wordcount: '1173'
ht-degree: 1%
---

# 创建分组审批

<span class="preview">此页面上的信息在“预览沙盒”环境中不可用，因为Frame.io集成在该环境中不可用。 此功能将于2026年10月14日和15日在生产环境中可用。</span>

分组的审批在单个审批工作流下捆绑了多个文档。 您可以使用基本和高级模式、多个阶段以及具有分组审批的并行路径，就像处理单个文档审批一样。

分组的审批仅在新的“文档”区域中可用，当您的组织使用Adobe云存储时，将显示该区域。 有关详细信息，请参阅[Adobe云存储概述](/help/quicksilver/review-and-approve-work/esm-overview.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto">
 <col>
 <col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront 包</td>
   <td> <p>任何使用Adobe云存储管理审批的工作流包</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront许可证</td>
   <td>
   <p>参与者或更高版本</p>
   <p>审核或更高</p>
   <p>对于使用Adobe云存储的对象，您必须具有Standard许可证才能创建批准工作流。</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader">访问级别配置</td>
   <td> <p>查看或更高权限的项目、任务、问题、模板、项目组合、程序、报告、功能板、日历和文档</p></td>
  </tr>
  <tr>
   <td role="rowheader">对象权限</td>
   <td> <p>管理与请求或审批关联的对象的访问权限</p></td>
  </tr>
 </tbody>
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 创建基本的分组审批

要创建单阶段分组审批，请执行以下操作：

1. 转到包含文档的项目、任务或问题，然后在左侧面板中选择&#x200B;**文档**。

1. 单击要包含的第一个文档，然后按住Shift并单击其他文档以选择多个文档。

1. 选择文档后，单击底部菜单中的&#x200B;**请求审批**。 **请求审批**&#x200B;对话框在基本模式下打开。

   ![创建分组审批](assets/requeset-grouped-approval.png)

1. 填写以下详细信息：

   <table>
   <tr>
   <td><strong>使用审批模板（可选）</strong></td>
   <td>默认情况下，“模板”字段处于折叠状态。 单击该字段以将其展开，然后从下拉菜单中选择一个模板。 如果模板具有一个路径和一个阶段，则它适用于基本模式。 如果模板具有多个阶段或多个路径，则该对话框会自动切换到“高级”模式，并且在“基本”模式下输入的任何输入都将被模板的内容替换。</td>
   </tr>
   <tr>
   <td><strong>在预览中添加人员或团队</strong></td>
   <td><p>开始键入用户名、团队或电子邮件地址，然后选择他们是<strong>审批者</strong>还是<strong>审阅者</strong>。 Workfront可单独添加团队的每个活动成员。</p>
   <p>注意：如果用户已添加或属于您添加的多个团队，则这些用户将被包含一次。</p></td>
   </tr>
   <tr>
   <td><strong>只需一个决策（可选）</strong></td>
   <td>第一个做出决策的人将完成阶段。</td>
   </tr>
   <tr>
   <td><strong>到期日期（可选）</strong></td>
   <td>设置审批的截止日期。 在指定到期日期的72小时之后24小时之前，会通过电子邮件向用户发送通知。</td>
   </tr>
   <tr>
   <td><strong>添加自定义消息（可选）</strong></td>
   <td>在<strong>添加自定义消息</strong>文本框中键入消息。 该消息会显示在批准电子邮件通知和Workfront的“批准”选项卡中。</td>
   </tr>
   </table>

1. （可选）单击&#x200B;**文档**&#x200B;选项卡以查看此审批中包含的文档。

1. 单击&#x200B;**请求审批**。

   ![基本分组审批](assets/basic-group-approval.png)

## 创建高级分组审批

高级模式支持并行路径。 每个路径都独立运行，并包含一个或多个顺序阶段。 当阶段中所有必需的决策都完成时，该路径中的下一阶段将开始，前一阶段将被锁定，新阶段的审阅人和批准者将收到电子邮件通知。

“需要工作”决策会停止它所在的路径，但不会影响其他路径上的审批工作流。

<!--
You can configure up to 30 paths and 100 stages total.
-->

要创建高级分组审批，请执行以下操作：

1. 转到包含文档的项目、任务或问题，然后在左侧面板中选择&#x200B;**文档**。

1. 单击要包含的第一个文档，然后按住Shift并单击其他文档以选择多个文档。

1. 选择文档后，单击底部菜单中的&#x200B;**请求审批**。

   ![创建分组审批](assets/requeset-grouped-approval.png)

1. 在&#x200B;**请求审批**&#x200B;对话框的右上角，单击&#x200B;**转到高级**。 您在基本模式下输入的任何输入都将被保留，并应用于&#x200B;**路径1**，**阶段1**。

   >[!TIP]
   >
   >创建审批时，单击右上方的&#x200B;**转到“基本”**，可返回到“基本”模式。 提交审批请求后，**转到基本**&#x200B;选项不再可用。

1. 填写路径1的第1阶段的详细信息：

   <table>
   <tr>
   <td><strong>阶段名称</strong></td>
   <td>默认情况下，阶段名为<em>阶段1</em>、<em>阶段2</em>，依此类推。 将阶段重命名为更具描述性的状态，如<em>初始审阅</em>或<em>最终批准</em>。</td>
   </tr>
   <tr>
   <td><strong>在预览中添加人员或团队</strong></td>
   <td><p>开始键入用户名、团队或电子邮件地址，然后选择他们是<strong>审批者</strong>还是<strong>审阅者</strong>。 Workfront可单独添加团队的每个活动成员。</p>
   <p>注意：如果用户已添加或属于您添加的多个团队，则这些用户将被包含一次。</p></td>
   </tr>
   <tr>
   <td><strong>只需一个决策（可选）</strong></td>
   <td>第一个做出决策的人将完成阶段。</td>
   </tr>
   <tr>
   <td><strong>到期日期（可选）</strong></td>
   <td>每个路径的第一阶段都支持绝对到期日期。 路径中的每个后续阶段都支持相对到期日期（从该阶段打开后的天数）。 到期日期前72小时，然后24小时通过电子邮件向用户发送通知。</td>
   </tr>
   <tr>
   <td><strong>添加自定义消息（可选）</strong></td>
   <td>在<strong>添加自定义消息</strong>文本框中键入消息。 该消息会显示在批准电子邮件通知和Workfront的“批准”选项卡中。<p>添加第二个阶段时，默认情况下会选中<strong>在所有阶段上显示此消息</strong>。 将其保留为选中状态，以便在每个阶段中使用相同的消息。 若要对每个阶段使用不同的消息，请清除<strong>在所有阶段上显示此消息</strong>，然后在每个阶段的<strong>添加自定义消息</strong>文本框中键入特定于阶段的消息。</p></td>
   </tr>
   </table>

1. （可选）向路径1添加其他阶段：
   1. 单击&#x200B;**添加阶段**&#x200B;以将另一个阶段添加到当前路径。 路径中的阶段将按其列出的顺序依次运行。
   1. 填写新阶段的详细信息，然后重复此步骤以根据需要添加更多阶段。

      >[!NOTE]
      >
      >您可以对路径中的阶段重新排序，但无法将阶段从一个路径移动到另一个路径。 每个路径可以有不同的阶段数。


1. （可选）添加并行路径：
   1. 在屏幕左侧的&#x200B;**并行路径**&#x200B;下，单击&#x200B;**添加路径**&#x200B;以添加其他路径。
   1. 按照相同的步骤将阶段和参与者添加到新路径中。 每个路径都独立运行，因此每个路径可以有不同的阶段数量和不同的参与者。

1. （可选）要删除路径，请将鼠标悬停在路径标签上并单击垃圾桶图标。 无法删除&#x200B;**路径1**，也无法对路径重新排序。 仅当路径中没有已锁定或已完成的阶段时，才能删除其他路径。

1. （可选）要清除所有路径和阶段并重新开始，请单击右上角的&#x200B;**重置**。

1. （可选）单击&#x200B;**文档**&#x200B;选项卡以查看此审批中包含的文档。

1. 单击&#x200B;**请求审批**。

   ![高级分组审批](assets/advanced-group-approval.png)


<!--

## Add additional documents to a grouped approval

You can add additional documents to a grouped approval after the approval has been created as long as the first stage has not been completed. 

To add an additional document to a grouped approval:

1. Click any document in the grouped approval, then click **Manage Approval** in the bottom menu.
1. Click **Documents on this approval**, then click **Add**.

   ![add document grouped approval](assets/add-document-to-grouped-approval.png)
1. Choose the documents you want to add, then click **Add to approval**. 
1. Once you add all of the documents, click **Edit approval**. The new documents are added to the grouped approval and all participants are notified of the change.

-->

## 已知限制

* 目前，在已分组的审批工作流创建后，您无法从工作流中添加或删除文档。 此功能计划在将来的版本中使用。
* 已分组的批准暂时限制为每个组3个路径和25个文档。