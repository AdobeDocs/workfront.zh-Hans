---
product-area: projects
navigation-topic: use-predecessors
title: 强制前置任务
description: 前置任务是指其他任务依赖于完成的任务。 前置任务关系会影响任务的开始和完成日期，并最终影响项目的时间轴。
author: Alina
feature: Work Management
exl-id: c3242b92-9036-4770-a073-2a9c393b97fd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---

# 强制前置任务

前置任务是指其他任务依赖于完成的任务。 前置任务关系会影响任务的开始和完成日期，并最终影响项目的时间轴。

有关前置任务的信息，请参阅 [任务前置任务概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

通过设置任务之间的前置任务关系，您可以定义从属任务的开始或结束取决于其前置任务的开始或结束的方式。 这是通过使用不同的依赖关系类型来完成的。

有关依赖关系类型的信息，请参阅 [任务依赖关系类型概述](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

## 强制前置任务概述

>[!IMPORTANT]
>
>您必须强制前任人员，以要求尊重前任关系。 如果不强制前置任务，则从属任务可以独立于其前置任务的开始和结束，而不管其依赖关系类型。

在项目中设置前置任务时，您可以强制执行前置任务关系。

如果强制执行前任，则在前任完成之前，将无法启动后继任务。 例如，在任务A和任务B之间强制实施“完成 — 开始”关系意味着任务B无法启动（状态必须保持为“新”，而“完成百分比”必须保持为0%），直到任务A标记为已完成。 强制关系适用于所有前置类型。

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
   <td> <p>编辑对任务和项目的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理任务和项目的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 在任务级别执行前置任务

1. 转到要强制执行其前置任务的后续任务。
1. 单击 **前置任务** 在左侧面板中，单击 **添加前置项**. 您可能需要单击 **显示更多**，则 **前置任务**.
1. （视情况而定）如果要添加跨项目前置项，请在 **父项目** 字段，并将其替换为其他项目。
1. 在 **任务** 字段。
1. 指定 **依赖关系类型** 这两个任务之间。

   默认 **依赖关系类型** is **完成开始**.

1. 选择 **强制** 字段来强制使用前置代理。
1. 单击&#x200B;**保存**。

## 在任务列表中强制执行前置任务

1. 转到项目上的任务列表。
1. 从 **查看** 下拉菜单中，选择 **标准视图**.

1. 在心理上记下要指定为前置任务的任务数。
1. 查找要强制执行其前置任务的后续任务。
1. 在 **前置任务** 列中，开始输入前置任务的编号，后跟“e”。 例如，键入“1e”将任务编号1添加为选定任务的前置任务。
1. 单击Enter以保存任务的前置信息。

   ![pricess_enforced_in_list.png](assets/predecessor-enforced-in-list-350x308.png)
