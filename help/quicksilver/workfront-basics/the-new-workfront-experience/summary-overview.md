---
content-type: overview
title: 摘要概述
description: 您可以使用“摘要”面板直接从任务问题、文档的列表或从的其他区域查看和更新工作项信息 [!DNL Adobe Workfront] 显示任务和问题。
feature: Get Started with Workfront
author: Nolan
exl-id: 5e4026b2-5f2f-45c1-bef1-04e20c62ed8a
source-git-commit: 5d6e9788ccbae7a8970cff56558233a57ceee1ab
workflow-type: tm+mt
source-wordcount: '992'
ht-degree: 2%

---

# [!UICONTROL 摘要] 概述

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers or in Production for customers who enabled fast releases. </span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release schedule, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span> -->

您可以使用 [!UICONTROL 摘要] 面板，直接从任务、问题、文档的列表或从的其他区域查看和更新工作项信息。 [!DNL Adobe Workfront] 显示任务和问题。

您的Workfront或组管理员可以修改“摘要”面板中显示的区域和字段。 他们最多可以向“摘要”面板添加16个字段。

>[!IMPORTANT]
>
>我们建议您将必须经常更新的字段添加到“摘要”面板，这样您便可以轻松访问和更新它们，而无需访问对象的主页。
>
>例如，您可以将以下经常更新的字段添加到任务和问题“摘要”面板：
>
>* 状态
>* 完成百分比
>* 承诺日期
>* 规划完成日期
>* 完成情况



下表显示您可以定位和使用 [!UICONTROL 摘要] 面板：

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td><b>任务</b></td> 
  </tr> 
  <tr> 
   <td> <p>中的任务列表</p> 
    <ul> 
     <li>项目</li> 
     <li>子任务</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作负载均衡器]的[！UICONTROL未分配]和[！UICONTROL已分配]工作区域中的任务</td> 
  </tr> 
   <tr> 
   <td>[！UICONTROL时间表]中的任务</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><b>问题</b></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>中的问题列表</p> 
    <ul> 
     <li>项目</li> 
     <li>任务</li> 
     <li>子任务</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL工作负载均衡器]的[！UICONTROL已分配工作]区域出现问题</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL请求]区域的[！UICONTROL已提交]部分中的问题</td> 
  </tr> 
</tr> 
   <tr> 
   <td>[！UICONTROL时间表]中的问题</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td><b>文档</b></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL文档]区域</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>任何对象（项目、任务、问题、项目、项目组合、模板、模板任务、用户）的[！UICONTROL文档]部分</td> 
  </tr> 
 </tbody> 
</table>

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront administrators can customize the Summary in the Layout Template. For more information, see <a href="../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p>
-->

本文介绍了如何访问和使用 [!UICONTROL 摘要] 列表中任务和问题的面板。

有关访问 [!UICONTROL 摘要] 在 [!UICONTROL 工作负载均衡器]，请参见 [更新中的工作项 [!UICONTROL 工作负载均衡器] 使用 [!UICONTROL 摘要]](../../resource-mgmt/workload-balancer/update-items-in-summary-panel-in-workload-balancer.md).

