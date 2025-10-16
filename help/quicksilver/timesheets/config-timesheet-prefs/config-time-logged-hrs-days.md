---
product-area: timesheets;setup
navigation-topic: configure-timesheet-preferences
title: 配置时间是以小时还是天为单位记录
description: 作为具有Plan许可证的用户，您可以配置是将时间记录在Adobe Workfront中是几小时还是几天。 系统管理员可以为单个用户或其组织中的多个用户配置此设置。 默认情况下，用户以小时为单位记录时间。
author: Lisa
feature: Timesheets
exl-id: 4f801a13-182d-4e06-98ea-f6863f6a8edf
source-git-commit: b0a3a11a3c04a0969bee99f8e1cea231911f0e6a
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 0%

---

# 配置时间是以小时还是天为单位记录

作为具有Standard或Plan许可证的用户，您可以配置是将时间记录在Adobe Workfront中是几小时还是几天。 系统管理员可以为单个用户或其组织中的多个用户配置此设置。 默认情况下，用户以小时为单位记录时间。 有关如何在Workfront中记录时间的信息，请参阅[记录时间](../../timesheets/create-and-manage-timesheets/log-time.md)。

>[!NOTE]
>
>我们建议在整个组织内以相同的方式记录时间（小时或天），以确保报告准确性。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td>
   <p>标准</p>
   <p>规划</p></td>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td><p>Standard和Plan用户可以为自己配置时间。 只有Workfront管理员可以为其他用户配置时间。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

1. 根据您的目标和系统中的访问级别，执行以下任一操作：

   * **Standard或Plan用户为自己配置时间日志记录：**&#x200B;单击Adobe Workfront右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](assets/main-menu-icon.png)，然后单击配置文件图片旁边的用户名。 或者（如果可用），单击顶部导航区域中的配置文件图片，然后单击&#x200B;**[!UICONTROL Workfront配置文件]**。 然后，单击您姓名旁边的&#x200B;**更多**&#x200B;图标并选择&#x200B;**编辑**。

   * **系统管理员为其他人配置时间日志记录：**&#x200B;如[编辑用户配置文件](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)中所述，开始编辑一个或多个用户帐户。

1. 在生成的对话框中，在&#x200B;**资源规划**&#x200B;部分中，找到&#x200B;**在**&#x200B;中记录时间选项。

   ![在选项中记录时间](assets/user-profile-log-time-options.png)

1. 从下列日志记录时间选项中选择：

   | 选项 | 描述 |
   |---|---|
   | **小时** | 用户在Workfront中记录时间时指定小时数。 |
   | **天** | 用户在Workfront中指定记录时间的天数。 |

1. （视情况而定）如果您选择以天为单位记录时间，请在&#x200B;**完整Workday的等效小时数**&#x200B;字段中，键入等于一整天的小时数。 用户时间表上的一天等同于您在此处输入的小时数。

   配置此设置时，请考虑以下事项：

   * 配置以小时为单位记录时间时，此选项不可用。
   * 此选项仅用于记录时间。 此选项与&#x200B;**计划**&#x200B;选项无关，该选项在编辑用户时也可用。 在计算时间表和Workfront的其他区域时，会使用&#x200B;**计划**&#x200B;选项。 （有关使用&#x200B;**计划**&#x200B;选项的详细信息，请参阅[创建计划](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。） 

1. 单击&#x200B;**保存更改**。
