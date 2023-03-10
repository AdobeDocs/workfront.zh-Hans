---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: 配置资源管理首选项
description: 作为 [!DNL Adobe Workfront] 管理员可以为系统配置资源管理首选项。 这些资源管理首选项决定如何计算用户可用性或容量以及FTE [!DNL Workfront] 资源调度和计划工具。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7cde2238-cb34-4bee-baba-69d256a3912d
source-git-commit: 921749caf6a61fa4f0efae9357c6e05c581421c5
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 0%

---

# 配置 [!UICONTROL 资源管理] 偏好设置

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

作为 [!DNL Adobe Workfront] 管理员您可以配置 [!UICONTROL 资源管理] 您系统的首选项。 这些首选项确定如何计算的用户小时数或FTE可用性或容量 [!DNL Workfront] 资源调度和计划工具。

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
   <td>[！UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>系统管理员访问级别</p> <p>有关更多信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> <p><b>注释</b>:

如果您仍然没有访问权限，请咨询 [!DNL Workfront] 管理员（如果他们在您的访问级别设置了其他限制）。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参见 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
 </tbody> 
</table>

## 计算用户容量时考虑的信息

在计算用户的容量时，Workfront会考虑以下信息：

* 计划的小时数，如用户的计划或Workfront系统的计划中定义 [!UICONTROL 默认计划]
* [!UICONTROL 计划] [!UICONTROL 例外] (取决于哪些 [!UICONTROL 计划] ，它可以是用户计划的例外，也可以是与 [!DNL Workfront] [!UICONTROL 默认计划])
* 用户的空闲时间
* 相当于全时的工作时间的值([!UICONTROL FTE])，或用户的 [!DNL Workfront] 系统。 此 [!UICONTROL FTE] 等于1表示用户全职工作，如计划中所定义。
* 的值 [!UICONTROL 工作时间] （指用户花费在项目相关工作上的时间）。 这不包括额外的时间，如会议和培训。 此 [!UICONTROL 工作时间] 等于1（当用户可工作整个时间时），如 [!UICONTROL FTE] 或者时间表，这意味着他们不会花任何时间在会议或培训等与项目无关的工作上。


有关中计划和计划资源的信息 [!DNL Workfront]，请参见 [资源管理入门](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).


## 配置 [!UICONTROL 资源管理] 偏好设置

>[!NOTE]
>
>由于这是全局设置，因此该选择会影响所有资源管理工具中整个系统、所有用户的所有计算。

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) （位于的右上角） [!DNL Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).
1. 单击 **[!UICONTROL 资源管理]**.
1. 选择以下方法之一以计算用户在中可用性 [!DNL Workfront]：

   * **默认计划**： [!DNL Workfront] 使用系统的默认计划和用户的单个FTE在资源管理工具中计算用户的可用小时数。

      有关时间表的详细信息，请参见 [创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      有关查找用户的 [!UICONTROL FTE]，请参见  [编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      当WorkfrontWorkfront管理员选择 [!UICONTROL 默认计划]：


      `User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * [!UICONTROL Work Time]`


      >[!INFO]
      >
      >例如，如果默认时间表是一周40小时，则用户配置文件中的FTE为0.5，用户一天有1小时的空闲时间，并且 [!UICONTROL 工作时间] 在用户配置文件中，用户为0.5，每周实际项目工作时间为9.5小时。
      >
      >如果用户一天有1小时的空闲时间，则其可用小时数的计算如下：
      >
      >
      >`User Available Hours = [((40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours`

      <!--This used to be the calculation before we implemented the Work Time field: 
    
      ```
      User Available Hours = ([!UICONTROL Default Schedule] Hours - Exceptions) * FTE - Time off hours
      ```

      >[!INFO]
      >
      > For example, if the [!UICONTROL Default Schedule] is 40 hours a week and the [!UICONTROL FTE] in the profile of the user is 0.5, the user is available to work for 20 hours a week.
      >If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:
      >
      >```
      >User Available Hours = [(40 - 0) * 0.5)] - 1 = 19 hours
      >```
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

   * **用户的计划**： [!DNL Workfront] 使用用户的计划以及 [!UICONTROL 默认计划] ，以计算可用的 [!UICONTROL FTE] 用户在resource management工具中的值。 可用小时数仅根据用户的计划计算。 的值 [!UICONTROL FTE] 忽略用户的ID。 这是默认设置。

      有关时间表的详细信息，请参见 [创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      有关用户的详细信息 [!UICONTROL 计划]，请参见  [编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      >[!NOTE]
      >
      >如果用户未与计划关联，则用户的可用小时数将只使用 [!UICONTROL 默认计划].

      用户的可用小时数按以下公式计算：


      `User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]`


      可用 [!UICONTROL FTE] ，按以下公式计算：


      `User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours`


      >[!INFO]
      >
      >例如，如果 [!UICONTROL 默认计划] 安排的时间是一周40小时，用户的时间安排是一周30小时，而用户的 [!UICONTROL 工作时间] 是0.5 [!UICONTROL FTE] 用户为0.35。
      >
      >如果用户一天有2小时的休息时间，则每周可用 [!UICONTROL FTE] 将按如下方式计算：
      >
      >
      >`User Weekly Available [!UICONTROL FTE] = [(30-2) * 0.5] / 40 = 0.35`

      <!--This used to be the calculation before we implemented the Work Time field: 
      

      The Available hours for the user are calculated by the following formula:

      ```
      User Available Hours = Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours
      ```  

      The Available [!UICONTROL FTE] for the user is calculated by the following formula:

      ```
      User Available [!UICONTROL FTE] = (Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours) / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >For example, if the [!UICONTROL Default Schedule] is 40 hours a week and the schedule of the user is 30 hours a week, the [!UICONTROL FTE] of the user is 0.70.
      >  
      >If the user has 2 hours of Time off one day, their Weekly Available [!UICONTROL FTE] will be calculated as follows:
      > 
      >```
      >User Weekly Available [!UICONTROL FTE] = (30-2) / 40 = 0.70
      >```
      -->

1. 单击&#x200B;**[!UICONTROL 保存]**。
