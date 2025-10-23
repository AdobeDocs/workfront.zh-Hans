---
content-type: overview
product-area: user-management
navigation-topic: configure-your-user-profile
title: 配置个人休息时间
description: 在Adobe Workfront中指明何时发生批准的休息时间非常重要，因为这会影响您的日程安排并影响您分配到的任务的规划完成日期。
author: Becky
feature: Get Started with Workfront
exl-id: e7710495-c418-47b1-8598-725580054fc5
source-git-commit: e25ea757129e9645f7b5f0729cd498d5947f49f2
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# 配置个人休息时间

<!-- Audited: 12/2023 -->

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览Sandbox”环境中可用，正在分阶段发布到生产环境。</span>

[!DNL Adobe Workfront]的设计目的不是复制或替换现有系统，用于管理、应计和跟踪个人休息时间。

但是，指明何时批准休息时间很重要，因为这会影响您的计划以及您分配到任务的[!UICONTROL 规划完成日期]。

例如，如果您被分配到一项计划休假2周的任务，并计划在休假3天，则[!DNL Workfront]会在任务时间表中添加三天以考虑休假。

资源管理工具还会使用您的个人休息时间来指示您何时可以安排工作。

>[!NOTE]
>
>为了确保与您安排的休息日期不会有任何不一致的情况，我们建议用户配置文件的时区与计划的时区相匹配。 有关更多信息，请参阅以下文章：
>
>* [创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
>

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 </col>
 <tbody> 
  <tr> 
   <td> Adobe Workfront包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td> <p>要配置个人休息时间，您必须拥有：</p>
        <p>标准（配置个人休息时间）</p>
        <p>工作或更高版本（用于配置个人休息时间）</p> </td>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td><p>要更改另一个用户的休息日日程表，您必须是该用户的经理并且拥有编辑用户访问权限。</p>
   <p><strong>注意：</strong>如果经理编辑另一个用户的个人休息时间日历，则所有条目都以用户的时区显示，而不是以经理的时区显示。</p></td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在[!DNL Workfront]中配置个人休息时间

{{step1-click-profile-pic}}

>[!NOTE]
>
>如果您在Adobe Unified Experience上，则可以通过单击顶部导航区域中的Adobe帐户菜单（您的配置文件图片），然后选择Workfront配置文件来访问您的Workfront配置文件。
>
>![workfront配置文件](assets/aue-profile.png)

1. 在左侧面板中，单击&#x200B;**[!UICONTROL 空闲时间]**。
1. 为您的个人休息时间选择所需的日期。

   <span class="preview">预览环境中的示例图像：</span>
   ![个人休息时间日历](assets/personal-time-off-calendar-0925.png)

   生产环境中的示例图像：
   ![个人休息时间日历](assets/personal-time-off-calendar.png)

1. 如果您要休一整天的假，请选择&#x200B;**[!UICONTROL 全天]**。

   如果您休假的时间少于一整天，请保持此复选框的清除，并指明休假的开始和结束时间。

1. 单击&#x200B;**[!UICONTROL 保存]**。

   您的休息时间现在可以在资源管理工具（如资源规划者和工作负载均衡器）的[!DNL Workfront]系统中看到。 在此期间为您分配了工作后，工具提示会告知用户您已计划休假。
