---
title: 创建字段
description: 在Adobe Workfront Planning中，您可以为每种记录类型创建自定义字段。 然后，您可以将该字段与Workfront Planning记录关联。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 7e2bb0ee-5f25-4307-9fec-876590c0ae1a
source-git-commit: 5c7b60ac5b78bd065ffc270588ec72ab3eb2f41d
workflow-type: tm+mt
source-wordcount: '3390'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!---
title: Create fields
description: In Adobe Workfront Planning, you can create custom fields for each kind of operational record type or taxonomy. You can then associate the field with records.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

<!--Should the structure of this article be like this one: https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/customize/custom-forms/custom-form-builder/use-the-custom-form-builder/add-a-custom-field-to-a-custom-form.html?lang=en ??-->

<!--will they add a way to create fields elsewhere than in a table?! - how will that change the structure of this article? -->

<!--Do we need this for FORMULAS: when we release permissions to RECORDS and we release referring lookup fields in a formula field, update considerations to say that lookup fields from linked records depends on the permissions to the record; if they have no permissions to view a linked record, they won't be able to use that records's lookup fields in a formula - not sure is needed??-->

# 创建字段

{{planning-important-intro}}

在Adobe Workfront Planning中，您可以为记录类型创建自定义字段。 然后，您可以将这些字段与Workfront Planning记录关联以增强记录信息。

在创建要与记录类型关联的字段之前，您必须先创建记录类型。 有关信息，请参阅[创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)。

在Workfront Planning中，您可以通过以下方式创建字段：

* 从头开始
* 通过连接记录类型
* 通过使用Excel或CSV文件导入记录类型
* 通过创建记录类型
* 通过从模板创建工作区

有关Workfront Planning字段的更多信息，请参阅[字段概述](/help/quicksilver/planning/fields/fields-overview.md)。

## 访问要求

+++ 展开以查看Workfront Planning的访问要求。

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 产品</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront协议</p></td>
   <td>
<p>您的组织必须注册到Workfront Planning的早期访问阶段 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront计划</p></td>
   <td>
<p>任何</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td>
   <td>
   <p>新增：标准</p> 
   <p>当前：计划</p>
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>访问级别配置</p></td>
   <td> <p>Workfront Planning没有访问级别控制</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>权限</p></td>
   <td> <p>管理工作区</a>的权限 </p>  
   <p>系统管理员有权访问所有工作区，包括他们未创建的工作区。</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>您的Workfront或组管理员必须在布局模板中添加Planning区域。 有关信息，请参阅<a href="/help/quicksilver/planning/access/access-overview.md">访问概述</a>。 </p>  
</td>
  </tr>

