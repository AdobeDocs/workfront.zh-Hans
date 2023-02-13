---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: 创建、编辑和共享默认过滤器、视图和分组
description: 您可以创建默认过滤器、视图和分组，然后将其提供给贵组织中的用户。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 32eb825c-ba50-4820-a659-adc924a6ae52
source-git-commit: 75c4abfa9aebf1d07a851486391291cddc94f1a9
workflow-type: tm+mt
source-wordcount: '822'
ht-degree: 0%

---

# 创建、编辑和共享默认过滤器、视图和分组

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

您可以创建默认过滤器、视图和分组，然后将其提供给贵组织中的用户。

如本文所述，在您创建默认过滤器、视图和分组时，与您共享这些内容的用户在查看其列表时能够利用这些内容。 用户可以根据您创建的过滤器、视图和分组创建自己的过滤器、视图和分组，但他们不能直接更改您创建的过滤器、视图和分组。

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

## 创建默认过滤器、视图或分组

{{step-1-to-setup}}

1. 根据您是创建还是编辑过滤器、视图还是分组，执行以下任一操作：

   * 单击 **[!UICONTROL 界面]** > **[!UICONTROL 过滤器]**.

   * 单击 **[!UICONTROL 界面] >** **[!UICONTROL 视图]**.

   * 单击 **[!UICONTROL 界面]** > **[!UICONTROL 分组]**.

1. 如果要创建过滤器、视图或分组，请单击 **[!UICONTROL 添加过滤器]**, **[!UICONTROL 添加视图]**&#x200B;或 **[!UICONTROL 添加分组]**，然后选择要与新过滤器、视图或分组关联的对象类型。

   或

   如果要编辑现有过滤器、视图或分组，请选择它，然后单击 **[!UICONTROL 编辑]** 图标 ![“编辑”图标](assets/edit-icon.png).

1. 配置过滤器、查看或分组。

   有关可用选项的信息，请参阅以下文章之一：

   * [过滤器概述 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [视图概述 [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [中的分组概述 [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

1. 单击 **[!UICONTROL 保存]** 在左下角附近。

您可以使系统中的用户可以使用过滤器、查看或分组。 有关与其他用户共享过滤器、视图或分组的更多信息，请参阅部分 [使过滤器、视图或分组对用户可用](#make-filters-views-or-groupings-available-to-users) 在本文中。


## 显示或隐藏布局模板中可用的过滤器、视图或分组

您可以选择在布局模板中显示或隐藏过滤器、视图或分组。 可见过滤器适用于系统范围内的所有用户。 您可以使用布局模板来隐藏特定用户或组的可见过滤器。

>[!NOTE]
>
>如果用户主动使用过滤器、视图或分组，然后管理员禁用该过滤器，则用户仍具有访问权限，直到他们选择新的过滤器、视图或分组。 在选择新过滤器、视图或分组后，他们将无法再还原到隐藏的过滤器、视图或分组。

要显示或隐藏布局模板中可用的过滤器、视图或分组，请执行以下操作：

1. 单击 **[!UICONTROL 界面]**，然后单击以下任一项： **[!UICONTROL 过滤器]**, **[!UICONTROL 视图]**&#x200B;或 **[!UICONTROL 分组]**.

1. （视情况而定）选择要向用户提供的过滤器、视图或分组，然后单击 **[!UICONTROL 启用系统范围]**.

   ![](assets/enable-system-wide-fvg.png)

   >[!TIP]
   >
   >如果您希望让过滤器、视图或分组对大多数用户可用，但将其对他用户隐藏，则可以使用布局模板。 有关更多信息，请参阅 [使用布局模板自定义过滤器、视图和分组](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. （视情况而定）选择要对用户隐藏的过滤器、视图或分组，然后单击 **[!UICONTROL 禁用系统范围]**. 禁用后，过滤器、视图或分组将在布局模板以及整个系统的用户中隐藏。


## 使过滤器、视图或分组对所有用户可用 {#make-filters-views-or-groupings-available-to-users}

这些步骤说明了如何通过 [!UICONTROL 共享] 对话框 [!UICONTROL 界面] 区域 [!UICONTROL 设置]. 此设置的作用类似于整个系统（包括布局模板）的开/关开关。

{{step-1-to-setup}}

1. 单击 **[!UICONTROL 界面]**，然后单击以下任一项： **[!UICONTROL 过滤器]**, **[!UICONTROL 视图]**&#x200B;或 **[!UICONTROL 分组]**.

1. 选择要向用户提供的过滤器、视图或分组，然后单击 **[!UICONTROL 共享]** 图标 ![“共享”图标](assets/share-icon.png) 打开 [!UICONTROL 过滤器访问], [!UICONTROL 查看访问]或 [!UICONTROL 分组访问] 表单。
1. （视情况而定）要使过滤器、查看或分组对系统中的所有用户可用，请单击 **[!UICONTROL 齿轮]** 下拉菜单 ![](assets/gear-menu-for-sharing-items.png)，然后单击 **[!UICONTROL 在系统范围内使此可见]**. 系统中的所有用户现在都可以查看过滤器、查看或分组。

   或

   开始键入要与其共享过滤器、查看或分组的特定用户、团队、角色、组或公司的名称，然后在下拉列表中显示该名称时单击该名称。

   有关共享的更多信息，请参阅 [对象共享权限概述](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. 单击&#x200B;**[!UICONTROL 保存]**。

   现在，您指定的用户在查看您与其关联的对象类型时可以查看默认过滤器、查看或分组。

## 删除过滤器、视图和分组

{{step-1-to-setup}}

1. 根据您删除的是过滤器、视图还是分组，执行以下任一操作：

   * 单击 **[!UICONTROL 界面]** > **[!UICONTROL 过滤器]**

   * 单击 **[!UICONTROL 界面]** > **[!UICONTROL 视图]**

   * 单击 **[!UICONTROL 界面]** > **[!UICONTROL 分组]**

1. 在列表中选择一个或多个项目，然后单击 **[!UICONTROL 删除]** 图标 ![“删除”图标](assets/delete.png).
1. 有关配置过滤器、查看或分组的详细信息，请参阅以下文章之一。

   * [过滤器概述 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [视图概述 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [中的分组概述 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)
