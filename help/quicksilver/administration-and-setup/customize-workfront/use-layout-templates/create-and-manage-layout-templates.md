---
title: 创建和管理布局模板
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: 作为Workfront管理员或组管理员，您可以创建和修改布局模板，以便为您的用户自定义Workfront中的布局元素。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 53076920-3b13-4b65-85cb-38096cf2d04d
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# 创建和管理布局模板

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

作为Workfront管理员或组管理员，您可以创建和修改布局模板，以在Workfront中为您的用户自定义以下布局元素：

* 主菜单
* 左侧导航面板
* 主页区域
* 人们用于列表和报告的视图、筛选器和分组。
* 屏幕术语

创建或修改布局模板后，可将其分配给单个用户、团队、组或工作角色。

每个用户的默认Workfront布局取决于其访问级别和许可证类型。 例如，某些用户可能看不到主菜单中的某些区域。 有关更多信息，请参阅 [关于默认Adobe Workfront布局](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

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

## 创建和管理布局模板的注意事项

* 用户可以自定义其自身布局的几个区域。 在更改布局模板时，所做更改会与所做的任何自定义项合并，而不会覆盖或重置这些自定义项。 如果将用户分配到新布局模板，也是如此。
* 您在Adobe Workfront Classic中创建的旧版面模板，自2019年秋季迁移以来，已自动放入新Adobe Workfront Experience的实例中。 2020年4月，迁移了在Adobe Workfront Classic中创建的布局模板。 我们建议您在新的Adobe Workfront Experience中更新这些布局模板，以便利用新功能并使它们在该环境中更加有用。
* 组管理员和具有计划许可证的用户（可以编辑其他用户）可以将系统级和组级布局模板添加到他们在编辑其配置文件时可以管理的用户。
* 组管理员无法将布局模板分配给工作角色或团队。

有关布局模板的详细信息，请参阅 [布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

## 创建或修改布局模板

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **界面** > **布局模板**.

1. 单击 **新建布局模板**.

   或

   单击要修改的布局模板的名称。

1. 如果要创建新布局模板，请键入 **布局模板名称** 和（可选）a **描述** 为了它。

1. 自定义用户界面的区域，如以下文章所述：

   * [使用布局模板自定义主菜单](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
   * [使用布局模板自定义左侧面板](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)
   * [使用布局模板自定义固定页面](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
   * [使用布局模板自定义详细信息视图](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)
   * [使用布局模板自定义主页和摘要](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   * [使用布局模板自定义登陆页面](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
   * [使用布局模板自定义筛选器、视图和分组](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   * [使用布局模板自定义用户界面术语](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-terminology.md)

1. 按照以下文章中的说明，继续测试布局模板并使其可供用户使用：

   * [测试新布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md)
   * [授予对布局模板的管理访问权限](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md)
   * [将用户分配给布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

您还可以通过复制并更改副本来创建新布局模板。 有关更多信息，请参阅 [复制布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/copy-a-layout-template.md).
