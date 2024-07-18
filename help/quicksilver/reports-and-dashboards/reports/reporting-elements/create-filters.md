---
product-area: reporting
navigation-topic: reporting-elements
title: 在Adobe Workfront中创建或编辑筛选器
description: 您可以通过过滤器限制在项目列表中屏幕上显示的信息量。 您可以根据对象的特定信息定义特定标准，并仅显示符合这些标准的对象。
author: Nolan
feature: Reports and Dashboards
exl-id: 2e912e32-7924-418d-9d55-ce3c09f67d3e
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '2461'
ht-degree: 1%

---

# 在Adobe Workfront中创建或编辑筛选器

<!--Audited: 12/2023-->

您可以通过过滤器限制在项目列表中屏幕上显示的信息量。 您可以根据对象的特定信息定义特定标准，并仅显示符合这些标准的对象。

您可以在Adobe Workfront中应用以下类型的过滤器：

* 对象列表中的快速过滤器，使用关键字查找项目。 这些是临时过滤器，您无法保存以供将来使用。

  有关快速筛选器的信息，请参阅[将快速筛选器应用到列表](../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md)。

* 永久过滤器，您可以将其保存并在多个列表和报告上多次使用。 本文介绍了如何创建永久过滤器或编辑列表或报告中的现有过滤器。

