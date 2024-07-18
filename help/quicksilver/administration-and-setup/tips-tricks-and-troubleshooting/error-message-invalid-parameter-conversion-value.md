---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '错误消息：无效参数：转化值'
description: “尝试更改现有自定义表单上的自定义字段格式时，收到以下错误消息：‘无效参数：转化值'&amp； lt；..&amp；gt；"
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7aac95-4afb-422d-877b-0fa49ef43883
source-git-commit: 62d1b9563d83bd82b569e143f69e379e2f4ffbc2
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# 错误消息：无效参数：转换值

## 问题

尝试更改现有自定义表单上的自定义字段格式时，您收到以下错误消息：“无效参数：转化值&quot;&lt;...>&quot;\
![custom_field_format_invalid_parameter_error.png](assets/custom-field-format-invalid-parameter-error-350x148.png)

## 原因

此消息出现在以下场景中：

例如，您有一个“自定义字段”，格式为“文本”。  现在，您需要将自定义字段的格式更改为货币。 在Adobe Workfront实例中的某个位置，此字段已附加到对象，并且其中包含已指定的信息。 至少一个此类字段中的现有信息已设置为文本格式。 因此，无法将字段的格式更改为货币。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><a href="https://www.workfront.com/plans" target="_blank">Workfront计划</a>*</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">许可证概述</a>*</p> </td> 
   <td>计划</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>访问级别*</strong> </td> 
   <td> <p>编辑以下项的访问权限：</p> 
    <ul> 
     <li> <p>创建报告、功能板和日历</p> </li> 
     <li> <p>创建筛选器、视图和分组</p> </li> 
    </ul> <p><b>注意</b>：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 解决方案

执行以下操作：

1. 为可能将此字段与其自定义Forms关联的所有对象生成报告。\
   有关生成报告的信息，请参阅[创建自定义报告](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

1. 将您尝试编辑的自定义字段包含在报表视图中，以便您能够查看哪个对象为该字段填充了文本值。
1. 更正以文本格式显示的对象的“自定义字段”值，并为它们赋予“货币”格式的值；然后再次尝试更改“自定义表单”上的“格式”字段。\
   或\
   如果您有太多字段值已填充了文本格式信息，请考虑将新的自定义字段添加到自定义表单并将其格式化为货币。
