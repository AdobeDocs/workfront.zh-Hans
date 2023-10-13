---
product-area: templates
navigation-topic: templates-navigation-topic
title: 复制项目模板
description: 您可以复制现有模板并根据需要进行更改，而不是从头开始创建新项目模板。
author: Alina
feature: Work Management
exl-id: b2e0878b-8245-4e01-819d-c3746f553d95
source-git-commit: e416a23cab139bff6d0d59b3816fb192c8f92b0b
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 3%

---

# 复制项目模板

您可以复制现有模板并根据需要进行更改，而不是从头开始创建新项目模板。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对模板的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看模板或更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。


## 有关复制模板的注意事项

始终将以下项从现有项目复制到新项目：

* 模板任务
* 模板任务默认信息(任务默认审批流程、任务默认自定义Forms)
* 自定义表单
* 风险
* 队列设置信息
* Portfolio和计划
* 审批
* 文档
* 原始模板任务转移到新模板的天数。 如果需要，必须更改模板的“开始”或“完成”日期（取决于其调度模式）以更新模板任务的日期。

绝不会将以下项从现有项目复制到新项目：

* 记帐费率
* 用户评论

## 复制模板

1. 转到要复制的模板。
1. 单击 **更多** 菜单 ![](assets/qs-more-icon-on-an-object.png)，然后单击 **复制**.
1. 在中指定模板的名称 **新模板名称** 字段。

   默认情况下，新名称为 **副本 `<original template name>`.**

1. 选择是否要 **保留任务和模板上的用户工作**：选择此选项以将原始模板中的所有任务和模板分配传送到新模板。
1. 单击 **保存** 创建模板的副本。
