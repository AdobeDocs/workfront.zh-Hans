---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: 在日历报告中使用自定义日期字段
description: 日历报告是一种动态报告，提供工作的可视化表示形式。 您可以在任务、问题和项目的日历报告中使用自定义日期字段。
author: Lisa
feature: Reports and Dashboards
exl-id: 40cc8628-7641-41ce-b8e5-7f5ed5ad36c7
source-git-commit: 880e82546ac0ca80be60f03db31b99ad1778c35a
workflow-type: tm+mt
source-wordcount: '696'
ht-degree: 1%

---

# 在日历报告中使用自定义日期字段

A [!UICONTROL 日历] 报告是一种动态报告，可直观地展示您的工作。 您可以在日历报表中为以下对象使用自定义日期字段：

* 任务
* 问题
* 项目

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[！UICONTROL计划] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>[！UICONTROL编辑]对[！UICONTROL报表]、[！UICONTROL功能板]和[！UICONTROL日历的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询 [!DNL Workfront] 管理员（如果他们在您的访问级别设置了其他限制）。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参见 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>[！UICONTROL Manage]对日历报表的访问权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

## 先决条件

1. 您必须具有自定义日期字段并在字段中提供值， [!DNL Workfront] 实例。 如果您未设置包含自定义日期的自定义表单，请按照 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. 将自定义表单附加到计划添加到日历的项目、任务或问题，并指定日期。 有关更多信息，请参阅 [向对象添加自定义表单](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## 设置项目组

您可以选择您希望项目组在日历上显示的方式。

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 位于的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 日历]**.

1. 选择要向其添加新项目组的日历。\
   或\
   单击 **[!UICONTROL +新建日历]** 并输入日历名称。

   >[!NOTE]
   >
   >您必须拥有 [!UICONTROL 编辑] 访问 [!UICONTROL 报表]， [!UICONTROL 仪表板]、和 [!UICONTROL 日历] 创建日历报表的访问级别。

1. 在左侧，单击 **[!UICONTROL 添加到日历]**，然后单击 **[!UICONTROL 添加高级项目]**.

1. 指定以下内容：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL命名这组项目]</strong></td>
      <td>键入项目组的名称。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL颜色]</strong></td>
      <td>选择项目组的颜色。 所有项目均以选定的颜色显示在日历报表中。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL日期字段]</strong></td>
      <td>选择 <strong>[！UICONTROL自定义日期]</strong>.<br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL在日历上，显示]</strong></td>
      <td><p>选择日期的显示方式：</p>
       <ul>
        <li><strong>[！UICONTROL单一日期]</strong>：日程表在单个日期显示对象。</li>
        <li><strong>[！UICONTROL Duration]（开始到结束）</strong>：日历显示天范围内的对象。<br><p>注意：如果选择 <strong>[！UICONTROL持续时间]</strong>，则指定的结束日期必须晚于开始日期，否则日历上将不会显示项目。</p></li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[！UICONTROL自定义日期]</strong></td>
      <td><p>输入附加到要跟踪的对象上的自定义日期名称。</p><p><strong>注意：</strong> 为避免性能问题，自定义日期名称的搜索限制为50个结果。</td>
     </tr>
    </tbody>
   </table>

1. 继续下一节。

## 将对象添加到项目组

设置项目显示方式后，您需要将要在日历上看到的对象添加到分组中。

1. 在 **[!UICONTROL 您希望向日历添加什么？]** 部分，选择

   * **[!UICONTROL 任务]**
   * **[!UICONTROL 项目]**
   * **[!UICONTROL 问题]**

1. 单击 **[!UICONTROL 添加任务]**， **[!UICONTROL 添加项目]**，或 **[!UICONTROL 添加问题]**，具体取决于您添加到日历中的对象类型。\
   ![选择日历对象](assets/field-name.png)

1. 在下拉菜单中，开始键入字段名称，然后选择要显示在日历上的对象的字段源(例如， **[!UICONTROL 延迟任务]**)。
1. 为日历分组设置条件语句。

   ![条件语句](assets/condition-statement-calendar.png)

   要了解如何设置条件，请参阅 [过滤器和条件修饰符](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. （可选）通过重复步骤1-4为日历分组指定其他对象。
1. 在 **[!UICONTROL 将任务/项目/问题标签设置为……]** 字段中，选择此日历分组中的对象在日历中的标签方式。

   >[!NOTE]
   >
   >如果某个对象无法使用默认标签选项，则会改为显示对象名称。 例如，当 [!UICONTROL 父任务] 已选择标签，并且没有与对象关联的父任务， [!DNL Adobe Workfront] 显示您在日历中查看的对象名称。

1. 单击&#x200B;**[!UICONTROL 保存]**。
