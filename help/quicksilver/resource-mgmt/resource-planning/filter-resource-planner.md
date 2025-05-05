---
product-area: resource-management
navigation-topic: resource-planning
title: 资源规划者中的过滤信息
description: 通过使用过滤器，您可以从存储在系统中的所有信息修改在资源规划者中显示的信息。
author: Lisa
feature: Resource Management
exl-id: 7186cae5-1e16-421e-b26d-afb50aa7f6eb
source-git-commit: a3b2ac192e1f37e0c3d16d059ed96e8d5cadf8be
workflow-type: tm+mt
source-wordcount: '2390'
ht-degree: 0%

---

# 资源规划者中的筛选信息

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(AL:*Iterate on this article: filtering by custom data. Other enhancements? Special characters caveat might change - follow the story to know when. It originally came in Beta 3 17.3.)</p>
-->

通过使用过滤器，您可以从存储在系统中的所有信息修改在资源规划者中显示的信息。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td><p>新建：任何</p>
       <p>或</p>
       <p>当前： Pro或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>新增：浅色或更高</p>
       <p>或</p>
       <p>当前：审阅或更高版本</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>查看对项目、用户和资源管理的访问权限或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看项目的权限或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 资源规划者筛选器概览

为了最大程度地减少资源规划者中显示的信息量，Adobe Workfront提供了一个具有预配置标准的默认过滤器。 有关默认筛选器的信息，请参阅本文中的资源规划者[&#128279;](#overview-of-the-default-filter-in-the-resource-planner)中默认筛选器的概述部分。

您还可以构建自定义的过滤器。 有关在资源规划者中自定义筛选器的信息，请参阅本文中的[创建资源规划者筛选器](#create-resource-planner-filters)部分。

在资源规划者中使用过滤器时，请考虑以下事项：

* 您创建的过滤器仅对您可见。 您可以共享过滤器，以供其他用户使用。
* 作为Workfront管理员，您只能查看自己创建的或与您共享的过滤器。
* 为资源规划者选择其他视图时，过滤的结果不会更改。\
  有关更改资源规划者中视图的更多信息，请参阅[资源规划者导航概述](../../resource-mgmt/resource-planning/resource-planner-navigation.md)中的“项目/角色/用户视图”选择部分。

* 应用过滤器不会更改项目、角色或用户的资源规划者中的分配和可用性数据。 过滤器仅更改您在资源规划程序中看到的对象数。
* 筛选条件适用于同时显示在资源规划程序中的所有对象。 例如，如果您筛选特定用户，则资源规划者仅显示以下结果：

   * 如果项目中的用户是资源池的一部分（对于项目和角色视图），或者在项目中有任务分配（对于用户视图）
   * 与这些项目中的用户关联的角色\
     与用户关联的项目中的其他角色或用户不会显示。

## 资源规划者中的默认筛选器概览 {#overview-of-the-default-filter-in-the-resource-planner}

在首次打开资源规划者时，Workfront应用默认过滤器。 您可以编辑“默认”筛选器以仅筛选要显示的项目。 有关修改筛选器的信息，请参阅本文中的[在资源规划者](#edit-a-filter-in-the-resource-planner)中编辑筛选器部分。

使用默认筛选器时，请考虑以下事项：

* 默认筛选条件仅从具有以下内容的项目中检索信息：

   * 在当前月份的第一天之后发生的计划完成日期
   * 计划开始日期早于当前日期后第四个月的最后一天
   * 当前或计划状态

  >[!IMPORTANT]
  >
  >默认过滤器从项目检索始终在四个月内发生的信息，从当月的第一天开始，而不管您选择要在资源规划者中显示的时间范围如何。

* 在“用户视图”中，将显示系统中的所有用户，但只有与已筛选项目关联的用户会显示小时信息。
* 您可以编辑默认筛选器中的信息而不保存该筛选器。
* 您可以复制并编辑默认筛选器的副本，更改其中所需的标准，然后将其另存为新筛选器。
* 您无法删除或共享默认筛选器。

  ![RP_new_default_fitler_criteria__1_.PNG](assets/rp-new-default-fitler-criteria--1--301x547.png)

## 创建资源规划者筛选器 {#create-resource-planner-filters}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: **^ This section is somewhat duplicated (format more than content) from the "Filtering Utilization Information" section in "Viewing Utilization Information for Projects, Programs, and Portfolios.")</p>
-->

在所有视图中，在资源规划者中创建过滤器的过程都是相同的。

在创建过滤器之前，确保已具备在资源规划程序中查看正确信息的先决条件。\
有关满足使用资源规划程序的必要先决条件的信息，请参阅[资源规划程序概述](../../resource-mgmt/resource-planning/get-started-resource-planner.md)文章中的“在资源规划程序中工作的先决条件”部分。

创建过滤器时，请考虑以下事项：

* 您可以同时过滤的对象数量没有限制。
* 可添加到筛选器的可用字段根据应用于资源规划者的视图的对象而更改。 例如，您可以仅在“用户视图”中过滤“问题”或“任务”字段，因为这些对象仅在“用户视图”中显示。 如果您在“用户”视图中为“问题”或“任务”构建过滤器，然后将其应用于“项目”或“角色”视图，则会忽略该过滤器，因为“项目”或“角色”视图中不存在字段。 在这种情况下，筛选器显示为不可用。

要在资源规划者中创建过滤器，请执行以下操作：

{{step1-to-resourcing}}

默认显示&#x200B;**规划者**。

默认情况下，首次访问资源规划者时应用<strong>默认筛选器</strong>。<br>有关默认筛选器的更多信息，请参阅本文的资源规划者</a>中的默认筛选器的<a href="#overview-of-the-default-filter-in-the-resource-planner" class="MCXref xref">概述部分。

1. 在的左上角，单击&#x200B;**筛选器**&#x200B;图标。
   ![filter_icon.png](assets/filter-icon.png)
或
展开&#x200B;**筛选器**&#x200B;下拉菜单，然后单击&#x200B;**添加新筛选器**。
   ![筛选器下拉列表](assets/rp-filter-dropdown-expanded-with-default-filter-selected-350x283.png)

1. 要使用内置标准构建过滤器，请指定以下任意字段：

   * **Portfolio**：开始键入包含要包含在资源规划者中的信息的项目组合的名称，然后在该名称出现在列表中时单击该名称。\
     重复此过程以包含来自多个项目组合的信息。

   * **项目状态**：展开“项目状态”下拉菜单，然后选择列表中可用的一个或多个项目状态。
   * **团队**：开始键入一个或多个团队的名称，这些团队与分配给您要查看项目中任务的用户相关联。
   * **工作角色**：开始键入与分配给您要查看项目中任务的用户关联的一个或多个工作角色的名称。
   * **池**：开始键入一个或多个资源池的名称，这些资源池与项目（用于项目视图）、用户（用于用户视图）或与您要查看的项目和用户（用于角色视图）相关联。
   * **组**：开始键入与您要查看的用户（在“用户”视图中）或项目（在“项目”和“角色”视图中）关联的一个或多个组的名称。

1. 单击&#x200B;**添加筛选规则**，然后在&#x200B;**键入以筛选项**&#x200B;框中开始键入要作为筛选依据的字段名称。 如果该字段可用，则会填充每个可关联该字段的对象。

   >[!IMPORTANT]
   >
   >引用自定义字段时，必须键入字段名称而非字段标签。 字段标签显示在附加到对象的自定义表单上。 有关标签与自定义字段名称之间差异的信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

1. 单击字段名称，以将其添加到列表中显示的过滤器。\
   有关您在列表中看到的字段的更多信息，请参阅[Adobe Workfront术语词汇表](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)。

1. （可选）为过滤器选择过滤器和条件修饰符。 可用的修饰符在[筛选器和条件修饰符](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)中描述。

   您可以使用基于用户或基于日期的通配符来过滤与登录用户相关的信息。\
   有关筛选器支持的通配符的信息，请参阅[通配符筛选器变量概述](../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)。

1. 单击&#x200B;**保存**&#x200B;以保存筛选规则。
1. （可选）单击&#x200B;**添加筛选器规则**&#x200B;为其他对象或字段添加新规则。
1. 单击&#x200B;**应用**&#x200B;以应用筛选器而不保存它。

   或

   单击&#x200B;**保存筛选器**&#x200B;以保存筛选器。\
   ![RP_Apply_or_Save_buttons_on_filters.png](assets/rp-apply-or-save-buttons-on-filters-320x79.png)

1. （视情况而定）单击&#x200B;**保存**&#x200B;后，在&#x200B;**保存筛选器**&#x200B;对话框的&#x200B;**筛选器名称**&#x200B;框中指定筛选器的名称。 这是必填字段。\
   ![RP_new_save_filter_box__with_Save_button__without_apply.png](assets/rp-new-save-filter-box--with-save-button--without-apply-350x175.png)

   >[!NOTE]
   >
   >如果过滤器名称包含特殊字符，则只能使用以下字符：
   >
   >* 逗号
   >* Slash
   >* 连字符
   >* 下划线

1. 单击&#x200B;**保存**。

   资源规划者中的结果现在按您在筛选规则中包括的信息进行筛选。

## 应用现有筛选器

当您或有权访问资源规划者的人保存过滤器时，所有使用资源规划者的用户都可以使用该过滤器。

要应用现有过滤器，请执行以下操作：

1. 转到资源规划者。
1. 在左上角，展开&#x200B;**筛选器**&#x200B;下拉菜单。

   您可以在此菜单中查看自己创建的过滤器或其他已创建并与您共享的过滤器。\
   ![RP_filter_drop_down.png](assets/rp-filter-drop-down-350x152.png)

1. 在下拉菜单中选择一个筛选器。 您可以在此菜单中查看您或其他用户创建的过滤器。\
   当您选择过滤器时，它会自动减少资源规划者中显示的信息量。

## 在资源规划程序中编辑过滤器 {#edit-a-filter-in-the-resource-planner}

您可以通过执行以下操作之一在资源规划程序中编辑过滤器：

* [重命名筛选器](#rename-a-filter)
* [编辑筛选器中的信息](#edit-the-information-in-a-filter)
* [复制筛选器](#duplicate-a-filter)

编辑过滤器时，系统中有权访问资源规划者的所有用户都将更新该过滤器。

### 重命名筛选器 {#rename-a-filter}

您可以更改过滤器的名称而不更改其条件。 我们建议让系统中的其他用户知道此更改，因为其他用户可看到过滤器。 此更改影响可以查看资源规划者的每个人的过滤器列表。

1. 转到资源规划者，并展开&#x200B;**筛选器**&#x200B;下拉菜单以选择已保存的筛选器。
1. 展开&#x200B;**筛选器**&#x200B;下拉菜单。 找到要重命名的过滤器，并将光标悬停在其名称上。
1. 选择筛选器名称旁边的&#x200B;**重命名筛选器**&#x200B;图标。

   ![编辑筛选器选项](assets/rp-filter-options-edit-350x154.png)

1. 在&#x200B;**筛选器名称**&#x200B;框中为筛选器指定新名称。
1. 单击&#x200B;**保存**。\
   过滤器中包含的信息是相同的，并且名称会更新。

### 编辑筛选器中的信息 {#edit-the-information-in-a-filter}

您可以更改包括在筛选器中的信息，而无需更改其名称。 我们建议让系统中的其他用户了解此更改，因为他们可以看到过滤器。 此更改影响可以查看资源规划者的每个人的过滤器列表。

1. 转到“资源规划者”，然后展开左上角的&#x200B;**筛选器**&#x200B;下拉菜单。
1. 选择要编辑的现有筛选器。
1. 单击&#x200B;**筛选器**&#x200B;图标。\
   ![filter_icon.png](assets/filter-icon.png)

1. 向筛选器添加新字段。\
   有关生成筛选器的信息，请参阅[创建资源规划者筛选器](#create-resource-planner-filters)。

1. 将鼠标悬停在为筛选器选择的现有字段上，然后单击&#x200B;**编辑**&#x200B;图标以选择其他字段，或单击&#x200B;**删除**&#x200B;图标以删除该字段。\
   ![RP_custom_filter_delete_and_edit_icons.png](assets/rp-custom-filter-delete-and-edit-icons-350x169.png)

1. （可选）单击&#x200B;**添加筛选器规则**&#x200B;以向筛选器添加新字段。\
   有关定义筛选条件的详细信息，请参阅[创建资源规划者筛选器](#create-resource-planner-filters)。

1. 单击&#x200B;**应用**&#x200B;以应用筛选器而不保存它。

   或

   单击&#x200B;**保存**&#x200B;以保存筛选器。\
   筛选器以相同的名称保存，但使用了新的筛选条件。

### 复制筛选器 {#duplicate-a-filter}

您可以复制现有筛选器。 原始筛选条件在复制的筛选器中保持不变，您可以按新名称保存新筛选条件。

1. 转到“资源规划者”，然后展开左上角的&#x200B;**筛选器**&#x200B;下拉菜单。
1. 将鼠标悬停在要复制的已保存过滤器的名称上。
1. 单击&#x200B;**复制**&#x200B;图标。

   ![重复的筛选器](assets/rp-filter-options---duplicate-350x154.png)\
   此时将显示“重复筛选器”框。

1. 在&#x200B;**筛选器名称**&#x200B;字段中，为复制的筛选器指定新名称。\
   新筛选器的默认名称为&#x200B;*`<Original Filter Name>`（副本）*。

1. 单击&#x200B;**保存**。 将创建一个与原始筛选器条件相同的新筛选器，并赋予新名称。

   >[!NOTE]
   >
   >尽管您可以拥有2个具有相同名称和相同标准的过滤器，但我们建议您在资源规划者中保存具有唯一过滤标准和名称的过滤器，以避免混淆。

## 删除筛选器

您可以删除不再需要的过滤器。 您不能删除默认筛选器。

有关默认筛选器的信息，请参阅本文的资源规划者[&#128279;](#overview-of-the-default-filter-in-the-resource-planner)中的默认筛选器的概述部分。

删除过滤器时，将删除所有有权访问资源规划者的Workfront用户的过滤器。 在删除过滤器之前，请确保您要删除的过滤器不再由在资源规划者中工作的任何其他人员使用。 无法恢复已删除的筛选器。

要删除过滤器，请执行以下操作：

1. 转到资源规划者。
1. 展开&#x200B;**筛选器**&#x200B;下拉菜单。
1. 找到要删除的过滤器，并将鼠标悬停在其名称上。
1. 选择筛选器名称旁边的&#x200B;**删除筛选器**&#x200B;图标。

   ![删除筛选器](assets/rp-filter-options---delete-350x154.png)

1. 在&#x200B;**删除筛选器**&#x200B;对话框中单击&#x200B;**删除**。

1. 该过滤器将从资源规划者中删除并删除。

## 共享过滤器

您可以共享已构建或有权与其他用户共享的过滤器。 您不能共享默认筛选器，但您可以复制它并共享副本。

>[!NOTE]
>
>所有用户(包括Workfront管理员)都只能访问已构建或已与其共享的过滤器。 您可以与特定用户共享过滤器，以使过滤器可用于所有资源规划者用户。

有关默认筛选器的信息，请参阅本文的资源规划者[&#128279;](#overview-of-the-default-filter-in-the-resource-planner)中的默认筛选器的概述部分。

有关复制筛选器的信息，请参阅本文中的[复制筛选器](#duplicate-a-filter)部分。

1. 转到资源规划者。
1. 展开&#x200B;**筛选器**&#x200B;下拉菜单。
1. 找到要共享的过滤器，并将鼠标悬停在其名称上。
1. 选择筛选器名称旁边的&#x200B;**共享筛选器**&#x200B;图标。

   ![共享筛选器](assets/rp-filter-options---share-350x154.png)

   此时将显示“筛选器访问”对话框。

1. （可选）要使筛选器对所有资源规划者用户可用，请单击&#x200B;**设置**&#x200B;图标，然后选择&#x200B;**在系统范围内可见**。

   ![在系统范围内可见](assets/make-this-visible-system-wide-350x119.png)

1. 在&#x200B;**授予资源规划者筛选器访问权限：**&#x200B;框中，开始键入要与其共享筛选器的用户、团队、角色、组或公司的名称。
1. 从以下权限级别中选择：

   * 查看
   * 管理

     有关Workfront中权限的信息，请参阅[对象权限共享概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)

1. （可选）单击&#x200B;**高级设置**&#x200B;以通过选择每个级别来添加权限，或通过取消选择每个级别来删除权限。

   ![共享筛选器](assets/rp-share-filter-manage-advanced-settings-350x271.png)

1. 单击&#x200B;**保存**。

   该筛选器已与您选择的实体共享，并显示在&#x200B;**与我共享**&#x200B;区域。

   ![与我共享](assets/rp-shared-with-me-area.png)
