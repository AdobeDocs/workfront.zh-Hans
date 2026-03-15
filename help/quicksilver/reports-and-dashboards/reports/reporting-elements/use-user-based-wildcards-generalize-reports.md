---
product-area: reporting
navigation-topic: reporting-elements
title: 使用基于用户的通配符来泛化报告
description: 在构建某些报告元素时，您可以使用通配符而不是特定信息来泛化报告。
author: Courtney
feature: Reports and Dashboards
exl-id: 216e2869-b4f8-4cc7-9497-a12ebe00fe49
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 6%

---

# 使用基于用户的通配符来泛化报告

<!-- Audited: 11/2024 -->

在构建某些报告元素时，您可以使用通配符而不是特定信息来泛化报告。 例如，如果要创建显示分配给特定用户的任务的报告，则可以在筛选器的“分配对象”字段中使用用户的名称。 但是，如果要创建显示分配给已登录用户的任务的报告，而不管该用户是谁，可以使用通配符来指示当有人查看报告时，它只显示与其相关的信息。 这样，只需构建一次报告，但由于在筛选器中使用通配符，因此每次其他人读取报告时，都会生成不同的结果。

在构建以下报告元素时，可以使用基于用户的通配符：

* 过滤器
* 自定义提示
* 添加列规则时的视图

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>“任一”</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</strong></td> 
   <td> 
    <p>标准</p>
    <p>规划</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>对筛选器、视图、组的编辑访问权限</p> <p>编辑对报表、仪表板、日历的访问权限，以编辑报表中的报表元素</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
    <td> <p>管理报表权限以编辑报表中的报表元素</p> <p>管理对视图或过滤器的权限以进行编辑</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

有关此表中的信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

必须先创建报告，然后才能向其添加通配符变量。

有关创建报告的说明，请参阅[创建报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)。

## 操作步骤

要在报表中插入基于用户的通配符，请执行以下操作：

1. 转到要为其插入基于用户的通配符的报告。
1. 单击&#x200B;**报告操作**，然后单击&#x200B;**编辑**。

1. 单击&#x200B;**筛选器**&#x200B;选项卡。
1. 单击&#x200B;**添加筛选规则**。
1. 开始键入要作为筛选依据的字段的名称。\
   您必须键入引用用户对象或用户信息的字段。
1. 在筛选器变量的下拉菜单中选择&#x200B;**Equal**。

   >[!TIP]
   >
   >在Adobe Workfront中使用通配符时，必须始终选择&#x200B;**等于**&#x200B;筛选器变量。

1. 在&#x200B;**开始键入名称……**&#x200B;框中，键入： `$$USER.ID`或`$$USER.name` (如果希望报告显示有关登录用户的信息，请根据用户的名称键入。 您可以插入其他通配符，以引用登录用户的组、团队、公司或其他信息。

   有关基于用户的通配符的完整列表，请参阅[通配符筛选器变量概述](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)。

1. 单击&#x200B;**保存+关闭**。

## 其他信息

另请参阅：

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [通配符筛选器变量概述](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [在Adobe Workfront中创建或编辑筛选器](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [过滤器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [向报表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [在视图中使用条件格式](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
