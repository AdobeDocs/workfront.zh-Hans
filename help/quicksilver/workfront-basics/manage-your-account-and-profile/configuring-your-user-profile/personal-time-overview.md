---
content-type: overview
product-area: user-management
navigation-topic: configure-your-user-profile
title: 配置个人休息时间
description: 在Adobe Workfront中指明何时发生批准的休息时间非常重要，因为这会影响您的日程安排并影响您分配到的任务的规划完成日期。
author: Becky
feature: Get Started with Workfront
exl-id: e7710495-c418-47b1-8598-725580054fc5
source-git-commit: f10b0a4897d6250f0c4decf1fad069c598536a38
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# 配置个人休息时间

<!-- Audited: 12/2023 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment, and is being released in a phased rollout to Production.</span>-->

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

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td> <p>新增：标准（用于配置个人休息时间）</p>
        <p>或</p>
        <p>当前：工作或更高（用于配置个人休息时间）</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>具有[!UICONTROL Edit User]访问权限的[!UICONTROL Manager] （更改其他用户的休息日日历）<br>
   <strong>注意：</strong>如果经理编辑另一个用户的个人休息时间日历，则所有条目都按用户的时区显示，而不是按经理的时区显示。</td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## 在[!DNL Workfront]中配置个人休息时间

{{step1-click-profile-pic}}

>[!NOTE]
>
>如果您在Adobe Unified Experience上，则可以通过单击顶部导航区域中的Adobe帐户菜单（您的配置文件图片），然后选择Workfront配置文件来访问您的Workfront配置文件。
>
>![workfront配置文件](assets/aue-profile.png)

1. 在左侧面板中，单击&#x200B;**[!UICONTROL 空闲时间]**。
1. 为您的个人休息时间选择所需的日期。

   <!--<span class="preview">Sample image in the Preview environment:</span>
   ![Personal time off calendar](assets/personal-time-off-calendar-0925.png)-->

   <!--Sample image in the Production environment:-->
   ![个人休息时间日历](assets/personal-time-off-calendar.png)

1. 如果您要休一整天的假，请选择&#x200B;**[!UICONTROL 全天]**。

   如果您休假的时间少于一整天，请保持此复选框的清除，并指明休假的开始和结束时间。

1. 单击&#x200B;**[!UICONTROL 保存]**。

   您的休息时间现在可以在资源管理工具（如资源规划者和工作负载均衡器）的[!DNL Workfront]系统中看到。 在此期间为您分配了工作后，工具提示会告知用户您已计划休假。
