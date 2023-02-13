---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 删除作业角色
description: 您可以删除贵组织不再使用的作业角色。 如果作业角色过去与工作项关联，我们建议不要删除这些角色。 为了保留有关工作分配的所有历史信息，我们建议您停用角色，而不是在角色过时时将其删除。 有关取消激活角色的信息，请参阅取消激活作业角色。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b0e81d76-5227-4fda-9a58-68fbce3f5b94
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 0%

---

# 删除作业角色

您可以删除贵组织不再使用的作业角色。 如果作业角色过去与工作项关联，我们建议不要删除这些角色。

为了保留有关工作分配的所有历史信息，我们建议您停用角色，而不是在角色过时时将其删除。 有关取消激活角色的信息，请参阅 [停用作业角色](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td>[!UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>对作业角色的管理访问权限</p> <p><b>注意</b>:如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 删除作业角色

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved from create and manage job roles)</p>
-->

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 单击 **[!UICONTROL 作业角色].**
1. 选择要删除的作业角色，然后单击 **[!UICONTROL 删除].**
1. 如果有任何对象（用户、任务、问题）被分配给作业角色，请执行以下操作之一：

   * **将作业角色替换为其他作业角色：** 从下拉列表中选择新的作业角色。

      与已删除的作业角色关联的任何当前和过去的资源分配都将转移至您选择的作业角色。

      只为用户分配了一个作业角色的用户，会被重新分配到您选择的作业角色；分配了辅助作业角色的用户不会被重新分配到您选择的作业角色。

   * **删除作业角色及其资源分配：** 选择 **[!UICONTROL 无]** 从下拉列表中。

      >[!IMPORTANT]
      >
      >删除作业角色会删除与所有项目的作业角色相关的所有当前和过去资源分配。

      例&#x200B;如，如果任务或问题仅被分配给该作业角色，则任务或问题在删除该作业角色后将未分配。

1. 单击  **[!UICONTROL 是，删除它]**.
