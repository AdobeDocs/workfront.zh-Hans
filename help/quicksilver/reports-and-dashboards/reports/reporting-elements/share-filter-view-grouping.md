---
product-area: reporting
navigation-topic: reporting-elements
title: 共享筛选器、视图或分组
description: 您可以与其他用户共享您有权查看的筛选器、视图和分组。
author: Lisa
feature: Reports and Dashboards
exl-id: 63a6db90-d52c-4147-a442-7904ef9e9d49
source-git-commit: b56e6591c7da166bd1548420b562b838cc7fe0f2
workflow-type: tm+mt
source-wordcount: '1362'
ht-degree: 0%

---

# 共享筛选器、视图或分组

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: CONSIDER SPLITTING THIS in three articles for each reporting element?)</p>
<p>(NOTE: This is linked from the TOC article in WF Basics > permissions section)&nbsp;</p>
</div>
-->

<span class="preview">请注意，在“预览”环境中，增强型过滤器体验（以前称为“beta”）现在为默认设置。 这些增强型过滤器现在是“标准”过滤器，而更早的过滤器体验是“旧版”。</span>

在分配访问级别时，您的Adobe Workfront管理员会授予用户查看或编辑对象的权限。 有关授予对象访问权限的详细信息，请参见 [创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

除了授予用户的访问级别之外，您还可以授予他们查看或编辑您创建或有权共享的特定对象的权限。 有关访问级别和权限的更多信息，请参阅 [访问级别和权限如何协同工作](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

您可以与其他用户共享您有权查看的筛选器、视图和分组。

与您共享筛选器、视图或分组时，您可以将该筛选器、视图或分组应用于列表。 根据授予您的访问权限，您也许能够修改它并与其他用户共享。

有关如何创建过滤器、视图或分组的信息，请参阅以下文章：

* [Adobe Workfront中的过滤器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Adobe Workfront中的视图概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Adobe Workfront中的分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront计划*</strong></td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront许可证*</strong></td> 
   <td> <p>请求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>查看或更高权限的“筛选器”、“视图”、“分组”</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>具有共享视图、筛选器或分组访问权限的视图或更高的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 共享筛选器、视图或分组

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: when the beta filters/ groupings come out either consider splitting this in different kinds of FVGs or splitting this article in FVGs for showing sharing on each one of them??)</p>
-->

您可以使用以下界面在选择列表中共享筛选器：

* 标准界面
* 测试版生成器界面

根据您用来共享筛选器的接口，选择列表中的共享筛选器会有所不同。 有关过滤器构建接口类型的信息，请参见 [在Adobe Workfront中创建或编辑筛选器](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

您只能在标准界面中共享视图和分组。

* [使用标准界面共享筛选器、视图和分组](#share-with-standard-interface)
* [使用Beta版生成器界面共享过滤器](#share-with-beta-builder-interface)

### 使用标准界面共享筛选器、视图和分组 {#share-with-standard-interface}

在标准界面中共享筛选器、视图和分组的操作是相同的。

1. 转到对象列表或报告。
1. （视情况而定）在列表中，单击 **筛选条件**， **视图**，或 **分组** 图标，然后将鼠标悬停在要共享的过滤器、视图或分组上，单击 **更多** 图标 ![“更多”图标](assets/more-icon.png)，则 **共享**.

   在报表中，单击 **筛选条件**， **视图**，或 **分组** 下拉菜单，然后选择要共享的筛选器、视图或分组。

1. （视情况而定）如果从报表进行共享，请单击 **筛选条件**， **视图**，或 **分组** 再次打开下拉菜单，然后单击 **共享筛选器**， **共享视图**，或 **共享分组**.\
   此 **筛选器访问权限**， **查看访问权限**，或 **分组访问权限** 对话框随即显示。

   ![共享筛选器](assets/share-filter-people-box-nwe-350x458.png)

1. 根据要与谁共享，完成以下任一操作：

   **要与个人用户、团队、角色、组或公司共享，请执行以下操作：** 在提供的字段中，开始键入要与之共享的用户、团队、角色、组或公司的名称，然后在名称出现在下拉列表中时单击该名称。\
   重复此过程可与多个用户、团队、角色、组或公司共享访问权限。

   >[!TIP]
   >
   >与组共享可将筛选器、视图或分组的权限授予组和所有子组的成员。


   **要与系统中的所有用户共享，请执行以下操作：** 单击 **设置** 图标，然后单击 **使其在系统范围内可见**.\
   您的管理员必须选择“共享系统范围”选项，此选项才可用。 有关更多信息，请参阅文章 [创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) 和 [共享报告、功能板和日历](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

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
      <td> <p>单击 <strong>高级设置</strong>，然后选择或清除 <strong>共享</strong> 选项，具体取决于您是否希望收件人能够与其他人共享。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存**。

   与您共享该过滤器、视图或分组的用户可以通过单击 **筛选条件**， **视图**，或 **分组** 下拉菜单或图标，并向下滚动到 **与我共享** 部分。

### 使用Beta版生成器界面共享过滤器 {#share-with-beta-builder-interface}

从项目、任务或问题列表共享过滤器时，您可以使用测试版生成器界面而不是标准界面共享它们。

测试版生成器界面不适用于Workfront中的任何其他对象。

生成报表时，无法在Beta版生成器界面中生成过滤器。

使用Beta版生成器界面共享过滤器：

1. 转到项目、任务或问题的列表。
1. 单击 **筛选条件** 图标 ![过滤器图标](assets/filter-nwepng.png)，然后启用 **测试版设置** ![测试版设置](assets/beta-toggle-white-on-existing-filters.png) 以访问测试版生成器。 默认情况下处于禁用状态。

   接下来，根据需要同意测试版协议。

   这将打开测试版过滤器生成器界面。

   >[!TIP]
   >
   >启用测试版生成器后，生成器界面的标题将变为蓝色。 启用测试版生成器界面后，Workfront会使其在所有可用区域保持启用状态。

   ![Beta版过滤器生成器](assets/new-filters-all-filter-types.png)

1. 查看以下筛选器列表：

   <table style="table-layout:auto">
   <col>
   <col>
   <tbody>
   <tr>
   <td role="rowheader"><strong>已收藏</strong></td>
   <td>您标记为收藏的过滤器。 当您收藏某个过滤器时，其原始位置将显示在过滤器名称下方，并且除非将其作为收藏项删除，否则该过滤器将从原始列表中隐藏。</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>已保存</strong></td>
   <td>您自己构建和保存的过滤器。</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>系统默认值</strong></td>
   <td>Workfront系统默认过滤器，以及Workfront管理员添加到您的过滤器列表中的过滤器（在系统级别或布局模板中）。</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>已与我共享</strong></td>
   <td>其他人创建并与您共享的过滤器或在系统范围内共享的过滤器。</td>
   </tr>
   </tbody>
   </table>

1. 将鼠标悬停在您至少有权查看和共享的过滤器上，然后单击 **更多** 菜单 ![“更多”菜单](assets/more-icon-spectrum.png)，然后单击 **共享**.

   ![更多菜单选项](assets/new-filters-more-menu-options-with-delete.png)

   此时将显示过滤器共享框。

1. 启用查看系统范围设置。 这将授予Workfront中的任何用户查看筛选器的权限。

   >[!IMPORTANT]
   >
   >请谨慎使用此设置。 为所有用户添加多个筛选器将会使筛选器体验杂乱，并使筛选器更难找到。

   或者开始键入要在中共享的用户、团队、角色、组或公司的名称 **授予访问权限** 字段。

   ![筛选器共享框](assets/new-filters-share-filter.png)

1. （可选）单击实体名称旁边的向右箭头以编辑其对筛选器的权限，然后启用 **视图** 或 **管理** 选项。 **视图** 为默认值。

   ![共享权限](assets/new-filters-sharing-permissions.png)

1. （可选）通过执行以下操作之一，启用或禁用实体的其他权限：

   1. 单击 **视图** 并禁用 **共享** 选项。 默认情况下处于启用状态。
   1. 单击 **管理** 并禁用 **共享** 或 **删除** 选项。 默认情况下启用它们。

      >[!NOTE]
      >
      >如果使用删除选项启用管理访问权限，则这些用户将能够从所有用户中删除该筛选器，即使他们并不拥有该筛选器。
   >[!TIP]
   >
   >用户获得的权限不能高于其访问级别。 如果他们无权在其访问级别访问“编辑筛选器”，则他们将无权管理筛选器。 Workfront对这些用户禁用了“管理”选项，并且该选项呈灰显状态。

1. 单击 **共享**. 该筛选器将与您指定的实体共享。

   >[!TIP]
   >
   >与组共享会将筛选器的权限授予该组的成员和所有子组。

   您共享的过滤器会显示在 **与我共享** 这些实体的过滤器面板的部分。

   ![与我共享的筛选器](assets/new-filters-shared-with-me.png)

