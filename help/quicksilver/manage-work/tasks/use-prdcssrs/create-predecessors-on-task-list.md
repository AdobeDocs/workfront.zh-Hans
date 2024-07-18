---
product-area: projects
navigation-topic: use-predecessors
title: 在任务列表上创建前置任务关系
description: 您可以使用前置任务（或只是前置任务）来链接依赖其他任务启动或完成的任务。 例如，在发出邀请（前置任务）之前，您不希望主持某方（依赖任务）。
author: Alina
feature: Work Management
exl-id: a84d88ac-8dd4-4952-b83f-02fafa61e68b
source-git-commit: 811eb1453c140808b0d6c5d9a3b4a0729cb16b2d
workflow-type: tm+mt
source-wordcount: '720'
ht-degree: 0%

---

# 在任务列表上创建前置任务关系

您可以使用前置任务（或只是前置任务）来链接依赖其他任务启动或完成的任务。 例如，在发出邀请（前置任务）之前，您不希望主持某方（依赖任务）。

本文说明如何在任务列表中创建前置任务。

您可以在Adobe Workfront的以下区域中查看任务的前置任务：

* 在“前置任务”列的任务列表中。
* 在甘特图中
* 在相关任务的“前置任务”部分中

有关详细信息，请参阅[前置任务概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)。

## 访问要求

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
   <td> <p>新增：标准 </p><p>当前：计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对任务和项目的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理任务和项目的权限</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。 有关访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## 创建前置任务

1. 转到项目。
1. 单击左侧面板中的&#x200B;**任务**。
1. 确保当前视图显示&#x200B;**前置任务**&#x200B;列。

   如果该视图不显示“前置任务”列，请更改为显示前置任务的视图，或将该列添加到视图中。

1. 选择要指定为从属任务的任务。
1. 单击&#x200B;**前置任务**&#x200B;列中的。
1. 键入要指定为选定任务的前置任务的任务编号，然后按&#x200B;**Enter**。

   >[!TIP]
   >
   >要添加跨项目前置任务，请执行以下操作：
   >
   >1. 单击&#x200B;**计划模式**&#x200B;图标，然后选择&#x200B;**自动保存**。
   >
   >1. 键入前置任务项目的参考编号，后跟冒号和任务的编号。 例如，键入：765021：12。 这表示前置任务项目的参考号为765021，并且前置任务是项目中的任务编号12。
   >
   >1. 为此前置任务添加依赖关系类型。 有关详细信息，请参阅[创建跨项目前置任务](/help/quicksilver/manage-work/tasks/use-prdcssrs/cross-project-predecessors.md)。
   >
   >按&#x200B;**Enter**。
   >
   >**重要信息**
   >
   >当任务列表以手动保存模式显示时，您无法添加跨项目前置任务。

   将前置任务标记为完成时，前置任务图标会变为绿色。 这表示依赖任务已准备好工作。

   有关“前置任务”列中可用的关系类型的详细信息，请参阅[任务前置任务概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)中的[任务前置任务概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)。

## 查看前置任务详细信息

您可以从任务列表中快速查看有关前置任务的详细信息。

1. 在任务列表中，将鼠标悬停在&#x200B;**前置任务**&#x200B;列中的前置任务编号上。

   此时将显示一个包含前置任务详细信息的框。

   ![前置任务详细信息](assets/predecessor-details-in-task-list.png)

   将显示以下详细信息：

   **前置任务名称：**&#x200B;正在引用的前置任务名称。 包括前置任务的任务编号。 单击任务名称以将其打开。 在上例中，前置任务为“生产”/“执行”/“交付”。

   **项目名称：**&#x200B;前置任务所在项目的名称。 如果前置任务属于与任务相同的项目，则项目被标识为当前项目；如果前置任务属于不同的项目，则项目被标识为跨项目。 在上例中，项目名称为Digital Asset Production (Integrated) - Project。 有关跨项目前置任务的详细信息，请参阅[创建跨项目前置任务](../../tasks/use-prdcssrs/cross-project-predecessors.md)。

   您可以展开项目详细信息以查看项目的计划开始和结束日期、条件、状态、完成百分比和所有者。 对于跨项目，您可以单击&#x200B;**查看项目**&#x200B;以打开该项目。

   **ID：**&#x200B;前置任务所在项目的参考编号。

   **计划开始日期：**&#x200B;前置任务的计划开始日期。

   **计划结束：**&#x200B;前置任务的计划完成日期。

   **前置任务数：**&#x200B;被引用的前置任务的前置任务数。 在上例中，被引用的前置任务有1个前置任务。

   **后置任务数：**&#x200B;被引用的前置任务的后置任务（或依赖任务）数。 在上例中，被引用的前置任务有1个后置任务。