</tbody>
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 从头开始创建字段 {#create-fields-from-scratch}

<!--in a table (not sure if this can be done elsewhere?!-->

{{step1-to-planning}}

1. 单击要为其创建字段的记录的工作区。

   此时会打开工作区，并显示记录类型。

1. 单击记录类型的卡。

   与记录类型关联的所有现有记录都会显示在表格视图的行中。

   >[!TIP]
   >
   >    如果没有显示记录，则表示您可能还没有任何记录，或者您可能应用了过滤器来限制您在屏幕上看到的内容。

   与记录类型关联的所有现有字段都会显示在表格视图的列中。

   >[!TIP]
   >
   >    某些字段可能已隐藏。 单击字段，然后启用在表格视图中作为列查看的字段的切换。

1. 单击表格视图右上角的&#x200B;**+**&#x200B;图标

   或

   将鼠标悬停在任何列的标题上，单击字段名称后面的向下箭头，然后单击&#x200B;**向左插入**&#x200B;或&#x200B;**向右插入**&#x200B;以添加新字段。
1. 在&#x200B;**新字段**&#x200B;选项卡中，搜索&#x200B;**字段类型**&#x200B;框中的字段类型，或从以下字段类型中选择：

   * [单行文本](#single-line-text)
   * [段落](#paragraph)
   * [多选](#multi-select)
   * [单选](#single-select)
   * [日期](#date)
   * [数字](#number)
   * [百分比](#percentage)
   * [货币](#currency)
   * [复选框](#checkbox)
   * [公式](#formula)
   * [人员](#people)
   * [创建者](#created-by)
   * [创建日期](#created-date)
   * [上次修改者](#last-modified-by)
   * [上次修改日期](#last-modified-date)

   >[!IMPORTANT]
   >
   >    保存字段后，无法更改该字段的字段类型。

1. 继续添加每个字段，如下节所述。

### 单行文本 {#single-line-text}

单行文本字段捕获有限的字母数字信息。 例如，您可以在一行文本字段中捕获“所有者”、“利益相关者”、“团队”或“组织”单位信息。 单行文本字段的内容最多可包含250个字符。<!-- asked Lilit if we can change this to "Single-line" since this can have numbers and text.-->

1. 按照本文中[从头开始创建字段](#create-fields-from-scratch)部分中的说明开始创建字段，然后选择&#x200B;**单行文本**&#x200B;字段类型。

   ![](assets/single-line-text-field-type.png)

1. 在&#x200B;**新建字段**&#x200B;选项卡中添加以下信息：
   * **名称**：字段类型的名称，它将显示在表或记录的详细信息页面中。<!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **描述**：有关该字段的其他信息。 当您将鼠标悬停在表中的字段列标题上时，将显示字段的描述。
1. 单击&#x200B;**创建**。

   新的单行字段作为列添加到记录类型，其值可以与记录相关联。


### 段落 {#paragraph}

段落字段捕获有关记录的其他字母数字信息，与描述字段类似。

>[!TIP]
>
>* 段落字段的内容最多可包含1,000个字符。
>
>* 当段落字段显示在记录的表视图或详细信息页面中时，您可以使用富文本格式来增强段落字段的内容。 有关信息，请参阅[编辑记录](/help/quicksilver/planning/records/edit-records.md)。

1. 按照本文中[从头开始创建字段](#create-fields-from-scratch)部分中的说明开始创建字段，然后选择&#x200B;**段落**&#x200B;字段类型。

   ![](assets/paragraph-field-type.png)


1. 在&#x200B;**新建字段**&#x200B;选项卡中添加以下信息：
   * **名称**：字段类型的名称，它将显示在表或记录的详细信息页面中。<!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **描述**：有关该字段的其他信息。 当您将鼠标悬停在表中的字段列上时，将显示字段的描述。
1. 单击&#x200B;**创建**。

   新的段落字段作为列添加到记录类型，其值可以与记录相关联。


### 多选 {#multi-select}

您可以从下拉菜单中选择多个选项，使用多选字段捕获任何格式的其他信息。

1. 按照本文中[从头开始创建字段](#create-fields-from-scratch)部分中的说明开始创建字段，然后选择&#x200B;**多选**&#x200B;字段类型。

   ![](assets/multi-select-field-type.png)


1. 在&#x200B;**新建字段**&#x200B;选项卡中添加以下信息：
   * **名称**：字段类型的名称，它将显示在表或记录的详细信息页面中。<!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **描述**：有关该字段的其他信息。 当您将鼠标悬停在表中的字段列上时，将显示字段的描述。
   * **选项**：保存字段后可从下拉菜单中选择的选项。 每个选择的名称可以同时包含数字和字母。
1. 单击&#x200B;**添加选项**&#x200B;可根据需要添加任意数量的选项。 您可以向多选字段添加的选项数量没有限制。
1. （可选）按所需顺序手动拖放每个选项，或选择
   如果要按字母顺序自动列出选项，请&#x200B;**对选项A-Z**&#x200B;进行排序。<!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. （可选）要删除某个选择，请单击其右侧的&#x200B;**x**&#x200B;图标。
1. 单击某个选项左侧的颜色样本可展开颜色选择器并自定义每个选项的颜色。
1. 单击&#x200B;**创建**。

   新的多选字段作为列添加到记录类型，其值可以与记录相关联。

### 单选 {#single-select}

通过从下拉菜单中选择一个选项，单选字段可以捕获任何格式的附加信息。

1. 按照本文中[从头开始创建字段](#create-fields-from-scratch)部分中的说明开始创建字段，然后选择&#x200B;**单选**&#x200B;字段类型。

   ![](assets/single-select-field-type.png)


1. 在&#x200B;**新建字段**&#x200B;选项卡中添加以下信息：
   * **名称**：字段类型的名称，它将显示在表或记录的详细信息页面中。<!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **描述**：有关该字段的其他信息。 当您将鼠标悬停在表中的字段列上时，将显示字段的描述。
   * **选项**：保存字段后可从下拉菜单中选择的选项。 每个选择的名称可以同时包含数字和字母。

1. 单击&#x200B;**添加选项**&#x200B;可根据需要添加任意数量的选项。 您可以向单选字段添加的选项数量没有限制。
1. （可选）按所需顺序手动拖放每个选项，或者如果要按字母顺序自动列出选项，请选择&#x200B;**将选项按A到Z排序**&#x200B;选项。<!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. （可选）要删除某个选择，请单击其右侧的&#x200B;**x**&#x200B;图标。
1. 单击某个选项左侧的颜色样本可展开颜色选择器并自定义每个选项的颜色。
1. 单击&#x200B;**创建**。

   新的单选字段作为列添加到记录类型，其值可以与记录相关联。

### 日期 {#date}

您可以使用日期字段以日期和时间格式捕获其他信息。

1. 按照本文中[从头开始创建字段](#create-fields-from-scratch)部分中的说明开始创建字段，然后选择&#x200B;**日期**&#x200B;字段类型。

   ![](assets/date-field-type.png)


1. 在&#x200B;**新建字段**&#x200B;选项卡中添加以下信息：
   * **名称**：字段类型的名称，它将显示在表或记录页中。<!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **描述**：有关该字段的其他信息。 当您将鼠标悬停在表中的字段列上时，将显示字段的描述。
   * **日期格式**：要在此字段中显示的日期格式类型。<!--update this casing - submitted bug for it-->

     从以下格式中选择：
      * **区域设置**：与浏览器的区域设置匹配。
      * **标准**： 05/16/2023
      * **长**：2023年5月16日
      * **欧洲**： 16/05/2023
      * **ISO**： 2023-05-16
   * **包含时间字段**：如果要包含时间戳，请选择此选项。 默认情况下，该选项处于未选中状态。<!--update this setting name - submitted bug for it to be changed-->

     从以下选项中选择：

      * **24hr**：例如：18:00
      * **12hr**：例如：下午6:00

1. 单击&#x200B;**创建**。

   新的日期字段作为列添加到记录类型，其值可以与记录相关联。

### 数字 {#number}

数字字段类型以数字格式捕获信息。

1. 按照本文中[从头开始创建字段](#create-fields-from-scratch)部分中的说明开始创建字段，然后选择&#x200B;**数字**&#x200B;字段类型。

   ![](assets/number-field-type.png)
1. 在&#x200B;**新建字段**&#x200B;选项卡中添加以下信息：

   * **名称**：字段类型的名称，它将显示在表或记录页中。
   * **描述**：有关该字段的其他信息。 当您将鼠标悬停在表中的字段列上时，将显示字段的描述。
   * **精度**：要为该字段记录的小数位数。 您最多可以显示6个小数。
   * **允许负数**：如果要允许该字段中存在负数，请选择此选项。 默认情况下，此选项处于未选中状态。

   >[!NOTE]
   >
   >    如果选择“允许负数”，并且负值存储在附加字段的记录中，则以后不能再取消选择该设置。

1. 单击&#x200B;**创建**。

   新的数字字段作为列添加到记录类型，其值可以与记录相关联。

### 百分比 {#percentage}

百分比字段类型以数字格式捕获信息，后跟百分比符号。

1. 按照本文中[从头开始创建字段](#create-fields-from-scratch)部分中的说明开始创建字段，然后选择&#x200B;**百分比**&#x200B;字段类型。

   ![](assets/percentage-field-type.png)

1. 在&#x200B;**新建字段**&#x200B;选项卡中添加以下信息：
   * **名称**：字段类型的名称，它将显示在表或记录页中。
   * **描述**：有关该字段的其他信息。 当您将鼠标悬停在表中的字段列上时，将显示字段的描述。
   * **精度**：要为该字段记录的小数位数。 您最多可以显示6个小数。
   * **允许负数**：如果要允许此字段中的负百分比值，请选择此选项。 默认情况下，此选项处于未选中状态。

   >[!NOTE]
   >
   >    如果选择“允许负数”，并且负值存储在附加字段的记录中，则以后不能再取消选择该设置。

1. 单击&#x200B;**创建**。

   新的百分比字段作为列添加到记录类型，其值可以与记录相关联。

### 货币 {#currency}

货币字段类型以数字格式捕获信息，该格式前面带有货币符号。

1. 按照本文中[从头开始创建字段](#create-fields-from-scratch)部分中的说明开始创建字段，然后选择&#x200B;**货币**&#x200B;字段类型。

   ![](assets/currency-field-type.png)

1. 在&#x200B;**新建字段**&#x200B;选项卡中添加以下信息：
   * **名称**：字段类型的名称，它将显示在表或记录页中。<!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **描述**：有关该字段的其他信息。 当您将鼠标悬停在表中的字段列上时，将显示字段的描述。
   * **货币**：要在此字段中显示的货币类型。 这是国际标准化组织(ISO)的货币列表。
   * **精度**：要为该字段记录的小数位数。 您最多可以显示6个小数。
   * **允许负数**：如果要允许在此字段中出现负货币值，请选择此选项。 默认情况下，此选项处于未选中状态。

   >[!NOTE]
   >
   >    如果选择“允许负数”，并且负值存储在附加字段的记录中，则以后不能再取消选择该设置。

1. 单击&#x200B;**创建**。

   新货币字段作为列添加到记录类型，其值可以与记录相关联。

### 复选框

您可以使用Checkbox字段类型将单个复选框选项添加到记录。 您可以使用此字段指明特定记录的特定属性或状态。 例如，您可以将其用作跟踪每个记录的完成、批准或任何其他二进制属性的标志。

1. 按照本文中[从头开始创建字段](#create-fields-from-scratch)部分中的说明开始创建字段，然后选择&#x200B;**复选框**&#x200B;字段类型。

   ![](assets/checkbox-field-type.png)

1. 在&#x200B;**新建字段**&#x200B;选项卡中添加以下信息：
   * **名称**：字段类型的名称，它将显示在表或记录页中。<!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **描述**：有关该字段的其他信息。 当您将鼠标悬停在表中的字段列上时，将显示字段的描述。
1. 单击&#x200B;**创建**。

   新的复选框字段作为列添加到记录类型，其值可以与记录相关联。

### 公式

公式字段使用记录类型中其他字段的现有值以及指示应如何计算现有值的函数来生成新值。

有关详细信息，请参阅[公式字段概述](/help/quicksilver/planning/fields/formula-fields.md)。

1. 按照本文中[从头开始创建字段](#create-fields-from-scratch)部分中的说明开始创建字段，然后选择&#x200B;**公式**&#x200B;字段类型。

   ![](assets/new-formula-field-with-list-of-expressions.png)

1. 在&#x200B;**新建字段**&#x200B;选项卡中添加以下信息：

   * **名称**：输入新字段的名称。
   * **描述**：添加有关新字段的信息。
   * **公式**：开始键入至少一个字符以访问表达式，然后在表达式显示在列表中时将其选定。

1. 单击所选表达式以显示定义并查看其格式。

   ![](assets/description-of-formula-expression.png)

   有关支持的表达式的详细信息，请参阅[公式字段概述](/help/quicksilver/planning/fields/formula-fields.md)。

1. 添加在Workfront Planning中显示的字段名称，以在公式中引用它们。

   >[!NOTE]
   >
   >* 不能在公式中添加多选类型字段。
   >
   >* 您可以引用与当前记录类型相距最多4级的字段。 例如，如果要为活动记录类型创建公式字段，并且活动连接到产品记录类型，而产品记录类型连接到市场活动记录类型，而市场活动记录类型连接到Workfront项目，则可以在为活动记录类型创建的公式中引用项目的预算。

1. 单击&#x200B;**创建**。

   新的公式字段作为列添加到记录类型，其值可以与记录相关联。


### 人员

您可以使用“人员”字段类型将用户<!--, job role, or team-->添加到记录。 这是预先输入字段，您只能添加您的Workfront实例中已存在的用户<!--, roles, or teams-->。

1. 按照本文中[从头开始创建字段](#create-fields-from-scratch)部分中的说明开始创建字段，然后选择&#x200B;**人员**&#x200B;字段类型。

   ![](assets/people-field-type.png)

1. 在&#x200B;**新建字段**&#x200B;选项卡中添加以下信息：
   * **名称**：字段类型的名称，它将显示在表或记录页中。
   * **描述**：有关该字段的其他信息。 当您将鼠标悬停在表中的字段列上时，将显示字段的描述。
   * **允许多个值**：如果要允许用户在此字段中添加多个用户，请选择此选项。 默认情况下，此选项处于未选中状态。

   >[!NOTE]
   >
   >    如果选择“允许多个值”，并且多个用户存储在字段附加到的记录中，则以后编辑此字段时，无法再取消选择设置。

1. 单击&#x200B;**创建**。

   新的People-type字段作为列添加到记录类型，其值可与记录相关联。

### 创建者

您可以使用“创建者”字段类型将创建记录的用户添加到记录。 这是只读字段，它会自动填充在创建记录时登录的用户名称。

1. 按照本文中[从头开始创建字段](#create-fields-from-scratch)部分中的说明开始创建字段，然后选择&#x200B;**创建者**&#x200B;字段类型。

   ![](assets/created-by-field-type.png)

1. 在&#x200B;**新建字段**&#x200B;选项卡中添加以下信息：

   * **名称**：字段类型的名称，它将显示在表或记录页中。<!--this might change and they might prepopulate it with "Created by"-->
   * **描述**：有关该字段的其他信息。 当您将鼠标悬停在表中的字段列上时，将显示字段的描述。

1. 单击&#x200B;**创建**。

   新的“创建者 — 类型”字段作为列添加到记录类型中，其值预先填充有创建每个记录的用户的名称。


### 创建日期

您可以使用创建日期字段类型将记录的创建日期添加到记录。 此字段为只读字段，并且会自动填充创建记录的日期(以及（可选）时间。

1. 按照本文中[从头开始创建字段](#create-fields-from-scratch)部分中的说明开始创建字段，然后选择&#x200B;**创建日期**&#x200B;字段类型。

   ![](assets/created-date-field-type.png)

   <!--check the image above - added bug fix for UI text changes-->

1. 在&#x200B;**新建字段**&#x200B;选项卡中添加以下信息：

   * **名称**：字段类型的名称，它将显示在表或记录页中。<!--this might change and they might prepopulate it with "Created date"-->
   * **描述**：有关该字段的其他信息。 当您将鼠标悬停在表中的字段列上时，将显示字段的描述。
   * **日期格式**：从以下格式中选择：

      * **区域设置**：与浏览器的区域设置匹配。
      * **标准**： 05/16/2023
      * **长**：2023年5月16日
      * **欧洲**： 16/05/2023
      * **ISO**： 2023-05-16
   * **包含时间字段**：如果要包含时间戳，请选择此选项。 默认情况下，该选项处于未选中状态。<!--submitted a UI text change for this - check the UI-->

     从以下选项中选择：

      * **24hr**：例如：18:00
      * **12hr**：例如：下午6:00

1. 单击&#x200B;**创建**。

   新的创建日期类型字段作为列添加到记录类型，其值预填充有创建记录的日期（或日期和时间）。


### 上次修改者

您可以使用“上次修改人”字段类型将上次修改记录的用户添加到记录。 此字段为只读字段，并且会自动填充上次更新记录时登录的用户的名称。

1. 按照本文中[从头开始创建字段](#create-fields-from-scratch)部分中的说明开始创建字段，然后选择&#x200B;**上次修改者**&#x200B;字段类型。

   ![](assets/last-modified-by-field-type.png)

1. 在&#x200B;**新建字段**&#x200B;选项卡中添加以下信息：

   * **名称**：字段类型的名称，它将显示在表或记录页中。<!--this might change and they might prepopulate it with "Created by"-->
   * **描述**：有关该字段的其他信息。 当您将鼠标悬停在表中的字段列上时，将显示字段的描述。

1. 单击&#x200B;**创建**。

   新的上次修改者类型字段作为列添加到记录类型，其值预填充有上次修改每个记录的用户的名称。


### 上次修改日期

您可以使用“上次修改日期”字段类型来添加上次将记录修改为记录的日期。 此字段为只读字段，并且会自动使用上次修改记录的日期(以及（可选）时间填充。

1. 按照本文中[从头开始创建字段](#create-fields-from-scratch)部分中的说明开始创建字段，然后选择&#x200B;**创建日期**&#x200B;字段类型。

   ![](assets/last-modified-date-field-type.png)

   <!--check the image above - added bug fix for UI text changes-->

1. 在&#x200B;**新建字段**&#x200B;选项卡中添加以下信息：

   * **名称**：字段类型的名称，它将显示在表或记录页中。<!--this might change and they might prepopulate it with "Created date"-->
   * **描述**：有关该字段的其他信息。 当您将鼠标悬停在表中的字段列上时，将显示字段的描述。
   * **日期格式**：从以下格式中选择：

      * **区域设置**：与浏览器的区域设置匹配。
      * **标准**： 05/16/2023
      * **长**：2023年5月16日
      * **欧洲**： 16/05/2023
      * **ISO**： 2023-05-16
   * **包含时间字段**：如果要包含时间戳，请选择此选项。 默认情况下，该选项处于未选中状态。<!--submitted a UI text change for this - check the UI-->

     从以下选项中选择：

      * **24hr**：例如：18:00
      * **12hr**：例如：下午6:00

1. 单击&#x200B;**创建**。

   新的“上次修改日期 — 类型”字段作为列添加到记录类型中，其值预填充有上次修改记录的日期（或日期和时间）。

## 通过连接记录类型创建字段

在两种记录类型之间添加新连接，或者从其它应用程序添加记录类型和对象类型时，可以创建链接记录字段。

有关连接Workfront Planning记录类型的信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)

## 通过使用Excel或CSV文件导入记录类型来创建字段

有关详细信息，请参阅[创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)。

## 通过创建记录类型创建字段

创建记录类型时，默认情况下还会创建与新记录类型关联的多个字段。 有关详细信息，请参阅[创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)。

## 通过从模板创建工作区来创建字段

从模板创建工作区时，Adobe Workfront Planning会为记录类型创建字段。

有关信息，请参阅[创建工作区](/help/quicksilver/planning/architecture/create-workspaces.md)。