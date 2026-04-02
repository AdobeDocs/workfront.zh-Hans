---
title: 创建和管理布局模板
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: 作为Workfront管理员或组管理员，您可以创建和修改布局模板，以为用户自定义Workfront中的布局元素。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 53076920-3b13-4b65-85cb-38096cf2d04d
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: b9e0747a58618353caf3ce1c7e8521d22d2b412d
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 5%

---

# 创建和管理布局模板

<!--Audited: 12/2023-->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

{{highlighted-preview}}

作为Adobe Workfront管理员或组管理员，您可以创建和修改布局模板，以在Workfront中为您的用户自定义以下布局元素：

* 主菜单
* 左侧导航面板
* 主页区域
* 摘要面板
* 人们用于列表和报告的视图、筛选器和分组。
* 屏幕术语
* <span class="preview">对象标头</span>
* 对象的<span class="preview">更多菜单（三点菜单）</span>

创建或修改布局模板后，可将其分配给单个用户、团队、组或工作角色。

每个用户的默认Workfront布局取决于其访问级别和许可证类型。 例如，某些用户可能不会在主菜单中看到某些区域。 有关详细信息，请参阅[关于默认Adobe Workfront布局](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 包</td> 
   <td><p>“任一”</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p>
       <p>规划</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td> <p>要在系统级别执行这些步骤，您需要系统管理员访问级别。</p>
        <p>要为组执行这些操作，您必须是该组的经理。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 创建和管理布局模板的注意事项

* 用户可以自定义其自身布局的几个区域。 在更改布局模板时，所做的更改会与所做的任何自定义设置合并，而不会覆盖或重置这些自定义设置。 如果将用户分配到新布局模板，也是如此。
* 组管理员和具有计划许可证的用户（可以编辑其他用户）可以将系统级和组级布局模板添加到他们在编辑其配置文件时可以管理的用户。
* 组管理员无法将布局模板分配给工作角色或团队。

有关布局模板的详细信息，请参阅[布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md)。

## 创建或修改布局模板

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**界面** > **布局模板**。

1. 单击&#x200B;**新建布局模板**。

   或

   单击要修改的布局模板的名称。

1. 如果要创建新的布局模板，请键入该模板的&#x200B;**布局模板名称**&#x200B;和&#x200B;**描述**（可选）。

1. 自定义用户界面的区域，如以下文章所述：

   * [使用布局模板自定义主菜单](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
   * [使用布局模板自定义左侧面板](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)
   * [使用布局模板自定义更多菜单](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-more-menu.md)
   * [使用布局模板自定义固定页面](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
   * [使用布局模板自定义详细信息视图](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)
   * [使用布局模板自定义摘要面板](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   * [使用布局模板自定义主页](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-new-home-layout-template.md)
   * [使用布局模板自定义登陆页面](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
   * [使用布局模板自定义筛选器、视图和分组](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   * [使用布局模板自定义用户界面术语](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-terminology.md)

1. 按照以下文章所述，继续测试您的布局模板并使其可供用户使用：

   * [测试新布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md)
   * [授予布局模板的管理访问权限](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md)
   * [将用户分配给布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

>[!TIP]
>
>您还可以通过复制布局模板并更改复制的版本来创建该布局模板。 有关详细信息，请参阅[复制布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/copy-a-layout-template.md)。

