---
title: 转换对象时传输自定义表单数据
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 当在工作项中定义的工作变得过大时，您可以将其转换为较大的工作项。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2d4d104a-1465-43e2-8184-83dd63d9681c
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# 转换对象时传输自定义表单数据

根据组织的业务需求，在任务或问题中定义的工作可能变得太大，无法在任务或问题中管理。 在这种情况下，您可以将它们转换为较大的工作项：

* 您可以将问题转化为任务或项目
* 您可以将任务转换为项目

要将自定义表单数据从问题传输到任务或项目，您必须按照以下顺序完成本文中的两个任务。

有关详细信息，请参阅[在Adobe Workfront中转化问题的概述](../../../manage-work/issues/convert-issues/convert-issues.md)或[在Adobe Workfront中转化问题的概述](../../../manage-work/issues/convert-issues/convert-issues.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront计划</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>
   <p>新增：标准</p>
   <p>或</p>
   <p>当前：计划</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>对自定义表单的管理访问权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 第一：向自定义表单添加其他对象

{{step-1-to-setup}}

1. 单击&#x200B;**自定义Forms**。
1. 查找所需的表单，然后单击![编辑图标](assets/edit-icon.png)。
1. 在表单顶部，添加您计划要将任务或问题转换到的对象。

   >[!INFO]
   >
   >**示例**：如果要将自定义表单数据传输到项目，请选择“项目”。

1. 单击表单底部的&#x200B;**应用**。

1. 继续到[秒：转换问题或任务并传输自定义表单数据](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data)。

## 第二：转换问题或任务并传输自定义表单数据 {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. 将其他对象添加到要转换的问题或任务的自定义表单中，如本文中[第一：将其他对象添加到自定义表单](#first-add-additonal-objects-to-the-custom-form)部分所述。
1. 使用显示的框中的&#x200B;**自定义Forms**&#x200B;选项转换问题或任务，以选择所需的自定义表单。 有关说明，请参阅以下文章：

   * [在Adobe Workfront中将问题转化为项目](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [在Adobe Workfront中将问题转化为任务](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
   * [将任务转换为项目](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md)

1. 在显示的&#x200B;**转换为（对象类型）**&#x200B;对话框中，单击&#x200B;**添加Forms**&#x200B;下拉菜单，然后选择您在上一节中复制的表单。

   现在，在问题的自定义字段中捕获的信息已转移到任务上的自定义表单中。


<!--
## First: Copy the custom form {#first-copy-the-custom-form}

First you need to make sure that you retain any custom form data on a task or issue you want to convert. Because the custom form data must be an exact match on the converted item, it is best practice to duplicate the form so that you can attach it to the new object.

>[!TIP]
>
>Another way to retain custom form data in this situation is to add the larger object type to the custom form. For instructions, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).

1. Click **Custom Forms**.
1. Select the task- or issue-type custom form, then click **Copy**.
1. In the **Custom Form** dialog box, specify a name for the new form.  

1. From the **Form Type** drop-down menu, select the type of object you want to create the new custom form for

   **Example:** If you want to transfer the custom form data to a project, select Project.

1. Click **Copy Form**.

   This copied custom form can now be attached to a task or project.

1. Continue on to [Second: Convert the issue or task and transfer the custom form data](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).
-->