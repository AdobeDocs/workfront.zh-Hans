---
product-area: reporting
navigation-topic: text-mode-reporting
title: 编辑分组中的文本模式
description: '注意：使所有FVG文章在文本模式下编辑时相同)'
author: Nolan
feature: Reports and Dashboards
exl-id: 2eeecc16-ea6d-4a56-8ea3-e213706e89bf
source-git-commit: dad054fe52bd7c5ca97144567c80e6d340541a50
workflow-type: tm+mt
source-wordcount: '1569'
ht-degree: 0%

---

# 编辑分组中的文本模式

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: make all FVG articles the same for editing in text mode)</p>
-->

您可以使用文本模式编辑列表或报表中的分组，以访问标准界面中不可用的字段，并创建更复杂的分组。

>[!TIP]
>
>我们建议您在标准模式下构建尽可能多的分组，然后将其转换为文本模式以进行编辑。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对筛选器、视图、分组的访问权限</p> <p>编辑对报告、功能板和日历的访问权限以编辑报告中的分组</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报告的权限以编辑报告中的分组</p> <p>管理群组权限以对其进行编辑</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 先决条件

在报表或列表中开始使用文本模式之前，请始终确保您熟悉Workfront文本模式语法。

有关更多信息，请参阅：

* [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [文本模式语法概述](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [自定义视图、筛选器和分组示例：文章索引](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## 编辑分组中的文本模式

使用文本模式编辑分组对于报告和列表是相同的。 从报表或列表访问分组的方式有所不同。

>[!NOTE]
>
>分组是在报表中创建图表的必需报表元素。 图表不支持文本模式分组。 有关将图表添加到报表的信息，请参阅[将图表添加到报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)。

有关生成分组的详细信息，请参阅[在Adobe Workfront中创建分组](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)。

有关创建报告的信息，请参阅[创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

1. 执行下列操作之一：

   1. 若要从报表访问分组，请转到该报表，然后单击&#x200B;**报表操作** > **编辑** > **分组**&#x200B;选项卡。
   1. 要从列表中访问分组，请转到该列表，然后从&#x200B;**分组**&#x200B;下拉菜单中，将鼠标悬停在要修改的分组上，然后单击&#x200B;**编辑**&#x200B;图标![](assets/edit-icon.png)。

      此时将打开分组生成器。

1. 单击&#x200B;**添加分组**&#x200B;以添加分组，然后单击生成器右上角的&#x200B;**切换到文本模式**。

   >[!TIP]
   >
   >在标准界面中最多可添加3个分组。 您只能使用文本模式添加第4个分组，并且Workfront中的分组级别不能超过4个。

1. 开始键入要作为分组依据的字段的名称。

   在列表中看到字段时，选择字段的名称。

1. 单击生成器右上角的&#x200B;**切换到文本模式**。

   然后，分组将以文本模式显示。

   在文本模式下编辑分组时，Workfront会添加

   ```
   textmode=true
   ```

   分组代码行。 这表示在文本模式下修改了分组。

   **示例：**&#x200B;要按项目名称再按主要被分配人的名称对任务列表进行分组，在文本模式下，您的分组应该如下所示。

   ```
   textmode=true<br>group.0.linkedname=project<br>group.0.namekey=view.relatedcolumn<br><strong>group.0.valuefield=project:name</strong><br>group.0.namekeyargkey.0=project<br>group.0.namekeyargkey.1=name<br><strong>group.0.valueformat=string</strong><br>group.1.linkedname=assignedTo<br>group.1.namekey=view.relatedcolumn<br><strong>group.1.valuefield=assignedTo:name</strong><br>group.1.namekeyargkey.0=assignedTo<br>group.1.namekeyargkey.1=name<br><strong>group.1.valueformat=string</strong>
   ```

   >[!IMPORTANT]
   >
   >粗体中的行是必填的。

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

   分组中的每个字段都有几行引用该字段的代码。

   下表概述了文本模式分组中的关键行。

   <!--
   <div data-mc-conditions="QuicksilverOrClassic.Draft mode">
   <p>(NOTE: Should I add the group.1. information to this table and break the snippet? If yes, delete the snippet)</p>
   <p>(NOTE: this is a snippet, same as view >> same fields >>> see the steps in creating a view and add the same steps here for making a grouping)</p>
   </div>
   -->

   >[!TIP]
   >
   >文本模式分组中的关键行与构建文本模式视图所需的行类似。

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
      <td><strong>组。&lt;数字&gt;.</strong> </td> 
      <td> <p>每行代码前面都带有此文本。 引用分组中所选相同字段的代码行使用相同的编号进行编号，如下所示：</p> 
       <ul> 
        <li>报表的第一个分组的组号为0。 引用第一个分组的所有行均以<code>group.0</code>开头。</li> 
        <li>报表的第二个分组的组号为1。 引用第二个分组的所有行均以<em><code>group.1</code></em>开头。</li> 
        <li>报表的第三个分组的组数为2。 引用第三个分组的所有行均以<em><code>group.2</code></em>开头。</li> 
        <li>仅在文本模式下，可以为第四个分组添加组号3。 引用第四组的所有行均以<em><code>group.3</code></em>开头。</li> 
       </ul> <p>注意：生成器不支持4个分组。 仅当使用文本模式时，才支持使用文本模式。 Workfront不支持超过4个级别的分组。</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valuefield</strong>=</p> </td> 
      <td> <p>这是对象或字段在数据库中显示的名称。 有关对象和字段如何在数据库中显示的详细信息，请参阅<a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API资源管理器</a>。</p> <p>存在以下情况：</p> 
       <ol> 
        <li value="1"> <p> 如果显示的字段名称是短语而不是单个名词，则必须使用<code>valuefield</code>的驼峰式大小写语法。 例如，对于任务的计划开始日期，代码为：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span><code>group.0.valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>如果要显示自定义字段，则<code>valuefield</code>值是字段的实际名称，如您在界面中所见。 例如，对于名为“更多信息”的自定义字段，代码为：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span><code>group.0.valuefield=More information</code> </p> </li> 
        <li value="3"> <p>如果要按使用<code>valuefield</code>行代码与其他对象相关的对象进行分组，则对象名称和属性用冒号分隔。</p> <p>例如，按Portfolio名称对任务列表进行分组时，valuefield行具有以下值：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span><code>group.0.valuefield=project:portfolio:name</code> </p> <p>这表示您可以从报表（任务）的对象访问下一个相关对象（项目）；从那里，您可以从项目（项目组合）访问以下相关对象；然后访问项目组合名称（名称）。</p> </li> 
       </ol> <p>有关对象如何相互连接的信息，请参阅<a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">了解Adobe Workfront中的对象</a>中的<a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">对象相互依赖性和层次结构</a>部分。</p> <p>注：如果在文本模式下选择的字段在标准界面中无效，并且切换到标准界面，则会删除该分组。</p> </td> 
     </tr> 
     <tr> 
      <td><strong>valueformat=</strong> </td> 
      <td> <p>此行表示用于显示<code>valuefield</code>的格式。 <code>valueformat</code>标识对象或字段是显示为文本、数字、百分比还是日期。</p> <p>我们建议对您的<code>valueformat</code>使用<code>HTML</code>，特别是在使用<code>valueexpression</code>时，以确保最准确地显示您的信息。</p> <p>有关此行的其他值的信息，请参阅<a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">在文本模式下使用条件格式</a>。</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valueexpression=</strong> </p> </td> 
      <td> <p>如果要按多个字段之间的计算对列表进行分组，可添加此行以替换<code>valuefield</code>。</p> <p>每次在<code>valueexpression</code>中使用对象时，必须将对象的<code>valuefield</code>括在大括号中。</p> <p>存在以下情况：</p> 
       <ol> 
        <li value="1"> <p>如果要以大写形式显示分组的名称，您可以使用：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span><code>group.0.valueexpression=UPPER({valuefield})</code> </p> <p>对象的<code>valuefield</code>在API Explorer中显示时拼写。</p> </li> 
        <li value="2">如果要通过在<code>valueexpression </code>行中将多个<code>valuefields</code>字符串在一起来添加它们，则必须用句点分隔它们。<p>例如，如果要在任务列表中以大写显示项目组合的名称，可在<code>valueexpression</code>行中使用以下代码：</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span><code>group.0.valueexpression=UPPER({project}.{portfolio}.{name})</code></p><p>如果要在<code>valueexpression</code>行中使用自定义字段，则必须在字段名称前面加上<code>DE:</code>，以指示它是自定义字段。 字段的名称在界面中显示时拼写。</p><p>重要提示： <span>如果您使用的自定义字段位于对某些用户具有限制权限的自定义表单分区中，则当这些用户在报表中查看此计算时，<code>valueexpression </code>的计算为空白。 有关调整自定义表单分区权限的信息，请参阅</span> <span href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">创建或编辑自定义表单</a></span>。</p><p>例如，如果您有一个标记为“开发人员姓名”的自定义字段，并且您想按此字段分组并以大写显示，则可以使用以下<code>valueexpression</code>来指示这一点：</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span><code>group.0.valueexpression=UPPER({DE:Developer Name}</code>)</p><p>在引用“预输入”类型自定义字段时，使用以下表达式来引用在标记为“开发人员名称”的字段中选择的对象的名称：</p><p><code>valueexpression=UPPER({DE:Developer Name:name})</code></p></li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td><strong>namekey= / name=</strong> </td> 
      <td> <p>此行定义分组标签。 在此例中，它使用基于键的缩写值。</p> <p>如果要修改分组名称，可将此值更改为以下值：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span><code>group.0.name=Your Value</code> </p> <p><code>Name</code> 允许您为分组名称输入任何文本，而<code>namekey</code>要求您输入用于翻译分组名称的键。</p> <p>要更改分组名称，您还可以添加<code>displayname </code>行（如果没有）。</p> </td> 
     </tr> 
     <tr> 
      <td><strong>displayname =</strong> </td> 
      <td> <p>您可以添加以下行来更改覆盖<code>namekey/name</code>值的列的名称：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span><code>group.0.displayname=Your Value</code> </p> <p>当您重命名分组时，我们建议删除所有包含<code>name </code>的行。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可选）将以下一行代码添加到任何分组中，以指示分组中的结果应显示在展开列表还是折叠列表中。 默认情况下，分组显示为展开状态：


   ```
   group.0.iscollapsed=true
   ```

   如果希望显示分组并折叠结果

   ```
   group.0.iscollapsed=false
   ```

   如果希望显示分组并展开结果

   <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Common uses of text mode, Edit groupings to organize reports, Create a Custom Report) </p>   
     -->

   >[!TIP]
   >   
   >* 当您在查看列表时手动调整分组时，Workfront会记住您的手动首选项，直到您注销。 重新登录时，将根据此设置显示列表。
   >* 从图表元素访问分组结果后，这些结果始终以展开形式显示。

1. 如果要保存更改并继续编辑分组或报告，请单击&#x200B;**完成**。
1. 单击列表中的&#x200B;**保存分组**&#x200B;或&#x200B;**保存+关闭**&#x200B;以保存报告。
