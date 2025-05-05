---
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: 使用自定义状态作为默认状态
description: 当自定义状态设置为默认状态时，新的默认状态将以各种方式在整个系统中使用。 其使用方式取决于其设置为默认的系统级状态，还是默认组级状态。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 5b137cee-e03a-4176-a683-b77f2b27f5ce
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 0%

---

# 使用自定义状态作为默认状态

当自定义状态设置为默认状态时，新的默认状态将以各种方式在整个系统中使用。 其使用方式取决于其设置为默认的系统级状态，还是默认组级状态。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任何</td> 
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
   <td>[!UICONTROL 系统管理员]</td>
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 自定义默认系统级别状态

当您将自定义状态设置为默认系统状态时，在系统中创建的任何新组都将继承该状态。

在设置新的默认系统状态时已存在的组不会自动继承它。

例如，假设您的Adobe Workfront环境中已创建两个组（营销和销售）。 您可以创建与“当前”相等的新自定义状态，并调用该状态“处理中”。 现在，您将创建一个名为工程的新组。 在此方案中，“工程”组继承新的默认状态，“营销”组和“销售”组则不继承。

## 自定义默认组级别状态

在以下情况下，将使用您设置为默认组状态的自定义状态：

* **当Workfront系统自动选择状态时，将使用默认组状态：**&#x200B;当Workfront系统自动为对象分配状态时，将使用您设置为默认组状态的自定义状态。

  例如，任务可以配置为当完成百分比达到100%时自动变为“完成”状态。 如果您创建了一个等同于完成的自定义状态，并将该自定义状态设置为默认状态，Workfront会将任务的状态更改为新的默认状态。

  自定义状态仅以这种方式用于与任务或问题关联的组状态。 自定义状态不能以这种方式用于与项目关联的状态。

* 项目的&#x200B;**状态由与项目关联的组决定**：如果与给定项目关联的组发生更改，则项目的状态会根据为该组定义的默认状态而变化。 （在编辑项目时，组可以通过组字段与项目关联。）

  如果该组发生更改，并且新组所定义的默认状态与项目的当前状态相同，则项目的状态也会更改。

  例如，项目可与营销组关联，且项目的状态设置为“计划”。 项目经过编辑，现在与Sales组相关联。 Sales组有一个名为Thinking的自定义默认组状态（此状态等于Planning）。 由于项目上的组已更改，因此项目的状态现在更改为“正在思考”。

如果您是组管理员，请参阅[将状态设置为组](/help/quicksilver/administration-and-setup/manage-groups/manage-group-statuses/use-custom-statuses-as-default-statuses-group.md)的默认状态。

## 问题状态

如果自定义状态是问题状态，则必须为其启用所有四种问题类型（错误报告、更改顺序、问题和请求）。 例如，在下面显示的问题状态中，由于未选择“更改单”问题类型，因此不能将“重新打开”状态用作默认状态：

![所有问题类型已启用](assets/all-4-issue-types-enabled.png)

## 将自定义状态设置为默认状态

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**项目首选项** > **状态**。
1. （视情况而定）如果要为组设置默认状态，请在右上角的菜单中开始键入组的名称，然后在该组出现时将其选定。
1. 打开&#x200B;**项目**、**任务**&#x200B;或&#x200B;**问题**&#x200B;选项卡，具体取决于要设置为默认状态的状态类型。
1. 单击&#x200B;**设置默认状态**&#x200B;下拉菜单。
1. 在显示的下拉区域中，在要设置默认状态的状态旁边，选择所需的默认状态。
1. 单击&#x200B;**保存**。
1. 将项目与状态所在的组关联。

   >[!NOTE]
   >
   >如果您正在设置组的自定义状态，并且稍后将项目分配给其他组，则项目状态将重新加载并可能更改。

   1. 转到要在其中使用自定义状态的项目。
   1. 单击“更多”菜单![更多图标](assets/more-icon.png)，然后单击&#x200B;**编辑**。
   1. 在显示的&#x200B;**编辑项目**&#x200B;框中，在&#x200B;**项目关联**&#x200B;下的&#x200B;**组**&#x200B;字段中，选择状态所在的组。
   1. 单击&#x200B;**保存更改**。
