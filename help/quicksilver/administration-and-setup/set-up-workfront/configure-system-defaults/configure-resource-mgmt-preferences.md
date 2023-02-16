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
source-git-commit: 95c999a72020ce825f3a8377662c71e35a194d80
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 0%

---

# 配置 [!UICONTROL 资源管理] 首选项

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

<span class="preview">此页面上突出显示的信息是指目前尚不普遍可用的功能。 它仅在“预览”环境中可用。</span>

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

## 计算用户容量时考虑的信息

在计算用户容量时，Workfront会考虑以下信息：

* 在用户的计划或Workfront系统的 [!UICONTROL 默认计划]
* [!UICONTROL 计划] [!UICONTROL 例外] (取决于 [!UICONTROL 计划] ，它可以是用户计划的例外，也可以是与 [!DNL Workfront] [!UICONTROL 默认计划])
* 用户的休息时间
* 全时等效项的值([!UICONTROL FTE])或 [!DNL Workfront] 系统。 的 [!UICONTROL FTE] 如计划中所定义，当用户全时工作时等于1。
* <span class="preview">的值 [!UICONTROL 工作时间] 用户，指用户在项目相关工作上花费的时间。 这不包括间接费用时间，如会议和培训。 的 [!UICONTROL 工作时间] 等于1，当用户在 [!UICONTROL FTE] 或是时间表，这意味着他们不会花时间从事与项目无关的工作，如会议或培训。</span>

有关中的计划和计划资源的信息 [!DNL Workfront]，请参阅 [资源管理入门](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).


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


      在生产环境中：

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

      <div class="preview">

      在预览环境中：

      ```
      User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * Work Time
      ```

      >[!INFO]
      >
      >例如，如果默认计划为每周40小时，则用户配置文件中的FTE为0.5，用户一天有1小时的休息时间，并且 [!UICONTROL 工作时间] 在用户的配置文件为0.5时，该用户可以在实际项目工作中每周工作9.5小时。
      >
      >如果用户有一天有1小时的休息时间，则其可用小时数将按如下方式计算：
      >
      >
      ```
      >User Available Hours = [(40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours
      >```

      </div>


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

      在生产环境中：


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

      <div class="preview">

      在预览环境中：

      用户的可用小时数使用以下公式计算：

      ```
      User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]
      ```

      可用 [!UICONTROL FTE] 对于用户，使用以下公式计算：

      ```
      User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >例如，如果 [!UICONTROL 默认计划] 为每周40小时，用户的计划为每周30小时，用户的 [!UICONTROL 工作时间] 是0.5 [!UICONTROL FTE] 0.35。
      >
      >如果用户一天有2个小时的休息时间，则每周可用 [!UICONTROL FTE] 的计算方式如下：
      >
      >
      ```
      >User Weekly Available FTE = [(30-2) * 0.5] / 40 = 0.35
      >```

      </div>

1. 单击&#x200B;**[!UICONTROL 保存]**。
