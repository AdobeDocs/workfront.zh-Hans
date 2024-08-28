---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 活动和已停用对象
description: 作为 [!DNL Adobe Workfront] 管理员，您可以激活或停用系统中的对象。 我们建议您永远不要删除可以取消激活的对象。 您应该简单地取消激活对象以防止将来使用，并从其他对象的下拉菜单中将其删除。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: a0617270-e233-4ebe-a5ee-8df7a8a85823
source-git-commit: 307bfb397555c7f9d424e429785dae36c639756a
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 2%

---

# 活动和已停用对象

作为[!DNL Adobe Workfront]管理员，您可以激活或停用系统中的对象。 我们建议您永远不要删除可以取消激活的对象。 您应该简单地取消激活对象以防止将来使用，并从其他对象的下拉菜单中将其删除。

例如，为了查看特定的[!UICONTROL 小时类型]，[!UICONTROL 小时类型]必须是活动的。 非活动或已禁用的[!UICONTROL 小时类型]未出现在[!UICONTROL 小时类型]下拉菜单中，而是保留在系统中，以保持此[!UICONTROL 小时类型]过去可能使用的历史记录的完整性。

术语“活动”用于标识系统中是否启用了某些对象。 在此上下文中，“活动”用于以下对象：

## 电子邮件通知

您可以激活电子邮件通知，以允许某些操作触发所有用户的电子邮件通知。

有关激活或停用电子邮件通知的信息，请参阅[为系统中的每个人配置事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)。

## 小时类型

您可以激活小时类型，以允许用户在记录时间时选择这些类型。

有关激活或停用小时类型的信息，请参阅[管理小时类型](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md)。

## 项目组合

项目组合必须处于活动状态才能出现在[!UICONTROL 新建项目（业务案例）]窗体中。

您可以在编辑项目组合时激活项目组合。

有关编辑项目组合的信息，请参阅[创建项目组合](../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md)。

## 项目群

项目群必须处于活动状态才能显示在项目的[!UICONTROL 项目群]字段中。

您可以在编辑程序时使程序处于活动状态。

有关编辑程序的信息，请参阅[创建程序](../../manage-work/portfolios/create-and-manage-programs/create-program.md)。

## 模板

模板必须处于活动状态才能显示在项目的“模板”字段中。

您可以在编辑模板时激活模板。

有关编辑模板的信息，请参阅[编辑项目模板](../../manage-work/projects/create-and-manage-templates/edit-templates.md)。

## 审批流程

审批流程必须处于活动状态才能显示在项目、任务或问题的[!UICONTROL 审批流程]字段中。

您可以在编辑审批流程时激活审批流程。

有关编辑审批流程的信息，请参阅[为工作项创建审批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)。

## 里程碑路径

里程碑路径必须处于活动状态才能显示在项目的[!UICONTROL 里程碑路径]字段中。

您可以在编辑里程碑路径时激活里程碑路径。

有关编辑里程碑路径的信息，请参阅[创建里程碑路径](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md)。

## 自定义表单

自定义表单必须处于活动状态才能显示在另一个对象的[!UICONTROL 自定义表单]字段中。

您可以在编辑自定义表单时将自定义表单设置为活动状态。

有关编辑自定义表单以及可与其关联的对象列表的信息，请参阅[使用表单设计器设计表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

## 公司

公司必须处于活动状态才能显示在项目、用户或模板的[!UICONTROL 公司]字段中。

您可以在编辑公司时激活公司。

有关信息，请参阅[创建和编辑公司](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)。

## 用户

用户必须处于活动状态，才能在分配或共享时出现在所有其他对象的预输入字段中。

您可以从用户页面取消激活用户，或者在编辑用户时取消激活。

有关停用用户的信息，请参阅[停用或重新激活用户](../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)。

>[!IMPORTANT]
>
>如果您的组织已载入[!DNL Adobe Business Platform]，则必须通过[!UICONTROL Adobe Admin Console]取消激活用户。
>
>有关在[!UICONTROL Adobe Admin Console]中停用用户的说明，请参阅[单独管理用户](https://helpx.adobe.com/enterprise/using/manage-users-individually.html)一文中的“删除用户”一节，或联系您的[!UICONTROL Adobe Admin Console]管理员。
>
>有关因贵组织是否已登记到[!DNL Adobe Business Platform]而不同的过程列表，请参阅[基于平台的管理差异(Adobe Workfront/Adobe业务平台)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)。

## 团队

在进行分配或共享时，团队必须处于活动状态，才能出现在所有其他对象的任何预输入字段中。

您可以在编辑团队时停用团队。

有关停用团队的信息，请参阅[停用团队](../../people-teams-and-groups/create-and-manage-teams/deactivate-a-team.md)。

## 职位角色

工作角色必须处于活动状态，才能在分配或共享时出现在所有其他对象的任何预输入字段中。

您可以在编辑工作角色时取消激活工作角色。

有关停用工作角色的信息，请参阅[停用工作角色](../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md)。

