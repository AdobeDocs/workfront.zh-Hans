---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 删除职位角色
description: 您可以删除组织不再使用的工作角色。 如果工作角色以前与工作项关联，我们建议您不要删除工作角色。 要保留有关工作分配的所有历史信息，我们建议您停用角色，而不是在角色过期时将其删除。 有关停用角色的信息，请参阅停用工作角色。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b0e81d76-5227-4fda-9a58-68fbce3f5b94
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 0%

---

# 删除职位角色

您可以删除组织不再使用的工作角色。 如果工作角色以前与工作项关联，我们建议您不要删除工作角色。

要保留有关工作分配的所有历史信息，我们建议您停用角色，而不是在角色过期时将其删除。 有关停用角色的信息，请参阅[停用工作角色](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md)。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td>[！UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>对工作角色的管理访问权限</p> <p><b>注意</b>：如果您仍然没有访问权限，请询问您的[!DNL Workfront]管理员是否对您的访问级别设置了其他限制。 有关[!DNL Workfront]管理员如何修改访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

## 删除工作角色

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved from create and manage job roles)</p>
-->

1. 单击[!DNL Adobe Workfront]右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 设置]** ![](assets/gear-icon-settings.png)。

1. 单击&#x200B;**[!UICONTROL 职位角色].**
1. 选择要删除的工作角色，然后单击&#x200B;**[!UICONTROL 删除]。**
1. 如果有任何对象（用户、任务、问题）被分配给工作角色，请执行以下操作之一：

   * **将工作角色替换为其他工作角色：**&#x200B;从下拉列表中选择新的工作角色。

     与已删除工作角色关联的任何当前和过去资源分配都将转移到您选择的工作角色。

     只分配了一个工作角色的用户会重新分配到您选择的工作角色；分配了辅助工作角色的用户不会重新分配到您选择的工作角色。

   * **删除工作角色及其资源分配：**&#x200B;从下拉列表中选择&#x200B;**[!UICONTROL 无]**。

     >[!IMPORTANT]
     >
     >删除工作角色将删除所有项目的所有与该工作角色相关的当前和过去资源分配。

     例&#x200B;如，如果仅将任务或问题分配给该工作角色，则删除工作角色后会取消分配任务或问题。

1. 单击&#x200B;**[!UICONTROL 是，将其删除]**。
