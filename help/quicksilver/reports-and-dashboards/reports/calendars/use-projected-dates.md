---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: 在日历报表中使用预计日期
description: 日历报表是动态报表，可直观地呈现您的工作。 您可以在日历报表中对任务、问题和项目使用“预计日期”字段。
author: Lisa
feature: Reports and Dashboards
exl-id: 39e16f0b-c10d-429e-9eb5-d4847c7e4ed9
source-git-commit: e5a3024b1657942cd7abdfff76a7a6795127a4f5
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 1%

---

# 使用 [!UICONTROL 预计日期] 在日历报表中

日历报表是动态报表，可直观地呈现您的工作。 您可以在日历报表中为以下对象使用“预计日期”字段：

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
   <td> <p>[!UICONTROL ]编辑对[!UICONTROL报表]、[!UICONTROL功能板]和[!UICONTROL日历]的访问权限</p> <p>注意：如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>[!UICONTROL管理]对日历报表的访问权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 设置项目组

您可以选择希望在日历上显示项目组的方式。

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **[!UICONTROL 日历]**.

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
      <td><p>选择 <strong>[!UICONTROL预计日期]</strong>. 有关预计日期的详细信息，请参阅 </p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-projected-start-date.md" class="MCXref xref">项目预计起始日期概览</a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">项目、任务和问题的预计完成日期概览</a><br></li>
       </ul></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL在日历上，show]</strong></td>
      <td><p>选择日期的显示方式：</p>
       <ul>
        <li><strong>[!UICONTROL仅开始日期]</strong>:日历在单个日期显示对象。</li>
        <li><strong>[!UICONTROL仅结束日期]</strong>:日历在单个日期显示对象。</li>
        <li><strong>[!UICONTROL持续时间]（从开始到结束）</strong>:日历会显示跨天的对象。</li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL切换到实际日期（如果可用）]</strong></td>
      <td><p>日历在可用时会自动切换到实际日期。 <br>选择 <strong>[!UICONTROL Yes]</strong> 或 <strong>[!UICONTROL No]</strong> 切换到实际日期（如果可用）。 有关实际日期的详细信息，请参阅</p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">项目实际开始日期概览 </a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">项目实际完成日期概览 </a></li>
       </ul></td>
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

1. 在下拉菜单中，开始键入字段名称，然后选择要在日历中显示的对象的字段源(例如， **[!UICONTROL 延迟任务]**)。
1. 为日历分组设置条件语句。

   ![条件语句](assets/condition-statement-calendar.png)

   要了解设置条件，请参阅 [过滤器和条件修饰符](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. （可选）重复步骤1-4为日历分组指定其他对象。
1. 在 **[!UICONTROL 将“任务/项目/问题”标签设置为……]** 字段中，选择此日历分组中对象在日历中的标记方式。

   >[!NOTE]
   >
   >如果默认标签选项对特定对象不可用，则会显示对象名称。 例如，如果选择了“父任务”标签，并且没有与对象关联的父任务， [!DNL Adobe Workfront] 显示您在日历中查看的对象名称。

1. 单击&#x200B;**[!UICONTROL 保存]**。
