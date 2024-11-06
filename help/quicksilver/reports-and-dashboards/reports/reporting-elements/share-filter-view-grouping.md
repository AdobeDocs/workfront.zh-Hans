---
product-area: reporting
navigation-topic: reporting-elements
title: 共享筛选器、视图或分组
description: 您可以与其他用户共享您有权查看的筛选器、视图和分组。
author: Nolan
feature: Reports and Dashboards
exl-id: 63a6db90-d52c-4147-a442-7904ef9e9d49
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '1178'
ht-degree: 1%

---

# 共享筛选器、视图或分组

<!-- Audited: 11/2024 -->

<!--(NOTE: CONSIDER SPLITTING THIS in three articles for each reporting element?)
(NOTE: This is linked from the TOC article in WF Basics > permissions section)-->

在分配访问级别时，您的Adobe Workfront管理员会授予用户查看或编辑对象的权限。 有关授予对象访问权限的详细信息，请参阅[创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

除了授予用户的访问级别之外，您还可以授予他们查看或编辑您创建或有权共享的特定对象的权限。 有关访问级别和权限的详细信息，请参阅[访问级别和权限如何协同工作](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md)。

您可以与其他用户共享您有权查看的筛选器、视图和分组。

当您共享某个筛选器、视图或分组时，您可以将该筛选器、视图或分组应用于您的列表。 根据授予您的访问权限，您也许能够修改它并与其他用户共享它。

有关如何创建过滤器、视图或分组的信息，请参阅以下文章：

* [筛选器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* 在Adobe Workfront中[查看概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Adobe Workfront中的分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront计划*</strong></td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront许可证*</strong></td> 
   <td> 
      <p>新增：</p>
         <ul>
         <li><p>参与者或更高版本</p></li>
         </ul>
      <p>当前：</p>
         <ul>
         <li><p>请求或更高版本</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>查看或更高权限的“筛选器”、“视图”、“分组”</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td><p>查看权限或更高权限可共享到视图、筛选器或分组</p></td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 共享筛选器、视图或分组

<!--(NOTE: when the beta filters/ groupings come out either consider splitting this in different kinds of FVGs or splitting this article in FVGs for showing sharing on each one of them??)-->

根据您从哪个界面共享筛选器，在选择列表中共享筛选器会有所不同：标准版或旧版。 有关筛选器生成界面类型的信息，请参阅[在Adobe Workfront中创建或编辑筛选器](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md)。

您只能在旧版界面中共享视图和分组。

### 使用标准生成器界面共享过滤器

可在标准界面中从项目、任务、问题、项目组合、程序、用户、模板或组列表中共享过滤器。 筛选器的标准生成器界面不适用于任何其他对象，也不适用于视图或分组。

使用标准生成器界面共享过滤器：

1. 转到项目、任务或问题的列表。
1. 单击&#x200B;**筛选器**&#x200B;图标![筛选器图标](assets/filter-nwepng.png)。

   ![标准筛选器生成器](assets/new-filters-all-filter-types.png)

1. 查看以下筛选器列表：

   <table style="table-layout:auto">
   <col>
   <col>
   <tbody>
   <tr>
   <td role="rowheader"><strong>已收藏</strong></td>
   <td>您标记为收藏的过滤器。 当您收藏某个过滤器时，其原始位置将显示在过滤器名称下方，并且除非将其作为收藏删除，否则它将在原始列表中隐藏。</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>已保存</strong></td>
   <td>您自己构建并保存的过滤器。 默认情况下，此列表以最近保存的顺序显示保存的筛选器，但可以拖动筛选器名称手动重新排序列表。</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>系统默认值</strong></td>
   <td>Workfront系统默认筛选器，以及Workfront管理员添加到您的筛选器列表中的筛选器，这些筛选器可以位于系统级别或布局模板中。</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>已与我共享</strong></td>
   <td>其他人创建并与您共享或在系统范围内共享的过滤器。</td>
   </tr>
   </tbody>
   </table>

1. 将鼠标悬停在您至少有权查看和共享的筛选器上，然后单击&#x200B;**更多**&#x200B;菜单![更多菜单](assets/more-icon-spectrum.png)，然后单击&#x200B;**共享**。

   ![更多菜单选项](assets/new-filters-more-menu-options-with-delete.png)

   此时将显示筛选器共享框。

1. 在&#x200B;**授予对**&#x200B;的访问权限字段中开始键入要与之共享的用户、团队、角色、组或公司的名称。

   ![筛选器共享框](assets/new-filters-share-filter.png)

1. （可选）单击实体名称旁边的右箭头以编辑其对筛选器的权限，然后启用&#x200B;**查看**&#x200B;或&#x200B;**管理**&#x200B;选项。 **视图**&#x200B;是默认视图。

   ![共享权限](assets/new-filters-sharing-permissions.png)

1. （可选）通过执行以下操作之一，启用或禁用实体的其他权限：

   1. 单击&#x200B;**查看**&#x200B;并禁用&#x200B;**共享**&#x200B;选项。 默认情况下处于启用状态。
   1. 单击&#x200B;**管理**&#x200B;并禁用&#x200B;**共享**&#x200B;或&#x200B;**删除**&#x200B;选项。 默认情况下启用它们。

      >[!NOTE]
      >
      >如果使用删除选项启用管理访问权限，则这些用户将从所有用户中删除该筛选器，即使他们并不拥有该筛选器。

   >[!TIP]
   >
   >用户获得的权限不能高于其访问级别。 如果他们无权在其访问级别编辑“筛选器”，则他们将无权管理筛选器。 Workfront对这些用户禁用了“管理”选项，并且该选项呈灰显状态。

1. 单击 **Share**。该筛选器将与您指定的实体共享。

   >[!TIP]
   >
   >与组共享会将筛选器的权限授予该组的成员和所有子组的成员。

   您共享的筛选器将显示在这些实体的筛选器面板的&#x200B;**与我共享**&#x200B;部分中。

   ![与我共享的筛选器](assets/new-filters-shared-with-me.png)

### 使用旧版界面共享过滤器、视图和分组

在旧版界面中共享筛选器、视图和分组的方式相同。

1. 转到对象列表或报告。
1. （视情况而定）在列表中，单击&#x200B;**筛选器**、**视图**&#x200B;或&#x200B;**分组**&#x200B;图标，然后将鼠标悬停在要共享的筛选器、视图或分组上，单击&#x200B;**更多**&#x200B;图标![更多图标](assets/more-icon.png)，然后单击&#x200B;**共享**。

   在报表中，单击&#x200B;**筛选器**、**视图**&#x200B;或&#x200B;**分组**&#x200B;下拉菜单，然后选择要共享的筛选器、视图或分组。

1. （视情况而定）如果从报表进行共享，请再次单击&#x200B;**筛选器**、**视图**&#x200B;或&#x200B;**分组**&#x200B;下拉菜单，然后单击&#x200B;**共享筛选器**、**共享视图**&#x200B;或&#x200B;**共享分组**。\
   将显示&#x200B;**筛选器访问**、**查看访问**&#x200B;或&#x200B;**分组访问**&#x200B;对话框。

   ![共享筛选器](assets/share-filter-people-box-nwe-350x458.png)

1. 根据要与谁共享，完成以下任一操作：

   **要与个人用户、团队、角色、组或公司共享：**&#x200B;在提供的字段中，开始键入要与其共享的用户、团队、角色、组或公司的名称，然后在名称出现在下拉列表中时单击该名称。\
   重复此过程可与多个用户、团队、角色、组或公司共享访问权限。

   >[!TIP]
   >
   >与组共享会将筛选器、视图或分组的权限授予该组的成员和所有子组的成员。

   **要与系统中的所有用户共享：**&#x200B;请单击“设置”图标&#x200B;****，然后单击“在系统范围内可见”图标&#x200B;****。\
   管理员必须选择“共享系统范围”选项才能使用此选项。 有关详细信息，请参阅文章[创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)和[共享报告、功能板和日历](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md)。

1. （视情况而定）如果要与个人用户、团队、角色、组或公司共享，请单击下拉菜单以定义要授予的访问权限级别。

   您可以从以下选项中进行选择：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>查看它</strong></td> 
      <td> <p>选择此选项可允许共享收件人仅使用共享筛选器、视图或分组。 选择此选项时，收件人无法对共享项目进行任何修改。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>管理它</strong></td> 
      <td> <p>选择此选项可允许共享收件人使用和修改共享筛选器、视图或分组。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>共享</strong></td> 
      <td> <p>单击<strong>高级设置</strong>，然后选择或清除<strong>共享</strong>选项，具体取决于您是否希望收件人能够与其他人共享。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存**。

   与您共享该筛选器、视图或分组的用户可以通过以下方式访问该筛选器：单击&#x200B;**筛选器**、**视图**&#x200B;或&#x200B;**分组**&#x200B;下拉菜单或图标，然后向下滚动到&#x200B;**与我共享**&#x200B;部分。


