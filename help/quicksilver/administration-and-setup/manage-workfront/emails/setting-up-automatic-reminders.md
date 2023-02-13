---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: 设置自动提醒
description: 设置自动提醒
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 37ad04a1-d3c8-48b2-aed8-fe40456196ec
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 1%

---

# 设置自动提醒

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

作为Adobe Workfront管理员，您可以设置自动提醒，以在所有任务或问题都到期、延迟或接近计划完成日期时触发电子邮件通知。 配置这些设置后，用户将无法禁用自动提醒。

对于延迟通知，在任务或问题完成之前，会在夜间发送电子邮件。

自动提醒可以发送到以下一个或多个：

* 分配给任务或问题的用户
* 用户的直接经理
* 直接经理的经理

>[!NOTE]
>
>您无法更改由自动提醒触发的电子邮件的内容或主题行。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>系统管理员</p> </td> 
  </tr> 
 </tbody> 
</table>

## 设置自动提醒

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **电子邮件** >**自动提醒**.

1. 在 **向发送延迟通知** 区域，选择以下任意选项：

   <table>
    <tr>
        <td>“分配给”用户</td>
        <td>如果希望分配给任务或问题的用户接收有关其工作项延迟的延迟通知，请选择此选项。</td>
        <td></td>
    </tr>
    <tr>
        <td>用户的经理</td>
        <td>如果希望用户的经理收到有关其直接报表工作项目延迟的通知，请选择此选项。</td>
        <td></td>
    </tr>
    <tr>
        <td>经理的经理</td>
        <td>如果希望直接经理的经理收到有关其某个直接报表用户的工作项延迟的通知，请选择此选项。</td>
        <td></td>
    </tr>
    <tr>
        <td>“分配给”用户</td>
        <td>(在 <b>向发送截止时间提醒</b> 区域。) 如果希望将用户分配到任务或问题以接收有关其工作项接近到期日期的通知，请选择此选项。</td>
        <td></td>
    </tr>
</table>

1. 通过选择工作项到期日期之前或之后的时间，选择自动提醒发送的时间。

   时间是根据任务或问题的计划完成日期计算的。

   指定将时间添加到任务或问题的计划完成日期的分钟、小时、天、周或月数。 选择 **已用分钟数**, **已用小时数**, **已用天数**&#x200B;或 **已用周数** 添加时间，其中包括您的计划中指明的任何周末、节假日和非工作时间。

   例如，如果在星期五分配了任务，并且该任务的持续时间为3天，则任务完成日期将设置为星期一（假定星期六和星期日是周末）。 如果任务的持续时间为3天（未经过），则任务完成日期将设置为星期三。

   ![](assets/time-increments-for-automatic-reminder.png)

1. 单击&#x200B;**保存**。

## 接收自动提醒

如果您是自动提醒通知中的指定实体，则在满足指定的截止时间时，您会收到一封电子邮件。 对于延迟通知，在任务或问题完成之前，会在夜间发送电子邮件。

具有某些依赖关系类型的任务可能会在指定的开始日期之后提交，即使它们已过期。 例如，如果某任务具有具有完成开始(fs)依赖关系的前置任务，则即使该任务已经过指定的开始日期，该任务也不会包含在电子邮件中，因为在前置任务完成之前，您无法启动该任务。

有关接收自动提醒电子邮件的更多信息，请参阅 [自动提醒](../../../workfront-basics/using-notifications/wf-notifications.md#automatic-reminders) 部分 [Adobe Workfront通知](../../../workfront-basics/using-notifications/wf-notifications.md).

## 发送自动提醒

在满足Workfront管理员选择的时间后，会立即发送自动提醒。

如果要手动触发发送自动提醒电子邮件的触发，则可以使用诊断程序执行此操作。 有关在Workfront中访问和使用诊断程序的详细信息，请参阅 [使用诊断触发自动化进程](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
