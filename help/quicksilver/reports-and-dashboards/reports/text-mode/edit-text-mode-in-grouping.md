---
product-area: reporting
navigation-topic: text-mode-reporting
title: 在分组中编辑文本模式
description: ‘注意：使所有FVG文章都相同，以便在文本模式下进行编辑)`
author: Nolan
feature: Reports and Dashboards
exl-id: 2eeecc16-ea6d-4a56-8ea3-e213706e89bf
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1559'
ht-degree: 1%

---

# 在分组中编辑文本模式

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: make all FVG articles the same for editing in text mode)</p>
-->

您可以使用文本模式在列表或报表中编辑分组，以访问标准界面中不可用的字段，并创建更复杂的分组。

>[!TIP]
>
>我们建议您在标准模式下尽可能多地构建分组，然后将其转换为文本模式以对其进行编辑。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对过滤器、视图、分组的访问权限</p> <p>编辑对报表、功能板、日历的访问权限，以编辑报表中的分组</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限以编辑报表中的分组</p> <p>管理分组的权限以对其进行编辑</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

开始在报表或列表中使用文本模式之前，请始终确保您熟悉Workfront文本模式语法。

有关更多信息，请参阅：

* [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [文本模式语法概述](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [自定义视图、过滤器和分组示例](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## 在分组中编辑文本模式

对于报表和列表，使用文本模式编辑分组的方式相同。 从报表或列表访问分组的方式有所不同。

>[!NOTE]
>
>分组是在报表中创建图表的必备报表元素。 图表不支持文本模式分组。 有关将图表添加到报表的信息，请参阅 [将图表添加到报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

有关构建分组的更多信息，请参阅 [在Adobe Workfront中创建分组](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

有关创建报表的信息，请参阅 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 执行下列操作之一：

   1. 要从报表访问分组，请转到报表，然后单击 **报表操作** > **编辑** > **分组** 选项卡。
   1. 要从列表访问分组，请转到列表，然后从 **分组** 下拉菜单中，将鼠标悬停在要修改的分组上，然后单击 **编辑** 图标 ![](assets/edit-icon.png).

      将打开分组生成器。

1. 单击 **添加分组** 要添加分组，请单击 **切换到文本模式** 中。

   >[!TIP]
   您可以在标准界面中最多添加3个分组。 您只能使用文本模式添加第4个分组，并且Workfront中的分组级别不能超过4个。

1. 开始键入要按其分组的字段名称。

   当您在列表中看到字段时，选择该字段的名称。

1. 单击 **切换到文本模式** 中。

   然后，将以文本模式显示分组。

   在文本模式下编辑分组时，Workfront会将

   ```
   textmode=true
   ```

   代码行到分组。 这表示在文本模式下修改了分组。

   **示例：** 要按项目名称，然后按主要被分派人的名称对任务列表进行分组，在文本模式下，分组应如下所示。

   ```
   textmode=true<br>group.0.linkedname=project<br>group.0.namekey=view.relatedcolumn<br><strong>group.0.valuefield=project:name</strong><br>group.0.namekeyargkey.0=project<br>group.0.namekeyargkey.1=name<br><strong>group.0.valueformat=string</strong><br>group.1.linkedname=assignedTo<br>group.1.namekey=view.relatedcolumn<br><strong>group.1.valuefield=assignedTo:name</strong><br>group.1.namekeyargkey.0=assignedTo<br>group.1.namekeyargkey.1=name<br><strong>group.1.valueformat=string</strong>
   ```

   >[!IMPORTANT]
   粗体行是必填的。

   <!--
   <div class="example" data-mc-autonum="<b>Example: </b>" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <span class="autonumber"><span><b>Example: </b></span></span>
   <p>To group a list of tasks by the Project Name and then by the name of the Primary Assignee, your grouping should look like the following, in text mode:</p>
   <p><code>textmode=true</code> </p>
   <p><code>group.0.linkedname=project</code> </p>
   <p><code>group.0.namekey=view.relatedcolumn</code> </p>
   <p><code style="font-weight: bold;">group.0.valuefield=project:name</code> </p>
   <p><code>group.0.namekeyargkey.0=project</code> </p>
   <p><code>group.0.namekeyargkey.1=name</code> </p>
   <p><code style="font-weight: bold;">group.0.valueformat=string</code> </p>
   <p><code>group.1.linkedname=assignedTo</code> </p>
   <p><code>group.1.namekey=view.relatedcolumn</code> </p>
   <p><code style="font-weight: bold;">group.1.valuefield=assignedTo:name</code> </p>
   <p><code>group.1.namekeyargkey.0=assignedTo</code> </p>
   <p><code>group.1.namekeyargkey.1=nam</code>e</p>
   <p><code style="font-weight: bold;">group.1.valueformat=string</code> </p> <note type="important">
   The lines in bold are mandatory.
   </note>
   </div>
   -->

   分组中的每个字段都有若干行引用该字段的代码。

   下表概述了文本模式分组中的关键行。

   <!--
   <div data-mc-conditions="QuicksilverOrClassic.Draft mode">
   <p>(NOTE: Should I add the group.1. information to this table and break the snippet? If yes, delete the snippet)</p>
   <p>(NOTE: this is a snippet, same as view >> same fields >>> see the steps in creating a view and add the same steps here for making a grouping)</p>
   </div>
   -->

   >[!TIP]
   文本模式分组中的键行与构建文本模式视图所需的行类似。

   <!--
   <note type="tip">  
   <p>The key lines in a text mode grouping are similar to the lines required to build text-mode views.</p>
   </note>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th><strong>示例行</strong> </th> 
      <th><strong>描述</strong> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td><strong>组.&lt;number&gt;.</strong> </td> 
      <td> <p>每行代码前面都有此文本。 引用在分组中选择的相同字段的代码行将使用相同的编号进行编号，如下所示：</p> 
       <ul> 
        <li>报表的第一组的组编号为0。 引用第一个分组的所有行均以 <code>group.0</code>.</li> 
        <li>报表的第二组的组编号为1。 引用第二个分组的所有行均以 <em><code>group.1</code></em>.</li> 
        <li>报表的第三组的组编号为2。 引用第三个分组的所有行均以 <em><code>group.2</code></em>.</li> 
        <li>只有在文本模式下，才能为第四个分组添加组编号3。 引用第四个分组的所有行均以 <em><code>group.3</code></em>.</li> 
       </ul> <p>注意：生成器不支持4个分组。 仅在使用文本模式时才支持这些键值。 Workfront不支持超过4个级别的分组。</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valuefield</strong>=</p> </td> 
      <td> <p>这是对象或字段在数据库中显示的名称。 有关对象和字段在数据库中的显示方式的详细信息，请参阅 <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> <p>存在以下情形：</p> 
       <ol> 
        <li value="1"> <p> 如果显示的字段名称是短语而不是单个名词，则必须对 <code>valuefield</code>. 例如，对于任务的计划起始日期，代码为：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例: </b></span></span><code>group.0.valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>如果要显示自定义字段，请 <code>valuefield</code> value是字段的实际名称，如您在界面中看到的。 例如，对于名为“More information”的自定义字段，代码为：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例: </b></span></span><code>group.0.valuefield=More information</code> </p> </li> 
        <li value="3"> <p>如果要按与其他对象相关的对象(使用 <code>valuefield</code> 代码行对象名称和属性以冒号分隔。</p> <p>例如，按Portfolio名称对任务列表进行分组，其值字段行的值如下所示：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例: </b></span></span><code>group.0.valuefield=project:portfolio:name</code> </p> <p>这表示从报表（任务）的对象中，可以访问下一个相关对象（项目）；在此，您可以从项目（项目组合）中访问以下相关对象；然后是组合名称（名称）。</p> </li> 
       </ol> <p>有关对象如何彼此连接的信息，请参阅部分 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">对象的相互依赖和层次结构</a> in <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">了解Adobe Workfront中的对象</a>.</p> <p>注意：如果在文本模式下选择的字段在标准界面中无效，并切换到标准界面，则会删除分组。</p> </td> 
     </tr> 
     <tr> 
      <td><strong>valueformat=</strong> </td> 
      <td> <p>此行表示用于显示 <code>valuefield</code>. 的 <code>valueformat</code> 标识对象或字段是显示为文本、数字、百分比还是日期。</p> <p>我们建议使用 <code>HTML</code> , <code>valueformat</code>，尤其是在使用 <code>valueexpression</code>，以确保最准确地显示您的信息。</p> <p>有关此行的其他值的信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">在文本模式中使用条件格式</a>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valueexpression=</strong> </p> </td> 
      <td> <p>您可以添加此行以替换 <code>valuefield</code>，以按多个字段之间的计算对列表进行分组。</p> <p>您必须将 <code>valuefield</code> 在 <code>valueexpression</code>.</p> <p>存在以下情形：</p> 
       <ol> 
        <li value="1"> <p>如果要以大写形式显示分组的名称，应使用：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例: </b></span></span><code>group.0.valueexpression=UPPER({valuefield})</code> </p> <p>的 <code>valuefield</code> 对象的拼写形式与在API资源管理器中显示的对象一样。</p> </li> 
        <li value="2">如果要添加多个 <code>valuefields</code> 把他们绑在一起 <code>valueexpression </code>行，必须按句点分隔。<p>例如，如果要在任务列表中以大写显示组合的名称，则可以在 <code>valueexpression</code> 行：</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例: </b></span></span><code>group.0.valueexpression=UPPER({project}.{portfolio}.{name})</code></p><p>如果要在 <code>valueexpression</code> 行，您必须在字段名称之前 <code>DE:</code> 来指示它是自定义字段。 字段名称在界面中显示时拼写。</p><p>重要信息： <span>当您使用放置在自定义表单部分中的自定义字段（该字段对某些用户的权限有限）时， <code>valueexpression </code>当这些用户在报表中查看此计算时，为空。 有关调整自定义表单部分权限的信息，请参阅</span> <span href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">创建或编辑自定义表单</a></span>.</p><p>例如，如果您有一个标有“开发人员名称”的自定义字段，并且您希望按此字段分组并以大写形式显示它，则可以使用以下内容 <code>valueexpression</code> 以指示：</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例: </b></span></span><code>group.0.valueexpression=UPPER({DE:Developer Name}</code>)</p><p>引用Typeahead类型自定义字段时，请使用以下表达式引用在标记为“开发人员名称”的字段中选择的对象的名称：</p><p><code>valueexpression=UPPER({DE:Developer Name:name})</code></p></li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td><strong>namekey= / name=</strong> </td> 
      <td> <p>此行定义分组标签。 在这种情况下，它使用基于键的缩写值。</p> <p>如果要修改分组名称，可将此值更改为：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例: </b></span></span><code>group.0.name=Your Value</code> </p> <p><code>Name</code> 允许您为分组名称输入任何文本，而 <code>namekey</code> 需要输入用于转换分组名称的键。</p> <p>要更改分组名称，您还可以添加 <code>displayname </code>行，如果没有。</p> </td> 
     </tr> 
     <tr> 
      <td><strong>displayname =</strong> </td> 
      <td> <p>您可以添加以下行来更改列的名称，该名称将覆盖 <code>namekey/name</code> 值：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例: </b></span></span><code>group.0.displayname=Your Value</code> </p> <p>我们建议删除包含 <code>name </code>重命名分组时。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可选）将以下代码行之一添加到任何分组，以指示分组中的结果是否应显示在展开或折叠的列表中。 默认情况下，分组显示会展开：


   ```
   group.0.iscollapsed=true
   ```

   如果希望在显示分组时折叠结果

   ```
   group.0.iscollapsed=false
   ```

   如果希望显示分组并展开结果

   <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Common uses of text mode, Edit groupings to organize reports, Create a Custom Report) </p>   
     -->

   >[!TIP]
   * 当您在查看列表时手动调整分组时，Workfront会在您注销之前记住您的手动首选项。 当您重新登录时，将根据此设置显示列表。
   * 从图表元素访问分组结果后，分组结果始终会显示为已展开。


1. 单击 **完成** 如果要保存更改并继续编辑分组或报表，请执行以下操作：
1. 单击 **保存分组** 列表或 **保存并关闭** 保存报表。
