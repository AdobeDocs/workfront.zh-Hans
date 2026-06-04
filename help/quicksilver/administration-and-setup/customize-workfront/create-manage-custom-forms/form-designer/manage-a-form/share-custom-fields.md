---
title: 配置自定义字段和小部件的共享
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 默认情况下，向自定义表单添加新的自定义字段或构件时，系统中有权访问自定义表单的任何人都可以编辑该项目的属性，例如其标签和名称。 您可以通过控制可与谁共享来更改此设置。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 4f591fa3-2cb9-4a22-bfb1-1b50cedfcf3d
TQID: https://experienceleague.adobe.com/KyrIWEpIQQb-f8YODUPz3-RbP5wFww8Vu7Ffy33wUog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 744
ht-degree: 2%

---

# 配置自定义字段和小部件的共享

默认情况下，向自定义表单添加新的自定义字段或构件时，系统中有权访问自定义表单的任何人都可以编辑该项目的属性，例如其标签和名称。 您可以通过控制可与谁共享来更改此设置。

有关自定义表单中的自定义字段和小部件的信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 包</td> 
   <td><p>“任一”</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p>
       <p>规划</p></td>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td> <p>对自定义表单的管理访问权限</p> </td> 
  </tr>  
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--

## Configure sharing a custom field or widget from the list of forms

{{step-1-to-setup}}

1. In the left panel, click **Custom Forms**.
1. Click **Fields** to open the Fields area.
1. Select the item you want to configure sharing for, then click ![Share icon](assets/share-icon.png).
1. In the Custom Field Access box that displays, specify who you want to share the item with and how you want to share it:

   1. Near the lower-left corner of the **Custom Field Access** box, under **Give custom field access to**, start typing the name of a user, team, job role, group, or company you want to share the item with, then click the name when it appears.

      ![Custom Field Access box](assets/share-field-give-access-to.jpg)

   1. If you want to be more specific about how you want to share the item, click the drop-down list to the right of the name, then use any of the following options:

      ![Sharing options](assets/share-field-view-mng-options.jpg)

      <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
        <tr> 
         <td role="rowheader">View it</td> 
         <td> <p>You can click <strong>Advanced Settings</strong> to specify whether you want the user or users to be able to use their access to add the item to a custom form or share it with other users.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader">Manage it</td> 
         <td> <p>Allows access to edit the custom field and to see it in the Field Library and on the page where you build custom forms.</p> <p>You can click <strong>Advanced Settings</strong> to specify whether you want the user or users to be able to use their access to delete the item from the system or share it with other users.</p> </td> 
        </tr> 
       </tbody> 
      </table>   

1. (Optional) Repeat the previous step to add other names to the list and configure their options.
1. (Optional) Click the gear icon ![Settings icon](assets/gear-icon-settings.png) in the top-right corner if you want to choose a system-wide sharing option for the field.

   Not all of the following options display in this drop-down menu at the same time. For example, the second one displays only when one of the other two are selected.

   * **Make this editable system-wide so that everyone in Workfront can edit it** (the default option)

     When you add a custom field or widget and you don't limit sharing for it, everyone in the system who has access to custom forms can view it and edit its properties.
   
   * **Remove system-wide edit access**

     Limits access to only those whom you added to the list. 
   
   * **Make this visible system-wide so that everyone in Workfront can see it**

1. Click **Save**.

-->

## 配置共享自定义字段或构件

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**自定义Forms**。
1. 要从表单和字段列表中共享，请执行以下操作：

   1. 单击&#x200B;**字段**&#x200B;以打开“字段”区域。
   1. 选择要共享的字段，然后单击![共享图标](assets/share-icon.png)。

1. 要从表单设计器共享，请执行以下操作：
   1. 打开自定义表单或创建新的自定义表单。
   1. 在表单设计器中，选择要共享的字段，然后单击右侧字段编辑区域中的&#x200B;**共享**。

1. 在共享框中，在&#x200B;**向**&#x200B;授予字段访问权限下，开始键入要与其共享项目的用户、团队、工作角色、组、公司或业务配置文件的名称，然后在名称显示时按&#x200B;**Enter**。
1. 如果您想更详细地了解如何共享项目，请单击名称右侧的下拉菜单，然后使用以下任一选项：

   * **查看**：单击&#x200B;**高级设置**&#x200B;图标![高级设置图标](assets/configure-options-icon.png)以指定您希望用户能够将该项目添加到自定义表单还是与其他用户共享。
   * **管理**：允许访问编辑自定义字段并在字段库和表单设计器中查看它。 单击&#x200B;**高级设置**&#x200B;图标![高级设置图标](assets/configure-options-icon.png)以指定您希望用户能够从系统中删除项目还是与其他用户共享该项目。

1. （可选）重复步骤5-6以向列表中添加其他名称并配置其选项。
1. （可选）为字段选择系统范围的共享选项：

   * **系统中的每个人都可以编辑**（默认选项）

     当您添加自定义字段或构件并且不限制其共享时，系统中有权访问自定义表单的每个人都可以查看并编辑其属性。

   * **系统中的每个人都可以查看**

     系统中有权访问自定义表单的每个人均可查看该字段，但不能对其进行编辑。

   * **只有受邀人员才能访问**

     限制仅访问您添加到列表中的用户。

   ![共享选项](assets/share-field-in-designer.png)

1. 单击&#x200B;**保存**。

## 共享自定义表单时继承对自定义字段和小部件的访问权限

当有人与组、工作角色、团队、公司或业务配置文件共享自定义表单时，收件人将继承对表单上任何自定义字段和小部件的查看访问权限。 对表单上这些项目的这种访问级别始终会保留，以便表单能够按创建者的预期用于收件人。 即使对于拥有表单编辑访问权限的收件人也是如此。

您可以查明继承了自定义字段或构件访问权限的用户，并且可以移除对它的访问权限。

>[!NOTE]
>
>如果收件人拥有对共享自定义表单上的自定义字段或小部件的管理访问权限，则该访问权限将保留给收件人。

### 了解谁继承了自定义字段或小部件的访问权限 {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**自定义Forms**。
1. 单击&#x200B;**字段**，然后选择该字段、图像或访问小组件。
1. 在显示的框中，单击&#x200B;**继承权限**&#x200B;并查看显示的名称。
1. 单击&#x200B;**取消**。

### 删除对已共享自定义表单中的自定义字段或小部件的访问权限 {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

如果您需要删除对已共享自定义表单中的自定义字段或小部件的访问权限，则需要取消共享该表单。 有关说明，请参阅[共享自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)一文中的[删除对自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#remove-access-to-a-custom-form)的访问权限。


