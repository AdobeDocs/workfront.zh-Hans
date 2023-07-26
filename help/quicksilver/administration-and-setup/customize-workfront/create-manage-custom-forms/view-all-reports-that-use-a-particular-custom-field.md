---
title: 查看使用特定自定义字段或小部件的所有报表
description: 您可以在“自定义Forms”区域中添加自定义视图，以显示哪些报表正在使用特定自定义字段或构件。 在需要编辑或删除字段或构件时，此功能非常有用，因为它可能已在一个或多个报表中实施。 评估这些报告是否需要调整才能保持正常工作很重要。
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: eaafe79b-bdbc-4fb9-b449-23e5a4bc455a
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 0%

---

# 查看使用特定自定义字段或小部件的所有报表

您可以在“自定义Forms”区域中添加自定义视图，以显示哪些报表正在使用特定自定义字段或构件。 在需要编辑或删除字段或构件时，此功能非常有用，因为它可能已在一个或多个报表中实施。 评估这些报告是否需要调整才能保持正常工作很重要。

有关自定义表单中的自定义字段和小部件的信息，请参阅 [将自定义字段添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 和 [在自定义表单中添加或编辑资源小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront计划*</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td>计划</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>对自定义表单的管理访问权限</p> <p>有关Workfront管理员如何授予此访问权限的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用户对特定区域的管理访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问级别配置，请与Workfront管理员联系。

## 列出使用特定自定义字段或小部件的报表

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **自定义Forms**.
1. 打开 **字段** 选项卡，显示一个列出Workfront实例中所有自定义字段和小部件的报告。

   ![](assets/fields-tab.png)

1. 单击 **视图** 顶部标题中的下拉菜单，然后检查列表中是否包含的任何自定义视图 **报表** 列（不是此选项卡上的默认列）。

   在“报表”列中，您可以看到哪些报表正在使用系统中添加到自定义表单的每个自定义字段和小部件。 有人可能已创建了一个视图，该视图包括 **报表** 列。

1. 如果您没有看到包含 **报表** 列中，创建一个包含该列的新视图：

   1. 单击 **视图** 下拉菜单，然后单击 **新建视图**.

   1. 在 **新建视图** 出现的页面，在左上角附近的框中，替换 **新建参数视图** 带有视图的描述性名称，例如 *字段和小部件*.

   1. 单击 **添加列** 靠近右下角。
   1. 在 **显示在此列中** 左上角附近显示的框，开始键入 *报告*，然后选择 **报表** 出现在框下方的列表中。

   1. （视情况而定）如果要移动 **报表** 将刚刚添加的列拖到不同的水平位置，将其标题放在 **列预览** 区域填充页面。

   1. 单击 **完成**，然后单击 **保存视图**.

1. 单击 **视图** 下拉菜单，然后选择刚刚创建的自定义视图的名称。
1. 在 **名称** 列中，找到要编辑或删除的自定义字段或构件，然后查看 **报表** 列以查看哪些报表使用它（如果有）。

   要查找此列的信息，Workfront将搜索所有报表过滤器、视图、分组中的自定义字段和小部件。

   如果您看到加号，则可以单击该文本行以显示一个框，其中列出了使用该字段或小部件的所有附加报表。

   >[!NOTE]
   >
   >此工具的初始加载时间可能为10秒到2.5分钟，具体取决于系统中的数据量。

   >[!TIP]
   >
   >如果没时间调查使用该自定义字段或小部件的报告，可以单击导出创建列出它们的文件。 如果您拥有使用该字段或小部件的报告，则可与所有人共享此文件，并讨论需要进行的更改、更改对报告可能产生的影响以及需要采取哪些措施来确保报告继续正常工作。
   >
   >此视图也可在参数报表中使用：
   >      
   > 1. 在主菜单中，单击 **报表**.
   > 1. 在左上角附近，单击 **新建报告**，然后单击 **参数** 在显示的列表中。
   > 1. 单击 **添加列** 靠近右下角。
   > 1. 在 **显示在此列中** 左上角附近显示的框，开始键入 *报告*，然后选择 **报表** 出现在框下方的列表中。
   > 1. （视情况而定）如果要移动 **报表** 将刚刚添加的列拖到不同的水平位置，将其标题放在 **列预览** 区域填充页面。
   > 1. 单击 **完成**，然后单击 **保存+关闭**.
   > 1. 为报表键入一个描述性名称，如 *字段和小部件*.
