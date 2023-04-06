---
user-type: administrator
product-area: system-administration
navigation-topic: run-diagnostics
title: 使用诊断触发自动化进程
description: 您可以使用诊断手动触发自动化流程，例如基于时间的脚本、重新计算或电子邮件通知。
feature: System Setup and Administration
role: Admin
exl-id: 9243ee60-006b-4628-bde7-5b037dde7511
source-git-commit: 5469598d57fec1a744ddb44cf2accb94e1f70941
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 6%

---

# 使用诊断触发自动化进程

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

您可以使用诊断手动触发自动化流程，例如基于时间的脚本、重新计算或电子邮件通知。

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront计划</a> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">旧版许可证概述</a> </td> 
   <td> <p>计划 </p>您必须是Workfront管理员。 有关Workfront管理员的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</td> 
  </tr> 
 </tbody> 
</table>

## 使用诊断触发自动化进程

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 展开 **系统**，然后单击 **诊断**.
1. 从以下任意选项中进行选择：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">发送超期通知</td> 
      <td> <p>手动发送逾期任务和问题的自动提醒通知。 </p> <p>有关设置自动提醒的更多信息，请参阅 <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">设置自动提醒</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">发送早期通知</td> 
      <td> <p>手动发送接近其到期日期的任务和问题的自动提醒通知。</p> <p>有关设置自动提醒的更多信息，请参阅 <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">设置自动提醒</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">发送提醒通知</td> 
      <td> <p>手动发送提醒通知。 </p> <p>有关设置提醒通知的更多信息，请参阅 <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">设置提醒通知</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">检查所有 POP 帐户</td> 
      <td> <p>检查是否有新电子邮件已发送到链接到Workfront的POP帐户。 </p> <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about Workfront and POP account integrations, see and <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.</p>
       --> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">重新计算时间线</td> 
      <td> <p>重新计算处于“当前”状态的Workfront中所有项目的时间表。 </p> <p>有关自动或手动计算项目时间轴的更多信息，请参阅 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">重新计算项目时间表</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">恢复默认客户报告</td> 
      <td>恢复最初随Workfront一起提交的默认报表，以便在 <strong>报表</strong> 部分。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">生成工时表</td> 
      <td>根据用户的定期工时单配置文件为用户生成工时单。 仅当时间表配置文件在分配给用户后发生重大更改，并且任何当前和未来时间表都被删除之后，才需要运行此选项。</td> 
     </tr> 
    </tbody> 
   </table>
