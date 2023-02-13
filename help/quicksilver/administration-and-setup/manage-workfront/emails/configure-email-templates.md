---
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: emails-administration
title: 配置电子邮件模板
description: 作为Adobe Workfront管理员，您可以配置电子邮件模板以支持提醒通知。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2ebc3be5-2734-4012-9277-86176c070137
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 1%

---

# 配置电子邮件模板

作为Adobe Workfront管理员，您可以配置电子邮件模板以支持提醒通知。

电子邮件模板包含在发起提醒通知时发送给用户的消息。\
如果没有电子邮件模板，则提醒通知将作为电子邮件正文中的空内容进行传递。

电子邮件模板可与问题、任务、项目和时间表的提醒通知关联。 创建电子邮件模板时，Workfront管理员可以提供电子邮件和主题行的内容。

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

## 创建新电子邮件模板 {#create-a-new-email-template}

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧的面板中，单击 **电子邮件** > **通知**.

1. 单击 **电子邮件模板** ，然后单击 **新电子邮件模板**.

1. 在 **新电子邮件模板** 框中，指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">电子邮件模板</td> 
      <td>电子邮件模板的标题（必需）。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">描述</td> 
      <td>模板的描述。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">对象类型</td> 
      <td>指定要将模板与关联的对象类型（必需，默认情况下将其设置为“问题”）。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">主题 </td> 
      <td>发送电子邮件时显示的主题（必需）。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> <p>发送电子邮件时显示的内容。</p> <p>您可以对电子邮件内容使用HTML格式，如 <a href="#add-html-formatting-to-an-email-template" class="MCXref xref">向电子邮件模板添加HTML格式</a> 在本文中。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存**。

## 向电子邮件模板添加HTML格式 {#add-html-formatting-to-an-email-template}

