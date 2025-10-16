---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: 使用特定状态列出具有未决批准流程的对象
description: 如果您尝试删除状态，则可能会出现一条错误消息，告诉您无法删除该状态，因为该状态正用于系统中对象的未决批准流程。 如果要查找并查看这些对象以决定需要执行的操作，可以运行列出这些对象的报表。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 52dd8750-9a6f-4ac6-9779-ba4ea9b6f4e0
source-git-commit: 366043a786c94f1bc40ad3b20af175bb84c94742
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---

# 使用特定状态列出具有未决批准流程的对象

如果您尝试删除状态，则可能会显示一条错误消息，告诉您无法删除该状态，因为它在您的系统中至少处于一个待审批流程中。 您可以运行报告以列出处于待审批流程中的对象，然后决定您需要为每个对象做什么。

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
   <td>
     <p>标准</p>
     <p>规划</p>
   </td> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td><p>编辑对报告、功能板和日历的访问权限</p><p>编辑对筛选器、视图、分组的访问权限</p></td>
  </tr>
  <tr> 
   <td>对象权限</td> 
   <td>您获取对所创建报告的管理权限。</td>
  </tr>
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在标准模式下

{{step1-to-reports}}

1. 单击&#x200B;**新建报告**，然后选择&#x200B;**项目报告**、**任务报告**&#x200B;或&#x200B;**问题报告**。
1. 打开&#x200B;**筛选器**&#x200B;选项卡。
1. 单击&#x200B;**添加筛选器规则**，然后执行以下操作以设置规则：
   1. 开始键入`status`，然后在显示时选择&#x200B;**状态**。
   1. 在第二个字段中保留&#x200B;**等于**。
   1. 在第三个字段中选择状态的名称。
1. 再次单击&#x200B;**添加筛选器规则**，然后执行以下操作以设置规则
   1. 开始键入`pending status`，然后在该项目显示在您要查看的对象类型下时选择该项目（**项目**、**任务**&#x200B;或&#x200B;**问题**）。
   1. 在第二个字段中保留&#x200B;**等于**。
   1. 在第三个字段中键入`in`。
1. 再次单击&#x200B;**添加筛选器规则**，然后执行以下操作以设置规则
   1. 开始键入审批流程，然后选择&#x200B;**组ID**（当它显示在&#x200B;**审批流程**&#x200B;下时）。
   1. 在第二个字段中选择&#x200B;**Is Blank**。
1. 单击&#x200B;**保存+关闭**&#x200B;以运行报告，并根据您指定的状态（**项目**、**任务**&#x200B;或&#x200B;**问题**）列出处于挂起状态的批准流程中指定的类型的所有对象。
1. 重复这些步骤查找其它两种对象类型的相同信息。


## 在文本模式下

{{step1-to-reports}}

1. 单击&#x200B;**新建报告**，然后选择&#x200B;**项目报告**、**任务报告**&#x200B;或&#x200B;**问题报告**。
1. 打开&#x200B;**筛选器**&#x200B;选项卡。
1. 选择&#x200B;**切换到文本模式**。
1. 将以下内容复制并粘贴到编辑窗口中，将XXX替换为状态的3个字母的键：

   `status=XXX`

   `status_Mod=in`

   `approvalProcess:groupID_Mod=isblank`

   您可以查看状态列表中的键，如以下文章中所示：
   * [访问系统项目状态的列表](project-statuses.md)
   * [访问系统任务状态的列表](task-statuses.md)
   * [访问系统问题状态的列表](issue-statuses.md)

1. 单击&#x200B;**保存+关闭**&#x200B;以运行报告，并根据您指定的状态（**项目**、**任务**&#x200B;或&#x200B;**问题**）列出处于挂起状态的批准流程中指定的类型的所有对象。
1. 重复这些步骤查找其它两种对象类型的相同信息。
