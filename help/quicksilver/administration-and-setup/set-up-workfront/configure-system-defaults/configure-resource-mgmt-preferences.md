---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: 配置资源管理首选项
description: 作为 [!DNL Adobe Workfront] 管理员可以为系统配置资源管理首选项。 这些资源管理首选项决定了如何为 [!DNL Workfront] 资源计划和规划工具。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7cde2238-cb34-4bee-baba-69d256a3912d
source-git-commit: 3486a2523a038bdd83c3c2001001a119fd0508ad
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# 配置 [!UICONTROL 资源管理] 首选项

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

<!--drafted for Work time field: <span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> -->

作为 [!DNL Adobe Workfront] 管理员，您可以配置 [!UICONTROL 资源管理] 系统的首选项。 这些首选项决定了计算用户小时数、FTE可用性或容量的方式 [!DNL Workfront] 资源计划和规划工具。

## 访问要求

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td>
   <p>Current license: [!UICONTROL Standard]</p>
   
   Or
   
   <p>Legacy license: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>System Administrator access level</p> <p>For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p><b>NOTE</b>: 
   
   If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td>[!UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>系统管理员访问级别</p> <p>有关更多信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> <p><b>注释</b>:

如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
 </tbody> 
</table>

<!--drafted for Work time field: 

## Information taken into account when calculating user's capacity

When calculating a user's capacity, Workfront takes into account the following information:

* The number of scheduled hours, as defined in either the Schedule of the user or the Workfront system's [!UICONTROL Default Schedule]
* [!UICONTROL Schedule] [!UICONTROL Exceptions] (depending on which [!UICONTROL Schedule] is used, it can be the exceptions of the user's schedule, or those associated with the [!DNL Workfront] [!UICONTROL Default Schedule])
* User's time off
* The value of the Full Time Equivalent ([!UICONTROL FTE]) of the user or that of the [!DNL Workfront] system. The [!UICONTROL FTE] equals 1 when the user works full time, as defined in the schedule. 

<!-drafted for Work Time field  

* <span class="preview">The value of [!UICONTROL Work Time] for the user which refers to time that the user spends on project-related work. This does not include overhead time, like meetings and training. The [!UICONTROL Work Time] equals 1 when the user is available for work the entire time as indicated by the [!UICONTROL FTE] or the schedule, which means they don't spend any time on non-project-related work like meetings or trainings.</span>

-->

有关中的计划和计划资源的信息 [!DNL Workfront]，请参阅 [资源管理入门](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

—>

## 配置 [!UICONTROL 资源管理] 首选项

>[!NOTE]
>
>由于这是全局设置，因此此选择会影响所有资源管理工具中整个系统（对于所有用户）的所有计算。

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).
1. 单击 **[!UICONTROL 资源管理]**.
1. 选择以下方法之一，以计算 [!DNL Workfront]:

   * **默认计划**: [!DNL Workfront] 使用系统的默认计划和用户的单个FTE来计算资源管理工具中用户的可用小时数。

      有关计划的详细信息，请参阅 [创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      有关查找用户值的更多信息 [!UICONTROL FTE]，请参阅  [编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      Workfront在Workfront管理员选择 [!UICONTROL 默认计划]:

      <!--drafted for Work Time field:
      In the Production environment: 
      -->

      ```
      User Available Hours = ([!UICONTROL Default Schedule] Hours - Exceptions) * FTE - Time off hours
      ```

      >[!INFO]
      >
      > 例如，如果 [!UICONTROL 默认计划] 每周40小时，而 [!UICONTROL FTE] 在用户的配置文件中，为0.5，用户每周可工作20小时。
      >如果用户有一天有1小时的休息时间，则其可用小时数将按如下方式计算：
      >
      >
      ```
      >User Available Hours = [(40 - 0) * 0.5)] - 1 = 19 hours
      >```
   <!--drafted for Work Time field

      <div class="preview">
      
      In the Preview environment: 

      ```
      User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * Work Time
      ```

      >[!INFO]
      >
      >For example, if the Default Schedule is 40 hours a week,  the FTE in the profile of the user is 0.5, the user has 1 hour of Time off one day, and the [!UICONTROL Work Time] in the profile of the user is 0.5, the user is available for actual project work for 9.5 hours a week.
      >
      >If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:
      >
      >```
      >User Available Hours = [(40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours
      >```

      </div>

   -->

   <!--      
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>In the Production environment: (NOTE: this is the old way it was working, before the 22.2 release)</p><p><code>User Available Hours = (Default Schedule Hours - (Schedule Exceptions + Time off hours)) * User FTE value</code></p>      
      <div class="example" data-mc-autonum="<b>Example: </b>">      
      <span class="autonumber"><span><b>Example: </b></span></span>      
      <div>      
      <p>For example, if the Default Schedule is 40 hours a week and the FTE in the profile of the user is 0.5, the user is available to work for 20 hours a week.</p>      
      <p>If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:</p>      
      <p><code>User Daily Available Hours = (40 - 1)* 0.5 = 19.5 hours</code></p>      
      </div>      
      </div></li>      
      -->

   * **用户的计划**: [!DNL Workfront] 使用用户的计划以及 [!UICONTROL 默认计划] 来计算 [!UICONTROL FTE] 资源管理工具中用户的值。 可用小时数仅根据用户的计划进行计算。 的值 [!UICONTROL FTE] 将忽略。 这是默认设置。

      有关计划的详细信息，请参阅 [创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      有关用户 [!UICONTROL 计划]，请参阅  [编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      >[!NOTE]
      >
      >如果用户未与计划关联，则仅使用 [!UICONTROL 默认计划].

      <!--drafted for Work Time field:
      In the Production environment: 
      -->

      用户的可用小时数使用以下公式计算：

      ```
      User Available Hours = Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours
      ```

      可用 [!UICONTROL FTE] 对于用户，使用以下公式计算：

      ```
      User Available [!UICONTROL FTE] = (Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours) / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >例如，如果 [!UICONTROL 默认计划] 为每周40小时，用户的计划为每周30小时， [!UICONTROL FTE] 0.70。
      >  
      >如果用户一天有2个小时的休息时间，则每周可用 [!UICONTROL FTE] 的计算方式如下：
      > 
      >
      ```
      >User Weekly Available [!UICONTROL FTE] = (30-2) / 40 = 0.70
      >```

      <!--drafted for Work Time field:

      <div class="preview">

      In the Preview environment: 
      
      The Available hours for the user is calculated by the following formula:

      ```
      User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]
      ```    

      The Available [!UICONTROL FTE] for the user is calculated by the following formula:

      ```
      User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >For example, if the [!UICONTROL Default Schedule] is 40 hours a week, the schedule of the user is 30 hours a week, and the user's [!UICONTROL Work Time] is 0.5 the [!UICONTROL FTE] of the user is 0.35.
      >
      >If the user has 2 hours of Time off one day, their Weekly Available [!UICONTROL FTE] will be calculated as follows:
      >
      >```
      >User Weekly Available FTE = [(30-2) * 0.5] / 40 = 0.35
      >```
      
      </div>
      -->
1. 单击&#x200B;**[!UICONTROL 保存]**。
