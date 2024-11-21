---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Google日历模块
description: 在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用Google Calendar的工作流，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: 168e8fce-645d-4108-84b7-46a113c83f41
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '3837'
ht-degree: 0%

---

# [!DNL Google Calendar]模块

在[!DNL Adobe Workfront Fusion]方案中，您可以自动执行使用[!UICONTROL Google Calendar]的工作流，并将其连接到多个第三方应用程序和服务。

如果需要有关创建方案的说明，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)中创建方案。

有关模块的信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)中的[模块。

## 访问要求

您必须具有以下权限才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td>
  <td> <p>[！UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td>
   <td> <p>[！UICONTROL计划]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td> 
   <td>
   <p>当前许可证要求：无[!DNL Workfront Fusion]许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]计划，则贵组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]才能使用本文中描述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]计划中。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]，才能使用本文中介绍的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 先决条件

要使用[!DNL Google Calendar]模块，您必须具有[!DNL Google]帐户。

## Google日历API信息

Google Calendar连接器使用以下对象：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">基本URL</td> 
   <td> https://www.googleapis.com/calendar/v3</td> 
  </tr> 
  <tr> 
   <td role="rowheader">API版本</td> 
   <td> v3 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API标记</td> 
   <td>v5.4.5</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Google Calendar]模块及其字段

配置[!DNL Google Calendar]模块时，[!DNL Workfront Fusion]显示下面列出的字段。 除此以外，可能还会显示其他[!DNL Google Calendar]字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关详细信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中将信息从一个模块映射到另一个模块。

![](assets/map-toggle-350x74.png)

* [活动](#events)
* [日程表](#calendars)
* [访问控制规则](#access-control-rules)
* [迭代器（已弃用）](#iterators-deprecated)
* [其他](#other)

### 活动

* [[!UICONTROL 观看活动]](#watch-events)
* [[!UICONTROL 搜索事件]](#search-events)
* [[!UICONTROL 获取事件]](#get-an-event)
* [[!UICONTROL 创建事件]](#create-an-event)
* [[!UICONTROL 更新事件]](#update-an-event)
* [[!UICONTROL 删除事件]](#delete-an-event)


#### [!UICONTROL 观看活动]

此触发器模块执行在您指定的日历中添加、更新、删除、启动或结束新事件的场景。 该模块返回与一个或多个记录关联的所有标准字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Google Calendar]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL日历] </td> 
   <td> <p>选择您希望模块使用的日历。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL监视活动]</td> 
   <td> <p>选择要按“创建日期”、“更新日期”、“开始日期”或“结束日期”监视事件。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL显示已删除的事件]</td> 
   <td> <p>启用此选项可包含已删除的事件。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Query] </td> 
   <td> <p>输入要搜索的文本。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL限制]</td> 
   <td> <p> 设置[!DNL Workfront Fusion]在一个周期内处理的最大事件数（每个方案运行的重复次数）。 如果该值设置得过高，则可能会中断与给定第三方服务的连接（超时）。 [!DNL Workfront Fusion]对此没有影响。 我们建议您设置较低的值，并为最大循环数定义较高的值，或者更频繁地运行方案。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜索事件]

此操作模块在选定日历中搜索事件。

指定搜索的日历和参数。

模块会返回事件的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td>有关将[!DNL Google Calendar]帐户连接到Workfront Fusion的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe Workfront Fusion的连接 — 基本说明</a></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL日历ID]</td> 
   <td> <p>选择要搜索的日历。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL开始日期]</td> 
   <td> <p> 输入或映射事件开始的日期。 此模块还会检索在此日期之前开始的、在输入的开始日期仍然发生的事件。 </p> <p>有关支持的日期和时间格式的列表，请参阅<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中键入强制。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL结束日期]</td> 
   <td> <p> 输入或映射事件结束的日期。 </p> <p> 有关支持的日期和时间格式的列表，请参阅<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中键入强制。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL单个事件]</td> 
   <td> <p> 启用此选项可将定期事件视为单个实例。 例如，如果您有一个每周会议并且启用了此选项，模块会将每周的会议作为单独事件返回。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Query]</td> 
   <td> <p>输入或映射要作为搜索依据的搜索词。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Order by]</td> 
   <td> <p>选择结果中返回的事件的顺序。</p> 
    <ul> 
     <li><strong>[！UICONTROL开始时间]</strong>：按开始日期和时间（升序）排序。 这仅在查询单个事件时可用。</li> 
     <li><strong>[！UICONTROL更新时间]</strong>：按上次修改时间（升序）排序。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL限制]</td> 
   <td> <p>设置在一个执行周期内返回的最大事件数[!DNL Workfront Fusion]。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取事件]

