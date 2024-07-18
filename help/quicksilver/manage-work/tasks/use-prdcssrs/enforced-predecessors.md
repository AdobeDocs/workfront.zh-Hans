---
product-area: projects
navigation-topic: use-predecessors
title: 强制前置任务
description: 前置任务是指其他任务需要完成才能执行的任务。 前置任务关系影响任务的开始和完成日期，并最终影响项目的时间表。
author: Alina
feature: Work Management
exl-id: c3242b92-9036-4770-a073-2a9c393b97fd
source-git-commit: 5cb07cb42c3264c6629bc0a038c0e70ffc2cb509
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# 强制前置任务

<!-- Audited: 2/2024 -->

前置任务是指其他任务需要完成才能执行的任务。 前置任务关系影响任务的开始和完成日期，并最终影响项目的时间表。

有关前置任务的信息，请参阅[前置任务概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)。

通过设置任务之间的前置任务关系，可以定义相关任务的开始或完成如何取决于其前置任务的开始或完成。 这是通过使用不同的依赖关系类型来实现的。

有关依赖关系类型的信息，请参阅[任务依赖关系类型概述](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)。

## 已强制实施的前置任务概述

>[!IMPORTANT]
>
>您必须强制前置任务，以要求前置任务关系必须得到遵守。 如果不强制实施前置任务，则相关任务可以独立于其前置任务的开始和结束而开始和完成，而不管其依赖关系类型如何。

在项目中设置前置任务时，您可以强制实施前置任务关系。

如果前置任务被强制执行，则前置任务不能在前置任务完成之前开始。 例如，在任务A和任务B之间强制实施“完成 — 开始”关系意味着在任务A标记为完成之前，任务B无法开始（“状态”必须保持为“新”，“完成百分比”必须保持为0%）。 强制关系适用于所有前置任务类型。

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
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>
      <p>新增：标准</p> 
      <p>或</p>
      <p>当前：计划</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对任务和项目的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td><p>管理任务和项目的权限</p></td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在任务级别强制前置任务

1. 转至要强制其前置任务的后续任务。
1. 单击左侧面板中的&#x200B;**前置任务**，然后单击&#x200B;**添加前置任务**。 您可能需要单击&#x200B;**显示更多**，然后单击&#x200B;**前置任务**。
1. （视情况而定）如果要添加跨项目前置任务，请在&#x200B;**父项目**&#x200B;字段中移除项目的名称，并将其替换为其他项目。
1. 在&#x200B;**任务**&#x200B;字段中指定前置任务的名称。
1. 指定这两个任务之间的&#x200B;**依赖关系类型**。

   默认&#x200B;**依赖项类型**&#x200B;为&#x200B;**Finish-Start**。

1. 选择&#x200B;**强制**&#x200B;字段以强制前置任务。
1. 单击&#x200B;**保存**。

## 在任务列表中强制前置任务

1. 转到项目上的任务列表。
1. 从&#x200B;**视图**&#x200B;下拉菜单中选择&#x200B;**标准视图**。

1. 在脑海中记下要指定为前置任务的任务数。
1. 查找要执行其前置任务的后续任务。
1. 在&#x200B;**前置任务**&#x200B;列中，开始输入前置任务的编号，然后输入“e”。 例如，键入“1e”将任务编号1作为前置任务添加到所选任务。
1. 单击Enter保存任务的前置任务信息。

   ![前置任务_强制_in_list.png](assets/predecessor-enforced-in-list-350x308.png)
