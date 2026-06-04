---
product-area: resource-management
navigation-topic: resource-planning
title: 从资源规划者导出信息
description: 您可以将资源规划者的任何视图中的信息导出到计算机上保存的Excel (.xlsx)文件。
author: Lisa
feature: Resource Management
exl-id: 07acd28a-5dc0-45b4-bdf2-20abbd5e098c
TQID: https://experienceleague.adobe.com/f1tAWm7-QiEGbN-ENKTlJumMK29mqdiZ5PgY-27gzc4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: d1573eb8-a2e8-4a06-9526-9c3410bf4914
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 582
ht-degree: 8%

---

# 从资源规划者导出信息

您可以将资源规划者的任何视图中的信息导出到计算机上保存的Excel (.xlsx)文件。

>[!IMPORTANT]
>
>显示的信息以及可从Resource Planner导出的信息存在限制。 有关这些限制的信息，请参阅[资源规划者显示限制](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
  <tr> 
   <td>Adobe Workfront 包</td> 
   <td><p>“任一”</p></td>
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>浅色或更高</p>
       <p>审核或更高</p></td> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td> <p>查看对项目、用户和资源管理的访问权限或更高版本</p></td> 
  </tr> 
  <tr> 
   <td>对象权限</td> 
   <td> <p>查看项目或更高权限</p></td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 从资源规划者导出信息

{{step1-to-resourcing}}

默认显示&#x200B;**规划者**。

1. 为规划者选择视图。 您可以选择以下选项之一：

   * 按用户查看
   * 按项目查看
   * 按角色查看

1. 单击&#x200B;**导出**。

   此时将显示“导出选项”对话框。

   ![导出选项](assets/rp-export-options-box-350x421.png)

1. 指定以下信息：\
   **开始日期**：导出的开始日期。 导出的文件包含从一周的第一天开始的分配和可用性信息，其中包含您在此指定的日期。\
   **句点数**：文件中要包含的时段数。 默认值为4个期间。\
   **类型**：要在导出的文件中显示信息所依据的时间段类型（周、月或季度）。\
   以下是您可以导出的最长时段：

   * 52 周
   * 36 个月
   * 12个季度

   **选择以导出**：根据您选择的视图，您可以选择导出屏幕上列出的所有对象或特定对象的可用性和预算信息。
您可以选择导出以下信息：

   * 在“项目视图”中，选择要导出：

      * 项目
      * 项目和角色
      * 全部（这是默认选项）

   * 在“用户视图”中，选择要导出：

      * 用户
      * 用户和项目
      * 全部（这是默认选项）

   * 在“角色视图”中，选择以导出：

      * 角色
      * 角色和项目
      * 全部（这是默认选项）

   **数据格式**：根据您希望Excel文件的显示方式，选择以下选项：

   * **原始**：选择此项可显示Excel文件中按其所属对象取消分组的可用性和分配信息。 （这是默认选项）
   * **已分组**：选择以显示按其所属对象分组的可用性和分配信息。 这将显示屏幕上显示的导出信息。

   “导出选项”对话框中显示了信息在导出文件中的外观示例。

1. 单击&#x200B;**导出**&#x200B;以从资源规划者导出信息。\
   仅导出已保存的信息。

1. （视情况而定）如果您在角色或项目视图中有未保存的预算小时数，请单击&#x200B;**保存并继续。**
Excel (.xlsx)文件已下载到您的计算机。\
   在文件准备下载时，从资源规划者导出不可用。\
   （视情况而定）如果导出大量数据，您将收到一封电子邮件，其中包含可供您下载文件的链接。\
   ![RP_eamil_with_exported_planner_attached.png](assets/rp-eamil-with-exported-planner-attached-350x116.png)

1. （视情况而定）当您收到包含导出文件的电子邮件时，单击&#x200B;**下载**&#x200B;以下载该文件。\
   这会将您带回Workfront，您可以在其中下载文件。\
   您必须登录到Workfront才能完成下载。\
   如果您在交付文件时没有下载文件，则启动导出后，下载链接将保持活动状态7天。