此操作模块返回指定日历中单个事件的元数据。

指定日历和事件。

该模块会返回事件的ID和所有关联的字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Google Calendar]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL日历ID]</td> 
   <td> <p>输入或映射包含要获取的事件的日历的ID。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL事件ID] </td> 
   <td> <p>输入要获取的现有[!DNL Google Calendar]事件的事件ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建事件]

此操作模块创建一个事件。

您可以指定事件的日历和参数。

模块会返回事件的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td>有关将[!DNL Google Calendar]帐户连接到Workfront Fusion的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe Workfront Fusion的连接 — 基本说明</a></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL创建事件]</td> 
   <td> <p>选择您希望如何创建事件。</p> 
    <ul> 
     <li><b>[！UICONTROL详细信息]</b><p>利用此选项，可更详细地介绍该事件。<br></p></li> 
     <li><b>[！UICONTROL快速]</b><p>您只需选择日历并输入事件名称即可。 您可以在名称中包含时间和地点详细信息，然后[!DNL Google Calendar]将为该时间和地点安排该事件。</p></li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL日历ID]</td> 
   <td> <p>选择要显示事件的日历。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL颜色]</td> 
   <td>选择事件在日历上显示的颜色。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL事件名称]</td> 
   <td> <p> 输入或映射事件的名称。 </p> <p>注意：如果您在[！UICONTROL创建事件]字段中选择了[！UICONTROL快速添加]，则可以包含事件的日期和时间，然后[!DNL Workfront Fusion]将针对该日期和时间创建该事件。 示例： <code>Appointment at Capitol Hill on June 3rd 10am-10:25am</code>。 如果您选择了[！UICONTROL快速添加]，但未在事件名称中包含日期和时间，则事件将从当前时间创建，并持续一小时。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL全天事件]</td> 
   <td>如果事件是全天事件（不需要开始和结束时间），则启用此选项。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL开始日期]</td> 
   <td> <p>如果这是全天事件，请输入事件的起始日期。 </p> <p>有关支持的日期格式的列表，请参阅<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中键入强制转换。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL结束日期]</td> 
   <td> <p> 如果这是全天事件，请输入事件的结束日期。 </p> <p>有关支持的日期格式的列表，请参阅<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中键入强制转换。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL描述]</td> 
   <td>输入或映射事件的描述。 此字段支持HTML。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL位置]</td> 
   <td>在文本表单中输入事件的位置。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL对此事件使用默认提醒设置]</td> 
   <td>启用此选项可使用默认提醒设置。 如果您在[！UICONTROL Reminder]字段中设置了自定义提醒，此值将设置为“否”。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL提醒] </td> 
   <td> <p>添加事件提醒。 对于每个提醒，选择要用于提醒的方法，并定义要提醒的事件之前的时长（以分钟为单位）。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL与会者]</td> 
   <td>将与会者添加到活动。 为每位与会者输入或映射其姓名和电子邮件地址。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL显示为]</td> 
   <td>选择您希望查看您的日历的人员在此活动期间将您视为“忙碌”或“可用”。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL可见性] </td> 
   <td> <p>选择此事件的可见性。 </p> 
    <ul> 
     <li> <p><b>[！UICONTROL Default]</b></p> <p>该事件具有您在日历设置中设置的可见性。</p> </li> 
     <li> <p><b>[！UICONTROL Public]</b></p> <p>与该日历共享的任何人都可以查看此事件。</p> </li> 
     <li> <p><b>[！UICONTROL Private]</b></p> <p>只有与会者才能看到此活动。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL发送有关事件创建的通知]</td> 
   <td> <p>选择是将有关创建新事件的通知发送给所有来宾、非[!DNL Google Calendar]来宾还是不发送给任何人。</p> <p>提示：我们建议仅在迁移用例中使用[！UICONTROL None]选项。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL来宾可以修改事件]</td> 
   <td> <p>如果希望来宾能够修改此事件，请启用此选项。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL循环]</td> 
   <td>添加要应用于此事件的任何周期性规则。 每个规则都需要一个[！UICONTROL RULE]、[！UICONTROL EXRULE]、[！UICONTROL RDATE]和[！UICONTROL EXDATE]行的列表才能处理定期事件。 请注意，此字段不允许出现[！UICONTROL DTSTART]和[！UICONTROL DTEND]行；事件的开始和结束时间在开始和结束字段中指定。 对于单个事件或定期事件的实例，将忽略此字段。 有关详细信息，请参阅<a href="https://tools.ietf.org/html/rfc5545#section-3.8.5">RFC5545</a>。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新事件]

