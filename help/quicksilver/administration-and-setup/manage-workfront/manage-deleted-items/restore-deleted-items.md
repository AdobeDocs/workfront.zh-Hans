---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: 恢复已删除的项目
description: 如果您是Workfront管理员，则可以恢复Adobe Workfront中的项目、任务、问题、文档和模板（如果这些项目在过去30天内已被删除）。 30天后，这些项目将被永久删除，无法恢复。 恢复对象时，其所有子对象和字段也会恢复。 例如，如果恢复项目，则项目中的所有任务、问题、文档、小时、注释、分配和自定义数据也会恢复。
feature: System Setup and Administration
role: Admin
exl-id: e5b63652-ce16-44a9-a806-a41f19970ee1
source-git-commit: 1fb283df7090173d8f4dd36b9474ced10c8d30d1
workflow-type: tm+mt
source-wordcount: '1076'
ht-degree: 1%

---

# 恢复已删除的项目

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

如果您是Workfront管理员，则可以恢复Adobe Workfront中的项目、任务、问题、文档和模板（如果这些项目在过去30天内已被删除）。 30天后，这些项目将被永久删除，无法恢复。

恢复对象时，其所有子对象和字段也会恢复。 例如，如果恢复项目，则还原项目中的所有任务、问题、文档、小时、注释、分配和自定义数据。

群组管理员还可以为他们管理的群组恢复这些对象。

>[!IMPORTANT]
>
>* 如果删除报表、功能板、用户、群组、团队或小版本，则无法恢复该报表。
>* 在组中，当组管理员以外的其他人将文档直接上传到对象的“文档”区域时，只有Workfront管理员才能恢复该文档。
>
>* 如果移动任务或问题，并选择不移动附加到任务或问题的文档，则这些文档将被删除并放入回收站30天。 管理员可以恢复这些任务，并将其重新附加到已移动的任务或问题。 如果任务或问题在移动后被删除，则文档将在恢复这些任务或问题的管理员用户页面的“文档”区域中恢复。


## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td>计划</td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划或许可证类型，请联系您的Workfront管理员。

## 在恢复项目、任务或问题时恢复的信息

在恢复项目、任务或问题时，会同时恢复以下关联信息：

* “更新”区域中的注释和回复
* 审批
* 分配
* 自定义表单
* 队列设置
* 业务案例，包括记分卡、目标和风险
* 项目团队
* 日期
* 问题
* 任务
* 子任务
* 状态
* 财务信息:

   * 账单记录
   * 账单费率
   * 费用

* 时间轴信息：

   * 前置任务
   * 任务约束
   * 持续时间类型

* 基线

   在恢复其父项目或任务时会恢复任务基线，但在恢复单独删除的任务时不会恢复任务基线。

* 小时（和小时ID）

   小时是否还原到已删除的项目取决于您在为工时单和小时配置首选项时选择的设置。 有关更多信息，请参阅 [配置在删除和还原对象时对小时数的影响](../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md).

* 项目的URL

   恢复后，项目的URL保持不变。 如果用户为项目创建了浏览器书签，则它们仍然有效。

* 访问和权限

   在删除项目之前有权访问该项目的用户在项目恢复后可重新获得访问权限。

* 文件（包括校样文件）

   恢复文档和文档版本时请考虑以下事项：

   * 单独删除的文档可以单独恢复。

      恢复父项时，会恢复已删除的文档及其父项目、任务或问题，但无法单独恢复它们。

   * 文档或文档校样的所有版本在恢复文档时都会恢复。\
      无法恢复单独删除的文档或文档校样的各个版本。

## 恢复项目、任务或问题时未恢复的信息

在恢复项目、任务或问题时，以下关联信息不会随之恢复：

* 称赞次数
* 认可
* 请求队列中的接收电子邮件地址
* 收藏夹

   在删除之前添加到“收藏夹”菜单的项目、任务或问题在恢复后不会重新出现在“收藏夹”菜单中。

* 解析对象

   解析对象是使用选项配置的已转换问题 **保留原始问题，并将其决议与此挂钩** &lt;**项目** 或 **task)**> 。 如果删除父项目或任务，则问题将不再被标识为解决对象，因为不再有链接将其连接到项目或任务。 如果恢复父项，则不会恢复链接。

   有关Workfront管理员或组管理员在转换时如何配置问题以匹配解决对象的详细信息，请参阅 [配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) 和 [为组配置任务和问题首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   有关转换问题的更多信息，请参阅 [转换Adobe Workfront中的问题概述](../../../manage-work/issues/convert-issues/convert-issues.md).

## 恢复项目

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **回收站** > **最近删除的**.
1. 单击 **项目**, **任务**, **问题**&#x200B;或 **文档** 选项卡，具体取决于要恢复的项目类型。

   项目按 **删除日期** 列。

1. 选择最多10个要恢复的项目。

   如果删除子任务，则该任务会显示在列表中。

   如果删除父任务，则列表中只显示父任务。 但是，在恢复父任务时，所有子任务都会恢复。

1. 单击 **还原** 将选定项目恢复到其原始位置。
1. （可选）要快速查看已恢复的项目，请按照 [查看还原的项目](../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md).

   有关恢复项目后所发生情况的详细信息，请参阅 [恢复项目后会发生什么情况](#what-happens-after-you-restore-items) 在本文中。

## 恢复项目后会发生什么情况 {#what-happens-after-you-restore-items}

* 恢复任务和子任务时，它们会按删除前的顺序显示。

   但是，如果在删除任务时其他任务的顺序发生更改，则任务可能会还原到任务或子任务列表的底部。

* 恢复项目后：

   * 此时将显示一条消息，告知您自己是否成功。

      您还会收到电子邮件通知。 如果还原了多个项目，则电子邮件会列出这些项目。

   * 项目、任务或问题的“更新”区域以及父对象的“更新”区域中会显示注释。

      恢复文档时不会发生这种情况。

## 还原的校样

此时，当有人还原有校样的文档时，校样的“校样活动”页面可能显示为您组织的实例列出的第一个活动的Workfront管理员的姓名（按用户档案ID的顺序），而不是显示还原校样的实际人员。
