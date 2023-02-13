---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Google日历模块
description: 在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用Google日历的工作流，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: 168e8fce-645d-4108-84b7-46a113c83f41
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '3773'
ht-degree: 0%

---

# [!DNL Google Calendar] 模块

在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!UICONTROL Google日历]，并将其连接到多个第三方应用程序和服务。

如果您需要有关创建方案的说明，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

有关模块的信息，请参阅 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## 访问要求

您必须具有以下访问权限才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td>
  <td> <p>[!UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td>
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 先决条件

使用 [!DNL Google Calendar] 模块，您必须 [!DNL Google] 帐户。

## [!DNL Google Calendar] 模块及其字段

配置 [!DNL Google Calendar] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!DNL Google Calendar] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [事件](#events)
* [日历](#calendars)
* [访问控制规则](#access-control-rules)
* [迭代器（已弃用）](#iterators-deprecated)
* [其他](#other)

### 事件

* [[!UICONTROL 观看事件]](#watch-events)
* [[!UICONTROL 搜索事件]](#search-events)
* [[!UICONTROL 获取事件]](#get-an-event)
* [[!UICONTROL 创建事件]](#create-an-event)
* [[!UICONTROL 更新事件]](#update-an-event)
* [[!UICONTROL 删除事件]](#delete-an-event)


#### [!UICONTROL 观看事件]

当在您指定的日历中添加、更新、删除、启动或结束新事件时，此触发器模块会执行一个方案。 模块会返回与记录或记录关联的所有标准字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Calendar] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接到Adobe [!DNL Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日历] </td> 
   <td> <p>选择您希望模块使用的日历。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch Events]</td> 
   <td> <p>选择要按创建日期、更新日期、开始日期还是结束日期来观看事件。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL显示已删除的事件]</td> 
   <td> <p>启用此选项可包含已删除的事件。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL查询] </td> 
   <td> <p>输入要搜索的文本。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL限制]</td> 
   <td> <p> 设置 [!DNL Workfront Fusion] 在一个周期内使用（每个方案运行的重复次数）。 如果该值设置得过高，则给定第三方服务的连接可能会中断（超时）。 [!DNL Workfront Fusion] 对此没有影响。 我们建议您设置一个较低的值，并为最大循环数定义一个较高的值，或者更频繁地运行该方案。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜索事件]

此操作模块会搜索选定日历中的事件。

指定搜索的日历和参数。

模块会返回事件的ID和任何关联的字段，以及连接访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td>有关连接 [!DNL Google Calendar] 帐户到Workfront Fusion，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe Workfront Fusion的连接 — 基本说明</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日历ID]</td> 
   <td> <p>选择要搜索的日历。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL开始日期]</td> 
   <td> <p> 输入或映射事件开始的日期。 此模块还会检索在此日期之前开始的事件，这些事件在输入的开始日期仍然会发生。 </p> <p>有关支持的日期和时间格式的列表，请参阅 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在中键入强制 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL结束日期]</td> 
   <td> <p> 输入或映射事件结束的日期。 </p> <p> 有关支持的日期和时间格式的列表，请参阅 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在中键入强制 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL单个事件]</td> 
   <td> <p> 启用此选项可将定期事件视为单个实例。 例如，如果您有每周会议，并且此选项处于启用状态，则模块会将每周的会议作为单独的事件返回。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL查询]</td> 
   <td> <p>输入或映射要搜索的搜索词。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Order by]</td> 
   <td> <p>选择在结果中返回的事件的顺序。</p> 
    <ul> 
     <li><strong>[!UICONTROL开始时间]</strong>:按开始日期和时间排序（升序）。 仅当查询单个事件时，才可使用此选项。</li> 
     <li><strong>[!UICONTROL更新时间]</strong>:按上次修改时间排序（升序）。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL限制]</td> 
   <td> <p>设置最大事件数 [!DNL Workfront Fusion] 在一个执行周期中返回。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取事件]

此操作模块会返回指定日历中单个事件的元数据。

指定日历和事件。

模块会返回事件的ID和所有关联字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Calendar] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接到Adobe [!DNL Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日历ID]</td> 
   <td> <p>输入或映射包含要获取事件的日历的ID。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL事件ID] </td> 
   <td> <p>输入现有 [!DNL Google Calendar] 事件。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建事件]

