---
title: 将用户分配给布局模板
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: 作为Adobe Workfront管理员，您可以将已创建的布局模板分配给需要使用该布局模板的任何用户、工作角色、团队或组。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: a2915f3a-071f-4e9f-88c9-338bf765f418
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 0%

---

# 将用户分配给布局模板

您可以将已创建的布局模板分配给需要使用该布局模板的任何用户、工作角色、团队或组。

对于没有为其分配布局模板的用户，使用默认布局。 要了解默认布局，请参阅 [关于默认Adobe Workfront布局](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

用户还可以向自己分配布局模板，如使用布局模板更改我的工作和工作请求区域中所述。

您可以将多个不同的布局模板分配给同一个名称。 有关对用户、角色、组或团队有效的布局模板的更多信息，请参阅 [布局模板分配优先级](#layout-template-assignment-priority) 本文后面部分。

有关布局模板的详细信息，请参阅 [布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

有关组的布局模板的信息，请参阅 [创建和修改组的布局模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

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
   <td> <p>要在系统级别执行这些步骤，您需要系统管理员访问级别。
要为组执行这些操作，您必须是该组的经理。</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 为用户分配布局模板

1. 开始使用布局模板，如中所述 [创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

   >[!TIP]
   >
   >当您对布局模板感到满意时，我们建议您对其进行测试，如中所述 [测试新布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md).

1. 单击 **将此项分配给** （在页面的顶部）。
1. 在出现的框中，单击 **添加用户、工作角色、团队或组**，开始键入用户、工作角色、团队或组的名称，然后在名称出现在下拉列表中时单击该名称。

   最近添加的名称以蓝色背景显示。 在编辑现有布局模板时，这很有用，因为您可以区分刚刚添加和列表中已存在的名称。

   “信息”图标 ![](assets/info-icon.png) 显示在已分配给其他布局模板的任何用户、工作角色、团队或组的名称的右侧。 您可以将鼠标悬停在该图标上以查看该布局模板的名称，并决定是否覆盖现有分配。

1. 重复前两个步骤，根据需要将布局模板分配给其他用户、工作角色、团队或组。

   一次最多可以分配100个用户。

1. 单击 **完成**，然后单击 **保存** 左下角。

   此步骤将完成创建和分配布局模板的过程。

## 布局模板分配优先级 {#layout-template-assignment-priority}

您和其他Workfront管理员可以通过以下四种方式将多个不同的布局模板分配给同一用户：

* 个人用户
* 到用户拥有的特定工作角色
* 对于用户所在的某个团队
* 对于用户所在的某个组

但是，在任何给定时间，用户只能看到一个布局模板。 可见的模板由以下优先级层次结构决定：

* **个人用户**：作为个人用户分配给该人员的布局模板将覆盖所有其他模板。 您可以覆盖先前进行的分配，这样单个用户便可以通过进行新的分配来完成；最新的分配优先。
* **主要工作角色**：如果人员未作为单个用户分配布局模板，他们将看到为其主要工作角色分配的模板。

  只有分配给用户的主要工作角色的布局模板对用户可见。 分配给用户拥有的任何辅助工作角色的模板不可见。

* **主团队**：如果人员未作为个人用户或具有主要工作角色的用户分配布局模板，他们将看到模板分配给其主团队。

  只有分配给用户主团队的模板对用户可见。 分配给用户为成员的其他团队的模板不可见。

* **主组**：如果人员未作为个人用户、具有主要工作角色的用户或主页团队成员分配布局模板，他们将看到模板分配给其主页组。

  只有分配给用户主组的模板对用户可见。 分配给其任何其他组的模板不可见。

## 分配给布局模板的大量用户

如果您编辑分配给2000多个用户的布局模板并对其进行更改，则只有前2000个用户将保留在布局模板上，并且会看到您所做的更改。 布局模板将从所有其他布局模板中删除。

如果要为布局模板分配超过2000个用户，我们建议您执行以下操作之一：

* 将用户组织到组或团队中，并将布局模板分配给这些组或团队。 有关更多信息，请参阅 [创建组](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) 和 [创建和管理团队](../../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md).

* 将工作角色分配给用户，并将布局模板分配给其主要工作角色。 有关更多信息，请参阅 [创建和管理职位角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
