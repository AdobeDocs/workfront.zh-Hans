---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 取消激活职位角色
description: 作为 [!DNL Adobe Workfront] 管理员或对工作角色具有管理访问权限的用户，您可以停用系统中已过时的工作角色。 当您停用而不是删除工作角色时，您可以保留与工作角色关联的任何历史信息。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 934cef1a-8157-45db-b000-24a08a94dd18
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 1%

---

# 取消激活工作角色

作为[!DNL Adobe Workfront]管理员或对工作角色具有管理访问权限的用户，您可以停用系统中已过时的工作角色。 当您停用而不是删除工作角色时，您可以保留与工作角色关联的任何历史信息。

您还可以重新激活之前已取消激活的工作角色。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td>
   <p>新文档： [！UICONTROL Standard]</p>
   <p>或</p>
   <p>当前： [！UICONTROL计划]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>对工作角色的管理访问权限</td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 停用工作角色的影响

如果停用工作角色，则它不再显示在以下区域中：

* [!UICONTROL 任务]预输入字段（用于任务、模板任务、问题、审批和路由规则）
* 列表和报告中的[!UICONTROL 工作总揽]字段
* 用户配置文件

  >[!NOTE]
  >
  >当用户添加新角色时，未显示已停用的工作角色。 但是，如果在停用工作角色之前用户与该工作角色相关联，则它将继续显示在[!UICONTROL 主要角色]和[!UICONTROL 其他角色]字段中。

* 对象的[!UICONTROL 共享]对话框，包括布局模板分配
* 自定义表单中的预输入字段
* [!UICONTROL 资源池]中的[!UICONTROL 池成员]字段
* 当用户覆盖项目的计费费率时，[!UICONTROL 计费费率]编辑屏幕的[!UICONTROL 工作角色]字段
* 项目中的[!UICONTROL 将工作分配添加到Kanban展示板]对话框
* 当有人使用[!DNL Adobe Workfront Scenario Planner]时，计划或计划的[!UICONTROL 工作角色]字段。

  [!DNL Scenario Planner]仅在新的[!DNL Adobe Workfront]体验中可用，并且需要额外的许可证。 有关[!DNL Workfront Scenario Planner]的信息，请参阅[概述 [!DNL Scenario Planner] ](../../../scenario-planner/scenario-planner-overview.md)。

>[!TIP]
>
>已停用的角色始终显示在列表、报告和其他工具（如[!UICONTROL 工作负载均衡器]）的过滤器中。

## 停用工作角色之前的注意事项

最好是停用，而不是删除已过时的职位角色，这样您就可以保留与过去可能使用的角色相关的所有历史信息。

>[!NOTE]
>
>在停用之前分配给工作角色的任何工作仍会得到分配。

我们建议您在停用未使用的工作角色之前执行以下操作：

* 为分配给您计划取消激活的角色的任何对象生成报告，并将它们重新分配给有效工作角色。 有关生成报告的信息，请参阅[创建报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)。

  >[!TIP]
  >
  >您可以创建一个报告，以筛选分配了已停用角色的任何任务或问题。 然后，使用该报告将未完成的任务或问题重新分配给活动角色。

* 收集所有审批流程、当前审批路径和工艺路线规则或分配给您计划停用的工作职责的其它对象的清单，并将它们重新分配给有效职责。

  >[!TIP]
  >
  >使用请求队列时，如果您停用在传送规则中指定为默认受分配人的工作角色，则角色会保留，并且请求仍会传送到已停用的角色。 我们建议在停用团队之前，使用活动角色更新路由规则。

  有关创建审批流程和传送规则的信息，请参阅以下文章：

   * [为工作项目创建审批流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)
   * [创建路由规则](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)

## 取消激活工作角色

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**[!UICONTROL 工作角色]。**
1. （可选）在&#x200B;**[!UICONTROL 筛选器]**&#x200B;下拉菜单中，选择&#x200B;**[!UICONTROL 活动]**&#x200B;以仅显示活动工作角色。
1. 单击要取消激活的工作角色的名称。
1. 在&#x200B;**[!UICONTROL 处于活动状态]**&#x200B;下拉菜单中，选择&#x200B;**[!UICONTROL 否]**。

   ![停用工作角色](assets/deactivate-job-role-edit-role-box-nwe.png)

1. 单击&#x200B;**[!UICONTROL 保存更改]**。

   工作角色已停用，无法再分配给工作、与布局模板关联等。 有关[!DNL Workfront]中所有工作角色用途的信息，请参阅[工作角色概述](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md)。
