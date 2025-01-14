---
product-area: projects
navigation-topic: create-tasks
title: 在项目中创建任务
description: 只有在创建项目后，您才能在项目中创建任务。
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 96f80e7b-6ad5-40ae-861d-8d97c570f2ac
source-git-commit: 00e58ea9a207037b701e1be010c2c4c2995d60e0
workflow-type: tm+mt
source-wordcount: '959'
ht-degree: 1%

---

# 在项目中创建任务

<!-- Audited: 10/2024 -->

您可以通过以下方式在Adobe Workfront中创建任务：

* 创建项目后，在项目中从头开始创建任务。

  创建项目后，您可以添加并修改任务以组织项目计划。 有关创建项目的详细信息，请参阅[创建项目](../../../manage-work/projects/create-projects/create-project.md)。

* 通过将模板添加到项目来创建任务。

  有关信息，请参阅[将模板附加到项目](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md)。

* 创建个人任务并将其移动到项目。

  您可以通过执行以下操作之一来创建个人任务：

   * 创建临时工作请求并将其发送给用户
   * 在“主页”区域创建待办事项

  有关创建不在项目中的个人任务的信息，请参阅[创建个人任务](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/create-personal-tasks.md)。

  您可以将个人任务移动到项目，这些任务会成为工作任务。

本文介绍了如何从头开始创建任务以及如何将个人任务移动到项目。

您还可以通过以下方式创建任务：

* 通过复制或复制现有任务。 有关信息，请参阅[复制和复制任务](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)。
* 通过将任务从一个项目移动到另一个项目。 有关信息，请参阅[移动任务](../../../manage-work/tasks/manage-tasks/move-tasks.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

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
   <td> <p>Contribute对项目的权限可添加任务或更高版本</p> <p>创建任务时，您会自动收到该任务的“管理”权限</p> <p> 有关任务权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">共享任务</a>。 </p> <p>有关请求其他权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在项目中创建任务

1. 转到要创建任务的项目。
1. 单击左侧面板中的&#x200B;**任务**。
1. （视情况而定）如果您当前在Agile视图中查看任务列表，请单击右上角的&#x200B;**列表视图**&#x200B;图标![](assets/list-view-in-agile-view-for-tasks.png)以显示任务列表。
1. （可选）单击&#x200B;**计划模式**&#x200B;图标![](assets/nwe-plan-mode-icon-task-list.png)并选择&#x200B;**手动保存**，然后选择&#x200B;**标准**&#x200B;或&#x200B;**时间表计划**。 这将禁用默认启用的&#x200B;**自动保存**&#x200B;选项。

   ![选择手动保存](assets/manual-save-option.png)

   >[!TIP]
   >
   >选择“手动保存”后，您可以撤消所做的更改。

1. 通过执行以下操作之一创建新任务：

   * 单击任务列表顶部的&#x200B;**新建任务**。
   * 单击任务列表底部的&#x200B;**添加更多任务**。

   ![](assets/qs-new-task-or-add-task-buttons-in-list-highlighted-350x242.png)

1. （视情况而定）如果您单击&#x200B;**新建任务**，请执行以下操作：

   1. 在&#x200B;**新建任务**&#x200B;框内的有限字段列表中指定任意字段，如果要快速创建任务，请单击&#x200B;**创建任务**。

      或

      要更新任务的所有字段，请单击&#x200B;**更多选项**&#x200B;以打开&#x200B;**创建任务**&#x200B;框。

      ![](assets/nwe-create-task-small-screen-350x272.png)

      将打开&#x200B;**创建任务**&#x200B;框。

      ![](assets/create-task-larger-box-nwe-350x244.png)

       

      >[!NOTE]
      >
      >根据Workfront管理员如何设置布局模板，创建任务框中的字段可能会显示您环境中的不同字段。 有关信息，请参阅[使用布局模板自定义详细信息视图](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)。

   1. 在“创建任务”框的左侧面板中指定以下区域的信息：

      * 任务名称
      * 概述
      * 任务
      * 自定义表单
      * 财务
      * 设置

        有关定义任务中所有任务相关字段的信息，请参阅[编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md)。

   1. （有条件，可选）如果希望任务为周期性任务，请更新&#x200B;**周期性频率**&#x200B;字段。 有关创建周期性任务的详细信息，请参阅[创建周期性任务](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md)。
   1. （可选）单击左侧面板中的&#x200B;**文档**&#x200B;以将文档附加到新任务，然后单击&#x200B;**添加或链接文件**&#x200B;以将文档从您的计算机或其他服务添加到任务，或者从您的计算机或其他服务链接文档和文件夹。

1. （视情况而定）如果您在步骤5中单击了&#x200B;**添加更多任务**，请开始使用内联编辑输入任务信息，然后按Enter。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this stays accurate)</p>
   -->

   我们建议使用此选项，尤其是在将多个任务添加到列表时。

   ![](assets/add-more-tasks-inline.png)

1. （视情况而定）执行以下操作之一：

   * 如果您在步骤5中单击了&#x200B;**新建任务**，请单击&#x200B;**创建任务**&#x200B;以保存您的更改并将新任务添加到您的项目中。

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?)</p>   
     -->

   * 如果您在步骤5中单击了&#x200B;**添加更多任务**，请执行以下操作：

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?) </p>   
     -->

      1. 单击浏览器中的任意位置以提交更改，或按Enter。
      1. （可选）在任务列表中，选择新创建的任务，然后单击&#x200B;**缩进**。

         这使新任务成为上一个任务的子任务或子任务。

         有关子任务的详细信息，请参阅[创建子任务](/help/quicksilver/manage-work/tasks/create-tasks/create-subtasks.md)。

      1. （视情况而定）如果在按&#x200B;**添加更多任务**&#x200B;后禁用了&#x200B;**自动保存**&#x200B;选项，则可以执行以下操作：

         * 随时单击&#x200B;**撤消**&#x200B;可撤消您上次所做的更改，或者单击&#x200B;**取消**&#x200B;可撤消您对任务列表所做的所有更改。
         * 如果您之前单击了&#x200B;**撤消**，请单击&#x200B;**重做**&#x200B;以重新应用您取消的上次更改。
         * 单击&#x200B;**保存**&#x200B;以保存对任务列表所做的更改。

## 通过将个人任务移动到项目来创建任务

1. （视情况而定）确保您或其他用户已创建个人任务。

   有关信息，请参阅[创建个人任务](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/create-personal-tasks.md)。
1. 创建个人任务筛选器并将其应用于任务报告或列表。

   有关信息，请参阅[筛选器：个人任务](/help/quicksilver/reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-personal-tasks.md)。

   ![](assets/personal-tasks-report.png)
1. 单击个人任务报告中的任务名称以将其打开。

   Workfront将个人任务保存在未列出的个人项目中，该项目始终按以下模式命名：“&lt;用户全名>”任务。 例如，可以将个人项目命名为“Rick&#39;s Tasks”。

1. 在任务页面中，单击&#x200B;**更多菜单** ![](assets/more-icon.png)，然后单击&#x200B;**移动**。 有关移动任务的详细信息，请参阅[移动任务](/help/quicksilver/manage-work/tasks/manage-tasks/move-tasks.md)。

   移动完任务后，该任务将显示在您选择的项目上。 项目时间表可能受新任务时间表的影响。
