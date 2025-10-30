---
title: 使用布局模板自定义登陆页面
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 作为Workfront管理员，您可以使用布局模板指定用户每次登录到Workfront时要查看的区域。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 57a1046a-434a-4453-a101-c5f0a16e079e
source-git-commit: a561620e218cafc0af861d2b157b8dc7c83dd7ed
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 5%

---

# 使用布局模板自定义登陆页面

{{preview-fast-release-general}}

作为Adobe Workfront管理员，您可以使用布局模板指定用户每次登录到Workfront时要查看的区域。

用户可以打开以下选项之一：

* 指定的Workfront区域
* 自定义仪表板。

有关创建布局模板的信息，请参阅[创建和管理布局模板](../use-layout-templates/create-and-manage-layout-templates.md)。

有关组的布局模板的信息，请参阅[创建和修改组的布局模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)。

配置布局模板后，必须将其分配给用户，以使您所做的更改对其他人可见。 有关将布局模板分配给用户的信息，请参阅[将用户分配给布局模板](../use-layout-templates/assign-users-to-layout-template.md)。

>[!NOTE]
>
>当请求设置为登录页时，分配给布局模板的参与者或请求者用户将改为将主页视为登录页。 除了针对投稿人或请求人用户的布局模板请求外，建议选择登陆页面。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td><p>任何</p></td> 
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

## 自定义登陆页面

1. 开始处理布局模板，如[创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)中所述。
1. 在&#x200B;**顶部导航区域**&#x200B;中，单击&#x200B;**选择登陆页面**，然后选择用户登录时要查看的区域。

   从以下区域进行选择，或添加自定义功能板：

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
   >要查看“方案”、“目标”和“规划”区域，需要额外的许可证。
   >
   >* 有关Workfront目标的信息，请参阅[Adobe Workfront目标概述](../../../workfront-goals/goal-management/wf-goals-overview.md)。
   >
   >* 有关Workfront Scenario Planner的信息，请参阅[Scenario Planner概述](../../../scenario-planner/scenario-planner-overview.md)。
   >
   >* 有关Workfront Planning的信息，请参阅[Adobe Workfront Planning概述](/help/quicksilver/planning/general/planning-overview.md)。

1. 在“预览”环境中：继续自定义布局模板。 <span class="preview">您可以随时单击&#x200B;**应用**&#x200B;以保存进度。</span>

   <span class="preview">或</span>

   <span class="preview">如果您已完成自定义，请单击&#x200B;**保存并关闭**。</span>

1. 在生产环境中：继续自定义布局模板。

   或

   如果您已完成自定义，请单击&#x200B;**保存**。

   >[!TIP]
   >
   >您可以随时单击&#x200B;**保存**&#x200B;以保存进度，然后稍后继续修改模板。
