---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 删除自定义表单上的对象类型
description: 在现有的自定义表单上，您可以删除与该表单关联的对象类型。 执行此操作后，用户无法再将表单附加到该类型的对象。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: ca6565c4-3d9e-4a11-a7b6-fce701923bf2
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# 删除自定义表单上的对象类型

{{form-designer-default}}

在现有的自定义表单上，您可以删除与该表单关联的对象类型。 执行此操作后，用户无法再将表单附加到该类型的对象。

## 访问要求

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

## 删除自定义表单上的对象类型

您可以从现有自定义表单中删除对象类型。

自定义表单必须至少具有一个对象类型。

>[!CAUTION]
>
>如果人们已经将自定义表单附加到要删除的类型的对象并向其添加数据，则当您删除表单上的该对象类型时，将会永久删除该数据。 它可能包含用户以后需要的历史信息。
>
>通常，我们建议最大限度地减少编辑已使用的自定义表单的次数。 没有通知系统来提醒使用自定义表单的人员您的更改。

{{step-1-to-setup}}

1. 单击左侧面板中的&#x200B;**自定义Forms**。
1. 选择要编辑的自定义表单，然后单击![编辑图标](assets/edit-icon.png)。
1. 单击要从表单中删除的任何&#x200B;**对象类型**&#x200B;上的X，然后在显示的警告消息上单击&#x200B;**删除**。

   ![](assets/click-x-object-types.jpg)

1. （可选）对要从表单中删除的任何其他对象类型重复上一步骤。
1. 单击&#x200B;**完成**，然后单击&#x200B;**保存并关闭**。
