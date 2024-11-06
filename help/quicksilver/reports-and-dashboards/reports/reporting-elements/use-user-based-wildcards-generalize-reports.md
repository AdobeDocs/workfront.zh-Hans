---
product-area: reporting
navigation-topic: reporting-elements
title: 使用基于用户的通配符对报告进行归纳
description: 在构建某些报表元素时，您可以使用通配符而不是特定信息来对报表进行泛化。
author: Nolan
feature: Reports and Dashboards
exl-id: 216e2869-b4f8-4cc7-9497-a12ebe00fe49
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 1%

---

# 使用基于用户的通配符对报告进行归纳

<!-- Audited: 11/2024 -->

在构建某些报表元素时，您可以使用通配符而不是特定信息来对报表进行泛化。 例如，如果要创建显示分配给特定用户的任务的报告，则可以在过滤器的“分配给”字段中使用用户的名称。 但是，如果您要创建显示分配给登录用户的任务的报表，而不考虑该用户的身份，则可以使用通配符来指示当有人查看报表时，该报表仅显示与他们有关的信息。 这样的话，您只需构建一次报表，但由于您在筛选器中使用了通配符，因此每当其他人读取此报表时，它都会生成不同的结果。

在构建以下报表元素时，您可以使用基于用户的通配符：

* 过滤器
* 自定义提示
* 添加列的规则时的视图

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront计划*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront许可证*</strong></td> 
   <td> 
      <p>新增：</p>
         <ul>
         <li><p>标准</p></li>
         </ul>
      <p>当前：</p>
         <ul>
         <li><p>计划</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>编辑对筛选器、视图、分组的访问权限</p> <p>编辑对报告、功能板和日历的访问权限以编辑报告中的报告元素</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>管理对报告的权限以编辑报告中的报告元素</p> <p>管理视图或筛选器的权限以编辑它们</p></td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

必须先创建报告，然后才能向其添加通配符变量。

有关创建报告的说明，请参阅[创建报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)。

## 操作步骤

要在报表中插入基于用户的通配符，请执行以下操作：

1. 转到要为其插入基于用户的通配符的报表。
1. 单击&#x200B;**报告操作**，然后单击&#x200B;**编辑**。

1. 单击&#x200B;**筛选器**&#x200B;选项卡。
1. 单击&#x200B;**添加筛选器规则**。
1. 开始键入要作为筛选依据的字段的名称。\
   您必须键入引用用户对象或用户相关信息的字段。
1. 在筛选器变量的下拉菜单中选择&#x200B;**等于**。

   >[!TIP]
   >
   >在Adobe Workfront中使用通配符时，必须始终选择&#x200B;**等于**&#x200B;筛选器变量。

1. 在&#x200B;**开始键入名称……**&#x200B;框中，键入： `$$USER.ID`或`$$USER.name`（如果希望报告显示有关登录用户的信息，基于其名称）。 您可以插入引用登录用户的组、团队、公司或其他信息的其他通配符。

   有关基于用户的通配符的完整列表，请参阅[通配符筛选器变量概述](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)。

1. 单击&#x200B;**保存+关闭**。

## 其他信息

另请参阅：

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [通配符筛选器变量概述](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [在Adobe Workfront中创建或编辑筛选器](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [筛选器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [向报告添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [在视图中使用条件格式](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
