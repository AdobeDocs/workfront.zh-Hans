---
title: 创建字段
description: 在Adobe管理器中，您可以为每种操作记录类型或分类创建自定义字段。 然后，可将该字段与Maestro记录相关联。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 28602d66b43ec4c30a9f13cff43157b978439d99
workflow-type: tm+mt
source-wordcount: '2555'
ht-degree: 2%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

<!--Should the structure of this article be like this one: https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/customize/custom-forms/custom-form-builder/use-the-custom-form-builder/add-a-custom-field-to-a-custom-form.html?lang=en ??-->

<!--will they add a way to create fields elsewhere than in a table?! - how will that change the structure of this article? -->

# 创建字段

>[!IMPORTANT]
>
>目前，AdobeMaestro是测试版计划的一部分，该计划对有限数量的客户开放。
>
>有关加入Maestro测试版计划的更多信息，请与您的客户代表联系。
>
>有关信息，请参阅 [Adobe大师概述](../maestro-overview.md).

在Adobe管理器中，您可以为操作记录类型或分类创建自定义字段。 然后，可将这些字段与Maestro记录关联以增强记录信息。

在创建要与记录类型关联的字段之前，您必须先创建记录类型。 有关信息，请参阅 [创建记录类型](../architecture-and-fields/create-record-types.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe产品</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront协议</p></td>
   <td>
<p>贵公司必须注册AdobeMaestro封闭测试版计划。 请联系您的客户代表以查询此新产品/服务。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront计划</p></td>
   <td>
<p>任何</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront许可证</p></td>
   <td>
   <p>任何</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">访问级别</td>
   <td> <p>任何</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">布局模板</td>
   <td> <p>系统管理员必须在布局模板中添加Maestro区域。 有关信息，请参阅 <a href="../access/grant-access.md">授予对Adobe大师的访问权限</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## 有关Maestro字段的注意事项

* 您只能从记录类型页面的表视图创建字段。 字段在表格视图中显示为列。

  有关管理表列（或记录字段）的信息，请参见 [管理表视图](../views/manage-the-table-view.md).

  有关管理字段的信息，另请参阅以下文章：

   * [编辑字段](../architecture-and-fields/edit-fields.md)
   * [删除字段](./delete-fields.md)

* 与记录类型关联的字段可用于与该类型的所有记录相关联。 <!--will this change and will the fields be available for other record types, too?! Also, the next bullet might need to change too if this one changes -->

* 无法将与记录类型关联的字段添加到其他记录类型。 <!-- this will change when they open the Field library tab when creating a field-->

* 您可以通过以下方式手动或自动创建字段：

   * 手动:

      * 通过在记录类型页的“表”视图中添加列。 表的列是与记录类型关联的字段。 这些是在记录的“详细信息”页面上显示的相同字段。

        不能从记录的详细信息页面创建字段。

        本文介绍了如何手动创建字段。

      * 通过将记录类型链接在一起。 在两个Maestro记录类型或记录类型与其他应用程序的对象类型之间添加新连接时，可以创建链接记录字段。

        <!--* Importing record types with fields using a CSV or an Excel file. - this is not available yet-->

        有关连接Maestro记录类型的详细信息，请参见 [连接记录类型](../architecture-and-fields/connect-record-types.md).

      * 通过使用Excel或CSV文件导入记录类型。 有关更多信息，请参阅 [创建记录类型](../architecture-and-fields/create-record-types.md).

   * 自动:

      * 默认情况下，每次创建记录类型时。

        以下是默认为每个新操作记录类型创建的标准字段：

         * 名称
         * 描述
         * 开始日期
         * 结束日期
         * 状态. 记录状态的默认值是：
            * 开发
            * 计划
            * 活动
            * 已完成
            * 保持

           您可以添加更多值或重命名现有值。

        以下是默认情况下，为每个新分类记录类型创建的标准字段：

         * 名称 <!--will more be added? If not, consider rephrasing this bullet-->

      * 从模板创建工作区时。 从模板创建工作区时，Maestro会为操作记录类型和分类创建字段。 有关信息，请参阅 [创建工作区](../architecture-and-fields/create-workspaces.md).



* 您可以查看和更新您或任何其他用户创建的字段的设置。 <!--this will change with access/ permissions-->

* 一个记录类型最多可以有500个字段。

* 字段名称最多可包含250个字符。

* 删除操作记录类型、分类或工作区时，与它们关联的所有字段以及字段的值也会被删除，并且无法恢复。 <!-- this might change with a possible recycle bin solution?!-->


## 从头开始创建字段 {#create-fields-from-scratch}

<!--in a table (not sure if this can be done elsewhere?!-->

1. 单击 **主菜单** 图标 ![](assets/main-menu-workfront.png) 在Workfront的右上角， <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> 然后单击 **大师** ![](assets/maestro-icon.png).

   默认情况下应打开上次访问的工作区。

1. （可选）展开现有工作区名称右侧的向下箭头，选择要为其创建字段的记录类型的工作区，然后单击记录类型。

   与记录类型关联的所有现有记录都会显示在表格视图的行中。

   >[!TIP]
   >
   >    如果没有显示记录，则表示您可能还没有任何记录，或者您可能应用了过滤器来限制您在屏幕上看到的内容。

   与记录类型关联的所有现有字段都会显示在表格视图的列中。 <!--caveat this for when we can hide the fields; mention that they can be hidden if they are not visible by default-->


1. 单击 **+** 图标来添加新字段。
1. 在 **新建字段** 选项卡，从以下字段类型中选择：

   * [单行文本](#single-line-text)
   * [段落](#paragraph)
   * [多选](#multi-select)
   * [单选](#single-select)
   * [日期](#date)
   * [数字](#number)
   * [百分比](#percentage)
   * [货币](#currency)
   * [复选框](#checkbox)

   >[!IMPORTANT]
   >
   >    保存字段后，无法更改该字段的字段类型。

1. 继续添加每个字段，如下节所述。

### 单行文本 {#single-line-text}

单行文本字段捕获有限的字母数字信息。 例如，您可以在一行文本字段中捕获“所有者”、“利益相关者”、“团队”或“组织”单位信息。 单行文本字段的内容最多可包含250个字符。 <!-- asked Lilit if we can change this to "Single-line" since this can have numbers and text.-->

1. 开始创建字段，如一节所述 [从头开始创建字段](#create-fields-from-scratch) 在本文中，然后选择 **单行文本** 字段类型。

   ![](assets/single-line-text-field-type.png)

1. 添加以下信息：
   * **名称**：字段类型的名称，它将显示在表或记录的详细信息页面中。 <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **描述**：有关字段的其他信息。 当您将鼠标悬停在表中的字段列标题上时，将显示字段的描述。
1. 单击&#x200B;**创建**。

   新的单行字段作为列添加到记录类型，其值可以与记录相关联。 字段还显示在记录的详细信息页面上。


### 段落 {#paragraph}

段落字段捕获有关记录的其他字母数字信息，与描述字段类似。 段落字段的内容最多可包含1,000个字符。

1. 开始创建字段，如一节所述 [从头开始创建字段](#create-fields-from-scratch) 在本文中，然后选择 **段落** 字段类型。

   ![](assets/paragraph-field-type.png)


1. 添加以下信息：
   * **名称**：字段类型的名称，它将显示在表或记录的详细信息页面中。 <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **描述**：有关字段的其他信息。 当您将鼠标悬停在表中的字段列上时，将显示字段的描述。
1. 单击&#x200B;**创建**。

   新的段落字段作为列添加到记录类型，其值可以与记录相关联。 字段还显示在记录的详细信息页面上。


### 多选 {#multi-select}

您可以从下拉菜单中选择多个选项，使用多选字段捕获任何格式的其他信息。

1. 开始创建字段，如一节所述 [从头开始创建字段](#create-fields-from-scratch) 在本文中，然后选择 **多选** 字段类型。

   ![](assets/multi-select-field-type.png)


1. 添加以下信息：
   * **名称**：字段类型的名称，它将显示在表或记录的详细信息页面中。 <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **描述**：有关字段的其他信息。 当您将鼠标悬停在表中的字段列上时，将显示字段的描述。
   * **选项**：保存字段后可从下拉菜单中选择的选项。 每个选择的名称可以同时包含数字和字母。
1. 单击 **添加选项** 根据需要添加任意数量的选项。 您可以向多选字段添加的选项数量没有限制。
1. （可选）按所需顺序手动拖放每个选项，或选择
   **将选项按A-Z排序** 选项。 <!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. 单击 **x** 图标以将其删除。
1. 单击某个选项左侧的颜色样本可展开颜色选择器并自定义每个选项的颜色。
1. 单击&#x200B;**创建**。

   新的多选字段作为列添加到记录类型，其值可以与记录相关联。 字段还显示在记录的详细信息页面上。

### 单选 {#single-select}

通过从下拉菜单中选择一个选项，单选字段可以捕获任何格式的附加信息。

1. 开始创建字段，如一节所述 [从头开始创建字段](#create-fields-from-scratch) 在本文中，然后选择 **单选** 字段类型。

   ![](assets/single-select-field-type.png)


1. 添加以下信息：
   * **名称**：字段类型的名称，它将显示在表或记录的详细信息页面中。 <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **描述**：有关字段的其他信息。 当您将鼠标悬停在表中的字段列上时，将显示字段的描述。
   * **选项**：保存字段后可从下拉菜单中选择的选项。 每个选择的名称可以同时包含数字和字母。

1. 单击 **添加选项** 根据需要添加任意数量的选项。 您可以向单选字段添加的选项数量没有限制。
1. （可选）按所需顺序手动拖放每个选项，或选择 **将选项按A-Z排序** 选项。 <!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. 单击 **x** 图标以将其删除。
1. 单击某个选项左侧的颜色样本可展开颜色选择器并自定义每个选项的颜色。
1. 单击&#x200B;**创建**。

   新的单选字段作为列添加到记录类型，其值可以与记录相关联。 字段还显示在记录的详细信息页面上。

### 日期 {#date}

您可以使用日期字段以日期和时间格式捕获其他信息。

1. 开始创建字段，如一节所述 [从头开始创建字段](#create-fields-from-scratch) 在本文中，然后选择 **日期** 字段类型。

   ![](assets/date-field-type.png)


1. 添加以下信息：
   * **名称**：字段类型的名称，它将显示在表或记录的详细信息页面中。 <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **描述**：有关字段的其他信息。 当您将鼠标悬停在表中的字段列上时，将显示字段的描述。
   * **日期格式**：要在此字段中显示的日期格式类型。

     从以下格式中选择：
      * **区域设置**：匹配浏览器的区域设置。
      * **标准**：2023年5月16日
      * **长**：2023年5月16日
      * **欧洲**：2023年16月5日
      * **ISO**：2023-05-16
   * **包括时间字段**：如果要包含时间戳，请选择此选项。 默认情况下，该选项处于未选中状态。

     从以下选项中选择：

      * **24小时**：例如：18:00
      * **12小时**：例如：6:00 PM

1. 单击&#x200B;**创建**。

   新的日期字段作为列添加到记录类型，其值可以与记录相关联。 字段还显示在记录的详细信息页面上。

### 数字 {#number}

数字字段类型以数字格式捕获信息。

1. 开始创建字段，如一节所述 [从头开始创建字段](#create-fields-from-scratch) 在本文中，然后选择 **数字** 字段类型。

   ![](assets/number-field-type.png)
1. 添加以下信息：

   * **名称**：字段类型的名称，它将显示在表或记录的详细信息页面中。
   * **描述**：有关字段的其他信息。 当您将鼠标悬停在表中的字段列上时，将显示字段的描述。
   * **精度**：要为字段记录的小数位数。 您最多可以显示6个小数。
   * **允许负数**：如果要允许此字段中存在负数，请选择此选项。 默认情况下，此选项处于未选中状态。

   >[!NOTE]
   >
   >    如果选择“允许负数”，并且负值存储在附加字段的记录中，则以后不能再取消选择该设置。

1. 单击&#x200B;**创建**。

   新的数字字段作为列添加到记录类型，其值可以与记录相关联。 字段还显示在记录的详细信息页面上。

### 百分比 {#percentage}

百分比字段类型以数字格式捕获信息，后跟百分比符号。

1. 开始创建字段，如一节所述 [从头开始创建字段](#create-fields-from-scratch) 在本文中，然后选择 **百分比** 字段类型。

   ![](assets/percentage-field-type.png)

1. 添加以下信息：
   * **名称**：字段类型的名称，它将显示在表或记录的详细信息页面中。
   * **描述**：有关字段的其他信息。 当您将鼠标悬停在表中的字段列上时，将显示字段的描述。
   * **精度**：要为字段记录的小数位数。 您最多可以显示6个小数。
   * **允许负数**：如果您希望此字段允许负百分比值，请选择此选项。 默认情况下，此选项处于未选中状态。

   >[!NOTE]
   >
   >    如果选择“允许负数”，并且负值存储在附加字段的记录中，则以后不能再取消选择该设置。

1. 单击&#x200B;**创建**。

   新的百分比字段作为列添加到记录类型，其值可以与记录相关联。 字段还显示在记录的详细信息页面上。

### 货币 {#currency}

货币字段类型以数字格式捕获信息，该格式前面带有货币符号。

1. 开始创建字段，如一节所述 [从头开始创建字段](#create-fields-from-scratch) 在本文中，然后选择 **货币** 字段类型。

   ![](assets/currency-field-type.png)

1. 添加以下信息：
   * **名称**：字段类型的名称，它将显示在表或记录的详细信息页面中。 <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **描述**：有关字段的其他信息。 当您将鼠标悬停在表中的字段列上时，将显示字段的描述。
   * **货币**：要在此字段中显示的货币类型。 这是国际标准化组织(ISO)的货币列表。
   * **精度**：要为字段记录的小数位数。 您最多可以显示6个小数。
   * **允许负数**：如果要允许此字段中存在负货币值，请选择此选项。 默认情况下，此选项处于未选中状态。

   >[!NOTE]
   >
   >    如果选择“允许负数”，并且负值存储在附加字段的记录中，则以后不能再取消选择该设置。

1. 单击&#x200B;**创建**。

   新货币字段作为列添加到记录类型，其值可以与记录相关联。 字段还显示在记录的详细信息页面上。

### 复选框

您可以使用Checkbox字段类型将单个复选框选项添加到记录。 您可以使用此字段指明特定记录的特定属性或状态。 例如，您可以将其用作跟踪每个记录的完成、批准或任何其他二进制属性的标志。

1. 开始创建字段，如一节所述 [从头开始创建字段](#create-fields-from-scratch) 在本文中，然后选择 **复选框** 字段类型。

   ![](assets/checkbox-field-type.png)

1. 添加以下信息：
   * **名称**：字段类型的名称，它将显示在表或记录的详细信息页面中。 <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **描述**：有关字段的其他信息。 当您将鼠标悬停在表中的字段列上时，将显示字段的描述。
1. 单击&#x200B;**创建**。

   新的复选框字段作为列添加到记录类型，其值可以与记录相关联。 字段还显示在记录的详细信息页面上。

## 通过将记录类型链接在一起来创建字段

在两个Maestro记录类型或记录类型与其他应用程序的对象类型之间添加新连接时，可以创建链接记录字段。

有关连接Maestro记录类型的信息，请参见 [连接记录类型](../architecture-and-fields/connect-record-types.md).

## 通过使用Excel和CSV文件导入记录类型来创建字段

有关更多信息，请参阅 [创建记录类型](../architecture-and-fields/create-record-types.md).

## 通过创建记录类型创建字段

创建记录类型时，默认情况下还会创建与新记录类型关联的多个字段。 有关更多信息，请参阅 [创建记录类型](../architecture-and-fields/create-record-types.md).

## 通过从模板创建工作区来创建字段

从模板创建工作区时，Maestro会为操作记录类型和分类创建字段。

有关信息，请参阅 [创建工作区](../architecture-and-fields/create-workspaces.md).


