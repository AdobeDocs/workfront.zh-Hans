---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: 复制功能板
description: 您可以复制功能板及其所有内容（报表、日历和外部页面）。 复制功能板的内容时，您可以选择保留它们在原始功能板上显示时的内容，或创建新项目，这些项目是原始功能板上这些内容的副本。 您还可以选择不转移或复制新功能板上的项目。
author: Nolan
feature: Reports and Dashboards
exl-id: a88cc171-2bb1-40f0-a778-8dac7eecb718
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# 复制功能板

您可以复制功能板及其所有内容（报表、日历和外部页面）。 复制功能板的内容时，您可以选择保留它们在原始功能板上显示时的内容，或创建新项目，这些项目是原始功能板上这些内容的副本。 您还可以选择不转移或复制新功能板上的项目。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront计划*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront许可证*</strong></td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>编辑对报表、功能板和日历的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>查看对功能板的访问</p> <p>您将获得对复制的功能板的管理访问权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 先决条件

您必须先创建功能板，然后才能复制它。

有关创建功能板的信息，请参阅 [创建功能板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## 复制功能板

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png)，然后单击 **功能板**.

1. 选择要复制的功能板，然后单击 **复制** ![](assets/copy-icon.png).\
   或\
   打开要复制的功能板，然后单击 **功能板操作** > **复制**.\
   此时将显示“功能板复制”对话框。 将显示原始功能板上的所有项目。

1. 在 **功能板名称** 字段，为功能板指定新名称。
1. 要选择现有功能板上的所有项目并将其复制到复制的功能板，请保留 **全选** 选项。 默认情况下，现有功能板上的报表、日历或列表将会复制到新功能板。\
   或\
   要仅将特定项目从原始功能板转移到新功能板，请取消选择您不希望在新功能板中显示的项目，然后针对每个选定项目，从以下选项中进行选择：

   * **制作副本：** 项目将从原始功能板复制，并且该项目的新版本将显示在新功能板中。 对新功能板上的项目所做的更改不会反映在原始功能板上的项目中。 同样，对原始功能板上的项目所做的更改也不会反映在新功能板上的项目中。\
      当您想要修改原始功能板上的原始报表时，请使用此选项。\
      例如，复制名为“Team B”的功能板，并将其重命名为“Team A”。 在“团队B”功能板中，有一个名为“团队B报表”的报表。 由于此报表包含特定于B团队的数据，因此您可以选择选项以复制此报表，以便您可以为A团队自定义此报表，并稍后将其重命名为“A团队报表”。\
      通过此选项，您可以从复制的报表中删除原始报表的共享权限。 在复制的报表中，运行此报表时其信息的访问权限将保持不变。

   * **使用原始：** 显示新功能板上的原始项目。 对新功能板上的项目所做的更改也会反映在原始功能板上的项目中。 同样，对原始功能板上的项目所做的更改也会反映在新功能板上的项目中。\
      通过此选项，您可以保留原始报表的共享权限。 使用信息的访问权限运行此报表也将保持不变。

1. （可选）重命名您选择的任何项目。
1. 单击 **复制功能板**.
1. （可选）如果要编辑复制的功能板中任何复制的报表、日历和外部页面，请执行以下任一操作：

   * 要编辑任何已复制报表的任何信息，请单击功能板上的报表名称，然后 **报表操作** > **编辑**.

      例如，您可能想要编辑视图、过滤器、分组、提示或图表或复制的报表。

   * 要恢复已复制报表的权限，请在新功能板中单击报表名称，然后单击 **报表操作** > **共享** 和更新报表的权限。

      在复制功能板时复制报表时，该报表的权限会被删除。

   * 要修改使用信息的访问权限运行此报表，请在新功能板中单击报表名称，然后 **报表操作** > **编辑** > **报表选项**.\
      复制报表后，仅在以下情况下才维护使用权限运行此报表：

      （如果这些条件均不满足，则删除具有权限的访问权限运行此报表，并且新的具有访问权限的运行此报表将更改为创建复制报表的用户。）

      如果复制功能板及其报表的用户具有管理员权限。

      * 如果复制功能板及其报表的用户具有管理员权限。
      * 如果复制功能板及其报表的用户当前设置为运行此报表，且其访问权限为要复制的报表。
      * 如果复制报表的用户具有对报表的管理权限。
