---
title: 使用布局模板自定义主菜单
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 作为Adobe Workfront管理员或组管理员，您可以使用布局模板配置用户在Workfront中打开主菜单时看到的选项。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: d4f02102-0378-472f-9ebb-753502ec048b
source-git-commit: dda00a43c5122a233ce2849d828d2e5e4555d2d9
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 4%

---

# 使用布局模板自定义主菜单

<!--Audited: 01/2024-->

作为Adobe Workfront管理员或组管理员，您可以使用布局模板配置用户在Workfront中打开主菜单时看到的选项。

![主菜单选项](assets/main-menu-with-blueprints-no-branding.png)

>[!NOTE]
>
>用户看到的主菜单选项取决于其许可证类型以及在访问级别中配置的设置。 某些将使用此布局模板的用户可能无法看到您在此处选择的所有选项。 有关详细信息，请参阅 [访问级别和权限如何协同工作](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md) 和 [可配置访问每种对象类型的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

有关创建布局模板的信息，请参阅 [创建和管理布局模板](../use-layout-templates/create-and-manage-layout-templates.md).

有关组布局模板的信息，请参阅 [创建和修改组的布局模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

配置布局模板后，必须将其分配给用户，以使您所做的更改对其他人可见。 有关为用户分配布局模板的信息，请参阅 [将用户分配给布局模板](../use-layout-templates/assign-users-to-layout-template.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront计划</strong></td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront许可证*</strong></td> 
   <td><p>当前：计划</p>
   或
   <p>新增：标准</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置</strong></td> 
   <td> <p>要在系统级别执行这些步骤，您需要系统管理员访问级别。</p>
    <p>要为组执行这些操作，您必须是该组的经理。</p> 
     </td> 
  </tr> 
 </tbody> 
</table>

*有关访问要求的详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 自定义主菜单

1. 开始使用布局模板，如中所述 [创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. 单击 **设置主菜单** 模板右上角的。

   主菜单框打开，您可以看到当前显示在模板的主菜单中的区域，以及可添加的项目。 以下是您可以添加的所有可能项目：
   * 主页

     >[!TIP]
     >
     >默认情况下，主菜单中的主页图标会为Review-license用户（在当前许可证计划中）显示My Updates区域，除非他们有一个与其配置文件关联的布局模板，除了主页区域外，该模板还包括主菜单中的我的更新区域。

   * 项目组合
   * 项目群
   * 项目
   * 报告
   * 仪表板
   * 日历
   * 资源
   * 方案

     >[!NOTE]
     >
     >Scenario Planner需要额外的许可证。 有关Workfront Scenario Planner的信息，请参阅 [Scenario Planner概述](../../../scenario-planner/scenario-planner-overview.md).

   * 团队
   * 用户

     >[!NOTE]
     >
     >只有具有“计划”许可证的用户（在当前许可证模型中）或具有“标准”许可证的用户（在新许可证模型中）才能看到“用户”区域 ![](assets/users-icon-in-main-menu.png) 在主菜单中。

   * 请求
   * 工时表
   * 文档
   * 模板
   * 分析
   * 校对
   * 目标

     >[!NOTE]
     >
     >目标需要额外的许可证。 有关Workfront目标的信息，请参阅 [Adobe Workfront目标概述](../../../workfront-goals/goal-management/wf-goals-overview.md).

   * 我的更新
   * 展示板
   * Blueprint

1. 执行以下任一操作：

   * 隐藏 ![](assets/remove-icon---x-in-circle.png) **活动项目** 您不想显示的内容
   * 显示 ![](assets/add-icon-plus-in-circle.png) **可用项目** 您想在主菜单上显示的内容。
   * 拖动 ![](assets/move-icon---dots.png) **活动项目** 更改主菜单上的显示顺序。

1. 单击 **完成**.

   您还可以单击 **取消** 随时放弃更改。

1. 继续自定义布局模板。

   或

   如果您已完成自定义，请单击 **保存**.

   >[!TIP]
   >
   >您可以随时单击保存以保存进度，然后继续修改模板。

有关布局模板的详细信息，请参阅 [创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