此操作模块更改现有事件。

请指定日历和事件ID。

模块会返回事件的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Google Calendar]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL日历] </td> 
   <td> <p>选择要使用的日历。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL事件ID] </td> 
   <td> <p>输入先前创建的[!DNL Google Calendar]事件中要更新的事件ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

您可以通过在所需字段中输入新值来更新事件信息。 有关各个字段的详细信息，请参阅[[!UICONTROL 创建事件]](#create-an-event)。

#### [!UICONTROL 删除事件]

此操作模块删除事件。

请指定日历和事件ID。

模块会返回事件的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Google Calendar]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL日历ID]</td> 
   <td> <p>选择包含要删除的事件的日历。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL事件ID]</td> 
   <td> <p> 输入您要删除的先前创建的[!DNL Google Calendar]事件的事件ID。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL发送有关事件删除的通知]</td> 
   <td>选择您希望向所有来宾、未使用[!DNL Google Calendar]的来宾或任何人发送有关事件删除的通知。</td> 
  </tr> 
 </tbody> 
</table>

### 日程表

* [[!UICONTROL 列出日历]](#list-calendars)
* [[!UICONTROL 获取日历]](#get-a-calendar)
* [[!UICONTROL 创建日历]](#create-a-calendar)
* [[!UICONTROL 更新日历]](#update-a-calendar)
* [[!UICONTROL 删除日历]](#delete-a-calendar)
* [[!UICONTROL 清除日历]](#clear-a-calendar)

#### [!UICONTROL 列出日历]

此操作模块返回用户日历列表中的日历。

模块会返回日历的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Google Calendar]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL最低访问角色]</td> 
   <td> <p>选择用户的最低访问角色。 模块会根据此最小访问角色返回日历。</p> 
    <ul> 
     <li><strong>[！UICONTROL忙/闲信息Reader]</strong>：用户可以读取忙/闲信息。 </li> 
     <li><strong>[！UICONTROL所有者]</strong>：用户可以读取和修改事件，并且可以访问控制列表。 </li> 
     <li><strong>[！UICONTROLReader]</strong>：用户可以读取非私有事件。 </li> 
     <li><strong>[！UICONTROL Writer]</strong>：用户可以读取和修改事件。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL显示隐藏日历]</td> 
   <td>启用此选项可在模块返回的列表中包含隐藏的日历。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>设置在一个执行周期内返回的最大日历数[!DNL Workfront Fusion]。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取日历]

此操作模块可检索日历。

您可以指定要检索的日历ID。

该模块返回记录ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Google Calendar]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL日历ID]</td> 
   <td> <p>选择要检索的日历。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建日历]

此操作模块将创建新日历。

指定日历的名称。

模块会返回日历的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Google Calendar]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL日历名称]</td> 
   <td> <p> 输入新日历的名称。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新日历]

此操作模块更新日历。

您可以指定要更新的日历的ID。

模块会返回日历的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Google Calendar]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL日历ID]</td> 
   <td> <p>选择要更新的日历。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL日历名称]</td> 
   <td> <p> 输入日历的新名称。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除日历]

此操作模块删除日历。

指定要删除的日历的ID。

模块会返回日历的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Google Calendar]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL日历ID]</td> 
   <td> <p>输入或映射要删除的日历的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 清除日历]

此操作模块将从帐户的主日历中删除所有事件。

您可以指定连接到包含要清除的日历的帐户的连接。

模块会返回日历的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Google Calendar]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
 </tbody> 
</table>

### 访问控制规则

