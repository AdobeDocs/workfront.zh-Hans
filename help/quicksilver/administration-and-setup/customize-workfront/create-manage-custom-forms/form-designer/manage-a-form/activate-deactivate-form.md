---
title: 停用或重新激活自定义表单
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以重新激活或取消激活自定义表单。 我们建议停用自定义表单，而不是删除您不再用于保留历史数据的表单。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 6d9a409d-8d16-4c58-ad02-f60aa1ac1714
source-git-commit: c1bc2832d1c52885e737056172e7aec93a951e6c
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# 停用或重新激活自定义表单

您可以重新激活或取消激活自定义表单。 我们建议停用自定义表单，而不是删除您不再用于保留历史数据的表单。

>[!NOTE]
>
>如果自定义表单被停用，但仍属于队列主题或请求队列定义，则会将其附加到新请求。 如果您不希望表单出现在请求中，则必须将其从请求队列中手动删除。

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
   <td> <p>对自定义表单的管理访问权限</p></td> 
  </tr>  
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 停用自定义表单

您可以停用不再使用的自定义表单，而不会丢失其关联的历史数据。 用户无法将非活动的自定义表单添加到对象，但仍可以查看数据并将其添加到已附加该表单的对象上的表单字段。

非活动自定义表单上的字段也仍可用于在视图中内联编辑。 如果用户在内联编辑期间从非活动自定义表单添加字段，即使自定义表单已停用，该表单也会自动附加到对象。

要停用自定义表单，请执行以下操作：

{{step-1-to-setup}}

1. 在左侧面板中，选择&#x200B;**自定义Forms**。
1. 在&#x200B;**Forms**&#x200B;区域，选择要取消激活的自定义表单。
1. 在“处于活动状态”列中，选择&#x200B;**False**&#x200B;并单击退出该列。 该表单不再处于活动状态。

## 重新激活自定义表单

如果重新激活自定义表单，则它会保留之前具有的设置，用户可以像从未停用它一样与它进行交互。

{{step-1-to-setup}}

1. 在左侧面板中，选择&#x200B;**自定义Forms**。
1. 在&#x200B;**Forms**&#x200B;区域，选择要重新激活的自定义表单。
1. 在“处于活动状态”列中，选择&#x200B;**True**&#x200B;并单击退出该列。 该表单现在处于活动状态。
