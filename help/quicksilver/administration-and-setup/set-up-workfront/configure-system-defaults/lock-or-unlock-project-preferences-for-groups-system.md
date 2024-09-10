---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 锁定或解锁系统中所有组的项目首选项
description: 组织中的组可能需要为其独特工作流以不同方式配置项目偏好设置。 您可以解锁整个组织中所有组的首选项，以便他们能够自行配置首选项。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f5a94eaf-ebb8-424b-80ff-ba40cc985a6e
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---

# 锁定或解锁系统中所有组的项目首选项

组织中的组可能需要为其独特工作流以不同方式配置项目偏好设置。 您可以解锁整个组织中所有组的首选项，以便他们能够自行配置首选项。

当首选项被解锁且组管理员修改时，与组关联的项目从组级别设置而不是系统级别设置获取该首选项的配置。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td><p>新文档： [！UICONTROL Standard]</p>
   或
   <p>当前： [！UICONTROL计划]</p>
   </td> 
  </tr>
  <tr> 
   <td role="rowheader">访问级别配置</td>
   <td>[！UICONTROL系统管理员]</td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 关于锁定和未锁定的首选项

锁定已在系统级别配置的项目、任务或问题首选项可确保每个人都使用该首选项的相同设置。 虽然您仍然可以重新配置已锁定的首选项，但组管理员无法为其组重新配置它。

相反，解锁项目、任务或问题首选项可让组管理员更灵活地管理其组处理这些项目的方式。 解锁某个首选项后，组管理员可以为其组重新配置该首选项。

如果字段没有锁定/解锁切换，则组管理员无法解锁该字段，无法在组级别配置设置。 配置仅在系统级别可用。

有关锁定或解锁系统级项目、任务或问题首选项的说明，请参阅[配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

>[!NOTE]
>
>在[!DNL Workfront]管理员在系统级别解锁首选项后，任何组管理员都可以对其进行配置并锁定它，以确保其组中的每个人和下面的子组都使用相同的配置。 此功能与[!DNL Workfront]管理员为系统中的每个人配置和锁定首选项的能力并行。 有关详细信息，请参阅[配置组的项目首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)和[锁定或解锁子组的项目、任务或问题首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md)。

## 解锁项目首选项，以便组可以对其进行配置

{{step-1-to-setup}}

1. 单击&#x200B;**[!UICONTROL 项目首选项]**，然后单击&#x200B;**[!UICONTROL 项目]**。

1. 执行以下任一操作：

   * 如果希望组管理员能够为其组配置首选项，请将其解锁![](assets/unlock-toggle-button.png)。
   * 如果您希望所有组都使用首选项的配置，请确保该首选项已锁定（这是默认设置）。

     >[!IMPORTANT]
     >
     >我们建议您与系统中的管理员和用户群组进行通信，以确保以配置锁定首选项的方式考虑所有需求。 锁定后，其配置将由系统中的所有组继承。 如果首选项已解锁任意时间段，则您的配置将替换组管理员可能已做出的配置。

1. 单击&#x200B;**[!UICONTROL 保存]**。
