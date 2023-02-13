---
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: 使用自定义状态作为默认状态
description: 将自定义状态设置为默认状态时，系统会以各种方式使用新的默认状态。 其使用方式取决于它是设置为默认系统级别状态还是默认组级别状态。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5b137cee-e03a-4176-a683-b77f2b27f5ce
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '833'
ht-degree: 0%

---

# 使用自定义状态作为默认状态

将自定义状态设置为默认状态时，系统会以各种方式使用新的默认状态。 其使用方式取决于它是设置为默认系统级别状态还是默认组级别状态。

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

## 自定义默认系统级别状态

将自定义状态设置为默认系统状态时，系统中创建的任何新组都会继承该状态。

设置新的默认系统状态时已存在的组不会自动继承它。

例如，假设已在您的Adobe Workfront环境中创建了两个组（营销和销售）。 您可以创建一个等于“当前”的新自定义状态，并调用“正在处理”状态。 您现在可以创建一个名为“工程”的新组。 在此方案中，工程组会继承新的默认状态；营销组和销售组不会。

## 自定义默认组级别状态

在以下情况下，将使用您设置为默认组状态的自定义状态：

* **当Workfront系统自动选择状态时，将使用默认组状态：** 当Workfront系统自动为对象分配状态时，将使用设置为默认组状态的自定义状态。

   例如，任务可配置为在完成百分比达到100%时自动更改为完成状态。 如果您创建等于“完成”的自定义状态，并将该自定义状态设置为默认状态，则Workfront会将任务的状态更改为新的默认状态。

   以这种方式使用自定义状态时，仅考虑与任务或问题关联的组状态。 对于与项目关联的状态，不能以这种方式使用自定义状态。

* 的 **项目的状态由与项目关联的组决定**:如果与给定项目关联的组发生更改，则项目的状态会根据为该组定义的默认状态而发生更改。 （在编辑项目时，可以通过组字段将组与项目关联。）

   如果该组发生更改，则如果新组定义了与项目当前状态等于的不同默认状态，则项目的状态会发生更改。

   例如，一个项目可以与营销组关联，并且项目的状态被设置为“计划”。 对项目进行了编辑，以使其现在与销售组关联。 销售组具有一个名为Thinking的自定义默认组状态（此状态等于Planning）。 由于项目组已更改，因此项目的状态现在更改为Thinking。

如果您是群组管理员，请参阅 [将状态设置为组的默认状态](/help/quicksilver/administration-and-setup/manage-groups/manage-group-statuses/use-custom-statuses-as-default-statuses-group.md).

## 问题状态

如果自定义状态为“问题”状态，则必须为其启用所有四种问题类型（错误报告、更改顺序、问题和请求）。 例如，在下面显示的问题状态中，由于未选中“更改订单”问题类型，因此无法将“重新打开”状态用作默认状态：

![](assets/all-4-issue-types-enabled.png)

## 将自定义状态设置为默认状态

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).
1. 在左侧面板中，单击 **项目首选项** > **状态**.
1. （视情况而定）如果为群组设置默认状态，请在右上角的菜单中开始键入群组名称，然后在显示时选择该群组。
1. 打开 **项目**, **任务**&#x200B;或 **问题** 选项卡，具体取决于要设置为默认状态的状态类型。
1. 单击 **设置默认状态** 下拉菜单。
1. 在显示的下拉区域中，在要设置默认状态的状态旁边，选择所需的默认状态。
1. 单击&#x200B;**保存**。
1. 将项目与状态所在的组关联。

   >[!NOTE]
   >
   >如果您正在为某个组设置自定义状态，稍后又将项目分配给其他组，则项目状态将重新加载，并且可能会发生更改。

   1. 转到要使用自定义状态的项目。
   1. 单击“更多”菜单 ![](assets/more-icon.png)，然后单击 **编辑**.
   1. 在 **编辑项目** 框中显示 **组** 字段 **项目关联**，选择状态所在的组。
   1. 单击 **保存更改**.
