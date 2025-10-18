---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 创建个人任务
description: 个人任务是指您发送给用户、自己或您在“主页”区域中为自己创建的待办事项的临时工作请求。 Workfront将临时工作请求和待办事项保存为个人任务。
author: Becky
feature: Get Started with Workfront
exl-id: b40d6b10-19c7-4e11-a74f-a8af3ebafb65
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---

# 创建个人任务

<!--Audited: 10/2024-->

个人任务是指您发送给用户、发送给您自己或您自己添加的临时工作请求。

Adobe Workfront将临时工作请求和待办事项保存为Wprfront自动为每个用户创建的用户个人项目上的个人任务。

以下是用户个人项目的特征：

* Workfront中的所有用户都有一个名为“&lt;用户的全名>的任务”的个人项目。 例如，“John Smith的任务”。
* 每个用户的个人项目不会显示在搜索中，而是处于隐藏状态。
* 无法删除个人项目，即使已停用用户也是如此。
* 个人项目的状态始终为“当前”。 无法完成或取消个人项目。
* 所有个人任务都存储在用户的个人项目中。
* 如果需要，您可以将个人任务移动到另一个项目。

您可以通过以下方式创建个人任务：

* 在主页区域创建待办事项

  有关信息，请参阅[从主页区域创建工作项和项目](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md)。

* 从用户配置文件页面创建个人工作请求并将其发送给另一个用户
* 从用户个人资料页面创建个人工作请求并发送给您自己

本文介绍了如何从用户配置文件页面为用户或您自己创建个人工作请求。

无论您如何添加个人任务，都可以在Workfront的相同区域中找到它们。 有关详细信息，请参阅本文中的[查找个人任务](#locate-personal-tasks)部分。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront包</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront许可证</strong></td> 
   <td> 
   <p>标准<p>
   <p>规划</p>
   <p>这是向其他用户发送请求所需的许可证。 所有用户均可为自己创建工作请求。</p> 
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置</strong></td> 
   <td> <p>编辑对用户的访问权限以为其创建工作请求。 查看访问权限，以便为自己创建个人工作请求。 </p>
   </td> 
  </tr>

</tbody> 
</table>

有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> 
   <p>New: Standard to send requests to other users. All users can create a work request for themselves.</p> 
   <p>Current: Plan to send requests to other users. All users can create a work request for themselves.</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations</strong></td> 
   <td> <p>Edit access to Users to create a work request for them. View access to create a personal work request for yourself. </p>
   </td> 
  </tr> 
 
 </tbody> 
</table>-->


## 创建个人工作请求

1. 转到您用户的配置文件页面，或转到您有权查看的其他用户的配置文件页面。

   >[!TIP]
   >
   >当某些用户配置您的访问级别时，您的Workfront管理员可能会阻止您查看这些用户。

1. 单击标题中用户名右侧的&#x200B;**更多菜单** ![](assets/more-menu.png)。
1. 单击&#x200B;**发送工作请求**。
显示&#x200B;**向用户发送工作请求**&#x200B;框。

   ![](assets/personal-task-box.png)
1. 更新以下信息：

   * **任务名称**：这是临时工作请求或个人任务的名称。
   * **描述**：添加任务的描述。
   * **分配给**：默认情况下显示选定用户的名称。 您可以添加更多用户或团队。
   * **到期日期**：这是您希望完成此任务的日期。 默认情况下，这是今天的日期。 您无法选择过去的日期
   * **时间**：这是您希望完成此任务的截止时间。 默认情况下，这是当前时间。

1. 单击&#x200B;**发送请求**&#x200B;以保存工作请求。

   工作请求将作为个人任务保存在Workfront中，并添加到用户主页区域的待办事项小部件中。 如果将工作请求发送给您自己，它会显示在“主页”的待办事项小部件中。


## 查找个人任务

您可以在以下区域查找个人任务：

* 将个人请求发送到的用户主页区域中的待办事项小组件。

  有关信息，请参阅[从主页区域创建工作项和项目](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md)。

* 个人任务报告或列表。 您可以构建个人任务筛选器并将其应用于任务报告或列表，以仅显示个人任务并排除项目任务。

  有关信息，请参阅[筛选器：个人任务](/help/quicksilver/reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-personal-tasks.md)。
