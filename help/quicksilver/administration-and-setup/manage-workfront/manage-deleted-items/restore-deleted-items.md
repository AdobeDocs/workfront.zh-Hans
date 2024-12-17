---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: 恢复已删除的项目
description: 如果您是Workfront管理员，则可以在Adobe Workfront中恢复项目、任务、问题、文档和模板（如果它们在过去30天内被删除）。 30天后，这些项目将永久删除且无法恢复。
feature: System Setup and Administration
author: Lisa
role: Admin
exl-id: e5b63652-ce16-44a9-a806-a41f19970ee1
source-git-commit: 36c4505b396f38617a7e82ae637596ff6c046d57
workflow-type: tm+mt
source-wordcount: '1052'
ht-degree: 2%

---

# 还原已删除的项目

<!--Audited: 12/2023-->

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

如果您是Workfront管理员，则可以在Adobe Workfront中恢复项目、任务、问题、文档和模板（如果它们在过去30天内被删除）。 30天后，这些项目将永久删除且无法恢复。

恢复对象时，也将恢复其所有子对象和字段。 例如，如果您恢复项目，则也会恢复项目中的所有任务、问题、文档、小时、注释、工作和自定义数据。

组管理员还可以为其管理的组恢复这些对象。

>[!IMPORTANT]
>
>* 如果删除报告、功能板、用户、组、团队或迭代，则无法恢复它。
>* 在组中，当除组管理员之外的人将文档直接上载到对象的“文档”区域时，只有Workfront管理员才能恢复文档。
>
>* 如果您移动任务或问题并选择不移动附加到任务或问题的文档，文档将被删除并放入回收站30天。 管理员可以恢复它们，并且它们被重新附加到移动的任务或问题。 如果任务或问题在移动后已被删除，文档将在管理员用户页面的“文档”区域中恢复，管理员负责恢复文档。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>新增：标准</p>
       <p>或</p>
       <p>当前：计划</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>[！UICONTROL系统管理员]</td>
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 恢复项目、任务或问题时恢复的信息

在恢复项目、任务或问题时，将同时恢复以下相关信息：

* “更新”区域中的评论和回复
* 审批
* 任务
* 自定义表单
* 队列设置
* 业务案例，包括记分卡、目标和风险
* 项目团队
* 日期
* 问题
* 任务
* 子任务
* 状态
* 财务资料：

   * 账单记录
   * 记帐费率
   * 费用

* 时间线信息：

   * 前置任务
   * 任务限制
   * 持续时间类型

* 基线

  在恢复父项目或任务时，任务基线会恢复，但在恢复单独删除的任务时不会恢复。

* 小时（和小时ID）

  是否将小时数还原到删除的项目取决于您在配置时间表和小时数的首选项时选择的设置。 有关详细信息，请参阅[在删除并还原对象时配置影响时间](../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md)。

* 项目的URL

  恢复后，该项目的URL将保持不变。 如果人员已经为项目创建了浏览器书签，则这些书签仍然有效。

* 访问和权限

  在项目被删除之前具有项目访问权限的用户会在项目恢复后重新获得访问权限。

* 文档（包括验证文档）

  恢复文档和文档版本时，请考虑以下事项：

   * 可以单独恢复单独删除的文档。

     当您恢复父级时，会恢复与其父级项目、任务或问题一起被删除的文档，但无法单独恢复它们。

   * 文档或文档验证的所有版本在文档恢复后都会恢复。\
     无法恢复单独删除的文档或文档验证的单独版本。

## 恢复项目、任务或问题时未恢复的信息

在恢复项目、任务或问题时，以下关联信息不会随项目一起恢复：

* 赞
* 认可
* 请求队列中的接收电子邮件地址
* 收藏夹

  在删除之前添加到“收藏夹”菜单的项目、任务或问题在恢复后不会重新出现在“收藏夹”菜单中。

* 解析对象

  解析对象是使用选项&#x200B;**保留原始问题并将其解决方案与此** &lt;**（项目**&#x200B;或&#x200B;**任务）**>配置的转换问题。 如果删除父项目或任务，则问题不再被标识为解析对象，因为不再有链接将其连接到项目或任务。 如果恢复父项，则不会恢复链接。

  有关Workfront管理员或组管理员如何在转换时配置问题以匹配解决对象的详细信息，请参阅[配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)和[为组配置任务和问题首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)。

  有关转换问题的更多信息，请参阅[在Adobe Workfront中转换问题的概述](../../../manage-work/issues/convert-issues/convert-issues.md)。

## 还原项目

{{step-1-to-setup}}

1. 单击&#x200B;**回收站** > **最近删除的**。
1. 根据要还原的项类型，单击&#x200B;**项目**、**任务**、**问题**、**模板**&#x200B;或&#x200B;**文档**&#x200B;选项卡。

   默认情况下，项按&#x200B;**删除日期**&#x200B;列排序。

1. 选择最多10个要恢复的项目。

   如果删除子任务，则它将显示在列表中。

   如果删除父任务，则列表中只会显示父任务。 但是，当您恢复父任务时，所有子任务都会恢复。

1. 单击&#x200B;**还原**&#x200B;以将所选项目还原到其原始位置。
1. （可选）要快速查看已还原的项目，请按照[查看已还原的项目](../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md)中的步骤操作。

   有关恢复项目后所发生情况的详细信息，请参阅本文中的[恢复项目后所发生的情况](#what-happens-after-you-restore-items)部分。

## 恢复项目后发生的情况 {#what-happens-after-you-restore-items}

* 恢复任务和子任务时，它们会按删除之前的顺序显示。

  但是，如果删除任务时其他任务的顺序发生更改，则任务可能会恢复到任务或子任务列表的底部。

* 恢复项目后：

   * 系统会显示一条消息，让您知道自己是否成功。

     您还会收到电子邮件通知。 如果恢复多个项目，电子邮件会列出它们。

   * 项目、任务或问题的更新区域以及父对象的更新区域中都将显示一个注释。

     当您恢复文档或模板时，不会发生这种情况。

## 已恢复校对

当有人恢复具有验证的文档时，验证的验证活动页面可能会显示您组织的实例中列出的第一个活动Workfront管理员的名称（按配置文件ID排序），而不是恢复验证的实际人员的姓名。