此操作模块会创建一个事件。

您可以指定事件的日历和参数。

模块会返回事件的ID和任何关联的字段，以及连接访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td>有关连接 [!DNL Google Calendar] 帐户到Workfront Fusion，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe Workfront Fusion的连接 — 基本说明</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL创建事件]</td> 
   <td> <p>选择创建事件的方式。</p> 
    <ul> 
     <li><b>[!UICONTROL详细信息]</b><p>利用此选项，可详细了解事件。<br></p></li> 
     <li><b>[!UICONTROL Quickly]</b><p>您只需选择日历并输入事件的名称即可。 您可以在名称中包含时间和位置详细信息，以及 [!DNL Google Calendar] 将安排该位置和时间的事件。</p></li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日历ID]</td> 
   <td> <p>选择要显示事件的日历。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL颜色]</td> 
   <td>选择事件在日历中显示的颜色。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL事件名称]</td> 
   <td> <p> 输入或映射事件的名称。 </p> <p>注意：如果您在[!UICONTROL创建事件]字段中选择了[!UICONTROL快速添加]，则可以包含事件的日期和时间，以及 [!DNL Workfront Fusion] 为该日期和时间创建事件。 示例: <code>Appointment at Capitol Hill on June 3rd 10am-10:25am</code>. 如果您选择了[!UICONTROL快速添加]，但事件名称中未包含日期和时间，则该事件将从当前时间创建，并持续一小时。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL All day event]</td> 
   <td>如果事件是一整天事件（不需要开始和结束时间），则启用此选项。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL开始日期]</td> 
   <td> <p>如果这是一个全天事件，请输入事件的开始日期。 </p> <p>有关支持的日期格式列表，请参阅 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在中键入强制 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL结束日期]</td> 
   <td> <p> 如果这是一个全天事件，请输入事件的结束日期。 </p> <p>有关支持的日期格式列表，请参阅 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在中键入强制 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL描述]</td> 
   <td>输入或映射事件的描述。 此字段支持HTML。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL位置]</td> 
   <td>在文本表单中输入事件的位置。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL使用此事件的默认提醒设置]</td> 
   <td>启用此选项可使用默认提醒设置。 如果在[!UICONTROL提醒]字段中设置了自定义提醒，则此值将设置为“否”。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL提醒] </td> 
   <td> <p>添加事件提醒。 对于每个提醒，选择要使用的提醒方法，并定义要提醒事件的时长（以分钟为单位）。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL与会者]</td> 
   <td>将与会者添加到活动。 对于每个与会者，输入或映射其姓名和电子邮件地址。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL将我显示为]</td> 
   <td>选择您希望查看日历的人员在此事件期间将您视为忙或可用。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL可见性] </td> 
   <td> <p>选择此事件的可见性。 </p> 
    <ul> 
     <li> <p><b>[!UICONTROL默认]</b></p> <p>该事件具有您在日历设置中设置的可见性。</p> </li> 
     <li> <p><b>[!UICONTROL Public]</b></p> <p>与共享日历的任何人都可以查看此事件。</p> </li> 
     <li> <p><b>[!UICONTROL Private]</b></p> <p>只有与会者才能看到此活动。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL发送有关事件创建的通知]</td> 
   <td> <p>选择是否将有关创建新事件的通知发送给所有来宾、非[!DNL Google Calendar] 客人，或者没人。</p> <p>提示：我们建议仅对迁移用例使用[!UICONTROL None]选项。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL来宾可以修改事件]</td> 
   <td> <p>如果希望来宾能够修改此事件，请启用此选项。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL循环]</td> 
   <td>添加要应用于此事件的任何循环规则。 每个规则都需要循环事件的[!UICONTROL RULE]、[!UICONTROL EXRULE]、[!UICONTROL RDATE]和[!UICONTROL EXDATE]行的列表。 请注意，此字段中不允许使用[!UICONTROL DTSTART]和[!UICONTROL DTEND]行；在开始和结束字段中指定事件开始和结束时间。 对于单个事件或定期事件的实例，将忽略此字段。 有关更多信息，请参阅 <a href="https://tools.ietf.org/html/rfc5545#section-3.8.5">RFC5545</a>.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新事件]

