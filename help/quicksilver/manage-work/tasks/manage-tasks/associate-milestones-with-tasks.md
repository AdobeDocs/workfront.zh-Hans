---
product-area: projects
navigation-topic: manage-tasks
title: 将里程碑与任务关联
description: 您可以将里程碑与任务关联，以指示在项目生命周期中何时达到重要步骤。 必须先将里程碑路径与项目关联，然后才能将里程碑与项目中的任务关联。
author: Alina
feature: Work Management
exl-id: 56410640-fde4-417f-8ea0-f089315476f7
source-git-commit: cf044c8cff6b1172ec460ae232cd07c9b7c808b7
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---

# 将里程碑与任务关联

<!--Audited: 01/2024-->

您可以将里程碑与任务关联，以指示在项目生命周期中何时达到重要步骤。

## 访问要求

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
   <td> <p>新许可证： Standard</p> 
   <p>当前许可证：工作或更高</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑任务访问权限</p> <p><b>注释</b>

如果您没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理任务的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

在将里程碑与任务关联之前，必须存在以下各项：

* Workfront管理员必须创建里程碑路径，如中所述 [创建里程碑路径](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).

* 您必须将里程碑路径关联到项目。

  有关信息，请参阅 [编辑项目](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

* 要将里程碑路径与项目关联，项目必须处于“计划”或“当前”状态。

  >[!TIP]
  >
  >要使用里程碑视图最好地了解项目中里程碑的进度，您应该创建父任务并将它们与项目的每个主要阶段关联。 然后，将这些父任务与里程碑路径的每个里程碑相关联。

## 将里程碑与任务关联

将里程碑路径与项目关联后，可以为任务分配里程碑。

1. 转到任务，然后单击 **更多** 图标 ![](assets/more-icon.png) 任务名称的右侧，然后 **编辑**.

   任务和里程碑之间有1:1的关系。 您不能将同一里程碑附加到多个任务。 每个任务都可以链接到单个里程碑，或者每个里程碑都可以映射到一项任务。

1. 单击 **设置**，然后在中选择里程碑 **里程碑** 任务的字段。
1. 单击&#x200B;**保存**。
1. （可选）在任务列表中，添加 **状态图标** 列，用于标识哪些任务具有里程碑。 里程碑菱形指示符显示在状态图标列中。

   有关信息，请参阅 [在Adobe Workfront中创建或编辑视图](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

   ![](assets/amwt3.png)

1. （可选）转到项目列表，选择 **里程碑** 视图以确定里程碑任务的进度。

   ![](assets/milestone-view-project-list.png)
