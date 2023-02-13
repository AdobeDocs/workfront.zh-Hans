---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 停用作业角色
description: 作为 [!DNL Adobe Workfront] 管理员或具有“作业角色”管理访问权限的用户，可以停用系统中已过时的作业角色。 当您停用作业角色而不是删除它时，可以保留与其关联的任何历史信息。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 934cef1a-8157-45db-b000-24a08a94dd18
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 0%

---

# 停用作业角色

作为 [!DNL Adobe Workfront] 管理员或具有“作业角色”管理访问权限的用户，可以停用系统中已过时的作业角色。 当您停用作业角色而不是删除它时，可以保留与其关联的任何历史信息。

您还可以重新激活之前已停用的作业角色。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront]计划*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront]许可证*</td> 
   <td>[!UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>对作业角色的管理访问权限</p> <p><b>注意</b>:如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 停用作业角色的影响

如果停用作业角色，该角色将不再显示在以下区域：

* 的 [!UICONTROL 分配] typeahead字段（用于任务、模板任务、问题、批准和路由规则）
* 的 [!UICONTROL 分配] 列表和报表中的字段
* 用户配置文件

   >[!NOTE]
   >
   >向用户添加新角色时，不显示已停用的作业角色。 但它仍会继续显示在 [!UICONTROL 主要角色] 和 [!UICONTROL 其他角色] 字段。

* 的 [!UICONTROL 共享] 对象的对话框，包括布局模板分配
* 自定义表单中的Typead字段
* 的 [!UICONTROL 池成员] 字段 [!UICONTROL 资源池]
* 的 [!UICONTROL 作业角色] 字段a [!UICONTROL 计费费率] 当用户覆盖项目的计费费率时，编辑屏幕
* 的 [!UICONTROL 向看板板添加分配] 对话框
* 的 [!UICONTROL 作业角色] 计划或计划的字段 [!DNL Adobe Workfront Scenario Planner].

   的 [!DNL Scenario Planner] 只能在新 [!DNL Adobe Workfront] 体验，并且需要其他许可证。 有关 [!DNL Workfront Scenario Planner]，请参阅 [的 [!DNL Scenario Planner] 概述](../../../scenario-planner/scenario-planner-overview.md).

>[!TIP]
>
>已停用的角色始终会显示在列表、报表及其他工具(如 [!DNL Workload Balancer].

## 停用作业角色之前的注意事项

最好停用已过时的作业角色，而不是删除这些角色，这样您就可以保留与您过去可能使用的角色相关联的所有历史信息。

>[!NOTE]
>
>在取消激活之前分配给作业角色的任何工作都将保留分配。

我们建议您在取消激活未使用的作业角色之前执行以下操作：

* 为分配给您计划停用的角色的任何对象生成报告，并将其重新指派给活动作业角色。 有关构建报表的信息，请参阅 [创建报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

   >[!TIP]
   >
   >您可以创建一个报表，以筛选分配了已停用角色的任何任务或问题。 然后，使用报告将未完成的任务或问题重新指派给活动角色。

* 盘点分配给您计划停用的作业角色的所有审批流程、当前审批路径、工艺路线规则或其他对象，并将其重新分配给活动角色。

   >[!TIP]
   >
   >在使用请求队列时，如果您停用作为路由规则中默认代理人的作业角色，则该角色仍然存在，并且请求仍被路由到已停用的角色。 我们建议您在停用团队之前，更新具有有效角色的路由规则。

   有关创建审批流程和路由规则的信息，请参阅以下文章：

   * [为工作项创建审批流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)
   * [创建路由规则](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)

## 停用作业角色

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单&#x200B;击 **[!UICONTROL 作业角色].**
1. （可选）在 **[!UICONTROL 过滤器]** 下拉菜单，选择 **[!UICONTROL 活动]** 以仅显示活动作业角色。
1. 单击要停用的作业角色的名称。
1. 在 **[!UICONTROL 处于活动状态]** 下拉菜单，选择 **[!UICONTROL 否]**.

   ![](assets/deactivate-job-role-edit-role-box-nwe.png)

1. 单击 **[!UICONTROL 保存更改]**.

   作业角色已停用，无法再分配给工作、与布局模板关联等。 有关中作业角色的所有用法的信息 [!DNL Workfront]，请参阅 [作业角色概述](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).
