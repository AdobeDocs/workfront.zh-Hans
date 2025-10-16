---
user-type: administrator
product-area: system-administration
navigation-topic: run-diagnostics
title: 使用诊断来触发自动化流程
description: 您可以使用诊断手动触发自动化流程，例如基于时间的脚本、重新计算或电子邮件通知。
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: 9243ee60-006b-4628-bde7-5b037dde7511
source-git-commit: 156341072c291b5c03432da399a509d9772b73ea
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 11%

---

# 使用诊断来触发自动化流程

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

您可以使用诊断手动触发自动化流程，例如基于时间的脚本、重新计算或电子邮件通知。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p>
       <p>规划</p></td>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>系统管理员</td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 使用诊断功能触发自动化流程

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![主菜单图标](assets/main-menu-icon.png)，然后单击&#x200B;**设置**![齿轮设置图标](assets/gear-icon-settings.png)。

1. 展开&#x200B;**系统**，然后单击&#x200B;**诊断**。
1. 从以下任一选项中选择：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">发送超期通知</td> 
      <td> <p>手动发送逾期任务和问题的自动提醒通知。 </p> <p>有关设置自动提醒的详细信息，请参阅<a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">设置自动提醒</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">发送早期通知</td> 
      <td> <p>手动发送临近到期日期的任务和问题的自动提醒通知。</p> <p>有关设置自动提醒的详细信息，请参阅<a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">设置自动提醒</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">发送提醒通知</td> 
      <td> <p>手动发送提醒通知。 </p> <p>有关设置提醒通知的详细信息，请参阅<a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">设置提醒通知</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">检查所有 POP 帐户</td> 
      <td>检查已发送到链接到Workfront的POP帐户的新电子邮件。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">重新计算时间线</td> 
      <td> <p>重新计算Workfront中所有处于当前状态的项目的时间表。 </p> <p>有关自动或手动计算项目时间表（一次一个项目）的详细信息，请参阅<a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">重新计算项目时间表</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">还原默认客户报告</td> 
      <td>恢复最初随Workfront一起提供的默认报告，以便所有用户在<strong>报告</strong>部分中都可以看到这些报告。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">生成时间表</td> 
      <td>根据用户的周期性时间表配置文件为用户生成时间表。 仅当时间表配置文件在分配给用户后发生了显着更改时，并且任何当前和未来时间表被删除后，才需要运行此选项。</td> 
     </tr> 
    </tbody> 
   </table>
