---
user-type: administrator
product-area: system-administration;setup
title: 查看和管理变更历史记录
description: 更改历史记录允许您查看对Workfront对象和字段的更改日志。
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: 100b900bd7419d78a3135358026ec5e27755fdeb
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 3%

---

# 查看和管理变更历史记录

{{preview-fast-release-general}}

更改历史记录允许您配置和跟踪对Adobe Workfront中的对象和特定字段的更改。 灵活的配置允许您设置确切要跟踪哪些对象和字段。

更改历史记录可以跟踪您定义的以下数据类型：

* “设置”区域中的活动，如创建或删除访问级别或工作角色
* 字段级更新，例如编辑项目描述或更改用户的布局模板
* 对象更新，例如更新项目状态或向任务附加自定义表单
* <span class="preview">统一审阅和审批工作流活动，包括参与者和决策</span>

有关定义跟踪哪些对象和字段的信息，请参阅[在更改历史记录中配置要跟踪的字段](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/configure-fields-in-change-history.md)。

在“更改历史记录列表”中，您可以查看对Workfront对象所做的更改日志，包括如下属性：

* 对象名称
* 对象类型
* 更改类型（操作）
* 更改日期和时间
* 更改的Source，如特定用户、API、Workfront Fusion、AI LLM或Workfront系统

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
   <td>[!UICONTROL 标准版]</td> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td><span class="preview">对更改历史记录的管理访问权限</span></td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--
## View the Configuration area for change tracking

>[!NOTE]
>
>In the Production environment, Configuration is currently available only as information and cannot be changed. The ability to change which fields are tracked will be available in the near future.

To view the types of changes that are tracked: 

{{step-1-to-setup}}

1. In the left panel, click **Change Tracking > Configuration**.
   
   Fields are displayed grouped by object type.

1. To display fields under a specific object, click the dropdown arrow next to the object type.
-->


## 查看更改历史记录列表

您可以在“设置”区域查看更改历史记录日志。

“更改历史记录列表”是一个增强型列表，具有筛选器、列、行高、日期选取器和搜索栏。

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**更改跟踪>更改历史记录列表**。

   将打开“更改历史记录列表”。

1. 要调整显示更改的日期，请单击日期选取器并选择新日期。

   更改适用于过去90天。

1. 要搜索特定术语，请在搜索框中单击并输入术语。 当您键入时，结果会在列表中加亮。
1. （可选）要按列筛选，请参阅文章[使用增强列表](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)中的[筛选增强列表](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#filter-items-in-an-enhanced-list)中的项。
1. （可选）要隐藏、显示或重新排序列，请参阅文章[使用增强列表](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)中的[自定义列](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#customize-columns)。
1. （可选）要添加或删除列，请参阅[使用增强列表](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)中的使用列管理器[&#128279;](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#add-and-remove-columns-with-the-column-manager)的添加和删除列。
1. （可选）要调整行高，请参阅文章[使用增强列表](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)中的[更改视图中的行高](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#change-the-row-height-in-a-view)。

## 导出更改历史记录

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**更改跟踪>更改历史记录列表**。
1. 筛选列表以显示要导出的项目。
1. 单击&#x200B;**导出**&#x200B;图标![导出图标](assets/export-icon.png)并选择保存为XLSX还是CSV格式。

   这将打开保存文件框，您可以将导出的文件保存在计算机上。
   完成保存导出的文件。您现在可以在计算机上找到该代码并与他人共享。



