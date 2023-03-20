---
title: 设置提醒通知
description: 设置提醒通知
author: Alina, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6c0fa8af-cd89-4941-a6f6-aa4e84a7dc67
source-git-commit: bbd99435bb07d68bf9058bcd3e8c6ef5d9df75a9
workflow-type: tm+mt
source-wordcount: '1146'
ht-degree: 1%

---

# 设置提醒通知

提醒通知会根据指定的条件向收件人发送电子邮件。 作为Adobe Workfront管理员或具有计划员访问权限级别和对提醒通知的管理访问权限的用户，您可以手动将提醒通知与工作项（如项目、任务、问题和时间表）关联。

<!--
DRAFTED IN FLARE:
An example of how this can be used would be helpful here and/or in the section </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications" class="MCXref xref">Reminder notifications</a>
 in </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md" class="MCXref xref">Adobe Workfront notifications</a>

-->

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>计划员或更高级别，具有提醒通知的管理访问权限</p> <p>有关授予计划用户管理访问权限的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用户对特定区域的管理访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 自定义提醒电子邮件

您可以使用包含自定义电子邮件主题和正文的自定义电子邮件自定义提醒通知。 电子邮件正文可以包含自定义HTML。

或者，您也可以使用提醒通知中包含的默认电子邮件。 默认电子邮件使用提醒通知名称作为电子邮件主题和电子邮件正文中的对象名称，包括触发通知的事件。

如果要自定义提醒电子邮件，您需要创建电子邮件模板并将其附加到提醒通知。

有关如何创建电子邮件模板的信息，请参阅 [配置电子邮件模板](../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md).

## 创建提醒通知

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **电子邮件** > **通知**.

1. 单击 **提醒通知** ，然后单击 **新提醒通知**.

1. 在下拉列表中，单击要与提醒通知关联的对象类型。

   例如，如果要将提醒通知附加到时间表，请单击 **时间表**.

1. 在 **新提醒通知** 框中，指定以下信息。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">提醒通知名称</td> 
      <td>指定提醒通知的名称。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">等待期</td> 
      <td> <p>在 <strong>计时</strong> 字段。</p> <p><b>注释</b>:  
        <ul> 
         <li> <p>提醒通知在指定日期后24小时开始，并在满足所有标准后开始。</p> </li> 
         <li> <p>项目、任务和问题的提醒通知会在美国山区时间的午夜触发。 从那天起符合提醒通知条件的所有对象都会在该时间后不久向指定用户发送通知。</p> </li> 
         <li> <p>工时单提醒通知会根据您所在的时区和工时单的“结束日期”、“开始日期”或“上次更新日期”在指定时间发送。</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">计时</td> 
      <td> <p>选择触发要计划的提醒通知的事件。</p> <p>如果提醒通知是针对项目、任务或问题发出的，则可用选项与完成日期或开始日期相关。 提醒通知会考虑项目、任务和问题的完成和开始日期上的时间戳。</p>

   <p>如果提醒通知适用于工时单，则可用选项与“结束日期”、“开始日期”或“上次更新日期”相关。 工时单提醒通知考虑工时单结束、开始和上次更新日期的时间戳。 时间表从开始日期的午夜（中午12:00）开始，直到结束日期的午夜（晚上11:59）结束。</p>

   <p><b>注释</b></p>
      <p>每24小时只分发一次时间表提醒通知。</p> <p>当您在24小时内设置多个提醒通知时，Workfront会发出一封通知电子邮件，其中包含该通知中包含的所有提醒。</p>
      <p>例如，如果将三个提醒通知配置为在到期日期前10小时、前2小时和前1小时触发，则如果这三个提醒都发生在同一天，则它们都将合并到同一通知中。</p> <p>但是，如果将提醒通知设置为26小时之前，将再设置一个提醒通知设置为1小时之后，用户将收到两个单独的通知。 </p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">标准</td> 
      <td> <p>选择标准以确定要计划的提醒通知。 除非满足标准选择，否则不会计划提醒通知。</p> <p>根据您在步骤4中选择的对象类型，可以使用以下标准选项：</p> 
       <ul> 
        <li><strong>当前项目中不完整：</strong> （可用于任务和问题提醒）仅当与提醒通知关联的对象状态为“未完成”且项目状态为“当前”时，才计划发送提醒通知。</li> 
        <li><strong>当前项目中的所有项目：</strong>（可用于任务和问题提醒）无论对象状态如何，并且仅当与提醒通知关联的项目状态为“当前”时，都会计划发送提醒通知。</li> 
        <li><strong>项目不完整：</strong> （可用于项目提醒）当项目状态为“完成”以外的任何情况时，将计划发送提醒通知。</li> 
        <li><strong>完成项目：</strong> （可用于项目提醒）将在项目状态为“完成”时发送提醒通知。</li> 
        <li><strong>打开工时单：</strong> （可用于工时单提醒）在工时单状态为“打开”时，将发送提醒通知。</li> 
        <li><strong>提交的工时单：</strong> （可用于工时单提醒）提醒通知计划在提交工时单状态时发送。</li> 
        <li><strong>每周打开工时单或少于40小时：</strong> （可用于工时单提醒）在工时单状态为“打开”或工时单记录时间少于40小时时，将发送提醒通知。</li> 
        <li><strong>电子邮件模板：</strong> 从下拉菜单中，选择要附加到提醒的电子邮件模板。<br>有关如何构建电子邮件模板的信息，请参阅 <a href="../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md" class="MCXref xref">配置电子邮件模板</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">收件人</td> 
      <td>选择要接收通知的用户类型。 从各种对象利益相关方（如所有者、审批者或代理人）中进行选择。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存**。
1. 将提醒通知附加到工作项，如 [将提醒通知附加到对象](../../../workfront-basics/using-notifications/attach-reminder-notification-object.md).

## 接收提醒通知

如果在附加了提醒通知的项目上满足条件，则会向在提醒通知中定义的用户触发电子邮件通知。

有关接收提醒通知的更多信息，请参阅 [提醒通知](../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications) 部分 [Adobe Workfront通知](../../../workfront-basics/using-notifications/wf-notifications.md).

## 测试提醒通知投放

提醒通知会在每天午夜（山区时间）触发。 符合提醒通知条件的所有对象都会在通知后不久向指定用户发送通知。

要手动触发提醒通知，必须首先满足提醒的条件。\
例如，如果将提醒设置为在项目的计划完成日期后一小时触发，则该时间必须在设置提醒时和现在之间经过。 在激活提醒之前已通过计划完成日期的任何项目将不会触发通知。

要手动触发提醒通知，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **系统** > **诊断** 在Workfront的左下角。

1. 单击 **发送提醒通知** 然后等待屏幕顶部的确认消息已发送。

   提醒通知中指定的用户会收到一封电子邮件。
