---
product-area: resource-management
keywords: 工作，团队，员工，资源
navigation-topic: the-workload-balancer
title: 找到工作负载均衡器
description: 工作负载均衡器可用于资源区域中的多个项目、团队、项目和用户。
author: Lisa
feature: Resource Management
exl-id: 88029c9d-b588-4d33-801a-04f49b12a6e8
source-git-commit: a63c53652491a25b909b7563990d4375d8f5885f
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 0%

---

# 找到工作负载均衡器

{{preview-fast-release-general}}

您可以使用工作负载均衡器来计划工作的资源，或查看其可用性和当前分配。

您可以通过以下方式访问工作负载均衡器：

* 从Adobe Workfront预定义的多个区域
* 将其添加到自定义分区

本文介绍了可以访问工作负载均衡器的区域。

>[!NOTE]
>
>无论您使用何种方法访问工作负载均衡器，导航它和管理资源都是相同的。
>
>有关工作负载均衡器以及如何使用它管理和计划您的工作资源的信息，请参阅以下文章：
>
>* [工作负载均衡器概述](../../resource-mgmt/workload-balancer/overview-workload-balancer.md)
>* [导航工作负载均衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)
>* [在工作负载均衡器中分配工作的概述](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)
>* [在工作负载均衡器中管理用户分配](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>新增：标准</p>
       <p>或</p>
       <p>当前：计划，在资源区域使用工作负载均衡器时；</br>
       工作，使用团队或项目的工作负载均衡器时</p>
       <p><span class="preview">注意：所有用户都可以在自己的用户配置文件中访问工作负载均衡器，而无需任何许可证要求。</span></p></td>
  </tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>查看以下内容或更高访问权限：</p> 
    <ul> 
     <li>资源管理</li> 
     <li>项目</li> 
     <li>任务</li> 
     <li>问题</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td>查看项目、任务和问题的权限或更高版本</td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在预定义区域访问工作负载均衡器

以下部分说明了可在Workfront中访问工作负载均衡器的位置。

### 在资源区访问多个项目的工作负载均衡器

{{step1-to-resourcing}}

1. 单击左侧面板中的&#x200B;**工作负载均衡器**。

   ![工作负载平衡器](assets/nwe-balancer-global.png)

   默认情况下，工作负载均衡器按资源区域中的信息显示以下内容：

   * **未分配的工作**：没有未分配的工作项。
   * **已分配的工作**：系统中的所有活动用户。

     在“已分配的工作”区域显示用户时，我们建议使用过滤器。 有关详细信息，请参阅工作负载均衡器[中的](../workload-balancer/filter-information-workload-balancer.md)过滤器信息。

### 访问团队的工作负载均衡器

有关Workfront中团队的更多信息，请参阅[团队概述](/help/quicksilver/people-teams-and-groups/create-and-manage-teams/teams-overview.md)。

{{step1-to-team}}

此时将显示您的主团队的页面。

1. 单击左侧面板中的&#x200B;**工作负载均衡器**。

   ![团队的工作负载均衡器](assets/nwe-balancer-team-350x172.png)

   默认情况下，团队的工作负载均衡器显示以下信息：

   * **未分配的工作**：已分配给团队但未分配给用户的项目。
   * **已分派的工作**：团队的所有成员及其所有分派的工作。

     >[!TIP]
     >
     >团队成员可能被分配到也分配给团队的工作，或被分配到其他团队或角色的工作。

### 访问项目的工作负载均衡器

{{step1-to-projects}}

1. 单击项目名称以打开项目页面。
1. 单击左侧面板中的&#x200B;**工作负载均衡器**。

   此时将显示项目的工作负载均衡器。

   ![项目的工作负载均衡器](assets/nwe-balancer-project-350x152.png)

   默认情况下，项目的工作负载均衡器按信息显示以下内容：

   * **未分配的工作**：项目中分配给工作角色或团队但未分配给用户的项。
   * **已分配工作**：已分配给项目项的用户。

     >[!TIP]
     >
     >通过启用“显示所有用户”选项，可以显示系统中的所有用户，而不仅仅是项目中的用户（在“已分配的工作”区域中）。 有关信息，请参阅[在工作负载均衡器](../workload-balancer/navigate-the-workload-balancer.md)中导航。

<div class="preview">

### 访问用户的工作负载均衡器

所有用户都有权在其自己的配置文件上查看工作负载均衡器。 用户的工作负载均衡器数据是只读的。 您不能在用户层分配工作、取消分配工作或调整分配。

所有显示设置都可用于用户的工作负载均衡器。 有关详细信息，请参阅[导航工作负载均衡器](/help/quicksilver/resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)。

{{step1-click-profile-pic}}

1. 单击左侧面板中的&#x200B;**工作负载均衡器**。

   此时将显示用户的工作负载均衡器。

   ![用户的工作负载均衡器](assets/workload-balancer-user.png)

   默认情况下，用户的工作负载均衡器按信息显示以下内容：

   * **已分配的工作**：已分配给特定用户的任务和问题。

</div>

## 将工作负载均衡器添加到自定义分区

您可以将工作负载均衡器添加到任何自定义分区。

将工作负载均衡器添加到自定义部分时，会保留已应用于工作负载均衡器的大多数自定义设置。

1. 访问工作负载均衡器，方法是转到以下任意区域：

   * 资源区域
   * 团队
   * 项目

1. 获取可共享链接并将其复制到剪贴板，如[使用链接](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md)共享工作负载均衡器中所述。
1. 创建包含外部页面的仪表板，如[在仪表板中嵌入外部网页](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md)中所述。 将您在步骤2中获得的可共享链接用于外部页面。

   <!--
      (NOTE: ensure this stays correct)
      -->

1. 按照[创建自定义选项卡或分区](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md)中的说明创建自定义分区，以将仪表板置于自定义选项卡上。

   从自定义部分访问工作负载均衡器时，您可以查看它，就像直接从步骤1中列出的其中一个原始区域访问它一样。

   <!--
      (NOTE: ensure this stays correct)
     -->

1. （可选）在布局模板中共享自定义选项卡，如[使用布局模板自定义左侧面板](../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)中所述。


<!--
For a team:

* From the Workload Balancer section of a team.

  You can adjust allocations and review or assign work from multiple projects to individual team members.

For a project:

  You can do the following when you use the Workload Balancer within a project:

   * Assign work on the project to users already assigned other work on the project.
   * Assign work to any user that might not be on the project.

   * View additional work that users are assigned to on other projects.
   * Adjust user allocations to work items.-->
