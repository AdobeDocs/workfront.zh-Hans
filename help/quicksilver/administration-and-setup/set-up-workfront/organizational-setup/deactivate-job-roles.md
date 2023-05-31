---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 取消激活工作角色
description: 作为 [!DNL Adobe Workfront] 管理员或对工作角色具有管理访问权限的用户，您可以停用系统中已过时的工作角色。 当您停用工作角色而不是删除它时，您可以保留与其关联的任何历史信息。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 934cef1a-8157-45db-b000-24a08a94dd18
source-git-commit: 9c0160dc5e43f36b65d9f2d4a3498a9c5f39f6f1
workflow-type: tm+mt
source-wordcount: '692'
ht-degree: 0%

---

# 取消激活工作角色

作为 [!DNL Adobe Workfront] 管理员或对工作角色具有管理访问权限的用户，您可以停用系统中已过时的工作角色。 当您停用工作角色而不是删除它时，您可以保留与其关联的任何历史信息。

您还可以重新激活之前已停用的工作角色。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront]计划*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront]许可证*</td> 
   <td>[！UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>对工作角色的管理访问权限</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询 [!DNL Workfront] 管理员（如果他们在您的访问级别设置了其他限制）。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参见 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

## 停用工作角色的影响

如果取消激活工作角色，它将不再显示在以下区域中：

* 此 [!UICONTROL 指定任务] 预输入字段（用于任务、模板任务、问题、批准和路由规则）
* 此 [!UICONTROL 指定任务] 列表和报告中的字段
* 用户配置文件

   >[!NOTE]
   >
   >向用户添加新角色时，未显示已停用的工作角色。 但是，它仍继续显示在 [!UICONTROL 主要角色] 和 [!UICONTROL 其他角色] 字段，表示用户在取消激活工作角色之前与工作角色相关联。

* 此 [!UICONTROL 共享] 对象对话框，包括布局模板分配
* 自定义表单中的预输入字段
* 此 [!UICONTROL 池成员] 中的字段 [!UICONTROL 资源池]
* 此 [!UICONTROL 工作角色] 字段 [!UICONTROL 记帐费率] 用户覆盖项目的计费率时的编辑屏幕
* 此 [!UICONTROL 将分配添加到Kanban板] 项目中的对话框
* 此 [!UICONTROL 工作角色] 当有人使用时，计划或计划的字段 [!DNL Adobe Workfront Scenario Planner].

   此 [!DNL Scenario Planner] 仅在新版本中可用 [!DNL Adobe Workfront] 体验，并需要额外的许可证。 欲知关于 [!DNL Workfront Scenario Planner]，请参见 [此 [!DNL Scenario Planner] 概述](../../../scenario-planner/scenario-planner-overview.md).

>[!TIP]
>
>已停用的角色始终显示在列表、报告和其他工具(例如 [!UICONTROL 工作负载均衡器].

## 停用工作角色之前的注意事项

最好是停用，而不是删除过时的职位角色，这样您就可以保留与过去可能使用的角色相关的所有历史信息。

>[!NOTE]
>
>在停用之前分配给工作角色的任何工作仍会保持分配状态。

我们建议您在停用未使用的工作角色之前执行以下操作：

* 为分配给您计划取消激活的角色的任何对象生成报告，并将其重新分配给活动工作角色。 有关生成报表的信息，请参阅 [创建报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

   >[!TIP]
   >
   >您可以创建一个报告，以筛选分配了已停用角色的任何任务或问题。 然后，使用该报告将未完成的任务或问题重新分配给活跃角色。

* 清点所有审批流程、当前审批路径和工艺路线规则或分配给您计划停用的工作职责的其它对象，并将其重新分配给有效职责。

   >[!TIP]
   >
   >使用请求队列时，如果您停用在传送规则中指定为默认被分配人的工作角色，则角色会保留，并且请求仍会传送到已停用的角色。 我们建议在停用团队之前，使用活动角色更新路由规则。

   有关创建审批流程和传送规则的信息，请参阅以下文章：

   * [为工作项创建批准流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)
   * [创建路由规则](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)

## 取消激活工作角色

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) （位于的右上角） [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击&#x200B;。 **[!UICONTROL 职位角色].**
1. （可选）在 **[!UICONTROL 筛选条件]** 下拉菜单，选择 **[!UICONTROL 活动]** 以仅显示活动的工作角色。
1. 单击要取消激活的工作角色的名称。
1. 在 **[!UICONTROL 处于活动状态]** 下拉菜单，选择 **[!UICONTROL 否]**.

   ![](assets/deactivate-job-role-edit-role-box-nwe.png)

1. 单击 **[!UICONTROL 保存更改]**.

   工作角色已停用，无法再分配给工作、与布局模板关联等。 有关中工作角色的所有用途的信息 [!DNL Workfront]，请参见 [工作角色概述](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).
