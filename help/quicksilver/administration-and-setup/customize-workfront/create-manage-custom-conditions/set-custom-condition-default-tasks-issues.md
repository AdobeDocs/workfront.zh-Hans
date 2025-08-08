---
title: 将自定义条件设置为任务和问题的默认值
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: 当用户单击处理它或向已分配他们的新任务添加更新注释（不手动设置任务的条件）时，Adobe Workfront显示任务的默认条件，在“设置”中配置。 同样的情况也适用于问题。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 40b426f4-0a9c-49a6-91c7-b5f8aa48bd37
source-git-commit: 1eab0317bfe72609133e71411ee24263517f1508
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 将自定义条件设置为任务和问题的默认值

当用户单击处理它或向已分配他们的新任务添加更新注释（不手动设置任务的条件）时，Adobe Workfront显示任务的默认条件，在“设置”中配置。 同样的情况也适用于问题。

Workfront使用内置条件“进展顺利”作为任务的默认条件，使用单独作为问题的默认条件。 作为Workfront管理员，您可以将这两种对象类型的默认条件更改为已创建的自定义条件。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>新增：标准</p>
       <p>或</p>
       <p>当前：计划</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>[！UICONTROL系统管理员]</td>
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 将自定义条件设置为任务或问题的默认条件：

{{step-1-to-setup}}

1. 单击&#x200B;**项目首选项** > **条件**。

1. 单击&#x200B;**任务**&#x200B;或&#x200B;**问题**&#x200B;选项卡。

1. 单击&#x200B;**设置默认条件**。
1. 在下拉菜单中，单击要作为任务（或问题）默认条件的自定义条件。
1. 单击&#x200B;**保存**。

>[!NOTE]
>
>* 分配了任务或问题的用户，或者具有任务或问题的管理权限的用户可以手动更改其条件。 有关详细信息，请参阅[任务和问题的更新条件](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md)。
>* Workfront提供的任务和问题的三个默认条件进展顺利，有一些问题，但也存在一些主要障碍。 不能隐藏或删除这些条件，但可以更改其名称和颜色。 或者，您可以按照[创建或编辑自定义条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)中的说明创建新条件以改用。

有关将自定义条件配置为项目的默认条件的信息，请参阅[将自定义条件设置为项目的默认条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md)。
