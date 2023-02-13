---
product-area: projects
navigation-topic: use-lists
title: 在 [!DNL Adobe Workfront]
description: 当对象在列表或报表中显示时，可以编辑内嵌对象。 编辑列表或报告中显示的对象的信息时，该对象会立即更新。
feature: Get Started with Workfront
author: Lisa
exl-id: a94b5aaf-71de-4fcd-946b-459ca3edf7e4
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 0%

---

# 在 [!DNL Adobe Workfront]

当对象在列表或报表中显示时，可以编辑内嵌对象。 编辑列表或报告中显示的对象的信息时，该对象会立即更新。

在内联编辑自定义表单中包含的未附加到对象的字段时，自定义表单会自动添加到对象中。 如果字段存在于多个自定义表单上，则最近更新的自定义表单会附加到对象。

有关列表的更多信息，请参阅 [开始使用 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

列表或报表中显示的大多数对象在 [!DNL Adobe Workfront]，则存在一些限制，包括：

* 您无法编辑计算字段或 [!DNL Workfront] 内置字段。
* 您只能编辑与列表中的对象直接关联的字段。 不能编辑属于与列表中的对象关联的对象的字段。\
   例如，您可以在任务报表中编辑任务的状态，但不能在同一报表中编辑与任务关联的项目的名称。 您只能在项目报表中编辑项目的名称。
* 当列表视图未显示默认货币时，无法在内联编辑字段。\
   有关显示默认货币的信息，请参阅部分 [编辑具有唯一货币的报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md#editing-reports-with-unique-currencies) 在文章中 [使用独特的汇率创建财务数据报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

* 您无法编辑列表中显示的标记和图标。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[!UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>[!UICONTROL Edit]对列表所在区域的访问</p> <p>例如，要在项目中内联编辑任务，您需要[!UICONTROL Edit]访问“项目”。</p> <p>注意：如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。<br>有关如何 [!DNL Workfront] 管理员可以更改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>[!UICONTROL管理]</p> <p>您还必须具有编辑某些字段的权限，例如自定义字段、状态等。</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 编辑内联对象

1. 转到要内联编辑的对象列表。

   列表应显示属于对象的字段，或属于与列表中的对象关联的对象的字段。

1. 找到要编辑的对象，然后在列表中的任意字段内单击。

   >[!TIP]
   >
   >如果您有多个页面，则可以使用以下方法查找对象：
   >
   >   
   >   
   >   * **分页**:单击向后和向前箭头可在页面之间导航。\
      >     位于列表右下角， [!UICONTROL 分页] 当您在列表中滚动时，区域会保持粘滞状态。
   >   * **快速筛选**:单击过滤器图标或键入Alt+F以打开快速过滤器，然后输入文本以仅显示包含输入文本的项目。\
      >     快速过滤器位于列表工具栏中。 有关更多信息，请参阅 [将快速过滤器应用到列表](../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).



   如果可以编辑该字段，则会将该字段以及列表中显示的所有其他字段转换为可编辑的单元格。

   ![](assets/nwe-editable-cells-350x131.png)

1. 编辑此单元格中的信息，然后按 [!UICONTROL 输入].

   >[!NOTE]
   >
   >如果自定义字段已配置为允许格式，则在更新列表中内联编辑该字段时，可以为文本添加粗体、斜体或下划线。\
   >有关为自定义字段配置格式的信息，请参阅 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).\
   >有关更新列表的信息，请参阅文章中的“更新列表与旧版列表之间的差异”部分 [开始使用 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

1. 按 [!UICONTROL 选项卡] ，以移至下一个可编辑的单元格。
1. （视情况而定）如果无法保存所做编辑，且单元格以红色列出，请单击字段内部以查看单元格旁边显示的验证消息，并进行相应更新。

   通常，当使用错误的格式或必填字段留空时会发生这种情况。

1. 修改完所有单元格后，按 [!UICONTROL 输入] 以保存更改。
