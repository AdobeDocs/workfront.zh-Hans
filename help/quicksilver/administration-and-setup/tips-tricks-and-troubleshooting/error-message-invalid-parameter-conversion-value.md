---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: “错误消息：参数无效：转化值'
description: “您在尝试更改现有自定义表单上自定义字段的格式时收到以下错误消息：'无效参数：转换值'&lt;...&gt;""
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7aac95-4afb-422d-877b-0fa49ef43883
source-git-commit: 5469598d57fec1a744ddb44cf2accb94e1f70941
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 1%

---

# 错误消息：参数无效：转化值

## 问题

尝试更改现有自定义表单上自定义字段的格式时，您会收到以下错误消息：&quot;无效参数：转换值&quot;&lt;...>&quot;&quot;\
![custom_field_format_invalid_parameter_error_png](assets/custom-field-format-invalid-parameter-error-350x148.png)

## 原因

此消息在以下情景中发生：

例如，您有一个自定义字段，其格式为“文本”。  现在，您要将自定义字段的格式更改为货币。 在您的Adobe Workfront实例中的某个位置，此字段已附加到对象，并且其中已指定信息。 至少一个此类字段中的现有信息已格式化为文本。 因此，不能将字段的格式更改为货币。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><a href="https://www.workfront.com/plans" target="_blank">Workfront计划</a>*</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">旧版许可证概述</a>*</p> </td> 
   <td>计划</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>访问级别*</strong> </td> 
   <td> <p>编辑对以下项的访问权限：</p> 
    <ul> 
     <li> <p>创建报表、功能板和日历</p> </li> 
     <li> <p>创建过滤器、视图和分组</p> </li> 
    </ul> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 解决方案

执行以下操作：

1. 为可能具有与其自定义Forms关联的此字段的所有对象生成报表。\
   有关生成报表的信息，请参阅 [创建自定义报表](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 包括您尝试在报表视图中编辑的自定义字段，以便您能够查看哪个对象已使用文本值填充此字段。
1. 更正以文本格式显示的对象的“自定义字段”值，并为其指定一个格式为“货币”的值；然后，尝试再次更改自定义表单上的“格式”字段。\
   或\
   如果已使用文本格式信息填充了太多字段值，请考虑向自定义表单中添加新的自定义字段，并将其格式化为货币。