* [[!UICONTROL 列出访问控制规则]](#list-access-control-rules)
* [[!UICONTROL 获取访问控制规则]](#get-an-access-control-rule)
* [[!UICONTROL 创建访问控制规则]](#create-an-access-control-rule)
* [[!UICONTROL 更新访问控制规则]](#update-an-access-control-rule)
* [[!UICONTROL 删除访问控制规则]](#delete-an-access-control-rule)

#### [!UICONTROL 列出访问控制规则]

此操作模块返回日历上访问控制列表中的规则。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Google Calendar]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL日历ID]</td> 
   <td> <p>选择包含要检索的访问控制规则的日历。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>设置在一个执行周期内返回的最大结果数[!DNL Workfront Fusion]。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取访问控制规则]

此操作模块返回访问控制规则的元数据。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Google Calendar]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL日历ID]</td> 
   <td> <p>选择包含要检索的访问控制规则的日历。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL访问控制规则ID]</td> 
   <td>选择要检索的访问控制规则。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建访问控制规则]

此操作模块将创建新的访问控制规则。

指定日历的名称。

该模块会返回访问控制规则的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Google Calendar]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL日历ID]</td> 
   <td> <p>选择要创建访问控制规则的日历。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL角色]</td> 
   <td> <p>选择要分配给访问规则的角色。 </p> 
    <ul> 
     <li><strong>[！UICONTROL忙/闲信息Reader]</strong>：用户可以读取忙/闲信息。 </li> 
     <li><strong>[！UICONTROL所有者]</strong>：用户可以读取和修改事件，并且可以访问控制列表。 </li> 
     <li><strong>[！UICONTROLReader]</strong>：用户可以读取非私有事件。 </li> 
     <li><strong>[！UICONTROL Writer]</strong>：用户可以读取和修改事件。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL类型]</td> 
   <td> <p>选择范围的类型。 </p> 
    <ul> 
     <li><strong>[！UICONTROL默认值]</strong>：公共作用域。 这是默认值。 </li> 
     <li><strong>[！UICONTROL用户]</strong>：将范围限制为单个用户。 </li> 
     <li><strong>[！UICONTROL组]</strong>：将范围限制为组。 </li> 
     <li><strong>[！UICONTROL域]</strong>：将范围限制为域。 </li> 
    </ul> <p>注意：授予[！UICONTROL Default]或公共范围的权限适用于未经身份验证或未经过身份验证的任何用户。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL值]</td> 
   <td>根据范围类型，输入用户或组的电子邮件地址，或域的名称。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL发送通知]</td> 
   <td> <p>启用此选项可发送有关访问更改的通知。 </p> <p>注意：访问删除时没有通知。 </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新访问控制规则]

此操作模块可更新访问控制规则。

指定日历的名称。

该模块会返回访问控制规则的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Google Calendar]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL日历ID]</td> 
   <td> <p>选择包含要更新的访问控制规则的日历。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL访问控制规则ID]</td> 
   <td>选择要更新的访问控制规则。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL角色]</td> 
   <td> <p>选择要分配给访问规则的角色。 </p> 
    <ul> 
     <li><strong>[！UICONTROL None]</strong>：此角色不提供访问权限。</li> 
     <li><strong>[！UICONTROL忙/闲信息Reader]</strong>：用户可以读取忙/闲信息。 </li> 
     <li><strong>[！UICONTROL所有者]</strong>：用户可以读取和修改事件，并且可以访问控制列表。 </li> 
     <li><strong>[！UICONTROLReader]</strong>：用户可以读取非私有事件。 </li> 
     <li><strong>[！UICONTROL Writer]</strong>：用户可以读取和修改事件。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL发送通知]</td> 
   <td> <p>启用此选项可发送有关访问更改的通知。 </p> <p>注意：访问删除时没有通知。 </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除访问控制规则]

此操作模块删除访问控制规则。

指定日历的名称。

该模块会返回访问控制规则的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Google Calendar]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL日历ID]</td> 
   <td> <p>选择或映射包含要删除的访问控制规则的日历的ID。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL访问控制规则ID]</td> 
   <td>选择或映射要删除的访问控制规则的ID。</td> 
  </tr> 
 </tbody> 
</table>

### 迭代器（已弃用）

