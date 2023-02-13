---
title: 停用或重新激活用户
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 作为Workfront管理员，您可以停用或重新激活用户。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: aba243ba-46c2-4eb7-b704-4368bf0ae3cc
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1139'
ht-degree: 0%

---

# 停用或重新激活用户

>[!IMPORTANT]
>
>此页面中描述的过程仅适用于尚未载入Admin Console的组织。 如果贵组织已载入Adobe Admin Console，则必须通过Adobe Admin Console执行此操作。
>
>有关在Adobe Admin Console中取消激活用户的说明，请参阅文章中的“删除用户”部分 [单独管理用户](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) 或联系Adobe Admin Console管理员。
>
>有关根据贵组织是否已载入Adobe Admin Console而有所不同的步骤列表，请参阅 [基于平台的管理差异(Adobe Workfront/Adobe业务平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

您的用户可能会离开组织，您可能需要从Adobe Workfront中删除他们。 它们不应在系统中保持活动状态，因为这样会在将其他用户添加到更新或为他们分配工作时，给其他用户造成混淆。 当您停用某个用户时，其他用户在系统中搜索人员时，将不再看到其名称。

管理员可以在“设置”区域中看到不活动的用户。

您可以随时重新激活用户。

>[!IMPORTANT]
>
>我们建议您停用已离开组织的用户，而不是删除他们。 如果删除了某个用户，则与该用户关联的Workfront中的所有历史记录都将丢失。 这包括其工作分配、与注释、小时数、文档以及创建后的所有其他对象的关联。
>
>在Workfront中取消激活用户会同时删除该用户的Workfront许可证和数字校对许可证。 此外，无法再为用户分配工作。 停用用户后，该用户的Workfront许可证和校对许可证将可供其他用户使用；已停用用户配置文件中的所有其他信息将保持原样。
>
>有关删除和取消激活用户的影响的更多信息，请参阅 [删除用户](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>计划 </p>   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须具有以下任一项：</p> 
    <ul> 
     <li> <p>系统管理员访问级别。 有关信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>. </p> </li> 
     <li> <p><b>用户</b> 在配置为 <b>编辑</b> 访问，使用 <b>创建</b> 至少两个中的一个 <b>用户管理员</b> 在 <b>优化设置</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>在这两个选项中，如果用户 <b>管理员（群组用户）</b> 启用后，您必须是用户所属的组的组管理员。</p> <p>有关 <b>用户</b> 在访问级别中设置，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 停用用户

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **用户** ![](assets/users-icon-in-main-menu.png).

1. 选择一个用户，单击更多图标 ![](assets/more-icon.png)，然后单击 **停用**.

1. 单击 **停用** 框中。

## 计划用户停用

作为经理，您可能希望在用户实际离开您的组织之前将其标记为停用。 例如，如果您与合同绑定的用户合作，则他们在您的系统中的时间会有限，并且您知道他们的终止日期。 您可以安排在该日期将其停用。

Workfront管理员和计划许可证用户可以在其用户配置文件中看到停用日期。

要计划用户停用，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **用户** ![](assets/users-icon-in-main-menu.png).

1. 选择用户的名称。

   或

   （可选）选择多个用户，以计划批量停用这些用户。

1. 单击编辑图标 ![](assets/edit-icon.png).
1. 在显示的“编辑用户”框中，单击 **资源计划** 去那个区域。
1. 启用 **计划停用** 选项。

1. 在显示的日历中，指定 **计划停用日期**.

   >[!NOTE]
   >
   >* 在时间框中，您只能选择整小时增量，而不能选择分钟。
   >* 如果您为当天（已过）选择时间，Workfront将安排在中午12:00停用次日。 所选时间与计划取消激活的用户的计算机时区匹配。


1. 单击 **保存更改**.

   有时，用户在选定的某天会在选定的时间后被停用。 如果您选择了多个要批量停用的用户，则有时在选定的时间之后，所有选定的用户都会在选定的日期被停用。

我们建议您为计划停用的用户构建报表，以便不断了解即将停用的用户。 无法确认在用户被停用后发生了停用。

## 重新激活用户

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **用户** ![](assets/users-icon-in-main-menu.png).

1. 选择一个用户，单击更多图标 ![](assets/more-icon.png)，然后单击 **激活**.

1. 分配新 **访问级别**&#x200B;中。

### 重新激活用户时的校对影响

已停用的用户将失去其分配的默认校样角色及其校样许可证(如果您在Workfront Premium旧版计划中)。 如果选择重新激活用户，则必须：

* 重新分配许可证(如果您在Workfront Premium旧版计划中)。 有关Workfront校对计划的更多信息，请参阅 [访问Workfront中的校对功能](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).
* 验证他们具有正确的校样角色。 重新激活的校样用户会被分配给新用户的任何指定作为默认校样角色的内容。 请参阅 [配置默认校对角色](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md) 以了解更多信息。

## 关于停用Workfront管理员和计划许可用户

在停用具有计划许可证的Workfront管理员或用户之前，请务必检查是否存在与该人员有关的Workfront对象和活动，然后根据需要将其与其他Workfront管理员或计划许可证用户关联。

这些对象和活动可能包括以下内容：

* 分配给用户的任务或问题
* 用户拥有的项目
* 设置为使用用户的访问权限运行的报表
* 用户拥有的模板
* 将用户设置为资源管理器的项目和模板
* 请求队列路由规则，其中Workfront管理员或计划许可证用户是默认代理人
* 具有阶段（包括用户）的审批流程（尤其是当他们是阶段中唯一的审批者时）
* 将用户列为审批者的时间表
* 将用户列为审批者的时间表配置文件
* 为包含用户的自动化工作流打样

## 在计划用户停用时，资源规划会产生影响

计划用户停用时，资源计划器中不再显示用户可用于预算小时数。 如果它们仍是资源池的一部分，则它们会显示在资源计划器中，但它们的可用性将从其计划停用日期开始设置为零小时。

资源计划员考虑用户的所有任务职责和任务的计划完成日期，并相应地计算资源。

有关资源计划员的详细信息，请参阅 [资源计划员概述](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).