您可以向电子邮件模板添加HTML标记以生成自定义通知。\
按照 [创建新电子邮件模板](#create-a-new-email-template).

HTML格式可扩充您的电子邮件模板，如以下部分所示。

* [链接到Workfront对象](#link-to-workfront-objects)
* [链接到包含HTML的自定义字段](#link-to-custom-fields-with-html)
* [HTML电子邮件示例](#html-email-examples)

### 链接到Workfront对象 {#link-to-workfront-objects}

您可以使用 `$$` 通配符，指示电子邮件生成器从与特定对象关联的数据库中查找值。

例如，通知的电子邮件正文可遵循以下结构：

```html
<html>
<p>$$assignedTo:firstName$$</p>
<p>You are assigned to work on <b><a href="https://<your domain>.my.workfront.com/task/view?ID=$$ID$$">$$name$$</a></b>, which is due to start on $$plannedStartDate$$.</p>
<table width="350" style="font-size:12px;">
<tr>
<td><b><strong>HEADING</b></td>
<td>$$WILDCARD$$</td>
</tr>
<tr>
<td><b>HEADING</b></td>
<td>$$WILDCARD$$</td>
</tr>
<tr>
<td><b>HEADING</b></td>
<td>$$WILDCARD$$</td></tr>
</table>
</html>
```

要为对象获取“通配符”值，请执行以下操作之一：

<!-- Refer to the API Explorer and select the names of your objects from the Fields tab of any object. For more information about the API Explorer, see [Adobe Workfront API](../../../wf-api/workfront-api.md).-->

* 使用在报表的文本模式视图中找到的“valuefield”值。 有关文本模式值的更多信息，请参阅 [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

   “标题”值可以是对象的名称，您希望它显示在电子邮件正文中。

### 链接到包含HTML的自定义字段 {#link-to-custom-fields-with-html}

您可以使用 **$** 通配符，以告知电子邮件生成器从与对象关联的数据库中查找值。 它们必须位于数据库属性引用的任一侧。

例如，将以下文本添加为HTML会将分配的用户的名字添加到与任务关联的提醒通知中：

`assignedTo:firstName`

要使用相同的格式添加自定义字段，您可以在电子邮件通知中添加以下内容：

`DE:Custom Field As It Appears in Workfront`

例如，这是一个电子邮件模板，其中包含对名为“提交日期”的自定义字段的引用，并且假定“提交日期”字段属于任务。

替换 `<your domain>` (在您公司的Workfront域中，不带括号：

```html
<html>
<p>$$assignedTo:firstName$$</p>
<p>You are assigned to work on <b><a href="https://<your domain>.my.workfront.com/task/view?ID=$$ID$$">$$name$$</a></b>, which has a Delivery Date of $$DE:Task:Delivery Date$$.</p>
<table width="350" style="font-size:12px;">
<tr>
<td><b>Project Name:</b></td>
<td>$$project:name$$</td>
</tr>
<tr>
<td><b>Description:</b></td>
<td>$$description$$</td>
<tr>
<td><b>Estimated Effort:</b></td>
<td>$$work$$ hours</td>
</tr>
<tr>
<td><b>Planned Completion Date:</b></td>
<td>$$plannedCompletionDate$$</td>
<td><b>Delivery Date:</b></td>
<td>$$DE:Task:Delivery Date$$</td>
</tr>
</table>
</html>
```

>[!NOTE]
>
>如果字段属于某个项目，请将任务替换为项目：
>
>`DE:Project:Delivery Date`

### HTML电子邮件示例 {#html-email-examples}

* [延迟项目提醒通知（示例）](#late-project-reminder-notification-example)
* [关于开始提醒的任务或问题（示例）](#task-or-issue-about-to-start-reminder-example)

#### 延迟项目提醒通知（示例） {#late-project-reminder-notification-example}

要编辑延迟项目提醒的电子邮件模板，请在“主题”和“内容”字段中考虑此信息。

替换 `<your domain>` 的Workfront域，不带括号。

**主题:**

您管理的项目已过时

**内容:**

```html
<html>
<p>The <b><a href="https://<your domain>.my.workfront.com/project/view?ID=$$ID$$">$$name$$</a></b> project you are assigned as the owner of just became late.</p>
<table width="350" style="font-size:12px;">
<tr>
<td><b>Project Name:</b></td>
<td>$$project:name$$</td>
</tr>
</tr>
<tr>
<td><b>Planned Completion Date:</b></td>
<td>$$plannedCompletionDate$$</td>
</tr>
</table>
<p>Please review the task plan and bring it up to date to reflect the progress made so far. If it is necessary to update the plan to bring it reflect reality going forward, be sure to speak to $$sponsor:name$$ for approval before make these changes to the work breakdown structure.</p>
</html>
```

此时会生成一封与以下内容类似的电子邮件：

![](assets/screen-shot-2016-09-16-at-3.52.54-pm-350x103.png)

#### 关于开始提醒的任务或问题 {#task-or-issue-about-to-start-reminder-example}

您可能还希望为即将执行的任务或问题创建提醒通知。

以下代码可包含在电子邮件模板中，用于在任务或问题的计划开始日期之前的任意天数发送任务和问题提醒通知。

替换 `<your domain>` 的Workfront域，不带括号。

要将此内容用于问题电子邮件，请更改 `/task/view.` 值 `/issue/view`.

**主题:**

`$$name$$ to start on $$plannedStartDate$$`

**内容:**

```html
<html>
<p>$$assignedTo:firstName$$</p>
<p>You are assigned to work on <b><ahref=https://<your domain>.my.workfront.com/task/view?ID=$$ID$$">$$name$$</a></b>, which is due to start on $$plannedStartDate$$.</p>
<tablewidth=350"style=font-size:12px;">
<tr>
<td><b>Task Name:</b></td>
<td>$$name$$</td>
</tr>
<td><b>Project Name:</b></td>
<td>$$project:name$$</td>
</tr>
</tr>
<td><b>Created on:</b></td>
<td>$$entryDate$$</td>
</tr>
<tr>
<td><b>Project Manager:</b></td>
<td>$$project:owner:name$$</td>
<tr>
<td><b>Priority:</b></td>
<td>$$priority$$</td>
</tr>
<tr>
<td><b>Who is assigned to:</b></td>
<td>$$assignedTo:name$$</td>
</tr>
<tr>
<td><b>When it's due:</b></td>
<td>$$estCompletionDate$$</td>
</tr>
</table>
</html>
```

![email_template_delivered.png](assets/email-template-delivered.png)

创建电子邮件模板后，用户可以将其与提醒通知关联，如 [设置提醒通知](../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).
