---
title: 管理日历视图
description: 您可以在日历视图中显示记录及其字段。 本文介绍了如何创建日历视图，以及如何编辑或删除现有视图。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 45b5be81-703c-45d5-a08c-60cb8ec5b103
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '1771'
ht-degree: 4%

---

# 管理日历视图

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

-->

{{planning-important-intro}}

您可以从记录类型页在日历视图中显示记录及其字段。

有关Adobe Workfront Planning视图以及如何管理这些视图的信息，请参阅[管理记录视图](/help/quicksilver/planning/views/manage-record-views.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront包</p></td> 
   <td> 
<p>任何Workfront和任何Planning包</p>
<p>任何工作流和任何计划包</p>
<p>有关每个Workfront Planning包中所包含内容的更多信息，请联系您的Workfront客户代表。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p> 用于创建和删除视图的标准</p>
   <p>更新视图元素的参与者或更高版本</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>   <p>管理视图的权限</p>  
   <p>查看对视图的权限以临时更改视图设置或复制它</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>版面模板</p></td>
   <td> 必须为具有轻度或参与者许可证的用户分配一个包括Planning的布局模板。
   <p>默认情况下，标准用户和系统管理员已启用Planning区域。</p></div></li></ul>
</td>
  </tr> 
</tbody> 
</table>

有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++ 

<!--Old:
 <table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
    <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard to create and delete views</p>
   <p>Contributor or higher to update view elements</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a view</p>  
   <p>View permissions to a view to temporarily change the view settings or to duplicate it</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
</td>
  </tr>

</tbody> 
</table> -->

## 管理日历视图 {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

请考虑以下事项：

* 仅当至少有两个日期字段与记录类型关联时，才能创建日历视图。 如果有一个或没有与记录类型关联的日期字段，则“日历”视图选项将灰显。

  您可以从记录日期字段中选择，或从连接的记录或对象类型中选择查找日期字段。
* 存在以下情况：

   * 当“起始日期”和“终止日期”均没有值时，这些记录不会显示在日历中
   * 当“开始”或“结束”日期没有值时，记录显示为一天事件
   * 当开始日期在结束日期之后时，该记录不会显示在日历上。

要管理日历视图，请执行以下操作：

1. 转到要查看其日历的记录类型页面。
1. 创建日历视图，如[管理记录视图](/help/quicksilver/planning/views/manage-record-views.md)一文中所述。

   ![日历视图示例](assets/calendar-view-example.png)

   与您选择的记录类型关联的记录在日历中显示为条形。 默认情况下，栏的颜色与记录图标的颜色匹配。

1. 执行以下操作之一以浏览日历：

   * 单击日历左上角的左右图标，或使用水平滚动在日历中前后移动。
   * 单击右上角的&#x200B;**今天**，将日历居中到今天的日期。
   * 从时间范围下拉菜单中选择以下选项之一以更新时间增量：

      * **月**：记录显示在每月日历中。

      * **周**：记录显示在以下区域中：

         * 跨越多天的记录将显示在日历顶部。
         * 持续一天或更短的记录，显示在日历视图的下半部分。 如果选择显示开始日期和结束日期的小时，则记录会在发生日期的相应时间显示。

1. （可选）单击&#x200B;**全屏**&#x200B;图标![打开全屏图标](assets/open-full-screen-icon.png)以全屏方式打开视图，然后单击&#x200B;**退出全屏**&#x200B;图标![退出全屏图标](assets/exit-full-screen-icon.png)或键盘上的Escape以退出全屏。

1. 要在日历视图中创建记录或编辑其日期，请执行下列操作之一：

   * 双击日历上的任意位置以创建记录。

     有关信息，请参阅[创建记录](/help/quicksilver/planning/records/create-records.md)。

   * 单击记录栏的左边距或右边距，然后将其拖放到新位置。 调整记录栏的大小会立即更新其开始或结束日期。

   * 拖放记录栏以更新其位置和日期。 移动记录的栏会立即更新其开始和结束日期。

     有关信息，请参阅[编辑记录](/help/quicksilver/planning/records/edit-records.md)。

1. 更新以下视图元素，如以下子部分所述：
   * [过滤器](#add-filters)
   * [行高](#modify-row-height)
   * [设置](#edit-the-calendar-view-settings)

   <!--* [Grouping](#add-grouping)-->
   <!--* [Sort](#add-sort) not sure if this is present in calendar views?!; also check the anchor and make sure it's correct-->

### 添加过滤器

您可以使用过滤器减少屏幕上显示的信息量。

在日历视图中使用过滤器时，请考虑以下事项：

<!-- this list is almost identical to the one for the table view - update both-->

* 您为日历视图创建的筛选器与应用于同一记录类型的任何其他视图中的筛选器是相互独立的。

* 这些过滤器对于您选择的视图是唯一的。 同一记录类型的两个日历视图可以应用不同的筛选器。

* 查看同一日历视图的两个用户会看到当前应用的同一筛选器。

* 无法为日历视图命名您构建的过滤器。

* 删除筛选器会将其从与您访问相同记录类型以及显示与您相同的视图的任何人中删除。

* 您可以按连接的记录字段或查找字段进行筛选。

* 您可以按显示多个值的查找字段进行筛选。

要将筛选器添加到日历视图，请执行以下操作：

1. 为记录类型页面创建日历视图，如文章[管理记录视图](/help/quicksilver/planning/views/manage-record-views.md)中所述。
1. 选择一个日历视图，然后单击日历工具栏中的&#x200B;**筛选器**。
1. 单击&#x200B;**添加条件**&#x200B;并添加以下信息：

   * **选择要按**&#x200B;筛选的字段<!-- the tip below might change-->

   * **选择一个选项**（或筛选器修饰符）以定义字段必须满足哪种条件

     下表显示了每种字段类型的可用修饰符。

     <table>
        <thead>
        <tr>
            <th><b>字段类型</b></th>
            <th><b>修饰符</b></th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <td>单行、段落、公式 </td>
            <td><p>包含</p>
            <p>不包含</p>
            <p>是</p>
            <p>不是</p>
            <p>为空</p>
            <p>不为空</p></td>
        </tr>
        <tr><td>单选</td>
            <td><p>是</p>
            <p>不是</p>
            <p>是任何</p>
            <p>不是任何</p>
            <p>为空</p>
            <p>不为空</p></td>
        </tr>
        <tr>
            <td>多选，人员</td>
            <td><p>具有任何</p>
            <p>包含所有</p>
            <p>正好</p>
            <p>没有</p>
            <p>为空</p>
            <p>不为空</p></td>
        </tr>
        <tr>
            <td>数字、百分比、货币</td>
            <td><p>=</p>
            <p>≠</p>
            <p> &lt; </p>
            <p>&gt;</p>
            <p>≤</p>
            <p>≥</p>
            <p>为空</p>
            <p>不为空</p></td>
        </tr>
        <tr>
            <td>日期</td>
            <td><p>是</p>
            <p>不是</p>
            <p>晚于</p>
            <p>早于</p>
            <p>介于</p><p>非介于</p>
            <p>为空</p><p>不为空</p></td>
        </tr>

     <tr>
            <td>复选框</td>
            <td><p>是</p>
        </tr>
        </tbody>
        </table>

   * 为所选字段选择值。

   ![筛选器UI表视图](assets/filter-ui-table-view.png)

   您可以添加的筛选条件数量没有限制。

1. （可选）单击&#x200B;**添加条件**&#x200B;以添加其他筛选选项并重复上述步骤。 应用的过滤器数显示在过滤器图标的左侧。
1. 单击以下运算符以指示连接筛选条件的方式以及应如何应用：

   * **AND**：必须满足所有指定的条件。
   * **OR**：必须满足任何指定的条件。 这是默认选项。

   1. （可选）在多个条件分组之间添加其他&#x200B;**AND**&#x200B;或&#x200B;**OR**&#x200B;运算符。

      ![视图中的多层筛选器](assets/multi-tiered-filters-in-views.png)

   系统会自动过滤记录列表。 <!--at this time, you can't name and save the filter - but will this change?!-->
   <!-- asked on the task for the simple filters whether there is a limitation for how many statements a filter can have?!-->

1. （可选）单击&#x200B;**x**&#x200B;图标可删除筛选条件。
1. （可选）单击&#x200B;**筛选器**&#x200B;以关闭筛选器框。<!--right now you cannot "clear all" for filters, but this might come later-->


### 修改行高

您可以修改日历单元格的行高，以增加或减少每个单元格中显示的记录条数。

日历中显示的记录数因您在记录栏中显示的字段数而异。

>[!TIP]
>
>此设置仅在按月查看日历时可用。


1. 为记录类型页面创建日历视图，如文章[管理记录视图](/help/quicksilver/planning/views/manage-record-views.md)中所述。
1. （视情况而定）按月显示日历视图，然后单击日历工具栏中的&#x200B;**行高**。
1. 从以下选项中进行选择：

   <table>
    <thead>
    <tr>
        <th><b>行高选项</b></th>
        <th><b>默认最大记录数</b></th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td>短</td>
        <td><p>包含：</p>

   <ul><li>2条记录显示1个字段</li>
    <li>显示1个以上字段的1条记录</li></ul>
        </td>
    </tr>
    <tr><td>标准</td>
        <td><p>包含：</p>

   <ul><li>4条记录显示1个字段</li>
    <li>显示1个以上字段的2条记录</li></ul>
        </td>
    </tr>
    <tr>
        <td>媒介</td>
        <td><p>包含：</p>

   <ul><li>8条记录显示1个字段</li>
    <li>显示1个以上字段的4条记录</li></ul>
        </td>
    </tr>
    <tr>
        <td>高</td>
        <td><p>包含：</p>

   <ul><li>显示1个字段的12条记录</li>
    <li>显示1个以上字段的6条记录</li></ul>
        </td>
    </tr>
    <tr>
        <td>适合内容</td>
        <td><p>所有记录都可见，最多500条记录</p></td>
    </tr>
    </tbody>
    </table>

1. （可选）如果日历中有不可见的记录，请单击&#x200B;**更多**。

</span>

### 编辑日历视图设置

更新日历视图设置以指示视图中显示的信息及其显示方式。

1. 为记录类型创建日历视图，如[管理记录视图](/help/quicksilver/planning/views/manage-record-views.md)一文中所述。
1. 单击&#x200B;**设置**。
1. 单击左侧面板中的&#x200B;**日期和时间**，然后选择要显示在日历上的&#x200B;**开始日期**&#x200B;和&#x200B;**结束日期**。 您可以选择默认的“开始”和“结束”日期，也可以选择任何可用的日期字段。

   表示记录的条形图从您为开始日期指定的日期开始，结束日期对应于结束日期。

   >[!NOTE]
   >
   >* 对于开始日期或结束日期没有值或者开始日期晚于结束日期的记录，不会显示在日历视图中。
   >
   >* 如果使用“细分”选项显示附加记录，则起始日期和终止日期是主记录的起始日期和终止日期。 您无法在此区域为连接的记录选择开始日期和结束日期。

1. 单击左侧面板中的&#x200B;**栏样式**&#x200B;以指示要在记录栏上显示的信息。

   默认情况下会选择记录的主字段（或标题），如在记录的表格视图中定义的那样。
   <!--adjust this when the primary field is released??-->

1. （可选且视情况而定）如果您将缩略图添加到记录，请选择&#x200B;**缩略图**&#x200B;选项以在记录栏中显示与记录关联的图像。

   >[!NOTE]
   >
   >    必须先在表格视图中添加缩略图，然后才能在日历视图中显示它们。 有关详细信息，请参阅[将缩略图添加到记录](/help/quicksilver/planning/records/add-thumbnails-to-records.md)。

1. 单击&#x200B;**添加字段**，然后在&#x200B;**搜索字段**&#x200B;框中单击，然后单击要添加的字段。

   >[!TIP]
   >
   >   * 必须先创建这些字段，然后才能将其添加到记录栏。
   > 
   >   * 您必须至少选择一个字段。 默认情况下已选择&#x200B;**名称**。
   >
   >   * 您最多可以添加5个字段。

   右侧将显示日程表上栏的外观。

   日历视图设置中的![条形样式节](assets/bar-style-section-in-calendar-view-settings-with-preview.png)

1. 单击左侧面板中的&#x200B;**颜色**&#x200B;以自定义日历上记录的颜色。

   日历视图设置上的![颜色面板](assets/color-panel-on-calendar-view-settings.png)

1. 在&#x200B;**将记录颜色设置为**&#x200B;部分中，从以下选项中进行选择以设置记录的颜色：

   * **记录类型**：日历中记录栏的颜色与您选择的记录类型的颜色相匹配。 这是默认选项。
   * **字段值**：记录的颜色与您指定的字段的颜色匹配。
   * **无**：记录显示在白色栏中。

1. （视情况而定）如果您为记录颜色选择了&#x200B;**字段值**，请从&#x200B;**将记录颜色与**&#x200B;下拉菜单中选择一个字段。

   ![日历视图的字段选择器下拉菜单](assets/field-selector-drop-down-menu-calendar-view.png)

   下拉菜单中仅显示具有颜色编码选项的字段。

   例如，多选或单选字段可以具有颜色编码选项。

   如果对于所选的记录类型没有带颜色编码选项的字段，则此选项将灰显。


1. 单击&#x200B;**保存**。

   这些记录将按照您选择的规范显示在日历视图中。