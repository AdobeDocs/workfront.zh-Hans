---
title: 创建和管理布局模板
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: 作为Workfront管理员或组管理员，您可以创建和修改布局模板，以为用户自定义Workfront中的布局元素。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 53076920-3b13-4b65-85cb-38096cf2d04d
source-git-commit: 5d8e189f01a52b2d1b605b497ed17737fb0a0924
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 0%

---

# 创建和管理布局模板

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

作为Adobe Workfront管理员或组管理员，您可以创建和修改布局模板，以在Workfront中为您的用户自定义以下布局元素：

* 主菜单
* 左侧导航面板
* 主页区域
* 人们用于列表和报告的视图、筛选器和分组。
* 屏幕术语
* 项目、任务和问题标题

创建或修改布局模板后，可将其分配给单个用户、团队、组或工作角色。

每个用户的默认Workfront布局取决于其访问级别和许可证类型。 例如，某些用户可能不会在主菜单中看到某些区域。 有关更多信息，请参阅 [关于默认Adobe Workfront布局](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

## 访问要求

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
   <td><p>新增：标准</p>
   或
   <p>当前：计划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>要在系统级别执行这些步骤，您需要系统管理员访问级别。</p>
<p>要为组执行这些操作，您必须是该组的经理。</p> <p><b>注意</b>：</p> <p>如果您没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。

有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
 </tbody> 
</table>

## 创建和管理布局模板的注意事项

* 用户可以自定义其自身布局的几个区域。 在更改布局模板时，所做的更改会与所做的任何自定义设置合并，而不会覆盖或重置这些自定义设置。 如果将用户分配到新布局模板，也是如此。
* 组管理员和具有计划许可证的用户（可以编辑其他用户）可以将系统级和组级布局模板添加到他们在编辑其配置文件时可以管理的用户。
* 组管理员无法将布局模板分配给工作角色或团队。

有关布局模板的详细信息，请参阅 [布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

<!--removed this from above, but keeping it for a bit, in case it will be needed - known issue around old templates still visible at time:
* Your older layout templates created in Adobe Workfront Classic have been automatically available in your instance of the new Adobe Workfront experience since they were migrated in early Fall 2019. Layout templates created in Adobe Workfront Classic after that time were migrated in April 2020. We recommend that you update these layout templates in the new Adobe Workfront experience to take advantage of new functionality and to make them even more useful in that environment.
-->

## 创建或修改布局模板

{{step-1-to-setup}}

1. 在左侧面板中，单击 **界面** > **布局模板**.

1. 单击 **新建布局模板**.

   或

   单击要修改的布局模板的名称。

1. 如果要创建新的布局模板，请键入 **布局模板名称** 和（可选） a **描述** 为了它。

1. 自定义用户界面的区域，如以下文章所述：

   * [使用布局模板自定义主菜单](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
   * [使用布局模板自定义左侧面板](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)
   * [使用布局模板自定义固定页面](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
   * [使用布局模板自定义详细信息视图](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)
   * [使用布局模板自定义主页和摘要](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   * [使用布局模板自定义登陆页面](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
   * [使用布局模板自定义筛选器、视图和分组](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   * [使用布局模板自定义用户界面术语](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-terminology.md)

1. 按照以下文章所述，继续测试您的布局模板并使其可供用户使用：

   * [测试新布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md)
   * [授予对布局模板的管理访问权限](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md)
   * [将用户分配给布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

>[!TIP]
>
>您还可以通过复制和更改副本来创建布局模板。 有关更多信息，请参阅 [复制布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/copy-a-layout-template.md).