已弃用[!UICONTROL 迭代附件]和[!UICONTROL 迭代出席者]模块。 若要迭代附件或与会者，请使用[!UICONTROL 流控件] > [!UICONTROL 迭代器]模块。 有关详细信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md)中的[迭代器模块

### 其他

* [[!UICONTROL 进行API调用]](#make-an-api-call)
* [[!UICONTROL 获取忙/闲信息]](#get-freebusy-information)

#### [!UICONTROL 进行API调用]

此模块允许您执行自定义API调用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Google Calendar]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL URL]</p> </td> 
   <td>输入相对于<code>https://www.googleapis.com/calendar</code>的路径。 示例： <code>/v3/users/me/calendarList</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL方法]</p> </td> 
   td&gt; <p>选择配置API调用所需的HTTP请求方法。 有关详细信息，请参阅[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP请求方法。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。例如，<code>{"Content-type":"application/json"}</code>。 [!DNL Workfront Fusion]为您添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查询字符串]</td> 
   <td> <p> 以标准JSON对象的形式添加API调用的查询。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Body]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的正文内容。</p> <p>注意：   <p>在JSON中使用条件语句（如<code>if</code>）时，请将引号放在条件语句之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取忙/闲信息]

此操作模块返回一组日历的空闲和忙碌信息。

模块会返回日历的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td>有关将[!DNL Google Calendar]帐户连接到Workfront Fusion的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe Workfront Fusion的连接 — 基本说明</a></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL最短时间]</td> 
   <td> <p> 输入要检索其信息的间隔的开始。</p> <p> 有关支持的日期和时间格式的列表，请参阅<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中键入强制。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL最大时间]</td> 
   <td> <p> 输入要检索其信息的间隔的结束。 </p> <p>有关支持的日期和时间格式的列表，请参阅<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中键入强制。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL日历]</td> 
   <td> <p>对于要从中检索信息的每个日历，单击<strong>添加</strong>并输入或映射日历ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 在事件之前触发方案

借助标准[!DNL Google Calendar]电子邮件提醒和[!UICONTROL Webhook] >[!UICONTROL 自定义mailhook]模块，您可以在事件之前的指定时间触发方案。

1. 使用[!UICONTROL Google日历] >[!UICONTROL 更新活动]模块向活动添加电子邮件提醒：

   ![](assets/trigger-scen-before-event-350x209.png)

1. 创建以[!UICONTROL Webhook] >[!UICONTROL 自定义mailhook]模块开头的新方案。

   1. 复制mailhook的电子邮件地址。
   1. 保存场景并执行它。

1. 在[!DNL Gmail]中，将[!DNL Google Calendar]电子邮件提醒重定向到邮件挂接的电子邮件地址：

   1. 打开您的&#x200B;**[!UICONTROL [!DNL Gmail]设置]**。
   1. 打开&#x200B;**[!UICONTROL 转发和POP/IMAP]**&#x200B;选项卡。
   1. 单击&#x200B;**[!UICONTROL 添加转发地址]。**
   1. 粘贴复制的邮件挂钩的电子邮件地址，单击&#x200B;**[!UICONTROL 下一步]**，在弹出窗口中按&#x200B;**[!UICONTROL 继续]**&#x200B;进行确认，然后单击&#x200B;**[!UICONTROL 确定]**。

   1. 在[!DNL Workfront Fusion]中，切换到应通过接收确认电子邮件完成其执行的新方案。
   1. 单击模块上方的气泡以检查模块的输出。
   1. 展开`Text`项目并复制确认代码：

      ![](assets/confirmation-code-350x252.png)

   1. 在Gmail中，将确认代码粘贴到编辑框中，然后单击&#x200B;**[!UICONTROL 验证]**：

      ![](assets/paste-code-350x46.png)

   1. 打开&#x200B;**[!UICONTROL 筛选器和阻止的地址]**&#x200B;选项卡。
   1. 单击&#x200B;**[!UICONTROL 创建新筛选器]**。
   1. 为来自`     calendar-notification@google.com`的所有电子邮件设置一个过滤器，然后单击&#x200B;**[!UICONTROL 创建过滤器]**：
   1. 选择&#x200B;**[!UICONTROL 将其转发到]**，然后从列表中选择邮件挂接的电子邮件地址。
   1. 单击&#x200B;**[!UICONTROL 创建筛选器]**&#x200B;以创建筛选器。

1. （可选）在[!DNL Workfront Fusion]中，在[!UICONTROL Webhooks] >[!UICONTROL 自定义mailhook]模块之后添加[!UICONTROL 文本解析器] > [!UICONTROL 匹配模式]模块，以解析电子邮件的HTML代码以获取您需要的任何信息。

   例如，您可以按如下方式配置模块，以获取事件的ID：

   *模式*： `<meta itemprop="eventId/googleCalendar" content="(?<evenitID>.*?)"/>`

   *文本*：从[!UICONTROL Webhook] >[!UICONTROL 自定义mailhook]模块输出的`HTML content`项目。
