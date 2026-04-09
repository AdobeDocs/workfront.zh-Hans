---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 创建高级工作
description: 您可以使用“高级工作”管理任务或问题工作。
author: Lisa
feature: Work Management, Resource Management
role: User
exl-id: 09780f78-4eb8-404d-859b-d066d462776d
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 676cd1697ae2f379a699075f4e1ab06886c6837a
workflow-type: tm+mt
source-wordcount: '3415'
ht-degree: 0%

---

# 创建高级工作

{{highlighted-preview}}

<!-- Audited: 11/2025-->

<!--remove the bullet indicated when we get rid of the new/old experience of editing tasks-->


<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>
-->

您可以使用“高级工作”管理任务或问题工作。

在进行高级分配时，您可以调整以下分配信息：

* 将用户分配给任务或问题（可在高级分配之外完成）。
* 调整并重新分配每个被分配人的分配小时数。
* 确定应指定为任务或问题的所有者或主要受分配人的用户。
* 指定每个用户在处理任务或问题时执行的角色。
* <span class="preview">在分配级别添加计费和成本费率信息。</span>
* <span class="preview">查看每个分配的以下详细信息：计划小时数、总成本和总收入。</span>

>[!NOTE]
>
>在分配用户进行工作时，其根据时间表的可用性会影响任务和问题的计划和预计日期。 有关计划的信息，请参阅[创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

## Adobe Workfront中可执行高级任务的区域

本文介绍了如何在任务或问题的标题中访问高级工作。

此外，您还可以在Workfront的以下区域进行高级分配：

* 在列表和报表中，当“工作总揽”字段显示在视图中时。
* 编辑任务时显示在“工作总揽”部分。 有关详细信息，请参阅[编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md)。<!--When we remove the old/ new experience: take this bullet out completely; in the new Edit Task experience, this is no longer possible-->
* 在任务或问题标题的工作区区域中。
* 在工作负载均衡器中。 有关详细信息，请参阅[使用工作负载均衡器手动分配工作](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 包</td> 
   <td> <p>要在任务分配中添加计费和成本率，并使用高级搜索：工作流Ultimate</p> <p>要创建高级分配：任何Workfront或工作流包</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td> <p>标准</p>
   <p>工作版或更高版本</p>
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

<div class="preview">

## 创建高级工作 — 工作流Ultimate包

此高级工作分配布局仅适用于任务。 有关问题，请参阅[创建高级工作 — 所有其他包](#create-advanced-assignments--all-other-packages)。

1. 转到要分配任务的项目。
1. 单击左侧面板中的&#x200B;**任务**&#x200B;或&#x200B;**问题**，然后单击列表中任务的名称。

   >[!TIP]
   >
   >您可以直接在任务列表中进行高级分配。 单击任务所在行上的&#x200B;**工作**&#x200B;字段，然后单击列表底部的&#x200B;**高级**&#x200B;或工作框右上角的&#x200B;**人员图标**以打开“高级工作”窗口。 跳至步骤5以继续创建高级工作。
   >![单击“高级”或“人员”图标](assets/access-aa-from-lists.png)

1. 在任务标题的&#x200B;**工作**&#x200B;字段中单击&#x200B;**分配给**

   或

   如果任务已分配，请单击其中一个已分配名称。

1. 单击&#x200B;**高级**。

   ![单击高级](assets/assignments-from-task-header-0825.png)

   此时将出现“高级分配”窗口。

   ![高级工作窗口](assets/advanced-assignments-031826.png)

1. 根据需要查看任务持续时间信息。 这些字段都是仅供查看的高级工作分配，您可以在任务中更新它们。

   有关任务持续时间、持续时间类型、时间单位和已计划小时数的信息，请参阅[任务持续时间和持续时间类型概览](/help/quicksilver/manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)。

   >[!NOTE]
   >
   >如果要查看的数据列未显示，您可以添加它。 请参阅下面的“高级工作分配”列表[中的](#add-and-remove-columns-on-the-advanced-assignments-list)添加和删除列。

1. （可选）选择&#x200B;**小时**、**FTE**&#x200B;或&#x200B;**百分比**&#x200B;以查看分配。

   您可以按容量百分比或FTE（全职等效人数，0-1分制）查看在计划小时数中分配的用户数量。 默认设置为“小时”。

   有关FTE的信息，请参阅[配置资源管理首选项](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

1. 单击&#x200B;**新行**&#x200B;以向任务添加分配。

1. 单击&#x200B;**代理人**&#x200B;列以添加用户或团队。 开始键入用户或团队的名称，然后在该名称出现在下拉列表中时单击该名称。

   >[!NOTE]
   >
   >如果名称包含特殊字符，则必须在搜索字段中包含特殊字符。

   添加具有主要工作角色的用户时，将填充&#x200B;**被分派人角色**。

   如果用户为其配置文件分配了属性，则这些属性将填充在任务分配中。

1. 要在不认识将处理任务的用户时添加工作角色，请单击&#x200B;**被分派人角色**&#x200B;列。 开始键入工作角色的名称，然后在该名称出现在下拉列表中时单击该名称。

   >[!NOTE]
   >
   >如果名称包含特殊字符，则必须在搜索字段中包含特殊字符。

   如果工作角色具有从项目的费率卡分配的属性，则这些属性将填充到任务分配中。

   当您稍后使用被分派人字段分配用户时，基本搜索将遵循此算法：

   * 完全匹配：工作角色和所有属性
   * 部分匹配：工作角色和一些属性
   * 仅工作角色匹配

   有关高级搜索的信息，请参阅本文中的[使用高级搜索](#use-the-advanced-search)。

1. （可选）继续在新行中添加被分配人，以将多个资源添加到该任务。

   >[!TIP]
   >
   >* 您可以分配多个用户、工作角色或团队。 您只能分配活动用户、工作角色和团队。 每个任务最多允许200个被分配人。
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

1. 要将被分派人标记为任务所有者，请选中该行的复选框，然后单击“高级工作”窗口底部操作栏中的&#x200B;**设置主要任务**。

   默认情况下，Workfront会将您分配给任务的第一个用户或工作角色标记为“所有者”或“主要分配”。 不能将团队指定为任务的主要所有者。

   如果未显示任务的主要所有者，您可以将&#x200B;**Is Primary**&#x200B;列添加到表中。

   >[!IMPORTANT]
   >
   >根据您的Workfront管理员或组管理员如何设置项目首选项，当您有多个用户分配到任务时，Workfront可能会使用任务所有者的时间表计算任务的时间表。 有关多个任务被分配人的信息，请参阅文章[分配任务](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md#considerations-for-multiple-assignments-to-job-roles-teams-and-users)中的[对工作角色、团队和用户的多个分配的注意事项](../../../manage-work/tasks/assign-tasks/assign-tasks.md)部分。

1. 对于&#x200B;**代理人**&#x200B;列中的每个用户，请指定以下信息：

   * （可选） **用于计费的工作角色**：搜索并选择用于为此特定被分配人和任务计费的工作角色。

     计费工作角色仅用于此分配，不会自动应用于用户的其他分配。 例如，用户的主要工作角色是Designer，但在某项任务中，他们作为高级Designer发挥作用，记帐费率应反映这一点。 用于计费的工作角色仅适用于用户，不能用于其他工作角色。

     当用户分配应用计费工作角色时，可以在计费和收入计算中使用附加到计费工作角色的费率，而不是用户或工作角色费率。

     也可以为用户设置项目级别的工作角色以进行计费，该值用于用户在该项目中的所有分配。

     有关详细信息，请参阅[设置工作角色以进行计费](/help/quicksilver/manage-work/projects/project-finances/set-up-job-role-for-billing.md)。

   * **分配**：当任务的持续时间类型为“简单”时，指定每个用户或工作角色应分配给该任务的小时数。 每个用户的所有分配小时数之和等于“高级分配”窗口顶部&#x200B;**计划小时数**&#x200B;字段中的数字。 在所有其它情况下，指定您希望被分派人解决任务所花费的时间（或分配）百分比。

     >[!TIP]
     >
     >在手动修改任务的分配分配后，任务的已计划小时数可能会相应地更新。 请注意，您不能手动修改分配给任务的团队的分配。 有关详细信息，请参阅文章[计划小时概述](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md#update-task-planned-hours-when-managing-user-allocations)中的[管理用户分配时更新任务计划小时数](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md)部分。

   * **属性**：任何可用于用户的属性都会显示在属性字段中。 管理员设置属性，这些属性将添加到用户配置文件或与费率卡中的工作角色关联。 有关详细信息，请参阅[定义费率属性](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md)和[编辑用户配置文件](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

     属性当前在用户分配上是只读的。 它们对于工作角色可编辑。

   * **费率币种**：记帐和成本费率的币种默认自项目，但您可以更改此分配的币种。

   * （可选） **记帐费率**：记帐费率可能来自系统的其他区域，如费率卡。 有关详细信息，请参阅[收入和成本层次结构概览](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)。 您可以在此字段中手动覆盖此特定分配的记帐费率，它将在收入计算中覆盖用户的所有其他费率。
   * （可选） **成本费率**：成本费率可能来自系统的其他区域。 有关详细信息，请参阅[收入和成本层次结构概览](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)。 您可以在此字段中人工改写此特定分配的成本费率，它将在成本计算中改写用户的所有其它费率。
   * **可记帐**：选择此选项可在财务计算中包括分配。 清除此选项可从财务计算中排除分配。

     当任务具有收入类型时，此字段默认对所有分配启用。

1. （可选）要按日期查看用户或角色的分配数据，请选择表行，然后单击“高级分配”窗口底部操作栏中的&#x200B;**按日期查看**。 有关详细信息，请参阅本文中的[按日期查看分配数据](#view-assignment-data-by-dates)。
1. （可选）要从列表中删除一个或多个分配，请选中每行的复选框，然后单击“高级分配”窗口底部操作栏中的&#x200B;**删除**。
1. 编辑完高级工作分配后，单击&#x200B;**保存**&#x200B;或&#x200B;**保存并关闭**。

### 在高级工作分配列表中添加和删除列

在将字段添加到列表之前，这些字段必须存在。

1. 单击列表右上角的&#x200B;**+**&#x200B;以打开&#x200B;**列管理器**。

   ![高级工作分配列管理器](assets/aa-column-manager.png)

1. 选择&#x200B;**属性**&#x200B;选项卡或&#x200B;**KPI**&#x200B;选项卡以选择要添加的字段类型。

   位置或成本中心等属性提供上下文信息。 时间分段KPI，例如跨时间期的收入或成本细分值。

1. 在&#x200B;**可用**&#x200B;部分中搜索现有对象字段，然后单击该字段名称右侧的&#x200B;**+**&#x200B;以将其添加到&#x200B;**已选定**&#x200B;列。
1. 单击&#x200B;**选定的**&#x200B;部分中字段右侧的&#x200B;**-**&#x200B;以将其从列表中删除。
1. 单击&#x200B;**保存**。

   有关列管理器的详细信息，请参阅[使用增强列表](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。

### 将视图应用于“高级工作”列表

视图是您可以应用于列表的列安排的个性化集。

1. 单击&#x200B;**视图**&#x200B;下拉列表，然后选择要应用于该列表的视图。

   **系统视图**&#x200B;是系统管理员添加的视图，无法对其进行更改。 **我的视图**&#x200B;是您创建的或与您共享的视图。

1. 单击&#x200B;**视图**&#x200B;下拉列表中的&#x200B;**新建视图**&#x200B;以创建视图。

   添加、删除或重新排序列时，更改将自动保存到视图中。 下次应用此视图时，列将保留您设置它们的方式。

   有关视图的详细信息，请参阅[使用增强列表](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。

### 使用高级搜索

高级搜索可帮助您找到要添加到分配的正确用户或工作角色。

1. 要打开高级搜索窗口，请执行下列操作之一：

   * 单击“高级工作”窗口右上角的&#x200B;**高级搜索**。
   * 选择一个分配行，然后单击“高级分配”窗口底部操作栏中的&#x200B;**高级搜索**。 这将打开高级搜索，并自动为该特定分配应用过滤器。

1. 在高级搜索窗口中选择用户或职位角色选项卡。
1. 根据需要应用过滤器：

   1. 单击列表上方的&#x200B;**筛选器**。
   1. 在“筛选器”框中，单击&#x200B;**添加条件**。
   1. 选择要作为筛选依据的字段。
   1. 选择过滤器修饰符，例如“具有任意”、“不具有任何”、“早于”或“晚于”。 根据过滤依据的字段类型，修改量选项会有所不同。
   1. 选择一个或多个字段值。 根据筛选依据的字段类型，系统可能会提示您从列表中选择项目、搜索该项目或使用日历选择日期范围。

   该过滤器将自动应用于列表。 有关筛选器的详细信息，请参阅[使用增强列表](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。

1. 搜索工作角色或用户。

   在搜索与工作角色分配匹配的用户时，仅显示完全匹配项（工作角色和所有属性）。

1. 单击&#x200B;**+**&#x200B;向表中添加列。 有关详细信息，请参阅[在高级工作分配列表](#add-and-remove-columns-on-the-advanced-assignments-list)中添加和删除列。
1. 选择一个或多个用户或工作角色，然后单击窗口底部操作栏中的&#x200B;**添加用户**&#x200B;或&#x200B;**添加角色**。

   这些分配将添加到“高级分配”窗口中。

### 按日期查看分配数据

高级分配的&#x200B;**按日期查看**&#x200B;窗口显示特定用户或角色的分配的整个日期有效历史记录。 将显示过去和将来的更改。

可能影响分配历史记录的日期有效项的示例包括：

* 用户的主要/其他职位角色
* 用于计费的项目级别工作角色
* 用户配置文件记帐/成本率
* 项目覆盖计费/成本率（用户或工作角色）
* 按工作角色/属性评级卡费率
* 用户属性
* 用户计划

请注意，这不是一个全面的列表，并且已更改的字段不一定显示在分配数据表中，但它会影响用户或工作角色的计费和成本费率或属性。

您只能按日期查看单个用户或角色的分配数据。

1. 为用户或角色选择表行，然后单击“高级工作”窗口底部操作栏中的&#x200B;**按日期查看**。

   出现&#x200B;**按日期查看**&#x200B;窗口。 数据是只读的。

   表中的每一行都表示分配的日期有效更改。 如果尚未进行任何日期有效更改，则该表将有一行显示当前数据。 突出显示的字段指示已更改的内容，并列出每次更新的开始和结束日期。 例如，如果记帐费率从8月20日的202改为8月21日的205，则会突出显示该费率。 括号中的文本指示对费率进行更改的位置，例如项目。

   ![按日期范围查看](assets/resource-changes-view-by-dates.png)

   查看完数据后，单击左上角的箭头返回“高级工作”窗口。

</div>

## 创建高级工作 — 所有其他包

此高级工作分配布局适用于任务和问题。

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

1. 对于&#x200B;**代理人**&#x200B;列中的每个用户，请指定以下信息：

   * **所有者**：将鼠标悬停在任务接受者的名称上，如果要将任务接受者标记为任务或问题所有者，请在“所有者”字段中单击&#x200B;**成为主要所有者**。 绿色复选框表示指定用户是任务或问题的主要联系人。 Adobe Workfront将您分配给任务或问题的第一个用户或工作角色标记为“所有者”或“主要分配”。 不能将团队指定为任务或问题的主要所有者。

     >[!IMPORTANT]
     >
     >根据您的Workfront管理员或组管理员如何设置项目首选项，当您有多个用户分配到任务时，Workfront可能会使用任务所有者的时间表计算任务的时间表。 有关多个任务被分配人的信息，请参阅文章[分配任务](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md#considerations-for-multiple-assignments-to-job-roles-teams-and-users)中的[对工作角色、团队和用户的多个分配的注意事项](../../../manage-work/tasks/assign-tasks/assign-tasks.md)部分。

   * **分派工作**：当任务的持续时间类型为“简单”时，指定每个用户或工作角色应分配给该任务的小时数。 每个用户的所有已分配小时数的总和等于“分配”列底部&#x200B;**已计划小时数**&#x200B;字段中的数字。 在所有其它情况下，指定您希望被分派人解决任务或问题所花费的时间（或分配）百分比。

     >[!TIP]
     >   
     >   * 在手动修改任务的分配分配后，任务的已计划小时数可能会相应地更新。 有关详细信息，请参阅文章[计划小时概述](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md#update-task-planned-hours-when-managing-user-allocations)中的[管理用户分配时更新任务计划小时数](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md)部分。
     >   * 您无法手动修改问题的分配分配。
     >   * 您无法手动修改分配给任务的团队的分配。

   * **被分派人的角色：**&#x200B;选择用户在完成此分派时应使用的角色。  默认情况下，将显示用户的主要角色。 单击&#x200B;**被分派人的角色**&#x200B;框以选择其他角色。 在将任务或问题首先分配给角色，然后添加可以履行该角色的用户作为第二次分配时，将为可以履行已分配给任务和问题的角色的用户过滤建议用户列表。

     ![被分派人的角色](assets/advanced-assignments-select-role.png)

   * **持续时间类型**：这仅适用于任务。 单击持续时间类型的名称，然后从下拉菜单中选择持续时间类型。 有关持续时间类型的信息，请参阅[任务持续时间和持续时间类型概览](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)。

   * **工期：**&#x200B;当您拥有任务的管理权限时，可以为任务更新此字段。

     有关详细信息，请参阅[任务持续时间和持续时间类型概述](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)。 批量编辑分配信息时，会出现一个类似的对话框，用于分配用户、小时、分配和任务所有者。

   * **计划小时数**：当持续时间类型为计算分配或简单时，更新计划小时数。 因此，每个资源的分配百分比或小时数会平均分配。 当持续时间类型为计算工作或投入比驱动时，Workfront会计算已计划小时数。 有关详细信息，请参阅[任务持续时间和持续时间类型概述](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)。

1. 单击&#x200B;**保存**。


