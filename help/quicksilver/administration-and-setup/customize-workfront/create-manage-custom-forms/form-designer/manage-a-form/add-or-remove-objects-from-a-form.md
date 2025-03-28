---
title: 在现有自定义表单中添加或删除对象类型
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以使用表单设计器向自定义表单添加对象类型或从自定义表单中删除对象类型。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c43ea6b2-7d5b-46f0-a092-f57128de60f0
source-git-commit: 554e08c22f6ee142a9ced8fa991d0126b6360b0c
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 0%

---

# 在现有自定义表单中添加或删除对象类型

您可以使用表单设计器从现有自定义表单添加或删除对象类型。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

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
   <td role="rowheader">访问级别配置*</td> 
   <td><p>管理自定义表单的访问权限</p></td> 
  </tr>  
 </tbody> 
</table>

有关此表中的信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 将对象类型添加到现有自定义表单

您可以向表单添加其他对象类型，以便将其附加到多个对象。

>[!NOTE]
>
>分区界限权限可能受对象类型影响。 自定义表单分区界限的“有限编辑”权限仅适用于“项目”、“任务”、“问题”和“用户”对象类型。
>
>有关详细信息，请参阅[多个对象类型如何影响分区符权限](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md#how-multiple-object-types-can-affect-section-break-permissions)。


{{step-1-to-setup}}

1. 单击左侧面板中的&#x200B;**自定义Forms**。

   在显示的视图中，您可以查看为组织创建的所有自定义表单。 您还可以查看每个表单的创建者、表单使用的对象类型以及表单是否处于活动状态。

1. 选择要添加其他对象类型的自定义表单，然后单击![编辑图标](assets/edit-icon2.png)。

1. 在表单顶部，单击&#x200B;**“对象类型”**&#x200B;后面的加号+，然后在显示的菜单中选择所需的类型。 您可以重复此操作以添加任意数量的对象类型。

   ![添加新对象](assets/add-new-object.png)

1. 单击&#x200B;**保存并关闭**。

   >[!TIP]
   >
   >在创建自定义表单时，您可以随时单击&#x200B;**应用**&#x200B;以保存更改并保持表单打开。

## 删除自定义表单上的对象类型

您可以从现有自定义表单中删除对象类型。 自定义表单必须至少具有一个对象类型。

>[!CAUTION]
>
>如果人们已经将自定义表单附加到要删除的类型的对象并向其添加数据，则当您删除表单上的该对象类型时，将会永久删除该数据。 它可能包含用户以后需要的历史信息。
>
>通常，我们建议最大限度地减少编辑已使用的自定义表单的次数。 没有通知系统可提醒使用自定义表单的人员注意您的更改。

要删除对象类型，请执行以下操作：

{{step-1-to-setup}}

1. 单击左侧面板中的&#x200B;**自定义Forms**。
1. 选择要编辑的自定义表单，然后单击![编辑图标](assets/edit-icon2.png)。
1. 单击要从表单中删除的任何&#x200B;**对象类型**&#x200B;上的X。

   ![删除对象类型](assets/delete-object-types.png)

1. （可选）对要从表单中删除的任何其他对象类型重复上一步骤。
1. 单击&#x200B;**应用**，然后单击&#x200B;**保存并关闭**。
