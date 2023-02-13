---
title: 创建或编辑自定义条件
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: 作为Adobe Workfront管理员，您可以为项目、任务和问题创建或编辑自定义条件，以符合您组织的需求。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5c950862-4358-4aab-997b-223972662150
source-git-commit: a3cb3d9d340d377e301c98480324bfe8bf507382
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 2%

---

# 创建或编辑自定义条件

作为Adobe Workfront管理员，您可以为项目、任务和问题创建或编辑自定义条件，以符合您组织的需求。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 创建或编辑自定义条件

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **项目首选项** > **条件**.

1. 单击对象类型的选项卡(**项目**, **任务**&#x200B;或 **问题**)，以将其与条件关联。

1. 要创建新条件，请单击 **添加新条件**.

   或

   要编辑现有条件，请将鼠标悬停在要编辑的条件上，然后单击 **编辑** 图标。

   ![](assets/custom-condition-edit-nwe.jpg)

1. 使用以下选项配置自定义条件：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>完成情况名称</td> 
      <td>（必需）为条件键入一个描述性名称。</td> 
     </tr> 
     <tr> 
      <td>描述</td> 
      <td>（可选）为将要使用该条件的人员键入条件用途的描述。</td> 
     </tr> 
     <tr> 
      <td>颜色</td> 
      <td>（可选）单击颜色图标，然后在项目、任务或问题中显示条件所需的颜色。 您还可以键入十六进制数。</td> 
     </tr> 
     <tr> 
      <td>等于 </td> 
      <td><p>（仅适用于项目）单击下拉列表中最能描述新条件函数的选项。 例如，对于名为“跟踪井”的条件，您可以单击“在目标上”。 这可确定默认条件的工作方式。 您创建的每个条件都必须等同于下拉菜单中的一个选项。</p>
      <p>有关默认条件的信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md" class="MCXref xref">将自定义条件设置为项目的默认条件</a> 和 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md" class="MCXref xref">将自定义条件设置为任务和问题的默认条件</a>.</p>
      <p>创建完条件后，无法修改此选项。</p></td> 
     </tr> 
     <tr> 
      <td>密钥</td> 
      <td><p>（必需）对于项目条件，请键入用户能够识别的字母数字缩写。 对于任务或问题条件，请键入一个介于01到99之间的两位数数字代码。 </p>
      <p>此键值（在API中使用并可用于报告目的）对于每个对象必须是唯一的。</p>
      <p>保存条件后，便无法更改条件的键。 </p></td> 
     </tr> 
     <tr> 
      <td>隐藏完成情况</td> 
      <td><p>（可选）此选项适用于您不再希望用户使用但出于历史原因而希望保留的自定义条件。 </p>
      <p>如果隐藏已用于工作项的自定义条件，则在隐藏该条件后，该条件会继续显示在这些工作项上。 </p></td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >您可以在所有三种对象类型中标准化条件术语和颜色。 为此，请将条件名称和颜色十六进制代码从一个选项卡（项目、任务、问题）复制到另两个选项卡的相应条件。

1. （可选）拖动 ![](assets/move-icon---dots.png) 新位置的任何条件来重新排序列表。

   这会更改条件在项目、任务和问题中显示的顺序：

   * 用户编辑项目时

      ![](assets/change-condition-edit-project.png)

   * 当用户在“更新”选项卡上更改任务或问题的条件时：

      ![](assets/change-condition-update-comment.png)

   * 当用户在列表视图中更改任务或问题的条件时：

      ![](assets/change-conditions-list-dropdown-only.png)

1. 单击&#x200B;**保存**。

您可以将自定义条件设置为项目或任务和问题的默认条件。 有关更多信息，请参阅 [将自定义条件设置为项目的默认条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md) 和 [将自定义条件设置为任务和问题的默认条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md).

有关自定义条件的更多信息，请参阅 [自定义条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
