---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: 恢复单个子对象
description: 本文档介绍如何获取帮助，以恢复之前不到30天从Adobe Workfront生产或预览环境中删除的各个子对象。
feature: System Setup and Administration
role: Admin
exl-id: e2e4fbb7-5433-4d88-8e36-d82f4cc8a194
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '575'
ht-degree: 0%

---

# 恢复单个子对象

本文档介绍如何获取帮助，以恢复之前不到30天从Adobe Workfront生产或预览环境中删除的各个子对象。

Workfront管理员可以恢复每个Workfront实例中的项目、任务、问题和文档，如 [恢复已删除的项目](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md). 但只有Workfront数据库团队可以独立于其父对象来恢复对象，如任务、问题、文档、自定义表单、小时数和注释。

预览沙盒中提供来自实时环境的数据，时间最长为7天。 这意味着您可以使用以下方法从预览沙盒环境中导出独立数据：

* Kick-Starts
* 构建报告并导出结果

有关从Workfront导出数据的更多信息，请参阅 [导出数据](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

您可以通过以下方式导入导出的数据：

* 手动（如果您使用的是导出的报表）
* 如果您使用的是“启动”，则批量处理

   有关使用Kick-Start将数据导入Workfront的更多信息，请参阅 [使用“启动”模板将数据导入Adobe Workfront](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

“预览沙盒”环境将在周末的维护窗口期间刷新。

有关预览沙盒环境维护窗口的更多信息，请参阅 [trust.workfront.com](https://trust.workfront.com/).

>[!IMPORTANT]
>
>文件是这些恢复方法的例外。 您可以从预览环境手动下载它们，然后将它们重新上传到生产环境。 如果要批量下载和上传文档，则需要从Workfront请求数据恢复。

## 数据还原所需的信息

确定删除的对象需要由我们的数据库团队进行还原后，收集与该对象有关的尽可能多的信息。 数据库管理员需要以下信息才能找到对象并启动还原：

* 对象名称
* 对象类型（任务、问题、项目等）
* 预计删除日期和时间
* 对象GUID（如果可能）

   在查找对象的GUID时，请参阅以下信息：

   * 可以通过引用通过与对象交互而触发的电子邮件通知（对的分配、对的注释等）来找到GUID
   * URL末尾的GUID示例： `yourdomain.my.workfront.com/issue/view?ID=568bfa96011220154c8ca4c4e691556b`

收集此信息或需要帮助后，请致电844-306-HELP(4357)联系客户支持团队或在线提交票证。

## 数据恢复过程

1. 在我们的客户支持团队收到您的信息后，他们会将其上报给我们的客户支持团队。
1. 我们的客户支持团队将联系我们的数据库团队。
1. 一旦数据库团队有机会查看要恢复的数据，就可以提供更准确的ETA估计。 恢复通常需要三天，但可能需要更长的时间，具体取决于要恢复的数据类型和卷。
1. 数据库团队会将信息还原到您的预览沙盒环境，您将有机会在该环境中查看还原的数据。 我们的客户支持团队将在预览沙盒中找到数据时通知您。
1. 在您对沙盒中的恢复感到满意后，请告知我们的客户支持团队，他们将联系我们的数据库团队，以通知他们可以将数据还原到您的生产环境。
1. 在请求关闭之前，您将有机会查看已还原的数据。
