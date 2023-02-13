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
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 0%

---

# 配置 [!UICONTROL 资源管理] 首选项

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

作为 [!DNL Adobe Workfront] 管理员，您可以配置 [!UICONTROL 资源管理] 系统的首选项。 这些首选项决定了如何为 [!DNL Workfront] 资源计划和规划工具。

有关中的计划和计划资源的信息 [!DNL Workfront]，请参阅 [资源管理入门](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

## 访问要求

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
   <td> <p>系统管理员访问级别</p> <p>有关更多信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> <p><b>注意</b>:如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 配置 [!UICONTROL 资源管理] 首选项

>[!NOTE]
>
>由于这是全局设置，因此此选择会影响整个系统、所有用户、所有资源管理工具以及所有资源池的所有计算。

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).
1. 单击 **[!UICONTROL 资源管理]**.
1. 选择以下方法之一，以计算 [!DNL Workfront]:

   * **默认计划**: [!DNL Workfront] 使用系统的默认计划和用户的单个FTE来计算资源管理工具中用户的可用小时数。\

      有关计划的详细信息，请参阅 [创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      有关用户FTE值的详细信息，请参阅  [编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      Workfront在Workfront管理员选择“默认计划”时使用以下公式计算用户的可用小时数：

      ```
      User Available Hours = (Default Schedule Hours - Exceptions) * FTE - Time off hours
      ```

      **示例:**\
      例如，如果默认计划为每周40小时，而用户配置文件中的FTE为0.5，则用户每周可工作20小时。

      如果用户有一天有1小时的休息时间，则其可用小时数将按如下方式计算：

      ```
      User Available Hours = (40 * 0.5) - 1 = 19 hours
      ```

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

   * **用户的计划**: [!DNL Workfront] 使用用户的计划和系统的默认计划来计算资源管理工具中用户的可用FTE值。 可用小时数仅根据用户的计划进行计算。 将忽略用户的FTE值。 这是默认设置。

      >[!NOTE]
      >
      >如果用户未与计划关联，则使用默认计划计算用户的可用小时数。

      用户的可用FTE由以下公式计算：

      ```
      User Available FTE = (Hours from the Schedule of the User - Time off hours) / Default Schedule Hours
      ```

      **示例：** 例如，如果默认计划为每周40小时，而用户的计划为每周30小时，则用户的FTE为0.75。

      如果用户有一天2小时的休息时间，则其每周可用FTE的计算方式如下：

      ```
      User Weekly Available FTE = (30-2) / 40 = 0.70
      ```

1. 单击&#x200B;**[!UICONTROL 保存]**。