* Workfront其他区域中的筛选器，列表和报告除外。

  有关Workfront中的所有筛选器以及可应用这些筛选器的区域的列表，请参阅[筛选器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront计划*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront许可证*</strong></td> 
   <td> <p>新文档：参与者或更高版本</p>

或

<p>当前：请求或更高版本</p>

<p><b>注意：</b></p>

要编辑报告中的过滤器，您必须具有以下许可证：

<p>新增：标准</p>

或

<p>当前：计划</p>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <ul><li><p>编辑对筛选器、视图和分组的访问权限</p></li></ul>
    <p><b>注意：</b></p>
   要在报表中编辑筛选器，除了具有筛选器、视图和分组的编辑访问权限之外，还必须具有以下访问级别配置：

<ul><li><p>编辑对报告、功能板和日历的访问权限</p></li></ul>

<p><b>注意：</b></p> <p> 如果您没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>管理筛选器的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

+++

## 过滤器构建界面的类型

您可以使用下表所述的过滤器构建器类型来创建过滤器：

<table style="table-layout:auto">
<col>
<col>
<col>
<tbody>
<tr>
<td><strong>生成器类型</strong></td>
<td><strong>筛选对象</strong></td>
<td><strong>可用时</strong></td>
</tr>
<tr>
<td>标准生成器</td>
<td>
<ul>
<li> <p>项目</p> </li>
<li> <p>任务 </p> </li>
<li> <p>问题</p> </li>
<li> <p>项目组合</p> </li>
<li> <p>项目群</p> </li>
<li> <p>用户</p> </li>
<li> <p>模板</p> </li>
<li> <p>组</p> </li>
</ul>
</td>
<td>
<ul>
<li> <p>列表 </p> </li>
</ul>
<ul>
<li> <p>方案规划器中的项目列表</p> <p>Scenario Planner需要额外的许可证。 有关Workfront Scenario Planner的信息，请参阅<a href="../../../scenario-planner/scenario-planner-overview.md">Scenario Planner概述</a>。 </p> </li>
</ul>
<p><b>注意：</b></p> <p>过滤器的标准生成器不可在报表中使用。
</td>
</tr>
<tr>
<td>旧版生成器</td>
<td>所有对象 </td>
<td>列表和报告</td>
</tr>
</tbody>
</table>

有关Workfront对象的信息，请参阅[了解Adobe Workfront中的对象](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)。

在使用不同界面创建过滤器时，请考虑以下事项：

* 您可以在上面表格中所列区域的旧版过滤器界面所在的相同位置找到标准生成器。
* 标准生成器是所有可用区域的默认体验。 若要切换到旧版筛选器生成器，请单击&#x200B;[!UICONTROL **筛选器**]&#x200B;旁边的&#x200B;**更多**&#x200B;菜单，然后选择&#x200B;[!UICONTROL **返回旧版筛选器**]。

  ![返回旧版筛选器](assets/use-legacy-filters.png)

* 保存的过滤器在两个构建器中均可用，无论您最初使用哪个体验构建它们。 例如，如果使用旧版生成器创建筛选器，则也可以在标准生成器界面中查找并修改该筛选器。

  >[!TIP]
  >
  >“全部”筛选器未包含在标准生成器中，因为未应用筛选器时会显示所有列表项。 单击生成器右上角的&#x200B;[!UICONTROL **全部清除**]&#x200B;可清除所有活动的筛选器并显示所有项目。 如果&#x200B;[!UICONTROL **全部清除**]&#x200B;灰显，则不会应用任何筛选器。

* 在构建组合了AND和OR运算符的多语句过滤器时，标准构建器和旧版构建器的语法略有不同。 因此，当您从一个生成器切换到另一个生成器时，这些筛选器的显示可能会有所不同。

  >[!INFO]
  >
  >存在以下方案：
  >
  >1. 使用标准生成器可创建具有以下语法的过滤器：
  >
  >      `(A OR B) AND C`
  >
  >1. 切换到旧版生成器，并使用旧版生成器的语法编辑筛选器，如本文中[在旧版生成器中创建或编辑筛选器](#create-filter-in-legacy-builder)部分所述。 旧版生成器的语法按以下方式显示filter语句：
  >
  >      `A AND C`
  >      `OR`
  >      `B AND C`
  >
  >1. 更改旧版界面中的筛选器。
  >1. 切换回标准生成器。 过滤器语句根据旧版生成器中支持的逻辑显示，如上所述。
  >
  >      过滤器在标准生成器界面中显示如下：
  >  
  >      `A AND C`
  >      `OR`
  >      `B AND C`
  > 
  >      发生这种情况是因为在旧版界面中修改了过滤器。

## 在标准生成器中创建或编辑过滤器

您可以使用标准生成器界面通过以下方式创建过滤器：

* 从头开始
* 编辑现有筛选器
* 复制现有筛选器
* 复制现有筛选器，编辑现有筛选器并将其另存为新筛选器

使用标准生成器界面创建过滤器：

1. 转到要创建过滤器或包含要自定义的过滤器的列表。
1. 单击&#x200B;**筛选器**&#x200B;图标![筛选器图标](assets/filter-nwepng.png)以打开生成器界面。

   ![标准筛选器生成器](assets/new-filters-all-filter-types.png)

1. 查看以下筛选器列表：

   <table style="table-layout:auto">
   <col>
   <col>
   <tbody>
   <tr>
   <td role="rowheader"><strong>已收藏</strong></td>
   <td>您标记为收藏的过滤器。 当您收藏某个过滤器时，其原始位置将显示在过滤器名称下方，并且除非将其作为收藏删除，否则它将在原始列表中隐藏。</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>已保存</strong></td>
   <td>您自己构建并保存的过滤器。 默认情况下，此列表以最近保存的顺序显示保存的筛选器，但可以拖动筛选器名称手动重新排序列表。</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>系统默认值</strong></td>
   <td>Workfront系统默认筛选器以及Workfront管理员添加到您的筛选器列表中的筛选器，这些筛选器位于系统级别或布局模板中。</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>已与我共享</strong></td>
   <td>其他人创建并与您共享或在系统范围内共享的过滤器。</td>
   </tr>
   </tbody>
   </table>

1. 执行下列操作之一：

   * 单击&#x200B;**新建筛选器**&#x200B;从头开始创建筛选器。
   * 将鼠标悬停在您有权管理的现有筛选器上，然后单击&#x200B;**编辑**&#x200B;图标![编辑图标](assets/edit-icon.png)以进行编辑。

     或

     将鼠标悬停在您有权查看的现有筛选器上，单击&#x200B;**更多**&#x200B;菜单![更多](assets/more-icon-spectrum.png)，然后单击&#x200B;**复制**&#x200B;以复制现有筛选器并编辑副本。

   ![更多菜单选项](assets/new-filters-more-menu-options-with-delete.png)

1. （视情况而定）根据您是要查找与筛选器组中的所有语句或任意语句匹配的对象，从以下选项中选择：

   <table style="table-layout:auto">
   <col>
   <col>
   <tbody>
   <tr>
   <td role="rowheader"><strong>在所有项为 true 时包含</strong></td>
   <td>过滤器找到的对象必须符合过滤器组中的所有过滤器条件。 在这种情况下，filter语句通过AND运算符连接。 这是默认选项。</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>在任意项为 true 时包含</strong></td>
   <td>过滤器找到的对象必须与过滤器组中的任意过滤器条件匹配。 在这种情况下，过滤器语句通过OR运算符连接。</td>
   </tr>
   </tbody>
   </table>

   ![Include if all、any或true下拉菜单](assets/new-filters-all-or-any-are-true-drop-down-menu-nwe.png)

   有关筛选器运算符的详细信息，请参阅[筛选器概述](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

1. 单击字段下拉菜单可查看最近使用的字段以及作为筛选依据的建议字段的列表。 建议的字段当前显示在您正在过滤的列表中。

   您还可以选择&#x200B;**浏览字段**&#x200B;以查看可按其筛选的所有字段的列表。 高级搜索中的字段按对象类别分组。

   ![查找要按其筛选的字段](assets/new-filter-search-for-field.png)

1. 单击修改量下拉菜单以选择修改量。 默认修饰符为“Equals”。

   有关详细信息，请参阅[筛选器和条件修饰符](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)。

   >[!TIP]
   >
   >构建过滤器时，结果会立即显示在列表中。 如果过滤器面板覆盖列表，则可以将其关闭以查看显示内容。 再次打开面板时，输入的信息仍会保留在生成器中。

1. 开始键入要作为筛选依据的字段值。 例如，如果要按`Issue:Name`筛选，则开始键入问题的名称。 选择显示在列表中的值。

   >[!TIP]
   >
   >根据您选择的修改量，您可以选择多个值。

1. 单击&#x200B;**添加筛选器**&#x200B;以选择另一个字段，并将筛选条件添加到筛选器语句中。
1. （可选）单击&#x200B;**删除**&#x200B;图标![删除图标](assets/delete.png)以删除现有的筛选器语句。

   或

   单击&#x200B;**全部清除**&#x200B;可清除所有筛选条件。

1. （可选）单击&#x200B;**添加筛选器组**&#x200B;以添加另一组筛选条件。 集合之间的默认运算符是&#x200B;**和**。 单击运算符以将其更改为&#x200B;**OR**。

   >[!TIP]
   >
   >当您希望组通过过滤器语句中的运算符以外的其他运算符连接时，您可能希望使用另一个过滤器组。

   >[!INFO]
   >
   >当您筛选名称中包含“营销”且未完成且未处于暂停状态的项目时，您可以使用以下多个筛选条件组：
   >`(Project: Name Contains Marketing AND Project: Percent Complete Does not equal 100)`
   >`OR`
   >`(Project: Name Contains Marketing AND Project: Status Does not equal On Hold)`
   >在这种情况下，每个过滤器语句通过AND相连，过滤器组通过OR相连。

1. （可选）单击&#x200B;**文本模式**&#x200B;以继续使用文本模式构建筛选器。

   ![选择文本模式](assets/new-filter-select-text-mode.png)

   此时会打开文本模式界面。

   ![文本模式界面](assets/text-mode-interface-for-beta-filters-nwe.png)

   >[!TIP]
   >
   >我们建议使用标准生成器界面并仅在必须修改仅支持文本模式的筛选器时，使用文本模式来生成尽可能多的筛选器。

   有关使用文本模式界面创建过滤器的详细信息，请参阅[使用文本模式编辑过滤器](/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)。

1. 单击&#x200B;**退出文本模式**&#x200B;以返回标准生成器界面。

   >[!WARNING]
   >
   >标准生成器或旧版界面不支持某些文本模式语句。 创建这些类型的语句后退出文本模式可能会生成警告消息。

1. （可选）单击&#x200B;**应用**&#x200B;以将筛选器应用到列表并查看结果。

   如果过滤器未生成任何结果，则列表为空。

1. 单击&#x200B;**另存为新筛选器**&#x200B;以保存筛选器以供将来使用。

   ![命名并保存筛选器](assets/save-as-untitled-filter-ui-nwe.png)

1. 选择&#x200B;**无标题的筛选器**，然后键入新筛选器的名称。

   >[!TIP]
   >
   >请确保命名该过滤器，以便稍后查找。 如果不命名过滤器，则系统中会将其称为“无标题过滤器”。

1. 从&#x200B;**图标**&#x200B;下拉菜单中选择新筛选器的图标。

   ![为筛选器选择一个图标](assets/new-filter-select-icon.png)

1. （可选）添加过滤器描述以指示其独特之处。 描述显示在筛选器列表中的筛选器名称下。

   >[!TIP]
   >
   >随时单击&#x200B;**取消**&#x200B;将返回过滤器构建区域。

1. 单击&#x200B;**保存**。 该过滤器将保存在“已保存”列表中，并应用于项目列表。
1. （可选）要将筛选器移至“收藏”列表，请将光标悬停在筛选器抽屉中的任意筛选器上，然后单击&#x200B;**收藏**&#x200B;图标![收藏](assets/favorites-icon-small.png)。

   或

   将鼠标悬停在筛选器抽屉中的任意筛选器上，单击“更多”菜单![“更多”菜单](assets/more-icon-spectrum.png)，然后单击“**收藏”**。

1. （可选）单击&#x200B;**栈叠筛选器**&#x200B;按钮以激活栈叠筛选器。 此选项允许您应用多个已保存的过滤器。 筛选规则会按照您选择它们的顺序进行应用。

   >[!TIP]
   >
   >您可以选择的过滤器数量没有限制。
   >
   >选择多个筛选器时，必须同时满足其所有条件才能显示匹配结果。

   ![栈叠筛选器](assets/new-filter-stack-filters.png)

   您选择的过滤器数显示在项目列表顶部的过滤器图标旁边。

   ![选择的筛选器数](assets/number-of-filters-selected.png)

1. （可选）执行以下操作之一：

   * 与其他人共享该过滤器，或使其在系统范围内可用。 有关详细信息，请参阅[共享筛选器、视图或分组](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md)。

   * 如果该过滤器不再有效或重复，请将其删除。 您只能删除自己拥有的过滤器。 您可以删除与您共享的过滤器。 有关信息，请参阅[删除筛选器、视图和分组](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md)。

## 在旧版生成器中创建或编辑筛选器 {#create-filter-in-legacy-builder}

您可以通过以下方式在列表和报表中创建旧版过滤器：

* 从头开始
* 编辑现有筛选器并将其另存为新筛选器

无论使用何种方法创建过滤器，从头开始或从现有过滤器创建过滤器都是类似的。

1. 转到包含要自定义的过滤器的列表或报表。
1. 单击&#x200B;**筛选器**&#x200B;图标![筛选器图标](assets/filter-nwepng.png)。

   >[!TIP]
   >
   >报告创建者必须允许编辑过滤器，才能在报告中查看过滤器下拉列表。 默认情况下，“报表默认”筛选器应用于报表。 仅当您编辑报告时，才能自定义报告默认筛选条件。

   ![筛选器下拉列表](assets/filter-drop-down-expanded-nwe.png)

1. 单击筛选器列表顶部的&#x200B;**新建筛选器**。

   或

   将鼠标悬停在要修改的筛选器上，然后单击&#x200B;**编辑**&#x200B;图标![](assets/edit-icon.png)。

   用于自定义筛选器的生成器启动项。

1. 执行以下任一操作：

   * 通过单击现有规则并选择新选项来修改现有筛选器规则。
   * 通过单击&#x200B;**添加其他筛选器规则**&#x200B;来添加筛选器规则，在&#x200B;**开始键入字段名称**&#x200B;框中开始键入要为其添加规则的选项的名称，然后当它出现在下拉列表中时单击它。

     与筛选器对象关联的字段列在&#x200B;**开始键入字段名称**&#x200B;框中。

   * 添加筛选规则时，单击&#x200B;**AND**&#x200B;或&#x200B;**OR**。\
     添加过滤器规则时，使用过滤器修饰符建立过滤器的条件。 有关筛选器修饰符的详细信息，请参阅[筛选器和条件修饰符](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)。

     >[!NOTE]
     >
     >当通过多个OR语句连接一组AND语句时，必须为每个语句组重复在OR语句之间没有更改的字段。
     >
     >![连接的筛选器语句](assets/filters-and-statements-connected-by-or-statements-builder-ui-old-filters-2022.png)
     >
     >在为包含“营销”一词、且处于当前或Planning状态的项目中的任务构建过滤器时，您必须具有以下过滤器规则：
     >
     >`Task: Name Contains Marketing`
     >`AND`
     >`Project: Status Equals Current`
     >`OR`
     >`Task: Name Contains Marketing`
     >`AND`
     >`Project: Status Equals Planning`
     >
     >虽然任务：名称包含“营销”在两个AND过滤器组之间不会发生更改，但在第二个过滤器中必须重复该名称。

   * 单击“X”图标可删除现有筛选规则。

1. （可选）单击&#x200B;**切换到文本模式**&#x200B;以使用文本模式界面添加筛选器。

   有关使用文本模式界面创建过滤器的详细信息，请参阅[使用文本模式编辑过滤器](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)。

1. 单击&#x200B;**保存筛选器**&#x200B;以创建筛选器或使用您的更改替换选定的筛选器。

   或

   单击&#x200B;**另存为新筛选器**&#x200B;以从选定筛选器创建筛选器。

   新筛选器将显示在筛选器列表中，并且会自动应用于您选择的列表或报表。

1. （可选）执行以下操作之一：

   * 将您创建的过滤器与其他用户共享，或使其在系统范围内可用。 有关信息，请参阅[共享筛选器、视图或分组](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md)。
   * 删除您不再希望在列表中显示的过滤器。 有关信息，请参阅[删除筛选器、视图和分组](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md)。


