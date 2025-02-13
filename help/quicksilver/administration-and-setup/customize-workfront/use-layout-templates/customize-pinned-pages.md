---
title: 使用布局模板自定义固定页面
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 在布局模板中，您可以将希望用户始终可用的页面固定在Adobe Workfront顶部。 这些页面可以通过主菜单或功能板访问。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 55cc75c5-8b8c-48e7-b114-b41fe3d545d8
source-git-commit: 2d40585a48f42c767d49530b427d2e4d66f88148
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 4%

---

# 使用布局模板自定义固定页面

在布局模板中，您可以将希望用户始终可用的页面固定在Adobe Workfront顶部。 这些页面可以通过主菜单![主菜单图标](assets/main-menu-icon.png)或主菜单![主菜单图标](assets/main-menu-icon.png)（可用时）访问或功能板访问。

用户自行添加的任何大头针都会显示在您在布局模板中添加的大头针的右侧。

有关固定页面的详细信息，请参阅[固定页面以自定义工作区](../../../workfront-basics/the-new-workfront-experience/pin-pages.md)。

有关布局模板的更多信息，请参阅[创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)。

有关组的布局模板的信息，请参阅[创建和修改组的布局模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)。

配置布局模板后，必须将其分配给用户，以使您所做的更改对其他人可见。 有关将布局模板分配给用户的信息，请参阅[将用户分配给布局模板](../use-layout-templates/assign-users-to-layout-template.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具备以下条件：

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
      <p>新增：</p>
         <ul>
         <li><p>标准</p></li>
         </ul>
      <p>当前：</p>
         <ul>
         <li><p>计划</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>要在系统级别执行这些步骤，您需要系统管理员访问级别。
要为组执行这些操作，您必须是该组的经理。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 使用布局模板固定页面

1. 开始处理布局模板，如[创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)中所述。
1. 在&#x200B;**顶部导航区域**&#x200B;下，单击&#x200B;**添加新pin**。

1. 在出现的下拉菜单中，执行以下任一操作：

   * 从以下区域中选择：

      * 分析
      * 日程表
      * 仪表板
      * 文档
      * 目标
      * 主页
      * 我的更新
      * 项目组合
      * 项目群
      * 项目
      * 报告
      * 请求
      * 资源
      * 方案
      * 团队
      * 模板
      * 时间表
      * 用户
      * Blueprint
      * 规划中

     >[!IMPORTANT]
     >
     >要查看“目标”、“方案”和“规划”区域，需要额外的许可证。
     >
     >* 有关Workfront目标的信息，请参阅[Adobe Workfront目标概述](../../../workfront-goals/goal-management/wf-goals-overview.md)。
     >
     >* 有关Workfront Scenario Planner的信息，请参阅[Scenario Planner概述](../../../scenario-planner/scenario-planner-overview.md)。
     >
     >* 有关Workfront Planning的信息，请参阅[Adobe Workfront Planning概述](/help/quicksilver/planning/general/planning-overview.md)。

   * 单击&#x200B;**添加仪表板**
      * 在&#x200B;<!--**Quick link name**-->**自定义名称**&#x200B;字段中键入描述性名称
      * 在&#x200B;**添加仪表板**&#x200B;字段<!-- dropdown for existing or canvas dashboard, called "Choose a dashboard" now -->中选择仪表板
      * 单击&#x200B;**添加**。

1. 重复上一步以固定任何其他页面。

1. （可选）若要移动图钉，请将鼠标悬停在该图钉上，然后单击该图钉名称旁边的“更多”菜单图标![更多图标](assets/more-icon.png)，然后单击&#x200B;**向左移动**&#x200B;或&#x200B;**向右移动**&#x200B;以按所选方向移动图钉，或单击&#x200B;**移动到前面**&#x200B;以将图钉移动到最左侧位置。

1. （可选）若要重命名某个图钉，请将鼠标悬停在该图钉上，单击该图钉名称旁边的“更多”菜单图标![更多图标](assets/more-icon.png)，然后单击&#x200B;**重命名图钉**。 输入新名称，然后单击&#x200B;**保存**。

1. （可选）若要删除pin，请将鼠标悬停在pin上，单击pin名称旁边的“更多”菜单图标![更多图标](assets/more-icon.png)，然后单击&#x200B;**删除pin**。

1. 继续自定义布局模板。

   或

   如果您已完成自定义，请单击&#x200B;**保存**。

   >[!TIP]
   >
   >您可以随时单击&#x200B;**保存**&#x200B;以保存进度，然后稍后继续修改模板。
