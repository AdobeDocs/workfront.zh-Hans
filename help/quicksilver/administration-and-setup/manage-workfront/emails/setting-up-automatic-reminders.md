---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: 设置自动提醒
description: 设置自动提醒
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 37ad04a1-d3c8-48b2-aed8-fe40456196ec
source-git-commit: 1c0a656f2603c5decabd2bb4e88da1b9530f9e1c
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 4%

---

# 设置自动提醒

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

作为Adobe Workfront管理员，您可以设置自动提醒，以在所有任务或问题到期、延迟或接近计划完成日期时触发电子邮件通知。 配置这些设置后，用户将无法禁用自动提醒。

对于延迟通知，在任务或问题完成之前，每夜发送电子邮件。

自动提醒可以发送到以下一项或多项：

* 分配给任务或问题的用户
* 用户的直属经理
* 直属经理的经理

>[!NOTE]
>
>您无法更改自动提醒触发的电子邮件的内容或主题行。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任何</td> 
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

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **电子邮件** >**自动提醒**.

1. 在 **发送延迟通知到** 区域，选择以下任一选项：

   <table>
    <tr>
        <td>“分配给”用户</td>
        <td>如果希望分配给任务或问题的用户收到关于其工作项延迟的延迟通知，请选择此选项。</td>
        <td></td>
    </tr>
    <tr>
        <td>用户的管理员</td>
        <td>如果希望用户的经理收到有关其直接下属的工作项延迟的延迟通知，请选择此选项。</td>
        <td></td>
    </tr>
    <tr>
        <td>经理的管理员</td>
        <td>如果希望直属经理的经理收到有关其直属下属用户的工作项延迟的通知，请选择此选项。</td>
        <td></td>
    </tr>
    <tr>
        <td>“分配给”用户</td>
        <td>(在 <b>发送截止日期提醒至</b> 区域。) 如果您希望分配给任务或问题的用户收到关于其工作项临近到期日期的通知，请选择此选项。</td>
        <td></td>
    </tr>
</table>

1. 通过选择工作项的到期日之前或之后的时间量，选择要发送自动提醒的时间。

   从任务或问题的规划完成日期开始计算时间。

   指定用于向任务或问题的计划完成日期添加时间的分钟数、小时数、天数、周数或月数。 选择 **经过的分钟数**， **经过小时数**， **经过的天数**，或 **经过的周数** 添加时间，包括计划中所指示的任何周末、节假日和非工作时间。

   例如，如果任务在星期五分配，其持续时间为经过的3天，则任务完成日期将设置为星期一（假设星期六和星期日为周末）。 如果任务的持续时间为3天（未经过），则任务完成日期将设置为星期三。

   ![](assets/time-increments-for-automatic-reminder.png)

1. 单击&#x200B;**保存**。

## 接收自动提醒

如果您是自动提醒通知中的指定实体，则会在满足指定截止日期时收到一封电子邮件。 对于延迟通知，在任务或问题完成之前，每夜发送电子邮件。

具有特定依赖关系类型的任务可能会在指定的开始日期之后交付，即使它们已过期。 例如，如果某个任务的前置任务具有完成 — 开始(fs)依赖关系，则即使该任务已超过指定的开始日期，它也不会包含在电子邮件中，因为在该前置任务完成之前，您无法启动该任务。

有关接收自动提醒电子邮件的详细信息，请参阅 [自动提醒](../../../workfront-basics/using-notifications/wf-notifications.md#automatic-reminders) 中的部分 [Adobe Workfront通知](../../../workfront-basics/using-notifications/wf-notifications.md).

## 发送自动提醒

在满足Workfront管理员选择的时间后，将立即发送自动提醒。

如果要触发手动发送自动提醒电子邮件，可以使用诊断程序执行此操作。 有关在Workfront中访问和使用诊断的详细信息，请参阅 [使用诊断触发自动化流程](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
