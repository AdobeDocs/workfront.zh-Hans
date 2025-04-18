---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 筛选器：显示计划提交的报表
description: 此报表过滤器显示所有计划在Adobe Workfront中自动交付的报表。 最好将其用于标准视图。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7b937384-80c9-4bc7-94be-5573cf86b35b
source-git-commit: e8acdf8f7b3859385237e788dfda34ee62ee11d1
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---

# 筛选器：显示计划提交的报表

<!--Audited: 10/2024-->

此报表过滤器显示所有计划在Adobe Workfront中自动交付的报表。 最好将其用于标准视图。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> 
    <p>新增：</p>
   <ul><li><p>修改过滤器的参与者 </p></li>
   <li><p>用于修改报告的标准</p></li> </ul>

<p>当前：</p>
   <ul><li><p>请求修改筛选器 </p></li>
   <li><p>计划修改报告</p></li> </ul></td> 
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

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 报告投放过滤器

要应用此过滤器，请执行以下操作：

1. 转到报告列表。

1. 从&#x200B;**筛选器**&#x200B;下拉菜单中，选择&#x200B;**新建筛选器**。

1. 单击&#x200B;**切换到文本模式**。

1. 在&#x200B;**为报表**&#x200B;设置筛选规则区域中，复制并粘贴以下代码：

   ```
   scheduledReportID=0
   scheduledReportID_Mod=notnull
   ```

1. 单击&#x200B;**保存筛选器**。
