---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 分组：项目发起人的小时数
description: 此小时分组按记录小时数的项目发起人组织小时数。 用于小时分组的标准Report Builder界面不提供到项目发起人字段的映射。 必须使用文本模式界面来访问此字段。
author: Nolan
feature: Reports and Dashboards
exl-id: 6b35b0ef-18b7-4121-ae39-d7957d76c04b
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# 分组：项目发起人的小时数

<!--Audited: 10/2024-->

此小时分组按记录小时数的项目发起人组织小时数。 用于小时分组的标准Report Builder界面不提供到项目发起人字段的映射。 必须使用文本模式界面来访问此字段。

![hour_report_grouped_by_sponner.png](assets/hour-report-grouped-by-sponsor-350x39.png)

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>修改过滤器的参与者或请求 </p>
   <p>用于修改报告的标准或计划</p>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限以修改报告</p> <p>编辑对筛选器、视图和分组的访问权限以修改筛选器</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p>  </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 按项目发起人分组小时数

要应用此分组，请执行以下操作：

1. 转到小时列表。
1. 从&#x200B;**分组**&#x200B;下拉菜单中，选择&#x200B;**新建分组**。

1. 单击&#x200B;**切换到文本模式**。
1. 移除所显示区域中的文本，然后使用以下代码替换该文本：

```
   group.0.linkedname=project:sponsor:name
   group.0.name=
   group.0.valuefield=project:sponsor:name
   group.0.valueformat=HTML
   textmode=true
```

1. 单击&#x200B;**完成**。
1. 更新分组名称，然后单击&#x200B;**保存分组**。
