---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '分组：项目百分比细分2'
description: '''在此自定义项目分组中，您可以显示按项目完成百分比值范围分组的项目。 细分显示完成百分比值10%点增量：0-10%、11-20%、21-30%等。'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7845fd66-8304-4154-8630-e72482cd753f
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 0%

---

# 分组：项目百分比细分2

在此自定义项目分组中，您可以显示按项目完成百分比值范围分组的项目。 细分显示完成百分比值10%点增量：0-10%、11-20%、21-30%等。

以下分组按完成百分比值将项目组织为以下分组之一：

* 0%
* 1-10%
* 11-20%
* 21-30%
* 31-40%
* 41-50%
* 51-60%
* 61-70%
* 71-80%
* 81-90%
* 91-99%
* 100%

![percent_complete_breakdown_for_projects_in_10__increments.png](assets/percent-complete-breakdown-350x94.png)

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>请求修改分组 </p>
   <p>计划修改报告</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限以修改报告</p> <p>编辑对筛选器、视图和分组的访问权限以修改分组</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 按项目百分比细分分组

要应用此分组，请执行以下操作：

1. 转到项目列表。
1. 从&#x200B;**分组**&#x200B;下拉菜单中，选择&#x200B;**新建分组**。

1. 单击&#x200B;**切换到文本模式**。
1. 移除框中的文本，并将以下代码粘贴到可用空间中：
   <pre>group.0.linkedname=direct<br>group.0.name=Percent Breakdown<br>group.0.notime=false<br>group.0.valueexpression=IF({percentComplete}=0，"0 %"，IF({percentComplete}&lt;=11，"1-10 %"，IF({percentComplete}&lt;=21，"11-20 %"，IF({percentComplete}&lt;=31，"21-30 %"，IF({percentComplete}&lt;41，"31-40 %"，IF( 8}&lt;51，"41-50 %"，IF({percentComplete}&lt;61，"51-60 %"，IF({percentComplete}&lt;71，"61-70 %"，IF({percentComplete}&lt;81，"71-80 %"，IF({percentComplete}&lt;91，"81-90 %"，IF({percentComplete}&lt;100，"91-99 %"，"100 %"))))))))))<br>textmode=true{percentComplete}</pre>

1. 单击&#x200B;**保存分组**。
