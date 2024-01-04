---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: 创建、编辑和共享默认筛选器、视图和分组
description: 您可以创建默认筛选器、视图和分组，然后将它们提供给贵组织中的用户。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 32eb825c-ba50-4820-a659-adc924a6ae52
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '820'
ht-degree: 0%

---

# 创建、编辑和共享默认筛选器、视图和分组

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

您可以创建默认筛选器、视图和分组，然后将它们提供给贵组织中的用户。

在按照本文所述创建默认筛选器、视图和分组时，与您共享这些筛选器的用户能够在查看其列表时利用它们。 用户可以根据您创建的过滤器、视图和分组创建自己的过滤器、视图和分组，但无法直接更改您创建的那些过滤器、视图和分组。

## 访问要求

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
   <td>[！UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是 [!DNL Workfront] 管理员。</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询 [!DNL Workfront] 管理员（如果他们在您的访问级别设置了其他限制）。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参见 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 创建默认筛选器、视图或分组

{{step-1-to-setup}}

1. 根据您是要创建或编辑筛选器、视图还是分组，执行以下任一操作：

   * 单击 **[!UICONTROL 界面]** > **[!UICONTROL 过滤器]**.

   * 单击 **[!UICONTROL 界面] >** **[!UICONTROL 视图]**.

   * 单击 **[!UICONTROL 界面]** > **[!UICONTROL 分组]**.

1. 如果要创建筛选器、视图或分组，请单击 **[!UICONTROL 添加筛选器]**， **[!UICONTROL 添加视图]**，或 **[!UICONTROL 添加分组]**，然后选择要与新的筛选器、视图或分组关联的对象类型。

   或

   如果您正在编辑现有的筛选器、视图或分组，请选择它，然后单击 **[!UICONTROL 编辑]** 图标 ![“编辑”图标](assets/edit-icon.png).

1. 配置过滤器、视图或分组。

   有关可用选项的信息，请参阅以下文章之一：

   * [过滤器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [中的视图概述 [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [中的分组概述 [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

1. 单击 **[!UICONTROL 保存]** 左下角附近。

您可以使过滤器、视图或分组对系统中的用户可用。 有关与其他用户共享过滤器、视图或分组的更多信息，请参阅部分 [使过滤器、视图或分组可供用户使用](#make-filters-views-or-groupings-available-to-users) 本文章中。


## 显示或隐藏布局模板中可用的筛选器、视图或分组

您可以选择在布局模板中显示或隐藏筛选器、视图或分组。 可见筛选器在系统范围内对所有用户都可用。 您可以使用布局模板来隐藏特定用户或组的可见筛选器。

>[!NOTE]
>
>如果用户主动使用筛选器、视图或分组，然后管理员禁用了它，则用户仍具有访问权限，直到他们选择新的筛选器、视图或分组。 选择新的筛选器、视图或分组后，他们将无法再还原到隐藏的筛选器、视图或分组。

显示或隐藏布局模板中可用的筛选器、视图或分组：

1. 单击 **[!UICONTROL 界面]**，然后单击以下任一项： **[!UICONTROL 过滤器]**， **[!UICONTROL 视图]**，或 **[!UICONTROL 分组]**.

1. （视情况而定）选择要提供给用户的过滤器、视图或分组，然后单击 **[!UICONTROL 在系统范围启用]**.

   ![](assets/enable-system-wide-fvg.png)

   >[!TIP]
   >
   >如果要使过滤器、视图或分组对大多数用户都可用，但对其他人隐藏它，则可以使用布局模板。 有关更多信息，请参阅 [使用布局模板自定义筛选器、视图和分组](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. （视情况而定）选择要对用户隐藏的筛选器、视图或分组，然后单击 **[!UICONTROL 在系统范围禁用]**. 禁用后，将从布局模板以及整个系统内的用户中隐藏过滤器、视图或分组。


## 使过滤器、视图或分组对所有用户可用 {#make-filters-views-or-groupings-available-to-users}

以下步骤说明了如何从以下位置提供过滤器、视图和分组： [!UICONTROL 共享] 中的对话框 [!UICONTROL 界面] 区域位于 [!UICONTROL 设置]. 此设置相当于整个系统的开/关开关，包括布局模板。

{{step-1-to-setup}}

1. 单击 **[!UICONTROL 界面]**，然后单击以下任一项： **[!UICONTROL 过滤器]**， **[!UICONTROL 视图]**，或 **[!UICONTROL 分组]**.

1. 选择您希望可供用户使用的筛选器、视图或分组，然后单击 **[!UICONTROL 共享]** 图标 ![“共享”图标](assets/share-icon.png) 以打开 [!UICONTROL 筛选器访问权限]， [!UICONTROL 查看访问权限]，或 [!UICONTROL 分组访问权限] 表单。
1. （视情况而定）要使过滤器、视图或分组对系统中的所有用户都可用，请单击 **[!UICONTROL 齿轮]** 下拉菜单 ![](assets/gear-menu-for-sharing-items.png)，然后单击 **[!UICONTROL 使其在系统范围内可见]**. 系统中的所有用户现在都可以查看过滤器、视图或分组。

   或

   开始键入要与其共享筛选器、视图或分组的特定用户、团队、角色、组或公司的名称，然后在名称出现在下拉列表中时单击该名称。

   有关共享的详细信息，请参阅 [对象权限共享概述](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. 单击&#x200B;**[!UICONTROL 保存]**。

   现在，在查看与指定的用户关联的对象类型时，该用户可看到默认筛选器、视图或分组。

## 删除筛选器、视图和分组

{{step-1-to-setup}}

1. 执行以下任一操作，具体取决于您是删除筛选器、视图还是分组：

   * 单击 **[!UICONTROL 界面]** > **[!UICONTROL 过滤器]**

   * 单击 **[!UICONTROL 界面]** > **[!UICONTROL 视图]**

   * 单击 **[!UICONTROL 界面]** > **[!UICONTROL 分组]**

1. 在列表中选择一个或多个项目，然后单击 **[!UICONTROL 删除]** 图标 ![“删除”图标](assets/delete.png).
1. 有关配置过滤器、视图或分组的详细信息，请参阅以下文章之一。

   * [过滤器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [中的视图概述 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [中的分组概述 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)
