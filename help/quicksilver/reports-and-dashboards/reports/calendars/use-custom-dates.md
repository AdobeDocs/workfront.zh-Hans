---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: 在日历报表中使用自定义日期字段
description: 日历报表是动态报表，可直观地呈现您的工作。 您可以在日历报表中为任务、问题和项目使用自定义日期字段。
author: Lisa
feature: Reports and Dashboards
exl-id: 40cc8628-7641-41ce-b8e5-7f5ed5ad36c7
source-git-commit: e5a3024b1657942cd7abdfff76a7a6795127a4f5
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 1%

---

# 在日历报表中使用自定义日期字段

A [!UICONTROL 日历] 报告是一种动态报告，可直观地呈现您的工作。 您可以在日历报表中为以下对象使用自定义日期字段：

* 任务
* 问题
* 项目

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[!UICONTROL计划] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>[!UICONTROL编辑]对[!UICONTROL报表]、[!UICONTROL功能板]和[!UICONTROL日历]的访问权限</p> <p>注意：如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>[!UICONTROL管理]对日历报表的访问权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 先决条件

1. 您必须在 [!DNL Workfront] 实例。 如果您没有设置自定义日期的表单，请按照 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. 将自定义表单附加到您计划添加到日历的项目、任务或问题，并指定日期。 有关更多信息，请参阅 [将自定义表单添加到对象](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## 设置项目组

您可以选择希望在日历上显示项目组的方式。

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 日历]**.

1. 选择要向其添加新项目组的日历。\
   或\
   单击 **[!UICONTROL +新建日历]** 并输入日历名称。

   >[!NOTE]
   >
   >您必须 [!UICONTROL 编辑] 访问 [!UICONTROL 报表], [!UICONTROL 功能板]和 [!UICONTROL 日历] 在访问级别创建日历报表。

1. 在左侧，单击 **[!UICONTROL 添加到日历]**，然后单击 **[!UICONTROL 添加高级项目]**.

1. 指定以下内容：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL将此组项目命名为]</strong></td>
      <td>键入项目组的名称。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL颜色]</strong></td>
      <td>为项目组选择一种颜色。 所有项目都以所选颜色显示在日历报表上。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL日期字段]</strong></td>
      <td>选择 <strong>[!UICONTROL自定义日期]</strong>.<br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL在日历上，show]</strong></td>
      <td><p>选择日期的显示方式：</p>
       <ul>
        <li><strong>[!UICONTROL单日期]</strong>:日历在单个日期显示对象。</li>
        <li><strong>[!UICONTROL持续时间]（从开始到结束）</strong>:日历会显示跨天的对象。<br><p>注意：如果您选择 <strong>[!UICONTROL持续时间]</strong>，则指定的结束日期必须晚于开始日期，否则日历上不会显示该项目。</p></li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL自定义日期]</strong></td>
      <td><p>输入附加到要跟踪的对象的自定义日期名称。</p></td>
     </tr>
    </tbody>
   </table>

1. 继续执行以下部分。

## 向项目组添加对象

设置项目显示方式后，您需要将要在日历上看到的对象添加到分组中。

1. 在 **[!UICONTROL 要向日历中添加什么？]** 选择

   * **[!UICONTROL 任务]**
   * **[!UICONTROL 项目]**
   * **[!UICONTROL 问题]**

1. 单击 **[!UICONTROL 添加任务]**, **[!UICONTROL 添加项目]**&#x200B;或 **[!UICONTROL 添加问题]**，具体取决于您添加到日历的对象类型。\
   ![为日历选择对象](assets/field-name.png)

1. 在下拉菜单中，开始键入字段名称，然后选择要在日历中显示的对象的字段源(例如， **[!UICONTROL 延迟任务]**)。
1. 为日历分组设置条件语句。

   ![条件语句](assets/condition-statement-calendar.png)

   要了解设置条件，请参阅 [过滤器和条件修饰符](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. （可选）重复步骤1-4为日历分组指定其他对象。
1. 在 **[!UICONTROL 将“任务/项目/问题”标签设置为……]** 字段中，选择此日历分组中对象在日历中的标记方式。

   >[!NOTE]
   >
   >如果默认标签选项对特定对象不可用，则会显示对象名称。 例如，当 [!UICONTROL 父任务] 标签，并且没有与对象关联的父任务， [!DNL Adobe Workfront] 显示您在日历中查看的对象名称。

1. 单击&#x200B;**[!UICONTROL 保存]**。
