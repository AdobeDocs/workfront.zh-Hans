---
title: 使用布局模板自定义对象标头
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 作为Adobe Workfront管理员或组管理员，您可以使用布局模板来配置用户在打开对象页面时在对象标题中看到的字段。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: cbeaa0d7-a61a-4806-a871-96663d9ce124
source-git-commit: a1ffec0d8a50ff7f025ff23370afa746cf0d6d3f
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# 使用布局模板自定义对象标头

作为Adobe Workfront管理员或组管理员，您可以使用布局模板来配置用户在打开对象页面时在对象标题中看到的字段。

>[!IMPORTANT]
>
>自定义对象标头当前可用于项目、任务和问题。


有关组布局模板的信息，请参阅 [创建和修改组的布局模板](../../manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

![](assets/object-header-fields.png)

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：


<table>
  <tr>
   <td><strong>Adobe Workfront计划</strong>
   </td>
   <td>任意
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront许可证</strong>
   </td>
   <td>计划
   </td>
  </tr>
  <tr>
   <td><strong>访问级别配置</strong>
   </td>
   <td>您必须是Workfront或组管理员。
<p>
   </td>
  </tr>
</table>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 [创建或修改自定义访问级别](../../add-users/configure-and-grant-access/create-modify-access-levels.md).

## 自定义对象标头

1. 开始使用布局模板，如 [创建和管理布局模板](../../customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. 在 **自定义用户看到的内容** 下拉菜单，选择 **项目**, **任务** 或 **问题**.

   <!--when this will be possible for more than 3 objects, at production, make this more general: update the sentence above to say "select an object you want to customize in the Customize what users see drop-down menu). -->

1. 在 [!UICONTROL 标题字段] 中，将鼠标悬停在显示的字段上，然后执行下列操作之一：
   * 单击 **x** 删除字段的图标

      或

   * 单击并按住 **抓** 图标，以将字段拖放到新位置。

   <!--(NOTE: make sure the default names of these fields have not changed; otherwise, update screen shot)-->

   ![](assets/object-header-field-x-and-grab-icons-in-lt.png)

1. 对象的标头中最多可包含五个字段。
如果已选择五个字段，则必须先删除一个字段，然后才能添加新字段。
1. 在 **添加字段** 框中，开始键入要添加的不可编辑的Workfront字段的名称，然后在该字段显示在列表中时将其选中。 该字段将添加到“添加”字段框的正右侧，并将显示为对象标题左上角的第一个字段。

   >[!TIP]
   >
   >* 您只能添加在对象“详细信息”(Details)部分的“概述”(Overview)区域中显示且不可编辑的字段。 不可编辑的字段是用户无法手动编辑的字段。 它们由Workfront自动计算。
   >
   >* 您可以添加已属于默认标题一部分的可编辑字段（例如，“项目所有者”、“状态”、“完成百分比”、“分配”）。
   >
   >* 在将“解决者”字段添加到问题标题时，如果存在与问题关联的解决对象，则该字段将变为“解决问题、任务或项目”。



   ![](assets/add-field-to-header-in-lt-list.png)


1. （可选）按不同顺序拖放添加的字段。

1. 继续自定义布局模板。

   或

   如果您已完成自定义，请单击 **保存**.

   >[!TIP]
   >
   >您可以随时单击保存以保存进度，然后稍后继续修改模板。
