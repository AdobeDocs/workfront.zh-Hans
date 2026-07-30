---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: 更改历史记录
description: 更改历史记录允许您查看对Workfront对象所做的更改日志
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: ba1843cf6be446a809f9526608a3ae3bef69c494
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 4%

---

# 查看和管理变更历史记录

您可以在“设置”的“变更跟踪”区域中查看变更历史记录，包括审核日志。

* **审核日志**是由用户触发的更改。
有关审核日志和审核日志区域的详细信息，请参阅[审核日志概述](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/audit-logs.md)
* **配置**显示为“更改历史记录列表”跟踪的字段。
配置当前仅作为信息提供，无法更改。在不久的将来，将可以更改跟踪哪些字段。
* **更改历史记录列表**&#x200B;允许您查看对Workfront对象的更改日志，包括如下属性：

  * 对象
  * 对象类型
  * 更改类型（操作）
  * 更改的Source，如特定用户、API、Workfront Fusion、AI LLM或Workfront系统

  <span class="preview">在“更改历史记录”中跟踪统一审阅和批准工作流活动，包括参与者和决策。</span>

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 包</td> 
   <td>“任一”</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 许可证</td> 
   <td>[！UICONTROL标准版]</td> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>系统管理员</td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 查看和管理审核日志

要查看和管理审核日志，请参阅[查看和导出审核日志](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md)。

## 查看更改跟踪的配置区域

>[!NOTE]
>
>配置当前仅作为信息提供，无法更改。 在不久的将来，将可以更改跟踪哪些字段。

要查看所跟踪的更改类型，请执行以下操作：

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**更改跟踪** ![更改历史记录图标](assets/change-history-icon.png)。
1. 单击&#x200B;**配置**。

   显示按对象类型分组的字段。

1. 要显示特定对象下的字段，请单击对象类型旁边的下拉箭头。

## 查看更改历史记录列表

Workfront管理员可以在“设置”区域查看更改历史记录。

“更改历史记录列表”是一个增强型列表，具有筛选器、列、行高、日期选取器和搜索栏。

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**更改跟踪** ![更改历史记录图标](assets/change-history-icon.png)。
1. 单击&#x200B;**更改历史记录列表**。

   将打开“更改历史记录列表”。

1. 要调整显示更改的日期，请单击日期选取器并选择新日期。

   更改适用于过去90天。

1. 要搜索特定术语，请单击搜索栏并输入术语。 当您键入时，结果会在列表中加亮。
1. （可选）要按列筛选，请参阅文章[使用增强列表](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)中的[筛选增强列表](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#filter-items-in-an-enhanced-list)中的项。
1. （可选）要隐藏、显示或重新排序列，请参阅文章[使用增强列表](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)中的[自定义列](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#customize-columns)。
1. （可选）要添加或删除列，请参阅[使用增强列表](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)中的使用列管理器](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#add-and-remove-columns-with-the-column-manager)的[添加和删除列。
1. （可选）要调整行高，请参阅文章[使用增强列表](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)中的[更改视图中的行高](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#change-the-row-height-in-a-view)。

## 导出更改历史记录

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**更改跟踪>更改历史记录列表**。
1. 筛选列表以显示要导出的项目。
1. 单击&#x200B;**导出**&#x200B;图标![导出图标](assets/export-icon.png)并选择保存为XLSX还是CSV格式。

   这将打开保存文件框，您可以将导出的文件保存在计算机上。
   完成保存导出的文件。您现在可以在计算机上找到该代码并与他人共享。



