---
title: 使用表单设计器从现有自定义表单添加或删除对象类型
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以使用表单设计器从自定义表单中添加或删除对象类型。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c43ea6b2-7d5b-46f0-a092-f57128de60f0
source-git-commit: ccb2b6bb9fa63d29523ff396490f9580ad130bdd
workflow-type: tm+mt
source-wordcount: '539'
ht-degree: 0%

---

# 使用表单设计器从现有自定义表单添加或删除对象类型

<span class="preview">此页面上高亮显示的信息是指尚未普遍可用的功能。 它只能在“预览”环境中用于所有客户，或者在“生产”环境中用于启用快速版本的客户。</span>

<span class="preview">有关快速版本的信息，请参阅 [为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">有关当前版本的信息，请参阅 [2024年第二季度发行版概述](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

您可以使用表单设计器从现有自定义表单中添加或删除对象类型。

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
   <td role="rowheader">访问级别配置*</td> 
   <td><p>对自定义表单的管理访问权限</p></td> 
  </tr>  
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 将对象类型添加到现有自定义表单

您可以向表单添加其他对象类型，以便将其附加到多个对象。

>[!NOTE]
>
>分区界限权限可能受对象类型影响。 自定义表单分区界限的“有限编辑”权限仅适用于“项目”、“任务”、“问题”和“用户”对象类型。
>
>有关更多信息，请参阅 [多个对象类型如何影响分区界限权限](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md#how-multiple-object-types-can-affect-section-break-permissions).


{{step-1-to-setup}}

1. 单击 **自定义Forms** 在左侧面板中。

   在显示的视图中，您可以查看为组织创建的所有自定义表单。 您还可以查看每个表单的创建者、表单使用的对象类型以及表单是否处于活动状态。

1. 选择要向其添加其他对象类型的自定义表单，然后单击 **编辑** <span class="preview">或 ![“编辑”图标](assets/edit-icon.png).</span>

1. 单击表单顶部的加号+之后 **对象类型**，然后在显示的菜单中选择所需的类型。 您可以重复此操作，以添加所需数量的对象类型。

   ![](assets/add-new-object.png)

1. 单击 **保存并关闭**.

   >[!TIP]
   >
   >您可以单击 **应用** 在创建自定义表单时，可随时保存更改并保持表单打开。

## 删除自定义表单上的对象类型

您可以从现有自定义表单中删除对象类型。 自定义表单必须至少具有一个对象类型。

>[!CAUTION]
>
>如果人们已经将自定义表单附加到要删除的类型的对象并向其添加数据，则当您删除表单上的该对象类型时，将会永久删除该数据。 它可能包含用户以后需要的历史信息。
>
>通常，我们建议最大限度地减少编辑已使用的自定义表单的次数。 没有通知系统来提醒使用自定义表单的人员您的更改。

要删除对象类型，请执行以下操作：

{{step-1-to-setup}}

1. 单击 **自定义Forms** 在左侧面板中。
1. 选择要编辑的自定义表单，然后单击 **编辑** <span class="preview">或 ![“编辑”图标](assets/edit-icon.png).</span>
1. 单击任意 **对象类型** 要从表单中删除的重复项。

   ![](assets/delete-object-types.png)

1. （可选）对要从表单中删除的任何其他对象类型重复上一步骤。
1. 单击 **完成**，然后单击 **保存并关闭**.