此操作模块会更改现有事件。

您可以指定日历和事件ID。

模块会返回事件的ID和任何关联的字段，以及连接访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Calendar] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接到Adobe [!DNL Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日历] </td> 
   <td> <p>选择要处理的日历。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL事件ID] </td> 
   <td> <p>输入之前创建的 [!DNL Google Calendar] 要更新的事件。</p> </td> 
  </tr> 
 </tbody> 
</table>

您可以通过在所需字段中输入新值来更新事件信息。 有关各个字段的详细信息，请参阅 [[!UICONTROL 创建事件]](#create-an-event).

#### [!UICONTROL 删除事件]

此操作模块会删除事件。

您可以指定日历和事件ID。

模块会返回事件的ID和任何关联的字段，以及连接访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Calendar] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接到Adobe [!DNL Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日历ID]</td> 
   <td> <p>选择包含要删除事件的日历。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL事件ID]</td> 
   <td> <p> 输入之前创建的事件ID [!DNL Google Calendar] 事件。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL发送有关事件删除的通知]</td> 
   <td>选择是否要向所有未使用的来宾和来宾发送有关事件删除的通知 [!DNL Google Calendar]，或者没有人。</td> 
  </tr> 
 </tbody> 
</table>

### 日历

* [[!UICONTROL 列出日历]](#list-calendars)
* [[!UICONTROL 获取日历]](#get-a-calendar)
* [[!UICONTROL 创建日历]](#create-a-calendar)
* [[!UICONTROL 更新日历]](#update-a-calendar)
* [[!UICONTROL 删除日历]](#delete-a-calendar)
* [[!UICONTROL 清除日历]](#clear-a-calendar)

#### [!UICONTROL 列出日历]

此操作模块会返回用户日历列表上的日历。

模块会返回日历和任何关联字段的ID，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Calendar] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接到Adobe [!DNL Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL最低访问角色]</td> 
   <td> <p>为用户选择最低访问角色。 模块会根据此最小访问角色返回日历。</p> 
    <ul> 
     <li><strong>[!UICONTROL Free BusyReader]</strong>:用户可以读取忙/闲信息。 </li> 
     <li><strong>[!UICONTROL所有者]</strong>:用户可以读取和修改事件，并可以访问控制列表。 </li> 
     <li><strong>[!UICONTROLReader]</strong>:用户可以读取非专用事件。 </li> 
     <li><strong>[!UICONTROL Writer]</strong>:用户可以读取和修改事件。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL显示隐藏的日历]</td> 
   <td>启用此选项可在模块返回的列表中包含隐藏的日历。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td>设置最大日历数 [!DNL Workfront Fusion] 在一个执行周期中返回。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取日历]

此操作模块检索日历。

您指定要检索的日历的ID。

模块会返回记录的ID和任何关联字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Calendar] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接到Adobe [!DNL Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL日历ID]</td> 
   <td> <p>选择要检索的日历。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建日历]

此操作模块会创建新日历。

您指定日历的名称。

模块会返回日历和任何关联字段的ID，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Calendar] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接到Adobe [!DNL Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日历名称]</td> 
   <td> <p> 输入新日历的名称。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新日历]

此操作模块会更新日历。

您指定要更新的日历的ID。

模块会返回日历和任何关联字段的ID，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Calendar] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接到Adobe [!DNL Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日历ID]</td> 
   <td> <p>选择要更新的日历。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日历名称]</td> 
   <td> <p> 输入日历的新名称。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除日历]

此操作模块会删除日历。

您指定要删除的日历的ID。

模块会返回日历和任何关联字段的ID，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Calendar] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接到Adobe [!DNL Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL日历ID]</td> 
   <td> <p>输入或映射要删除的日历的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 清除日历]

此操作模块会从帐户的主日历中删除所有事件。

您指定连接到包含要清除的日历的帐户的连接。

模块会返回日历和任何关联字段的ID，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Calendar] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接到Adobe [!DNL Workfront Fusion]  — 基本说明</a></p> </td> 
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

