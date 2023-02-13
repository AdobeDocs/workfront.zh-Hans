---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: “计算的自定义字段示例：在“自定义表单”中显示状态时间戳
description: 以下计算字段显示对象状态标记为“进行中(INP)”的日期。 对于问题、任务或项目，您可以对计算的自定义字段使用相同的信息。
author: Nolan
feature: Reports and Dashboards
exl-id: 55817a68-3655-4288-8cc7-48547829c46e
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# 计算的自定义字段示例：在自定义表单中显示状态时间戳

以下计算字段显示对象状态标记为“进行中(INP)”的日期。 对于问题、任务或项目，您可以对计算的自定义字段使用相同的信息。

>[!NOTE]
>
>如果对象的状态更改为INP，然后该对象更改为其他状态，然后返回到INP，则Adobe Workfront仅捕获对INP进行首次更改的时间戳。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <caption style="text-align: left;"> 
  <p>*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。</p> 
 </caption> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront计划*</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront许可证*</p> </td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td><strong>访问级别配置*</strong> </td> 
   <td> <p>编辑对创建报表、功能板和日历的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>对象权限</strong> </p> </td> 
   <td> <p>管理附加了表单的对象的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.<br>有关功能板权限的更多信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md" class="MCXref xref">共享报表、功能板和日历 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 先决条件

要向自定义表单添加显示字段编辑历史记录的计算字段，您必须先创建自定义表单。

## 在自定义表单中显示状态时间戳

1. 转到要添加字段的自定义表单。
1. 单击 **已计算** 向表单中添加计算的自定义字段。
1. 键入 **标签** (例如 *状态时间戳自定义字段*.
1. 单击 **完成**，然后单击 **保存并关闭**.
1. 重新打开自定义表单，然后选择新的 **状态时间戳自定义字段** 在窗体上。
1. 在 **计算** 框中，复制并粘贴自定义字段的以下计算：

   ```
   IF({status}='INP',IF(ISBLANK({DE:Status Timestamp Custom Field}),$$NOW,{DE:Status Timestamp Custom Field}),{DE:Status Timestamp Custom Field})  
   ```

   >[!NOTE]
   >
   >对于所有对象和所有状态，此计算是相同的。 在此计算中，必须始终使用三字母键，而不是对象状态的状态名称。
   >
   >有关状态键的更多信息，请参阅 [创建或编辑状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. 单击 **保存并关闭**.

   您现在可以报告状态时间戳自定义字段，或将其用于其他计算、报表或自定义字段。
