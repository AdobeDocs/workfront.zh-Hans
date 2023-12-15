---
content-type: overview
product-area: user-management
navigation-topic: configure-your-user-profile
title: 配置个人休息时间
description: 在Adobe Workfront中指明何时发生批准的休息时间非常重要，因为这会影响您的日程安排并影响您分配到的任务的规划完成日期。
author: Lisa
feature: Get Started with Workfront
exl-id: e7710495-c418-47b1-8598-725580054fc5
source-git-commit: 91d757513792604677d6285baafa795629b4506d
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 0%

---

# 配置个人休息时间

<!-- Audited: 12/2023 -->

[!DNL Adobe Workfront] 不是为了复制或替换您现有的系统，用于管理、积累和跟踪个人休息时间。

但是，请务必指明何时发生批准的休息时间，因为这会同时影响您的计划和 [!UICONTROL 计划完成日期] 您分配到的所有任务。

例如，如果您被分配到一项计划为两周时间的任务，并计划在此期间休假3天， [!DNL Workfront] 向任务时间线添加三天以考虑空闲时间。

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
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>新增：标准（用于配置个人休息时间）</p>
        <p>或</p>
        <p>当前：工作或更高（用于配置个人休息时间）</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td>具有[！UICONTROL Edit User]访问权限的[！UICONTROL Manager] （更改其他用户的休息日日历）<br>
   <strong>注意：</strong> 如果经理编辑另一个用户的个人休息时间日程表，则所有条目都按用户的时区显示，而不是按经理的时区显示。</td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

## 在中配置个人休息时间 [!DNL Workfront]

{{step1-click-profile-pic}}

1. 在左侧面板中，单击 **[!UICONTROL 空闲时间]**.
1. 为您的个人休息时间选择所需的日期。

   ![个人休息时间日程表](assets/personal-time-off-calendar.png)

1. 选择 **[!UICONTROL 全天]**，请您休一整天的假。

   如果您休假的时间少于一整天，请保持此复选框的清除，并指明休假的开始和结束时间。

1. 单击&#x200B;**[!UICONTROL 保存]**。

   您的空闲时间现在可以在以下位置看到： [!DNL Workfront] 系统中的资源管理工具，如资源规划者和工作负载均衡器。 在此期间为您分配了工作后，工具提示会告知用户您已计划休假。
