---
product-area: projects
navigation-topic: create-tasks
title: 在项目中创建任务
description: 只有在创建项目后，您才能在项目中创建任务。
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 96f80e7b-6ad5-40ae-861d-8d97c570f2ac
source-git-commit: c593eab154a0942995b1f913e7189450913faac0
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 1%

---

# 在项目中创建任务

<!-- Audited: 1/2024 -->

只有在创建项目后，您才能在项目中创建任务。

例如，在创建项目后，您可能需要添加任务并修改这些任务以组织项目计划。 有关创建项目的详细信息，请参阅 [创建项目](../../../manage-work/projects/create-projects/create-project.md).

有关创建不在项目中的个人任务的信息，请参阅 [创建个人任务](../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-personal-task) 部分内容 [从主页区域创建工作项](../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

本文介绍了如何从头开始创建任务。 您还可以通过以下方式创建任务：

* 通过复制或复制现有任务。 有关信息，请参阅 [复制和复制任务](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).
* 通过将任务从一个项目移动到另一个项目。 有关信息，请参阅 [移动任务](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## 访问要求

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Adobe Workfront许可证</p> </td> 
   <td><p>当前：工作或更高</p> 
   或
   <p>新增：标准</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对任务和项目的访问权限</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>将权限分配给能够添加任务或更高权限的项目</p> <p>创建任务时，您会自动收到该任务的“管理”权限</p> <p> 有关任务权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">共享任务 </a>. </p> <p>有关请求其他权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 在项目中创建任务

1. 转到要创建任务的项目。
1. 单击 **任务** 在左侧面板中。
1. （视情况而定）如果您当前正以Agile视图查看任务列表，请单击 **列表视图** 图标 ![](assets/list-view-in-agile-view-for-tasks.png) 图标，以显示任务列表。
1. （可选）单击 **计划模式** 图标 ![](assets/nwe-plan-mode-icon-task-list.png) 并选择 **手动保存**，然后选择 **标准** 或 **时间线规划**. 这将禁用 **自动保存** 选项，默认情况下会启用此选项。

   ![选择手动保存](assets/manual-save-option.png)

   >[!TIP]
   >
   >选择“手动保存”后，您可以撤消所做的更改。

1. 通过执行以下操作之一创建新任务：

   * 单击 **新建任务** 在任务列表的顶部。
   * 单击 **添加更多任务** 位于任务列表底部。

   ![](assets/qs-new-task-or-add-task-buttons-in-list-highlighted-350x242.png)

1. （视情况而定）如果您单击 **新建任务** 执行以下操作：

   1. 在有限字段列表中，指定任意字段 **新建任务** 框，然后单击 **创建任务** 如果您想要快速创建任务。

      或

      要更新任务的所有字段，请单击 **更多选项** 以打开 **创建任务** 盒子。

      ![](assets/nwe-create-task-small-screen-350x272.png)

      此 **创建任务** 框打开。

      ![](assets/create-task-larger-box-nwe-350x244.png)

       

      >[!NOTE]
      >
      >根据Workfront管理员如何设置布局模板，创建任务框中的字段可能会显示您环境中的不同字段。 有关信息，请参阅 [使用布局模板自定义详细信息视图](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   1. 在“创建任务”框的左侧面板中指定以下区域的信息：

      * 任务名称
      * 概述
      * 分配
      * 自定义表单
      * 财务
      * 设置

        有关定义任务中所有与任务相关的字段的信息，请参阅 [编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

   1. （有条件，可选）如果您希望任务定期执行，请更新 **周期性频率** 字段。 有关创建周期性任务的详细信息，请参阅 [创建周期性任务](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md).
   1. （可选）单击 **文档** 在左侧面板中将文档附加到新任务，然后单击 **添加或链接文件** 将文档从您的计算机或其他服务添加到任务中，或者从您的计算机或其他服务链接文档和文件夹。

1. （视情况而定）如果您单击 **添加更多任务** 在步骤5中，开始使用内联编辑输入任务信息，然后按Enter键。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this stays accurate)</p>
   -->

   我们建议使用此选项，尤其是在将多个任务添加到列表时。

   ![](assets/add-more-tasks-inline.png)

1. （视情况而定）执行以下操作之一：

   * 如果您单击 **新建任务** 在步骤5中，单击 **创建任务** 以保存所做更改并将新任务添加到项目中。

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?)</p>   
     -->

   * 如果您单击 **添加更多任务** 在步骤5中，执行以下操作：

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?) </p>   
     -->

      1. 单击浏览器中的任意位置以提交更改，或按Enter。
      1. （可选）在任务列表中，选择新创建的任务，然后单击 **缩进**.

         这使新任务成为上一个任务的子任务或子任务。

         有关子任务的详细信息，请参阅 [创建子任务](/help/quicksilver/manage-work/tasks/create-tasks/create-subtasks.md).

      1. （视情况而定）如果您已禁用 **自动保存** 选项（按下） **添加更多任务**，您可以执行以下操作：

         * 单击 **还原** 随时撤消上次更改，或 **取消** 以撤消您对任务列表所做的所有更改。
         * 如果您之前已单击 **还原**，单击 **重做** 以重新应用您取消的上次更改。
         * 单击 **保存** 以保存对任务列表所做的更改。
