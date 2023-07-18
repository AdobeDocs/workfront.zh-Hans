---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: 创建计划
description: 您可以使用计划定义用户的工作周。 您可以将计划与用户或项目关联。 这允许 [!DNL Workfront] 以计算时间线和用户可用性。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f7347ba6-68bf-45d8-b5d2-6136f3e696c9
source-git-commit: 3aad2a3d9ad32313cb14670965bc3ad05ab215d3
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 0%

---

# 创建计划

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
Linked to Editing Users, Editing Projects, Creating and managing groups
-->

作为 [!DNL Adobe Workfront] 管理员，您可以使用计划定义工作周。 您可以将计划与用户或项目关联。 这允许 [!DNL Workfront] 以计算时间线和用户可用性。

如果您的用户在不同的时区工作，则在每个时区创建一个时间表，并将其与这些用户关联，可以确保他们的工作记录在 [!DNL Workfront] 实时提供，并且随时可根据工作情况准确提供这些服务。

有关将时间表与用户和项目关联的信息，请参阅以下文章：

* [编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
* [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md)

组管理员还可以创建与其管理的组相关联的计划。 有关更多信息，请参阅 [创建和修改组的计划](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

有关使用计划帮助用户进行协作的信息 [!DNL Workfront] 跨时区，请参见 [跨时区工作](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

有关如何将计划用于资源计划的信息，请参阅 [时间表概述](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md) 和 [资源规划者概述](/help/quicksilver/resource-mgmt/resource-planning/get-started-resource-planner.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront]计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td>[！UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是 [!DNL Workfront] 管理员。</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询 [!DNL Workfront] 管理员（如果他们在您的访问级别设置了其他限制）。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参见 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 创建计划

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) （位于的右上角） [!DNL Adobe] Workfront，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).
1. 单击 **[!UICONTROL 时间表]**.
1. 单击 **[!UICONTROL 新建计划]**.
1. 指定调度的名称。
1. （可选）选择 **[!UICONTROL 默认计划]** 以将此计划标识为默认值。

   中可以有多个计划 [!DNL Workfront]，但您只能有一个默认计划。

   中必须至少有一个计划 [!DNL Workfront]. 如果您只有一个，则指定为默认计划。

   >[!NOTE]
   >
   >如果您是组管理员，则不能将时间表指定为默认时间表。 仅a [!DNL Workfront] 管理员可以指定时间表作为系统的默认设置。

   ![](assets/new-schedule.png)

1. 在 **[!UICONTROL 计划]** 选项卡，通过跨小时块拖动蓝色大纲以突出显示它们来选择每日计划。

   我们建议您在9小时的时段内选择8个一小时的块。 这适合午餐或其他休息时间。

   ![](assets/new-schedule-with-exceptions.png)

1. 在 **[!UICONTROL 详细信息]** 选项卡中，指定以下信息：

   <table style="table-layout:auto">
    <tr>
     <td>具有管理访问权限的[！UICONTROL组]</td>
     <td><p>指示其管理员有权编辑此计划的组。</p>
     <p><b>重要</b>：</p>
      <ul>
       <li>
       <p>如果您是创建计划的组管理员，则此字段为必填字段。</p>
       <p>作为组管理员，只有在为指定为管理员的组或子组指定调度时，才能创建调度。</p>
       <p>如果您只管理一个组，则默认情况下会在此字段中选择该组。</p>
       <p>如果管理多个组，则必须先在此字段中选择一个组，然后才能保存计划。</p></li>
       <li>如果您是 [!DNL Workfront] 管理员创建计划，此字段是可选的。 创建时间表而不将其与组关联时，时间表将另存为系统级别时间表，任何组的组管理员都不能管理该时间表。
       <p>分配给帐户或项目的计划对可以编辑这些对象的所有用户可见。 对于系统级别和组级别的计划，情况都是这样。</p>
       </li>
       <p>为调度指定具有管理访问权限的组不会将调度分配给组中的用户；它仅允许组中的组管理员编辑、删除和复制调度。</p>
       <p>组管理员无法编辑、删除或复制系统级别的计划。 有关更多信息，请参阅 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">组管理员</a>.
     </td>
    </tr>
    <tr>
     <td>具有视图访问权限的[！UICONTROL组]</td>
     <td><p>选择对此计划可见的、具有[！UICONTROL视图]访问权限的组。</p>
     <p>只有此处指定的组中的用户在将其分配给用户或项目时，才能在下拉菜单中查找计划。</p></tr>
    <tr>
     <td>[！UICONTROL时区]</td>
     <td><p>为您的计划选择时区。</p>
     <p>如果将调度与某个用户关联，我们建议调度的时区与用户的时区匹配。有关用户的时区信息，请参见 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">编辑用户的配置文件。
     </td>
    </tr>
   </table>


1. 在 **[!UICONTROL 例外]** 选项卡，指定调度的例外。

   例外情况是需要从时间表中排除的全天或半天，例如假日或公司活动。

   >[!NOTE]
   >
   >如果您已经知道定期计划例外是什么，则可以定义未来许多年的计划例外。

   可以从工作计划中排除全部或部分天数。 单击日期以将其选作例外，然后选择 **[!UICONTROL 全天]** 用于指示异常是否为全天的字段。

   ![](assets/schedule-adding-an-all-day-exception.png)

1. 指定部分天例外的开始和结束时间。

   ![partial-day-exception-on-schedules.png](assets/partial-day-exception-on-schedules.png)

1. 单击 **[!UICONTROL 保存]**，然后单击 **[!UICONTROL 保存] 更改**.

1. （可选）将计划与用户关联。

   有关信息，请参阅 [编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. （可选）将计划与项目关联。

   有关信息，请参阅 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md).