此操作模块返回日历访问控制列表中的规则。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Calendar] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接到Adobe [!DNL Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL日历ID]</td> 
   <td> <p>选择包含要检索的访问控制规则的日历。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td>设置最大结果数 [!DNL Workfront Fusion] 在一个执行周期中返回。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取访问控制规则]

此操作模块会返回访问控制规则的元数据。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Calendar] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接到Adobe [!DNL Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL日历ID]</td> 
   <td> <p>选择包含要检索的访问控制规则的日历。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL访问控制规则ID]</td> 
   <td>选择要检索的访问控制规则。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建访问控制规则]

此操作模块会创建新的访问控制规则。

您指定日历的名称。

模块会返回访问控制规则的ID和任何关联的字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Calendar] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接到Adobe [!DNL Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日历ID]</td> 
   <td> <p>选择要创建访问控制规则的日历。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL角色]</td> 
   <td> <p>选择要分配给访问规则的角色。 </p> 
    <ul> 
     <li><strong>[!UICONTROL Free BusyReader]</strong>:用户可以读取忙/闲信息。 </li> 
     <li><strong>[!UICONTROL所有者]</strong>:用户可以读取和修改事件，并可以访问控制列表。 </li> 
     <li><strong>[!UICONTROLReader]</strong>:用户可以读取非专用事件。 </li> 
     <li><strong>[!UICONTROL Writer]</strong>:用户可以读取和修改事件。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type]</td> 
   <td> <p>选择范围类型。 </p> 
    <ul> 
     <li><strong>[!UICONTROL默认]</strong>:公众范围。 这是默认值。 </li> 
     <li><strong>[!UICONTROL用户]</strong>:将范围限制为单个用户。 </li> 
     <li><strong>[!UICONTROL组]</strong>:将范围限制为组。 </li> 
     <li><strong>[!UICONTROL域]</strong>:将范围限制为域。 </li> 
    </ul> <p>注意：授予[!UICONTROL Default]或公共范围的权限适用于任何经过身份验证的用户。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL值]</td> 
   <td>根据范围类型，输入用户或群组的电子邮件地址或域名。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL发送通知]</td> 
   <td> <p>启用此选项可发送有关访问更改的通知。 </p> <p>注意：没有关于删除访问权限的通知。 </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新访问控制规则]

此操作模块更新访问控制规则。

您指定日历的名称。

模块会返回访问控制规则的ID和任何关联的字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Calendar] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接到Adobe [!DNL Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日历ID]</td> 
   <td> <p>选择包含要更新的访问控制规则的日历。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL访问控制规则ID]</td> 
   <td>选择要更新的访问控制规则。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL角色]</td> 
   <td> <p>选择要分配给访问规则的角色。 </p> 
    <ul> 
     <li><strong>[!UICONTROL无]</strong>:此角色不提供访问权限。</li> 
     <li><strong>[!UICONTROL Free BusyReader]</strong>:用户可以读取忙/闲信息。 </li> 
     <li><strong>[!UICONTROL所有者]</strong>:用户可以读取和修改事件，并可以访问控制列表。 </li> 
     <li><strong>[!UICONTROLReader]</strong>:用户可以读取非专用事件。 </li> 
     <li><strong>[!UICONTROL Writer]</strong>:用户可以读取和修改事件。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL发送通知]</td> 
   <td> <p>启用此选项可发送有关访问更改的通知。 </p> <p>注意：没有关于删除访问权限的通知。 </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除访问控制规则]

此操作模块会删除访问控制规则。

您指定日历的名称。

模块会返回访问控制规则的ID和任何关联的字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Calendar] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接到Adobe [!DNL Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日历ID]</td> 
   <td> <p>选择或映射包含要删除的访问控制规则的日历的ID。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL访问控制规则ID]</td> 
   <td>选择或映射要删除的访问控制规则的ID。</td> 
  </tr> 
 </tbody> 
</table>

### 迭代器（已弃用）

