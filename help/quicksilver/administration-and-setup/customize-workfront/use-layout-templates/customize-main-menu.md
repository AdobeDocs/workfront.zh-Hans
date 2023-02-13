---
title: 使用布局模板自定义主菜单
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 作为Adobe Workfront管理员或组管理员，您可以使用布局模板配置用户在Workfront中打开主菜单时看到的选项。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d4f02102-0378-472f-9ebb-753502ec048b
source-git-commit: 9c78d8e08e62c86a4e1340644ed76c61ce7f2674
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 4%

---

# 使用布局模板自定义主菜单

作为Adobe Workfront管理员或组管理员，您可以使用布局模板配置用户在Workfront中打开主菜单时看到的选项：

![主菜单选项](assets/main-menu-with-blueprints-no-branding.png)

>[!NOTE]
>
>用户看到的主菜单选项取决于其许可证类型以及其访问级别中配置的设置。 某些使用此布局模板的用户可能看不到在此处选择的所有选项。 有关详细信息，请参阅 [访问级别和权限如何协同工作](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md) 和 [可配置地访问每种对象类型的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

有关组布局模板的信息，请参阅 [创建和修改组的布局模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront计划</strong></td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront许可证</strong></td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置</strong></td> 
   <td> <p>要在系统级别执行这些步骤，您需要系统管理员访问权限级别。
要为组执行这些操作，您必须是该组的经理。</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 自定义主菜单

1. 开始使用布局模板，如 [创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. 单击 **设置主菜单** 在右上角附近。

   在显示的“主菜单”框中，您可以看到模板的“主菜单”中当前处于活动状态的项目以及可添加的项目。 以下是可添加的所有可能项目：

   * 主页

      >[!TIP]
      >
      >默认情况下，“主页”会显示为“审阅许可证”用户的“我的更新”，除非他们有一个与其配置文件关联的布局模板，该模板包含“主菜单”中的“我的更新”区域。

   * 项目组合
   * 项目群
   * 项目
   * 报告
   * 仪表板
   * 日历
   * 资源
   * 场景

      >[!NOTE]
      >
      >方案规划器仅在新的Adobe Workfront体验中可用，并且需要额外的许可证。 有关Workfront方案规划器的信息，请参阅 [方案计划员概述](../../../scenario-planner/scenario-planner-overview.md).

   * 团队
   * 用户

      >[!NOTE]
      >
      >只有具有计划许可证的用户才能看到用户 ![](assets/users-icon-in-main-menu.png) 中。

   * 请求
   * 时间表
   * 文档
   * 模板
   * 分析
   * 验证
   * 目标

      >[!NOTE]
      >
      >这需要额外的许可证。 有关Workfront目标的信息，请参阅 [Adobe Workfront目标概述](../../../workfront-goals/goal-management/wf-goals-overview.md).

   * 我的更新
   * 展示板
   * Blueprint

1. 执行以下任一操作：

   * 隐藏 ![](assets/remove-icon---x-in-circle.png) **活动项目** 你不想展示
   * 显示 ![](assets/add-icon-plus-in-circle.png) **可用项目** 显示在“主菜单”(Main Menu)中。
   * 拖动 ![](assets/move-icon---dots.png) **活动项目** 更改其在主菜单上的显示顺序。

1. 单击 **完成**.

   您还可以单击 **取消** 随时放弃更改。

1. 继续自定义布局模板。

   或

   如果您已完成自定义，请单击 **保存**.

   >[!TIP]
   >
   >您可以随时单击保存以保存进度，然后稍后继续修改模板。

有关布局模板的更多信息，请参阅 [创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
