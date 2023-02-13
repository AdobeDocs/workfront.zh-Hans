---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: “过滤器：通过比较两个字段来消除列表中的项目
description: 您可以通过比较列表中的两个字段来筛选项目。 例如，您只能显示任务的实际完成日期大于计划完成日期的任务。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# 过滤器：通过比较两个字段来消除列表中的项目

您可以通过比较列表中的两个字段来筛选项目。 例如，您只能显示任务的实际完成日期大于计划完成日期的任务。

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

## 通过比较两个字段过滤项目

1. 转到任务列表。
1. 从 **过滤器** 下拉菜单，选择 **新建过滤器**.

1. 单击 **添加过滤器规则** 添加 **实际完成日期** >**大于** > **选择日期**.

   >[!TIP]
   >
   >选择要用于选定字段的过滤器修饰符（如果可用）。

1. 单击 **切换到文本模式**.
1. 在 **为报表设置过滤器规则** 区域，添加以下代码：

   ```
   actualCompletionDate=FIELD:plannedCompletionDate<br>actualCompletionDate_Mod=gt
   ```

1. 单击 **完成**，则 **保存过滤器**.