的 [!UICONTROL 迭代附件] 和 [!UICONTROL 邀请与会者] 模块已弃用。 要迭代附件或与会者，请使用 [!UICONTROL 流量控制] > [!UICONTROL 迭代器] 模块。 有关更多信息，请参阅 [中的迭代器模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md)

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
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Google Calendar] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接到Adobe [!DNL Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td>输入相对于 <code>https://www.googleapis.com/calendar</code>. 示例: <code>/v3/users/me/calendarList</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL方法]</p> </td> 
   td&gt; <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。例如， <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] 为您添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查询字符串]</td> 
   <td> <p> 以标准JSON对象的形式添加API调用的查询。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主体]</td> 
   <td> <p>以标准JSON对象的形式为API调用添加正文内容。</p> <p>注释:   <p>使用条件语句时，例如 <code>if</code> 在JSON中，将引号放置在条件语句的外部。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取忙/闲信息]

此操作模块会返回一组日历的忙闲信息。

模块会返回日历和任何关联字段的ID，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td>有关连接 [!DNL Google Calendar] 帐户到Workfront Fusion，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe Workfront Fusion的连接 — 基本说明</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Minimum Time]</td> 
   <td> <p> 输入要检索其信息的间隔的开始。</p> <p> 有关支持的日期和时间格式的列表，请参阅 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在中键入强制 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximum time]</td> 
   <td> <p> 输入要检索其信息的间隔的结尾。 </p> <p>有关支持的日期和时间格式的列表，请参阅 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在中键入强制 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日历]</td> 
   <td> <p>对于要从中检索信息的每个日历，单击 <strong>添加</strong> 并输入或映射日历ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 在事件之前触发方案

您可以在标准帮助下，在事件之前的指定时间触发方案 [!DNL Google Calendar] 电子邮件提醒和 [!UICONTROL Webhooks] >[!UICONTROL 自定义邮件挂接] 模块。

1. 使用 [!UICONTROL Google日历] >[!UICONTROL 更新事件] 用于向事件添加电子邮件提醒的模块：

   ![](assets/trigger-scen-before-event-350x209.png)

1. 创建新方案，从 [!UICONTROL Webhooks] >[!UICONTROL 自定义邮件挂接] 模块。

   1. 复制邮件挂接的电子邮件地址。
   1. 保存方案并执行它。

1. 在 [!DNL Gmail]，重定向 [!DNL Google Calendar] 电子邮件提醒邮件挂接的电子邮件地址：

   1. 打开 **[!UICONTROL [!DNL Gmail]设置]**.
   1. 打开 **[!UICONTROL 转发和POP/IMAP]** 选项卡。
   1. 单击 **[!UICONTROL 添加转发地址].**
   1. 粘贴复制的邮件挂接的电子邮件地址，单&#x200B;击&#x200B;**[!UICONTROL 下一个]**，按确认 **[!UICONTROL 继续]** 在弹出窗口中，单击 **[!UICONTROL 确定]**.

   1. 在 [!DNL Workfront Fusion]，切换到应通过接收确认电子邮件来完成其执行的新方案。
   1. 单击模块上方的气泡以检查模块的输出。
   1. 展开 `Text` 项目，并复制确认代码：

      ![](assets/confirmation-code-350x252.png)

   1. 在Gmail中，将确认代码粘贴到编辑框中，然后单&#x200B;击&#x200B;**[!UICONTROL 验证]**:

      ![](assets/paste-code-350x46.png)

   1. 打开 **[!UICONTROL 过滤器和阻止的地址]** 选项卡。
   1. 单击 **[!UICONTROL 创建新过滤器]**.
   1. 为来自的所有电子邮件设置过滤器 `     calendar-notification@google.com` 单击&#x200B;**[!UICONTROL 创建过滤器]**:
   1. 选择 **[!UICONTROL 将其转发到]** 并从列表中选择邮件挂接的电子邮件地址。
   1. 单击 **[!UICONTROL 创建过滤器]** 来创建过滤器。

1. （可选）在 [!DNL Workfront Fusion]，添加 [!UICONTROL 文本解析器] > [!UICONTROL 匹配模式] 模块之后 [!UICONTROL Webhooks] >[!UICONTROL 自定义邮件挂接] 模块，用于解析电子邮件的HTML代码以获取您需要的任何信息。

   例如，您可以按如下方式配置模块以获取事件的ID:

   *图案*: `<meta itemprop="eventId/googleCalendar" content="(?<evenitID>.*?)"/>`

   *文本*:的 `HTML content` 从 [!UICONTROL Webhooks] >[!UICONTROL 自定义邮件挂接] 模块。
