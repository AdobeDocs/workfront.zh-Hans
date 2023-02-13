---
title: 将用户分配到布局模板
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: 作为Adobe Workfront管理员，您可以将您创建的布局模板分配给需要使用该模板的任何用户、作业角色、团队或组。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: a2915f3a-071f-4e9f-88c9-338bf765f418
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 0%

---

# 将用户分配到布局模板

您可以将您创建的布局模板分配给需要使用该模板的任何用户、作业角色、团队或组。

对于未为其分配布局模板的用户，将使用默认布局。 要了解默认布局，请参阅 [关于默认Adobe Workfront布局](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

用户还可以自行分配布局模板，如使用布局模板更改我的工作和工作请求区域中所述。

您可以为同一名称分配多个不同的布局模板。 有关对用户、角色、组或团队有效的布局模板的更多信息，请参阅 [布局模板分配优先级](#layout-template-assignment-priority) 更新。

有关布局模板的更多信息，请参阅 [布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

有关组布局模板的信息，请参阅 [创建和修改组的布局模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

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
   <td> <p>要在系统级别执行这些步骤，您需要系统管理员访问权限级别。
要为组执行这些操作，您必须是该组的经理。</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 为用户分配布局模板

1. 开始使用布局模板，如 [创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

   >[!TIP]
   >
   >如果您对布局模板满意，我们建议您测试布局模板，如 [测试新布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md).

1. 单击 **将其分配给** 中的“隐藏主体”。
1. 在显示的框中，单击 **添加用户、作业角色、团队或组**，开始键入用户、作业角色、团队或群组的名称，然后在下拉菜单中显示该名称时单击该名称。

   最近添加的名称显示为蓝色背景。 当您编辑现有布局模板时，这非常有用，因为您可以将刚刚添加的名称与列表中已添加的名称区分开来。

   “信息”图标 ![](assets/info-icon.png) 在已分配给其他布局模板的任何用户、作业角色、团队或组的名称的右侧显示。 您可以将鼠标悬停在图标上以查看该布局模板的名称，并确定是否要覆盖现有分配。

1. 重复上述两个步骤，根据需要将布局模板分配给其他用户、工作角色、团队或组。

   您一次最多可以分配100个用户。

1. 单击 **完成**，然后单击 **保存** 在左下角。

   此步骤将完成创建和分配布局模板的过程。

## 布局模板分配优先级 {#layout-template-assignment-priority}

您和其他Workfront管理员可以通过以下四种不同方式为同一用户分配多个不同的布局模板：

* 对单个用户
* 对于用户具有的特定作业角色
* 对于用户所在的特定团队
* 对于用户所在的特定组

但是，用户在任何给定时间都只能看到一个布局模板。 可见的模板由以下优先级层次结构确定：

* **单个用户**:作为单个用户分配给人员的布局模板将覆盖所有其他用户。 您可以通过执行新分配来覆盖先前的分配，以便单个用户；最近的一个优先。
* **主要作业角色**:如果未将人员分配为单个用户的布局模板，则他们会看到为其主要作业角色分配的模板。

   只有分配给用户主作业角色的布局模板对用户可见。 分配给用户担任的任何辅助作业角色的模板不可见。

* **主队**:如果人员未作为单个用户或具有主要工作角色的用户分配布局模板，则他们会看到分配给其主团队的模板。

   只有分配给用户主页团队的模板才对用户可见。 分配给用户为成员的其他团队的模板不可见。

* **家庭组**:如果人员既未作为单个用户分配布局模板，也未作为具有主要工作角色的用户分配布局模板，或者未作为主团队成员分配布局模板，则他们将看到分配给其主组的模板。

   只有分配给用户主页组的模板对用户可见。 分配给其任何其他组的模板不可见。

## 分配给布局模板的大量用户

如果您编辑分配给2000多个用户的布局模板并对其进行更改，则只有前2000个用户将保留在布局模板上，并将看到您所做的更改。 布局模板将从所有其他模板中删除。

如果您有2000名以上的用户要分配给布局模板，我们建议您执行以下操作之一：

* 将用户组织到组或团队中，并将布局模板分配给这些组或团队。 有关更多信息，请参阅 [创建群组](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) 和 [创建和管理团队](../../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md).

* 为用户分配作业角色，并将布局模板分配给其主作业角色。 有关更多信息，请参阅 [创建和管理作业角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
