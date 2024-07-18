---
product-area: resource-management
navigation-topic: resource-planning
title: 从资源规划者导出信息
description: 您可以将资源规划者的任何视图中的信息导出到计算机上保存的Excel (.xlsx)文件。
author: Alina
feature: Resource Management
exl-id: 07acd28a-5dc0-45b4-bdf2-20abbd5e098c
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '661'
ht-degree: 3%

---

# 从资源规划者导出信息

您可以将资源规划者的任何视图中的信息导出到计算机上保存的Excel (.xlsx)文件。

>[!IMPORTANT]
>
>显示的信息以及可从Resource Planner导出的信息存在限制。 有关这些限制的信息，请参阅[资源规划者显示限制](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>专业及更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>审核或更高 <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       (this seems to be the case in NWE only, not classic. Waiting on Vazgen's response for this)
      </MadCap:conditionalText>
     --></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看或更高权限的项目、用户和资源管理</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看项目的权限或更高版本</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 从资源规划者导出信息

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)。

1. 单击&#x200B;**资源**。 默认显示&#x200B;**规划者**。

1. 为规划者选择视图。 您可以选择以下选项之一：

   * 按用户查看
   * 按项目查看
   * 按角色查看

1. 单击&#x200B;**导出**。

   此时将显示“导出选项”对话框。

   ![](assets/rp-export-options-box-350x421.png)

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
