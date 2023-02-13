---
title: 创建里程碑路径
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: 作为Adobe Workfront管理员，您可以创建里程碑路径，然后将该路径应用于系统中的任何项目。 您对此区域中的里程碑路径所做的更改会影响整个Workfront系统。
author: Alina, Caroline
feature: System Setup and Administration
role: Admin
exl-id: c1e2f374-576c-4f1c-b502-281e8ee9e7df
source-git-commit: fe399743ee495334face9d4d632686d9472bc8ef
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 2%

---

# 创建里程碑路径

<!--
NOTE: DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

作为Adobe Workfront管理员，您可以创建里程碑路径，然后将该路径应用于系统中的任何项目。 您对此区域中的里程碑路径所做的更改会影响整个Workfront系统。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 里程碑和里程碑路径

您可以将项目中的关键任务与预定义里程碑相关联。 这一职能可为管理人员和其他利益攸关方提供关于项目进展情况的高级别概述。

所有预定义里程碑的总和称为里程碑路径。

构建里程碑路径的第一步是确定里程碑步骤和建立里程碑。 由于您可以将一个里程碑路径关联到多个项目，因此，里程碑步骤必须是任何项目的常规阶段或阶段。

有关如何将里程碑路径与项目关联以及将里程碑与任务关联的详细信息，请参阅 [将里程碑与任务关联](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

## 创建里程碑路径

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **流程** > **里程碑路径**.
1. 单击 **新建里程碑路径。**
1. 在 **基本信息** 区域：

   <table style="table-layout:auto">
    <tr>
      <td>创建里程碑路径</td>
       <td>输入里程碑路径的名称。</td>
    </tr>
    <tr>
      <td>描述</td>
      <td>输入描述以定义里程碑路径。</td>
    </tr>
    <tr>
       <td>活动</td>
      <td>如果希望里程碑路径处于活动状态，请选中此复选框。 其他用户在创建或编辑项目时可以找到此路径并将其附加到项目。 不活动的里程碑路径不能附加到项目。 默认情况下，此设置处于启用状态。</td>
    </tr>
    <tr>
      <td>组</td>
      <td>选择列出的组，以允许这些组中的用户查看此里程碑路径并将其应用于其项目。 默认情况下，会选择进入里程碑路径的用户的主组。</td>
    </tr>
   </table>

1. 在 **里程碑** 区域：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">名称</td> 
      <td>为每个里程碑键入描述性名称。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">描述</td> 
      <td>键入里程碑的描述。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">颜色</td> 
      <td> <p>选择要与里程碑关联的颜色。 </p> <p>如果您没有选择颜色，系统将选择里程碑路径中使用的最后一种颜色。 我们建议您为每个里程碑选择唯一的颜色。 颜色用于可视和报告目的。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **添加里程碑** 并继续根据需要添加里程碑，直到路径完成。
1. 单击 **创建里程碑路径** 以保存更改。

   您的里程碑路径已准备好与项目关联。

   有关如何将里程碑路径与项目和里程碑与任务关联的更多信息，请参阅 [将里程碑与任务关联](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).