有关访问 [!UICONTROL 摘要] 有关文档，请参阅 [[!UICONTROL 摘要] （文档）概述](../../documents/managing-documents/summary-for-documents.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>新文档：参与者或更高版本</p>
   或
   <p>当前：[！UICONTROL Request]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置</strong></td> 
   <td> <p>[！UICONTROL视图]或更高的任务、问题、文档访问权限</p> <p>[！UICONTROL View]或更高权限访问您要查看其文档[！UICONTROL Summary]的任何对象</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>[！UICONTROL视图]或任务、问题或文档的更高权限</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。 有关更多信息，请参阅 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 查看 [!UICONTROL 摘要] 任务或问题列表中的面板

1. 转到任务或问题，然后在列表中选择一个项目。
1. 单击 **[!UICONTROL 摘要]** 图标 ![](assets/qs-summary-in-new-toolbar-small.png)

   或

   单击 **[!UICONTROL 打开摘要]** 图标 ![](assets/open-summary-with-text-nwe.png) 在 [!UICONTROL 已提交] 的部分 [!UICONTROL 请求] 区域。

   打开“摘要”后，在单击或选择其他任务或问题时，它保持打开状态，直到手动关闭它为止。

   >[!TIP]
   >
   >您一次只能选择一个任务或一个问题，以在 [!UICONTROL 摘要] 面板。

   ![摘要面板](assets/summary-panel-for-task-new-comments.png)

1. （可选）关闭 [!UICONTROL 摘要] 面板，执行以下操作之一：

   * 在任务或问题列表中，单击 **[!UICONTROL 打开摘要]** 图标 ![](assets/summary-panel-icon.png)

     或

     单击 **X** 图标（位于的右上角） [!UICONTROL 摘要] 面板。

   * 在 [!UICONTROL 已提交] 的部分 [!UICONTROL 请求] 区域，单击 **[!UICONTROL 关闭摘要]** 图标 ![](assets/close-summary-with-text-nwe.png)

     或

     单击 **X** 图标（位于“摘要”面板右上角）。

## [!UICONTROL 完成百分比]

使用顶部的进度条 [!UICONTROL 摘要] 更新您选择的任务或问题的完成百分比。 输入一个数字或将栏拖到正确的百分比上。

![摘要面板中的完成百分比](assets/summary-overview-percent-complete.png)

## [!UICONTROL 更新]

使用 [!UICONTROL 更新] 的部分 [!UICONTROL 摘要] 查看最近的更新，并对您选择的任务或问题进行更新。 单击 **[!UICONTROL 查看全部]** 直接转到 [!UICONTROL 更新] 选项卡上。

![“摘要”面板中的“更新”部分](assets/summary-updates-section.png)

## [!UICONTROL 文档]

使用 [!UICONTROL 文档] 的部分 [!UICONTROL 摘要] 以查看附加到所选任务或问题的文档。 单击缩略图以打开文档预览。 直接转到 [!UICONTROL 文档] 选项卡，单击 **[!UICONTROL 文档]** 标题。

![摘要面板中的文档部分](assets/summary-documents-section.png)

## [!UICONTROL 详细信息]

使用 [!UICONTROL 详细信息] 的部分 [!UICONTROL 摘要] 要查看高级别工作项详细信息、进行分配或添加开始日期，请执行以下操作： 单击 **[!UICONTROL 查看全部]** 直接转到 [!UICONTROL 详细信息] 选项卡。

>[!NOTE]
>
>此部分中显示的字段与主页右侧面板中显示的字段相同。 您可以自定义这些字段 [自定义 [!UICONTROL 主页] 和 [!UICONTROL 摘要] 使用布局模板](../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).

![摘要面板中的“详细信息”部分](assets/summary-details-section.png)

## [!UICONTROL 子任务]

此部分仅适用于任务。 使用 [!UICONTROL 子任务] 的部分 [!UICONTROL 摘要] 查看 [!UICONTROL 新建]， [!UICONTROL 进行中]、和 [!UICONTROL 已关闭] 您选择的任务的子任务。 单击 **[!UICONTROL 状态]** 下拉菜单以在状态之间切换。 直接转到 [!UICONTROL 子任务] 选项卡上，单击 **[!UICONTROL 子任务]**&#x200B;标题&#x200B;。

如果尚未向任务添加任何子任务，请单击 **[!UICONTROL 在此处添加一个]** 直接转到 [!UICONTROL 子任务] 选项卡上。

![摘要面板中的“子任务”部分](assets/summary-subtasks-section.png)

## [!UICONTROL 小时]

使用 [!UICONTROL 小时] 的部分 [!UICONTROL 摘要] 以记录所选任务或问题的小时数。 单击 **[!UICONTROL 记录时间]** 并输入您的小时数。 要直接转到任务或问题的小时数选项卡，请单击 **[!UICONTROL 小时]** 标题。

中的小时数 [!UICONTROL 摘要] 显示您记录的小时数。 其他用户在 [!UICONTROL 摘要] 取决于用户登录任务的时间。

如果没有计划 [!UICONTROL 小时] 对于任务或问题，如果您已经记录时间，则小时栏显示红色。

![摘要面板中的“小时”部分](assets/summary-hours-section.png)

## 审批

使用 [!UICONTROL 审批] 的部分 [!UICONTROL 摘要] 查看附加到所选任务或问题的审批。 如果您尚未添加任何批准，请从下拉菜单中选择一个现有批准，或单击 **[!UICONTROL 创建单一使用审批流程]** 直接转到 [!UICONTROL 审批] 选项卡。

直接转到 [!UICONTROL 审批] 选项卡，单击 **[!UICONTROL 审批]** 标题。

![摘要面板中的“审批”部分](assets/summary-approvals-section.png)
