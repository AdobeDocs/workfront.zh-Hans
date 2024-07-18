---
product-area: projects
navigation-topic: use-lists
title: 在 [!DNL Adobe Workfront]的列表中内联编辑项目
description: 当对象显示在列表或报表中时，您可以内联编辑对象。 编辑列表或报告中显示的对象信息时，对象会立即更新。
feature: Get Started with Workfront
author: Lisa
exl-id: a94b5aaf-71de-4fcd-946b-459ca3edf7e4
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '747'
ht-degree: 0%

---

# 在[!DNL Adobe Workfront]的列表中内联编辑项目

当对象显示在列表或报表中时，您可以内联编辑对象。 编辑列表或报告中显示的对象信息时，对象会立即更新。

当内联编辑自定义表单中包含的字段未附加到对象时，自定义表单会自动添加到对象中。 如果该字段存在于多个自定义表单中，则最近更新的自定义表单会附加到对象。

有关列表的详细信息，请参阅[开始使用 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)中的列表。

虽然列表或报表中显示的大多数对象都可以在[!DNL Adobe Workfront]中内联编辑，但存在一些限制，包括：

* 您无法编辑计算字段或[!DNL Workfront]内置的计算字段。
* 您只能编辑与列表中对象直接关联的字段。 您无法编辑属于与列表中对象关联的对象的字段。\
   例如，您可以在“任务”报告中编辑任务的状态，但无法在同一报告中编辑与任务关联的项目的名称。 您只能在项目报告中编辑项目名称。
* 当列表视图未显示默认货币时，您无法内联编辑字段。\
   有关显示默认货币的信息，请参阅[创建具有唯一汇率的财务数据报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md)一文中的[编辑具有唯一货币的报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md#editing-reports-with-unique-currencies)部分。
* 您无法编辑列表中显示的标志和图标。
* 您无法内联编辑源自其他报表的报表字段。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[！UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>[！UICONTROL Edit]对列表所在区域的访问权限</p> <p>例如，要在项目中内联编辑任务，您需要[！UICONTROL Edit]项目访问权限。</p> <p>注意：如果您仍然没有访问权限，请询问您的[!DNL Workfront]管理员是否对您的访问级别设置了其他限制。<br>有关[!DNL Workfront]管理员如何更改访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>[！UICONTROL管理]</p> <p>您还必须有权编辑某些字段，例如自定义字段、状态等。</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

## 编辑内联对象

1. 转到要内联编辑的对象列表。

   该列表应显示属于对象的字段，或属于与列表中对象相关联的对象的字段。

1. 找到要编辑的对象，然后在列表中的任意字段中单击。

   >[!TIP]
   >
   >如果您有多个页面，则可以使用以下方法查找对象：
   >
   >   
   >   
   >   * **分页**：单击向后和向前箭头可在页面之间导航。\
   >     位于列表的右下角，滚动列表时[!UICONTROL 分页]区域保持粘性。
   >   * **快速筛选器**：单击筛选器图标或键入Alt+F以打开快速筛选器，然后输入文本以仅显示包含输入文本的项目。\
   >     快速筛选器位于列表工具栏中。 有关详细信息，请参阅[将快速筛选器应用到列表](../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md)。


   如果字段可以编辑，这会将字段和列表中显示的所有其他字段转换为可编辑的单元格。

   ![](assets/nwe-editable-cells-350x131.png)

1. 编辑此单元格中的信息，然后按[!UICONTROL Enter]。

   >[!NOTE]
   >
   >如果自定义字段已配置为允许设置格式，则在更新列表中内联编辑该字段时，您可以对文本使用粗体、斜体或下划线。
   >有关为自定义字段配置格式的信息，请参阅[使用表单设计器设计表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。
   >有关更新列表的信息，请参阅[在 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)中开始使用列表一文中的“更新列表与旧列表之间的差异”部分。

1. 按[!UICONTROL Tab]移至下一个可编辑的单元格。
1. （视情况而定）如果无法保存编辑内容并且单元格以红色列出，请单击字段中的以查看单元格旁边显示的验证消息并进行相应的更新。

   最常见的情况是，当使用的格式错误或必填字段留空时，会发生这种情况。

1. 修改完所有单元格后，按[!UICONTROL Enter]保存更改。
