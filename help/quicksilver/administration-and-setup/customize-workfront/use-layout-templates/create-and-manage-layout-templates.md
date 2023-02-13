---
title: 创建和管理布局模板
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: 作为Workfront管理员或组管理员，您可以创建和修改布局模板，以在Workfront中为用户自定义布局元素。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 53076920-3b13-4b65-85cb-38096cf2d04d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# 创建和管理布局模板

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

作为Workfront管理员或组管理员，您可以创建和修改布局模板，以在Workfront中为用户自定义以下布局元素：

* 主菜单
* 左侧导航面板
* 主区
* 用户在列表和报表中使用的视图、过滤器和分组。
* 屏幕术语

在创建或修改布局模板后，您可以将其分配给各个用户、团队、组或作业角色。

每个用户的默认Workfront布局取决于其访问级别和许可证类型。 例如，某些用户可能在主菜单中看不到某些区域。 有关更多信息，请参阅 [关于默认Adobe Workfront布局](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

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

## 创建和管理布局模板的注意事项

* 用户可以自定义自己布局的几个区域。 当您更改布局模板时，所做的更改会与它们所做的任何自定义项合并，而不会覆盖或重置它们。 如果将用户分配给新布局模板，则也是如此。
* 自2019年秋季初迁移以来，您在Adobe Workfront Classic中创建的旧版布局模板已在新Adobe Workfront体验的实例中自动可用。 此后在Adobe Workfront Classic中创建的布局模板在2020年4月进行了迁移。 我们建议您在新的Adobe Workfront体验中更新这些布局模板，以利用新功能，并在该环境中使它们更有用。
* 具有计划许可证且可以编辑其他用户的群组管理员和用户可以在编辑其配置文件时向其管理的用户添加系统级别和群组级别布局模板。
* 群组管理员无法将布局模板分配给作业角色或团队。

有关布局模板的更多信息，请参阅 [布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

## 创建或修改布局模板

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **界面** > **布局模板**.

1. 单击 **新布局模板**.

   或

   单击要修改的布局模板的名称。

1. 如果要创建新布局模板，请键入 **布局模板名称** 和（可选）a **描述** 为了它。

1. 按照以下文章所述，自定义用户界面的区域：

   * [使用布局模板自定义主菜单](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
   * [使用布局模板自定义左侧面板](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)
   * [使用布局模板自定义固定的页面](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
   * [使用布局模板自定义详细信息视图](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)
   * [使用布局模板自定义主页和摘要](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   * [使用布局模板自定义登陆页面](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
   * [使用布局模板自定义过滤器、视图和分组](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   * [使用布局模板自定义用户界面术语](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-terminology.md)

1. 继续测试布局模板并将其提供给用户，如以下文章所述：

   * [测试新布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md)
   * [授予布局模板的管理访问权限](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md)
   * [将用户分配到布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

您还可以通过复制布局模板并更改副本来创建新布局模板。 有关更多信息，请参阅 [复制布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/copy-a-layout-template.md).
