---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 锁定或解锁系统中所有组的项目首选项
description: 组织中的组可能需要以不同方式为其唯一工作流程配置项目首选项。 您可以解锁组织中所有组的首选项，以便他们可以自行配置该首选项。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f5a94eaf-ebb8-424b-80ff-ba40cc985a6e
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 0%

---

# 锁定或解锁系统中所有组的项目首选项

组织中的组可能需要以不同方式为其唯一工作流程配置项目首选项。 您可以解锁组织中所有组的首选项，以便他们可以自行配置该首选项。

解锁首选项并修改该首选项后，与组关联的项目将从组级别设置而不是系统级别设置中获取该首选项的配置。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td>[!UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>你必须是 [!DNL Workfront] 管理员。</p> <p><b>注意</b>:如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 关于锁定和解锁的首选项

锁定您在系统级别配置的项目、任务或问题首选项可确保每个人都使用该首选项的相同设置。 虽然您仍可以重新配置您锁定的首选项，但组管理员无法为其组重新配置该首选项。

相反，解锁项目、任务或问题首选项可让组管理员更灵活地管理其组处理这些项目的方式。 解锁首选项后，组管理员可以为其组重新配置该首选项。

有关锁定或解锁系统级别项目、任务或问题首选项的说明，请参阅 [配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>在 [!DNL Workfront] 管理员在系统级别解锁首选项，任何组管理员都可以对其进行配置，然后将其锁定，以确保其组和以下子组中的每个人都使用相同的配置。 这与 [!DNL Workfront] 管理员必须为系统中的每个人配置并锁定首选项。 有关更多信息，请参阅 [为组配置项目首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) 和 [锁定或解锁子组的项目、任务或问题首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

## 解锁项目首选项，以便组可以对其进行配置

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 单击 **[!UICONTROL 项目首选项]**，然后单击 **[!UICONTROL 项目]**.

1. 执行以下任一操作：

   * 如果希望群组管理员能够为其群组配置首选项，请解锁 ![](assets/unlock-toggle-button.png).
   * 如果希望所有组都使用您的配置作为首选项，请确保该配置已锁定（这是默认设置）。

      >[!IMPORTANT]
      >
      >我们建议您与整个系统中的管理员和组中的用户通信，以确保通过配置锁定首选项的方式满足所有需求。 锁定后，系统中的所有组都会继承您的配置。 如果该首选项已在任意时间段内解锁，则您的配置将替换组管理员可能已设置的配置。

1. 单击&#x200B;**[!UICONTROL 保存]**。
