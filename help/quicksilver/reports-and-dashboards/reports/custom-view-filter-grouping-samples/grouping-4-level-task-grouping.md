---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '分组：针对Portfolio所有者、项目群所有者、项目所有者和项目状态的4层任务分组'
description: 此任务分组提供4个级别的分组。 在这种情况下，任务按Portfolio所有者、项目群所有者、项目所有者和项目状态分组。 使用标准界面时，您最多只能有3个级别的分组。 要添加第四级，必须使用文本模式。 您不能同时按4个以上的标准对报表进行分组。
author: Nolan
feature: Reports and Dashboards
exl-id: a1780a57-b94c-4d3a-b526-9bf45dba21f1
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---

# 分组：Portfolio责任人、方案责任人、项目责任人和项目状态的4层任务分组

<!--Audited: 10/2024-->

此任务分组提供4个级别的分组。 在这种情况下，任务按Portfolio所有者、项目群所有者、项目所有者和项目状态分组。 使用标准界面时，您最多只能有3个级别的分组。 要添加第四级，必须使用文本模式。 您不能同时按4个以上的标准对报表进行分组。

![four_tier_grouping_for_tasks.png](assets/four-tier-grouping-for-tasks-350x239.png)

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

## 为Portfolio所有者、项目群所有者、项目所有者和项目状态创建4层任务分组

要应用此分组，请执行以下操作：

1. 转到任务列表。
1. 从&#x200B;**分组**&#x200B;下拉菜单中，选择&#x200B;**新建分组**。

1. 单击&#x200B;**切换到文本模式**。
1. 删除&#x200B;**对您的报告分组**&#x200B;区域中的文本。
1. 将显示的框中的文本替换为以下代码：
   <pre>group.0.linkedname=project<br>group.0.name=Portfolio所有者<br>group.0.notime=false<br>group.0.valuefield=project:portfolio:所有者：name<br>group.0.valueformat=string<br>group.1.linkedname=project<br>group.1.name=项目所有者<br>group.1.notime=false<br>group.1.valuefield=project:program:所有者：name<br>group.1.valueformat=string<br>group.2.linkedname=projectOwnerMM <br>group.2.listgrouingparsedmethod=nested(project)。nested(owner)。string(name)<br>group.2.namekey=projectownermm<br>group.2.notime=false<br>group.2.valuefield=projectOwnerMM：name<br>group.2.valueformat=string<br>group.3.enumclass=com.attask.common.constants.ProjectStatusEnum<br>group.3.linkedname=project<br>group.3.group.3 namekey=view.relatedcolumn<br>group.3.namekeyargkey.0=project<br>group.3.namekeyargkey.1=status<br>group.3.notime=false<br>group.3.valuefield=project：status<br>group.3.valueformat=val</pre>

1. 单击&#x200B;**完成**，然后单击&#x200B;**保存分组**。
1. （可选）更新分组的名称，然后单击&#x200B;**保存分组**。
