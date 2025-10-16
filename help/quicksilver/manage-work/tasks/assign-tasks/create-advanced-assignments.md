---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 创建高级工作
description: 您可以使用“高级工作”管理任务或问题工作。
author: Lisa
feature: Work Management, Resource Management
role: User
exl-id: 09780f78-4eb8-404d-859b-d066d462776d
source-git-commit: e1580f7b9065fce7bb31ab0c7edb00fd2856e1df
workflow-type: tm+mt
source-wordcount: '1118'
ht-degree: 0%

---

# 创建高级工作

<!-- Audited: 07/2024-->

您可以使用“高级工作”管理任务或问题工作。

在进行高级分配时，您可以调整以下分配信息：

* 将用户分配给任务或问题（可在高级分配之外完成）。
* 调整并重新分配每个被分配人的分配小时数。
* 确定应指定为任务或问题的所有者或主要受分配人的用户。
* 指定每个用户在处理任务或问题时执行的角色。
  <!--* <span class="preview">Override the billing rate for a job role.</span>-->

>[!NOTE]
>
>在分配用户进行工作时，其根据时间表的可用性会影响任务和问题的计划和预计日期。 有关计划的信息，请参阅[创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

## Adobe Workfront中可执行高级任务的区域

本文介绍了如何在任务或问题的标题中访问高级工作。

此外，您还可以在Workfront的以下区域进行高级分配：

* 在列表和报表中，当“工作总揽”字段显示在视图中时。
* 编辑任务时显示在“工作总揽”部分。 有关详细信息，请参阅[编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md)。
* 在任务或问题标题的工作区区域中。
* 在工作负载均衡器中。 有关详细信息，请参阅[使用工作负载均衡器手动分配工作](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td> <p>标准</p>
   <p>工作或更高</p>
   </td> 
  </tr> 
  <tr> 
   <td role>访问级别配置</td> 
   <td> <p>编辑对任务和问题的访问权限</p>  </td> 
  </tr> 
  <tr> 
   <td>对象权限</td> 
   <td> <p>向任务或问题分配或更高权限</p></td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 进行高级工作

1. 转到要分配任务或问题的项目。
1. 单击左侧面板中的&#x200B;**任务**&#x200B;或&#x200B;**问题**，然后单击列表中任务或问题的名称。

   >[!TIP]
   >
   >您可以直接在任务或问题列表中进行高级分配。 单击任务或问题所在行上的&#x200B;**工作**&#x200B;字段，然后单击列表底部的&#x200B;**高级**&#x200B;或工作框右上角的&#x200B;**人员图标**以打开“高级工作”窗口。 跳至步骤5以继续创建高级工作。
   >![单击“高级”或“人员”图标](assets/access-aa-from-lists.png)

1. 单击任务或问题标题中&#x200B;**工作**&#x200B;字段中的&#x200B;**分配给**

   或

   如果任务或问题已分配，请单击其中一个已分配名称。

1. 单击&#x200B;**高级**。

   ![单击高级](assets/assignments-from-task-header-0825.png)

1. 在&#x200B;**搜索人员、角色和团队**&#x200B;字段中，开始键入用户、角色或团队的名称，然后在该名称出现在下拉列表中时单击该名称。

   >[!NOTE]
   >
   >如果用户名包含特殊字符，则必须在搜索字段中包含特殊字符。

1. （可选）继续在&#x200B;**搜索人员、角色和团队**&#x200B;框中添加被分配人，以将多个资源添加到任务或问题。

   >[!TIP]
   >
   >* 您可以分配多个用户、工作角色或团队。 您只能分配活动用户、工作角色和团队。
   >
   >
   >* 添加用户分配时，请注意头像、用户的主要角色或其电子邮件地址，以区分具有相同名称的用户。
   >用户必须与至少一个工作角色关联，才能在添加时查看工作角色。
   >您必须在访问级别中启用“查看联系信息”设置，用户才能查看用户的电子邮件。 有关信息，请参阅[授予用户访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)。
   >
   >
   >* 如果在停用用户、工作角色或团队之前已分配用户、工作角色或团队，则仍将其分配给工作项目。 在这种情况下，我们建议执行以下操作：
   >   
   >   * 将工作项重新分配给活动资源。
   >   * 将已停用团队中的用户与活动团队关联，并将工作项重新分配给活动团队。

   <!-- SHOULD BE THIRD BULLET POINT IN TIP TABLE WHEN THIS FEATURE IS RELEASED 
    * <span class="preview">When adding a job role assignment, you can search for the job role or location. Select the System/Default Job Role to use the default billing rate for the assignment, or select a Rate Card Job Role to override the rate at the assignment level. For more information on rate cards, see [Manage rate cards](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>
    -->

1. 对于&#x200B;**代理人**&#x200B;列中的每个用户，请指定以下信息：


   * **所有者**：将鼠标悬停在任务接受者的名称上，如果要将任务接受者标记为任务或问题所有者，请在“所有者”字段中单击&#x200B;**成为主要所有者**。 绿色复选框表示指定用户是任务或问题的主要联系人。 Adobe Workfront将您分配给任务或问题的第一个用户或工作角色标记为“所有者”或“主要分配”。 不能将团队指定为任务或问题的主要所有者。

     >[!IMPORTANT]
     >
     >根据您的Workfront管理员或组管理员如何设置项目首选项，当您有多个用户分配到任务时，Workfront可能会使用任务所有者的时间表计算任务的时间表。 有关多个任务被分配人的信息，请参阅文章[分配任务](../../../manage-work/tasks/assign-tasks/assign-tasks.md)中的“将多个用户分配给任务”部分。

   * **分派工作**：当任务的持续时间类型为“简单”时，指定每个用户或工作角色应分配给该任务的小时数。 每个用户的所有已分配小时数的总和等于“分配”列底部&#x200B;**已计划小时数**&#x200B;字段中的数字。 在所有其它情况下，指定您希望被分派人解决任务或问题所花费的时间（或分配）百分比。

     >[!TIP]
     >   
     >   * 在手动修改任务的分配分配后，任务的已计划小时数可能会相应地更新。 有关更多信息，请参阅文章[计划小时数概述](../../../manage-work/tasks/task-information/planned-hours.md)中的“管理用户分配时更新任务计划小时数”部分。
     >   * 您无法手动修改问题的分配分配。
     >   * 您无法手动修改分配给任务的团队的分配。

   * **被分派人的角色：**&#x200B;选择用户在完成此分派时应使用的角色。  默认情况下，将显示用户的主要角色。 单击&#x200B;**被分派人的角色**&#x200B;框以选择其他角色。 在将任务或问题首先分配给角色，然后添加可以履行该角色的用户作为第二次分配时，将为可以履行已分配给任务和问题的角色的用户过滤建议用户列表。

     ![被分派人的角色](assets/advanced-assignments-select-role.png)

   <!--<div class="preview">

   * **Location**: The location comes from the rate card, if a rate card attached to the project uses locations with the job roles. The location can't be changed. 

   * **Billing Rates**: The billing rate for a user comes from the system rate for the user or their associated job role. The billing rate for a job role comes from the system rate or from the rate card, if a rate card is attached to the project. Existing billing rates are not displayed in this field. Click in the field to change the billing rate for this specific task assignment.

   </div>-->

   * **持续时间类型**：这仅适用于任务。 单击持续时间类型的名称，然后从下拉菜单中选择持续时间类型。 有关持续时间类型的信息，请参阅[任务持续时间和持续时间类型概览](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)。

   * **工期：**&#x200B;当您拥有任务的管理权限时，可以为任务更新此字段。

     有关详细信息，请参阅[任务持续时间和持续时间类型概述](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)。 批量编辑分配信息时，会出现一个类似的对话框，用于分配用户、小时、分配和任务所有者。

   * **计划小时数**：当持续时间类型为计算分配或简单时，更新计划小时数。 因此，每个资源的分配百分比或小时数会平均分配。 当持续时间类型为计算工作或投入比驱动时，Workfront会计算已计划小时数。 有关详细信息，请参阅[任务持续时间和持续时间类型概述](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)。

1. 单击&#x200B;**保存**。
