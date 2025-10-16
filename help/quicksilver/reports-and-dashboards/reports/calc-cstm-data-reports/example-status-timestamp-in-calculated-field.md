---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 计算自定义字段示例：在自定义表单中显示状态时间戳
description: 以下计算字段显示对象状态标记为进行中(INP)的日期。 您可以为问题、任务或项目的计算自定义字段使用相同的信息。
author: Jenny
feature: Reports and Dashboards
exl-id: 55817a68-3655-4288-8cc7-48547829c46e
source-git-commit: a1ead6d0c1c85bfbe6d7302506743db8d8b3e205
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# 计算自定义字段示例：在自定义表单中显示状态时间戳

以下计算字段显示对象状态标记为进行中(INP)的日期。 您可以为问题、任务或项目的计算自定义字段使用相同的信息。

>[!NOTE]
>
>如果对象的状态更改为INP，然后又更改为其他状态，然后再更改为INP，则Adobe Workfront将仅捕获首次更改为INP的时间戳。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront包</p> </td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront许可证</p> </td> 
   <td>
      <p>标准</p>
      <p>规划</p></td>
  </tr> 
  <tr> 
   <td><p>访问级别配置</p></td> 
   <td> <p>编辑创建报告、功能板和日历的权限</p> </td> 
  </tr> 
  <tr> 
   <td> <p>对象权限</p> </td> 
   <td> <p>管理附加表单的对象权限</p></td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

要将显示字段编辑历史记录的计算字段添加到自定义表单，您必须先创建自定义表单。

## 在自定义表单中显示状态时间戳

1. 转到要添加字段的自定义表单。
1. 单击&#x200B;**已计算**&#x200B;以将已计算的自定义字段添加到表单。
1. 为自定义字段键入&#x200B;**标签**。 例如，“状态时间戳自定义字段”。
1. 单击&#x200B;**保存+关闭**。
1. 重新打开该自定义表单，然后在表单上选择新的&#x200B;**状态时间戳自定义字段**。
1. 在&#x200B;**计算**&#x200B;框中，复制并粘贴自定义字段的以下计算：

   ```
   IF({status}='INP',IF(ISBLANK({DE:Status Timestamp Custom Field}),$$NOW,{DE:Status Timestamp Custom Field}),{DE:Status Timestamp Custom Field})  
   ```

   >[!NOTE]
   >
   >对于所有对象和所有状态，此计算都是相同的。 必须始终使用三个字母的键，而不是此计算中对象状态的状态名称。
   >
   >有关状态键的更多信息，请参阅[创建或编辑状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)。

1. 单击&#x200B;**保存+关闭**。

   您现在可以报告状态时间戳自定义字段，或将其用于其他计算、报表或自定义字段。
