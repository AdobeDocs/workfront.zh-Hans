---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: 配置资源管理首选项
description: 作为 [!DNL Adobe Workfront] 管理员，您可以为系统配置资源管理首选项。 这些资源管理首选项决定如何为 [!DNL Workfront] 资源计划和计划工具计算用户可用性或容量和FTE。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7cde2238-cb34-4bee-baba-69d256a3912d
source-git-commit: 7f0aac7c8519b1e570e29fedf1492918e8120ad2
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# 配置[!UICONTROL 资源管理]首选项

<!-- Audited: 5/2025 -->

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

作为[!DNL Adobe Workfront]管理员，您可以为系统配置[!UICONTROL 资源管理]首选项。 这些首选项确定[!DNL Workfront]资源计划和计划工具的用户小时或FTE可用性或容量的计算方式。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

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
   <td><p>新增：标准</p>
   或
   <p>当前：计划</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>系统管理员</td>
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 计算用户容量时考虑的信息

在计算用户的容量时，Workfront会考虑以下信息：

* 计划的小时数，如用户的计划或Workfront系统的默认计划中定义。
* 计划例外(根据使用的计划，它可以是用户计划的例外，也可以是与Workfront默认计划关联的例外)。
* 用户的休息时间。
* 用户或[!DNL Workfront]系统的等效全职([!UICONTROL FTE])值。 按照计划中的定义，当用户全职工作时，[!UICONTROL FTE]等于1。
* 用户的[!UICONTROL 工作时间]值，该值表示用户用于项目相关工作的时间。 这不包括额外的时间，如会议和培训。 当用户按照[!UICONTROL FTE]或计划指示的整个时间可用于工作时，[!UICONTROL 工作时间]等于1，这意味着他们不会花费任何时间在会议或培训等与项目无关的工作上。


有关[!DNL Workfront]中计划和计划资源的信息，请参阅[资源管理入门](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md)。


## 配置[!UICONTROL 资源管理]首选项

>[!NOTE]
>
>由于这是全局设置，因此该选择将影响所有资源管理工具中整个系统、所有用户的所有计算。

{{step-1-to-setup}}

1. 单击&#x200B;**[!UICONTROL 资源管理]**。
1. 选择下列方法之一以计算[!DNL Workfront]中用户的可用性：

   * **默认计划**： [!DNL Workfront]使用系统的默认计划和用户的个人FTE在资源管理工具中计算用户的可用小时数。

     有关详细信息，请参阅[创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)和[编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

     选择此选项后，Workfront使用以下公式计算用户的可用小时数：


     `User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * [!UICONTROL Work Time]`


     >[!INFO]
     >
     >例如，如果默认计划为一周40小时，用户配置文件中的FTE为0.5，用户一天有1小时的空闲时间，用户配置文件中的[!UICONTROL 工作时间]为0.5，并且用户每周有9.5小时的实际项目工作时间。
     >
     >如果用户在一天中有1小时的空闲时间，则其可用小时数计算如下：
     >
     >
     >`User Available Hours = [((40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours`
     >

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

   * **用户的计划**： [!DNL Workfront]使用用户的计划以及系统的[!UICONTROL 默认计划]计算资源管理工具中用户的可用[!UICONTROL FTE]值。 可用小时数仅根据用户的计划计算，并且忽略用户的[!UICONTROL FTE]的值。 这是默认设置。

     有关详细信息，请参阅[创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)和[编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

     >[!NOTE]
     >
     >如果用户未与计划关联，则仅使用[!UICONTROL 默认计划]计算用户的可用小时数。

     用户的可用小时数按以下公式计算：


     `User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]`


     用户可用的[!UICONTROL FTE]按以下公式计算：


     `User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours`


     >[!INFO]
     >
     >例如，如果[!UICONTROL 默认计划]是一周40小时，用户的计划是一周30小时，用户的[!UICONTROL 工作时间]是0.5，用户的[!UICONTROL FTE]是0.35。
     >
     >如果用户一天有2小时的休息时间，其每周可用时间[!UICONTROL FTE]的计算如下：
     >
     >
     >`User Weekly Available [!UICONTROL FTE] = [(30-2) * 0.5] / 40 = 0.35`
     >

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
