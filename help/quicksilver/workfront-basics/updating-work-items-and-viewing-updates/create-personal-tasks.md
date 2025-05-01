---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Create Personal Tasks
description: Personal tasks are ad hoc work requests that you send to a user, to yourself, or to-do items that you create for yourself in your Home area. Workfront saves ad hoc work requests and to do items as personal tasks.
author: Lisa
feature: Get Started with Workfront
exl-id: b40d6b10-19c7-4e11-a74f-a8af3ebafb65
source-git-commit: a1081b7ce0877b08f9546ab57cfac3f2a580ea76
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 0%

---

# 创建个人任务

<!--Audited: 10/2024-->

Personal tasks are ad hoc work requests that you send to a user or send to or add for yourself.

Adobe Workfront saves ad hoc work requests and to do items as personal tasks on a user&#39;s personal project that is Wprfront automatically creates for each user.

The following are characteristics of a user&#39;s personal project:

* All users in Workfront have a personal project called &quot;&lt; User&#39;s full name>&#39;s Tasks&quot;. For example, &quot;John Smith&#39;s Tasks&quot;.
* The personal project of each user does not display in searches and it is hidden.
* A personal project cannot be deleted, even if users have been deactivated.
* The Status of a personal project is always Current. Personal projects cannot be completed or canceled.
* 所有个人任务都存储在用户的个人项目中。
* 如果需要，您可以将个人任务移动到另一个项目。

您可以通过以下方式创建个人任务：

* 在主页区域创建待办事项

  For information, see [Create work items and projects from the Home area](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

* Create and send a personal work request to another user from the user profile page
* Create and send a personal work request to yourself from your user profile page

This article describes how you can create a personal work request for a user or for yourself from the user profile page.

Regardless how you add a personal task, you can find them in the same areas of Workfront. For more information, see the section [Locate personal task](#locate-personal-tasks) in this article.

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront计划</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront许可证*</strong></td> 
   <td> 
   <p>New: Standard to send requests to other users. All users can create a work request for themselves.</p> 
   <p>Current: Plan to send requests to other users. All users can create a work request for themselves.</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置</strong></td> 
   <td> <p>Edit access to Users to create a work request for them. View access to create a personal work request for yourself. </p>
   </td> 
  </tr>

</tbody> 
</table>

*有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


## 创建个人工作请求

1. 转到您用户的配置文件页面，或转到您有权查看的其他用户的配置文件页面。

   >[!TIP]
   >
   >当某些用户配置您的访问级别时，您的Workfront管理员可能会阻止您查看这些用户。

1. 单击标题中用户名右侧的&#x200B;**更多菜单** ![](assets/more-menu.png)。
1. Click **Send work request**.
The **Send user a work request** box displays.

   ![](assets/personal-task-box.png)
1. 更新以下信息：

   * **Task Name**: This is the name of the ad hoc work request or the personal task.
   * **Description**: Add a description for the task.
   * **Assign to**: The name of the user that you selected displays by default. You can add more users or teams.
   * **Due date**: This is the date by which you&#39;d like this task to be completed. By default, this is today&#39;s date. You cannot select a date in the past
   * **Time**: This is the time by which you&#39;d like this task to be completed. By default, this is the current time.

1. Click **Send Request** to save the work request.

   The work request is saved as a personal task in Workfront and it is added to the user&#39;s To-dos widget in their Home area. If you send the work request to yourself, it displays in your To-dos widget in Home.


## 查找个人任务

您可以在以下区域查找个人任务：

* 将个人请求发送到的用户主页区域中的待办事项小组件。

  有关信息，请参阅[从主页区域创建工作项和项目](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md)。

* 个人任务报告或列表。 You can build and apply a personal task filter to a task report or list to display only personal tasks and exclude project tasks.

  For information, see [Filter: personal tasks](/help/quicksilver/reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-personal-tasks.md).
