---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: 恢复单个子对象
description: 本文介绍了如何获取有关恢复已从Adobe Workfront生产或预览环境中删除的单个子对象的帮助，这些环境在30天之前未删除。
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: e2e4fbb7-5433-4d88-8e36-d82f4cc8a194
source-git-commit: 156341072c291b5c03432da399a509d9772b73ea
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 0%

---

# 恢复单个子对象

本文介绍了如何获取有关恢复已从Adobe Workfront生产或预览环境中删除的单个子对象的帮助，这些环境在30天之前未删除。

Workfront管理员可以恢复每个Workfront实例中的项目、任务、问题和文档，如[恢复已删除的项](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)中所述。 但只有Workfront数据库团队可以恢复对象，例如任务、问题、文档、自定义表单、小时和注释，而不依赖于其父对象。

来自实时环境的数据在预览Sandbox中可用长达7天。 这意味着您可以使用以下方法从预览Sandbox环境中导出独立数据：

* Kick-Starts
* 构建报告并导出结果

有关从Workfront导出数据的详细信息，请参阅[导出数据](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md)。

可通过以下方式导入导出的数据：

* 手动（如果您使用导出的报告）
* 批量使用Kick-Starts

  有关使用Kick-Start将数据导入Workfront的更多信息，请参阅[使用Kick-Start模板将数据导入Adobe Workfront](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)。

在周末的维护时段中刷新预览Sandbox环境。

有关“预览Sandbox”环境的维护窗口的详细信息，请参阅[Adobe状态网站](https://status.adobe.com)。

>[!IMPORTANT]
>
>文档是这些恢复方法的例外。 您可以从预览环境中手动下载它们，并将它们重新上传到生产环境中。 如果要批量下载和上传文档，您需要从Workfront请求数据恢复。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p>
       <p>规划</p></td>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>系统管理员</td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 数据恢复所需的信息

确定已删除的对象需要由我们的数据库团队恢复后，请收集您掌握的有关该对象的信息。 数据库管理员需要以下信息才能找到对象并启动还原：

* 对象名称
* 对象类型（任务、问题、项目等）
* 预计删除日期和时间
* 对象GUID（如果可能）

  找到对象的GUID时，请参阅以下信息：

   * 通过引用通过与对象交互而触发的电子邮件通知（分配、评论等），可以找到GUID
   * 在URL末尾找到的GUID示例： `yourdomain.my.workfront.com/issue/view?ID=568bfa96011220154c8ca4c4e691556b`

收集完此信息或需要帮助后，请致电我们的客户支持团队：844-306-HELP(4357)，或在线提交票证。

## 数据恢复过程

1. 我们的客户支持团队收到您的信息后，会将其上报给我们的客户支持团队。
1. 我们的客户支持团队将与我们的数据库团队联系。
1. 一旦数据库小组有机会审查正在恢复的数据，就可以提供对ETA的更准确的估计。 恢复通常需要三天，但可能需要更长的时间，具体取决于要恢复的数据类型和卷。
1. 数据库团队将信息还原到预览沙盒环境，您可以在其中查看还原的数据。 我们的客户支持团队将告知您何时可在预览Sandbox中找到数据。
1. 在您对沙盒中的恢复感到满意后，请让我们的客户支持团队知道，他们将与我们的数据库团队联系，通知他们可以将数据恢复到您的生产环境。
1. 在请求关闭之前，您将有机会查看已还原的数据。
