---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: “分组：“Portfolio责任人”、“项目责任人”、“项目责任人”和“项目状态”的4层任务分组
description: 此任务分组提供4个分组级别。 在这种情况下，任务按“Portfolio所有者”、“项目所有者”、“项目所有者”和“项目状态”进行分组。 使用标准界面最多只能有3个级别的“分组”。 要添加第四级，必须使用文本模式。 不能同时按4个以上的标准对报表进行分组。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a1780a57-b94c-4d3a-b526-9bf45dba21f1
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---

# 分组：Portfolio责任人、项目责任人、项目责任人和项目状态的4层任务分组

此任务分组提供4个分组级别。 在这种情况下，任务按“Portfolio所有者”、“项目所有者”、“项目所有者”和“项目状态”进行分组。 使用标准界面最多只能有3个级别的“分组”。 要添加第四级，必须使用文本模式。 不能同时按4个以上的标准对报表进行分组。

![four_tier_grouping_for_tasks.png](assets/four-tier-grouping-for-tasks-350x239.png)

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报表、功能板、日历的访问</p> <p>编辑对过滤器、视图、分组的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 为Portfolio责任人、项目责任人、项目责任人和项目状态创建4层任务分组

要应用此分组，请执行以下操作：

1. 转到任务列表。
1. 从 **分组** 下拉菜单，选择 **新建分组**.

1. 单击&#x200B;**切换到文本模式**.
1. 删除 **对报表进行分组** 的上界。
1. 将文本替换为以下代码：

   <pre>group.0.linkedname=project<br>group.0.name=Portfolio所有者<br>group.0.notime=false<br>group.0.valuefield=project:portfolio:owner:name<br>group.0.valueformat=string<br>group.1.linkedname=project<br>group.1.name=程序所有者<br>group.1.notime=false<br>group.1.valuefield=project:program:owner:name<br>group.1.valueformat=string<br>group.2.linkedname=projectOwnerMM<br>group.2.listgroupingparsedmethod=nested(project)。nested(owner)。string(name)<br>group.2.namekey=projectownermm<br>group.2.notime=false<br>group.2.valuefield=projectOwnerMM:name<br>group.2.valueformat=string<br>group.3.enumclass=com.attask.common.constants.ProjectStatusEnum<br>group.3.linkedname=project<br>group.3.namekey=view.relatedcolumn<br>group.3.namekeyargkey.0=project<br>group.3.namekeyargkey.1=status<br>group.3.notime=false<br>group.3.valuefield=project:status<br>group.3.valueformat=val</pre>

1. 单击 **保存分组**.
