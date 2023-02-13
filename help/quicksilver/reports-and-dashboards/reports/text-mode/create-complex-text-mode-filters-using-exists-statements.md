---
product-area: reporting
navigation-topic: text-mode-reporting
title: 使用EXISTS语句创建复杂的文本模式筛选器
description: 使用EXISTS语句创建复杂的文本模式筛选器
author: Nolan
feature: Reports and Dashboards
exl-id: 106f7c9d-46cc-46c5-ae34-93fd13a36c14
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '2803'
ht-degree: 0%

---

# 使用EXISTS语句创建复杂的文本模式筛选器

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: do not EVER&nbsp;delete this article as long as Text Mode still exists in the system.&nbsp;Google ordered this article to be written and we wrote it with the help of consultants, so the use case is very complex and very hard to understand without this. It is also very much used by many customers)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;Alina: **~ Replace screen shot of icons when list/ reporting UI changes)</p>
-->

>[!IMPORTANT]
>
>本文要求您对Adobe Workfront API和文本模式报告界面有透彻的了解。 有关Workfront API的信息，请参阅 [API基础知识](../../../wf-api/general/api-basics.md).\
>有关使用文本模式的信息，请参阅 [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Workfront中的对象关系概述

所有对象都链接到Workfront数据库中的其他对象。

了解对象的层次结构和相互依赖关系有助于您了解哪些对象可以在报表中引用。

有关Workfront中对象及其层次结构和相互依赖关系的信息，请参阅 [了解Adobe Workfront中的对象](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

在构建过滤器时，您可以使用标准报告界面引用最多2个级别的关系中连接到过滤器对象的其他对象。

例如，您可以在问题筛选器中引用PortfolioID，以使用标准界面仅显示与特定项目组合关联的项目中的问题。 在这种情况下，资产组合距离问题有2个级别。

但是，您不能使用标准界面在问题筛选器中引用“Portfolio所有者”，以仅显示与所有者是特定用户的项目关联的问题。 您必须使用文本模式来访问Portfolio所有者名称字段，该字段距离问题有三个级别。

![issue_to_portfolio_owner_sraight_line_icons.PNG](assets/issue-to-portfolio-owner-sraight-line-icons-350x83.png)

有关Workfront中对象的完整列表，请参阅 [API Explorer](../../../wf-api/general/api-explorer.md).

有关如何导航API资源管理器和查找对象的信息，请参阅 [使用API资源管理器](../../../wf-api/general/using-api-explorer.md).

构建过滤器时，必须在文本模式界面中构建复杂语句以引用这些类型的对象。

有关构建复杂过滤器的信息，请参阅 [使用EXISTS语句的复杂文本模式过滤器概述](#overview-of-complex-text-mode-filters-that-use-exists-statements) 中。

## 使用EXISTS语句的复杂文本模式过滤器概述 {#overview-of-complex-text-mode-filters-that-use-exists-statements}

在对象层次结构中创建跨多个级别的过滤器或筛选缺少的对象时，请考虑以下事项：

* 如果要引用未直接连接到过滤器对象的对象，则必须创建复杂的过滤器。
* 必须使用EXISTS语句来执行以下操作：

   * 创建跨多个级别的过滤器。
   * 创建过滤器以查找缺少的对象。\
      例如，在生成用户报表时，您可以过滤某些时间段内未记录时间的用户。

在过滤器中使用EXISTS语句时，请考虑以下规则：

* 在EXISTS筛选器中可以引用三个对象：

   * 筛选器的对象（原始对象）。
   * 要引用其字段的对象（目标对象）。
   * 连接“原始”(Original)和“目标”(Target)对象（如果它们之间没有直接连接）的对象(“链接”(Linking)对象)。

* 使用EXISTS的过滤器包含两个以等号链接的单独语句：

   * 等号前的语句引用您引用的对象（链接对象或目标对象）。
   * 等号后的语句引用您引用的对象（原始对象）。

* 必须使用链接对象的对象代码来连接语句。\
   您可以在API资源管理器中找到所有对象的对象代码。\
   有关API资源管理器的信息，请参阅 [API Explorer](https://one.workfront.com/s/api-explorer).

* 如果由于原始对象与目标对象直接连接而缺少链接对象，则可以使用目标对象的对象代码而不是链接对象。
* 您可以在同一对象（目标对象）上引用多个字段（目标字段），在这种情况下，必须通过AND连接引用字段的行。\
   有关筛选属于目标对象的多个字段的示例，请参阅 [示例4:按多个字段过滤：按Portfolio所有者名称和Portfolio协调记分卡ID列出的任务](#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id) 章节。

* EXISTS语句支持的唯一修饰符是NOTEXISTS。

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
   <td> <p>编辑对过滤器、视图、分组的访问权限</p> <p>编辑对报表、功能板、日历的访问权限，以编辑报表中的过滤器</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限以编辑报表中的过滤器</p> <p>管理过滤器的权限以对其进行编辑</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 创建对象层次结构中跨多个级别的复杂文本模式过滤器

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***[This information is somewhat duplicated from the section below: Create Text-Mode Filters for Missing Objects])</p>
-->

您可以构建一个过滤器，该过滤器在存在过滤器对象的对象层次结构的多个级别中引用对象。 例如，您可以针对与特定Portfolio所有者无关联的项目中的问题构建问题过滤器。

必须始终使用EXISTS语句和文本模式界面来构建此过滤器。

有关过滤器的示例，请参阅 [示例1:按Portfolio所有者名称过滤问题](#example-1-filter-for-issues-by-portfolio-owner-name) 章节。

要创建跨对象层次结构中多个级别的过滤器，请执行以下操作：

1. 识别过滤器的对象。 我们将此对象称为“原始对象”(Original Object)。\
   例如，问题。
1. 识别要过滤的字段。 我们将此对象称为属于目标对象的目标字段。\
   例如，所有者ID字段（目标字段），它属于Portfolio（目标对象）。
1. （视情况而定）如果原始对象（问题）和目标字段(ownerID)未直接连接，则必须找到第三个对象，即连接它们的链接对象（项目）。 链接对象必须至少有一个字段，该字段是从原始对象的“字段”或“引用”选项卡引用的（在原始对象上显示的链接字段），并且该字段还必须有一个链接字段，该字段显示在链接对象的“字段”或“引用”选项卡中。 链接字段必须与目标字段匹配，该字段显示在链接对象上（或链接对象上显示的链接字段）。\
   例如，（项目）ID（原始对象上显示的链接字段）是从问题（原始对象）中引用的。 (Portfolio)ownerID（将字段链接到目标对象）显示在项目（关联对象）的字段选项卡中。 PortfolioownerID也是目标对象(Portfolio)上的字段。 链接对象上的链接字段与目标字段匹配。\
   ![portfolio_id_in_the_project_api_object.PNG](assets/portfolio-id-in-the-project-api-object-350x88.png)

1. 使用API资源管理器，识别 **对象代码** 链接对象（项目）的子目录访问Advertising Cloud帮助。\
   例如，项目的对象代码为PROJ。\
   ![project_objCode_in_the_API.PNG](assets/project-objcode-in-the-api-350x84.png)

1. 为原始对象创建过滤器。\
   例如，创建问题过滤器。\
   有关创建过滤器的信息，请参阅 [过滤器Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. 单击 **切换到文本模式**.
1. 将以下公式示例粘贴到新筛选器的文本模式界面中，并将建议的文本替换为正确的对象和字段：

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object>
   EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object>
   EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field>
   ```

   有关使用我们上面标识的字段的示例，请参阅 [示例1:按Portfolio所有者名称过滤问题](#example-1-filter-for-issues-by-portfolio-owner-name) 章节。

1. 单击 **保存过滤器**.

## 为缺少的对象创建复杂的文本模式筛选器

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: **^[This information is somewhat duplicated from the section above: Create Text-Mode Filters that Span Multiple Levels in the Object Hierarchy])</p>
-->

您可以构建引用缺失对象的过滤器。 例如，您可以构建一个用户过滤器，以显示哪些用户未在Workfront中记录小时。

您必须始终使用 *存在* 语句和用于构建此过滤器的文本模式界面。

有关缺少对象的过滤器示例，请参阅本文的以下部分：

* [示例2:筛选缺少的对象：任何自定义表单中未显示的自定义字段](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms)
* [示例3:筛选缺少的对象：某个时间段内未记录时间的用户](#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time)

要创建引用缺少对象的过滤器，请执行以下操作：

1. 识别过滤器的对象。 我们将此对象称为“原始对象”(Original Object)。\
   例如，“参数”或“自定义字段”。
1. 识别要过滤的字段。 我们将此对象称为属于目标对象的目标字段。\
   例如，类别ID字段（目标字段）属于类别（目标对象）。
1. 由于原始对象（参数）和目标字段(categoryID)之间没有直接连接，因此您必须找到第三个对象，即链接对象（类别参数），用于连接它们。 链接对象必须至少有一个字段，该字段是从原始对象的“字段”或“引用”选项卡引用的（在原始对象上显示的链接字段），并且该字段还必须有一个链接字段，该字段显示在链接对象的“字段”或“引用”选项卡中。 链接字段必须与目标字段匹配，该字段显示在链接对象上（或链接对象上显示的链接字段）。\
   例如，类别参数（在原始对象上显示的链接字段）的ID是从参数（原始对象）中引用的。 参数ID（链接字段到目标对象）显示在类别参数（链接对象）的“字段”选项卡中。 链接对象上显示的链接字段与目标字段匹配。
1. 使用API资源管理器，识别 **对象代码** 链接对象（类别参数）的URL。\
   例如，类别参数的对象代码为CTGYPA。\
   ![category_parameter_objcode_in_api.PNG](assets/category-parameter-objcode-in-api-350x79.png)

1. 为原始对象创建过滤器。\
   例如，创建一个参数过滤器。\
   有关创建过滤器的信息，请参阅 [过滤器Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. 单击 **切换到文本模式**.
1. （视情况而定）如果要筛选缺少的对象，请将以下公式示例粘贴到新筛选器的文本模式界面中，并将建议的文本替换为正确的对象和字段：

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

   有关与自定义Forms无关联的自定义字段的报告示例，请参阅 [示例2:筛选缺少的对象：任何自定义表单中未显示的自定义字段](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms) 章节。

1. 单击 **保存过滤器**.

## 跨对象层次结构中多个级别的文本模式过滤器示例

* [示例1:按Portfolio所有者名称过滤问题](#example-1-filter-for-issues-by-portfolio-owner-name)
* [示例2:筛选缺少的对象：任何自定义表单中未显示的自定义字段](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms)
* [示例3:筛选缺少的对象：某个时间段内未记录时间的用户](#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time)
* [示例4:按多个字段过滤：按Portfolio所有者名称和Portfolio协调记分卡ID列出的任务](#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id)

### 示例1:按Portfolio所有者名称过滤问题 {#example-1-filter-for-issues-by-portfolio-owner-name}

使用文本模式界面，您可以构建问题列表的过滤器，以便仅显示与所有者是特定用户的项目关联的项目上的问题。

要按Portfolio所有者名称过滤问题，请执行以下操作：

1. 创建问题过滤器。\
   有关创建过滤器的信息，请参阅 [过滤器Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. 单击 **切换到文本模式**.
1. 请参阅以下通用代码：

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field>
   ```

1. 在 **为报表设置过滤器规则** 替换上述通用代码的区域：

   <pre>存在:A:$$OBJCODE=PROJ<br>存在:A:ID=FIELD:projectID<br>存在:A:portfolio:ownerID=4d94d7da001699b19edf50de15682221</pre>

   >[!NOTE]
   >
   >* “原始对象”(Original Object)是报表的对象：问题
   >* 目标对象为Portfolio。
   >* 链接对象为项目。
   >* 目标字段和指向从链接对象引用的目标对象的链接字段为ownerID。
   >* 此处链接对象的对象代码为PROJ。
   >* “原始对象”上显示的“链接”字段为projectID，“链接”字段为ID。


1. 将最后一个语句中目标字段(ownerID)的值替换为您环境中的用户ID。
1. 单击 **保存过滤器**.

### 示例2:筛选缺少的对象：任何自定义表单中未显示的自定义字段 {#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms}

使用文本模式界面，您可以构建一个过滤器以查看与自定义Forms（类别）无关联的自定义字段（参数）。 此过滤器将参数链接到类别，这些类别通过另一个对象“类别参数”(Category Parameter)连接。 由于这两个字段之间没有直接连接，并且由于您正在筛选缺少的信息，因此必须使用EXISTS语句。

>[!IMPORTANT]
>
>参数是自定义表单中引用的字段库中存在的字段。 类别参数是特定窗体上显示的字段版本。 例如，如果同一字段出现在5个表单上，则Workfront数据库中将有1个参数和5个类别参数。

要筛选未与自定义表单关联的自定义字段，请执行以下操作：

1. 创建参数或自定义字段过滤器。\
   有关创建过滤器的信息，请参阅 [过滤器Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. 单击 **切换到文本模式**.
1. 请参阅以下通用代码：

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

1. 在 **为报表设置过滤器规则** 替换上述通用代码的区域：

   <pre>存在:A:$$OBJCODE=CTGYPA<br>存在:A:parameterID=FIELD:ID<br>存在:A:$$EXISTSMOD=NOTEXISTS</pre>

   >[!NOTE]
   >
   >* “原始对象”(Original Object)是报表的对象：参数。
   >* 目标对象为类别。
   >* 链接对象是类别参数。
   >* 链接对象的对象代码为CTGYPA。
   >* 链接到目标对象的字段是parameterID，因为链接对象表和目标对象表中都存在parameterID。
   >* 原始对象上显示的链接字段是ID（类别参数的ID）。


1. 单击 **保存过滤器**.

### 示例3:筛选缺少的对象：某个时间段内未记录时间的用户 {#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time}

使用文本模式界面，您可以构建一个过滤器，以查看在特定时间段内没有记录时间的用户。 此过滤器将用户链接到“小时”，这些“小时”直接彼此连接。 但是，必须使用EXISTS语句和文本模式界面才能过滤缺少的信息。

要筛选上周未记录时间的用户，请执行以下操作：

1. 创建用户过滤器。\
   有关创建过滤器的信息，请参阅 [过滤器Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. 单击 **切换到文本模式**.
1. 请参阅以下通用代码：

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

1. 在 **为报表设置过滤器规则** 替换上述通用代码的区域：

   ```
   EXISTS:A:$$OBJCODE=HOUR<br>EXISTS:A:ownerID=FIELD:ID<br>EXISTS:A:entryDate=$$TODAYb-1w<br>EXISTS:A:entryDate_Range=$$TODAYe-1w<br>EXISTS:A:entryDate_Mod=between<br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

   >[!NOTE]
   >
   >* “原始对象”(Original Object)是报表的对象：用户。
   >* 目标对象为Hour。
   >* 在本例中，您不需要链接对象，因为用户和小时数直接连接在Workfront数据库中。
   >* 由于没有链接对象，因此您必须使用目标对象的对象代码：小时。
   >* 目标对象的链接字段为ownerID(显示在原始对象上；链接对象缺失)。
   >* 原始对象上显示的链接字段是ID（小时）（在目标对象上显示）；缺少链接对象。)
   >* 存在:A:entryDate语句是指定义目标对象（小时）并使用与常规筛选器语句相同语法的字段。 这可确保您仅显示在特定时间段（本例中为前一周）内未记录时间的用户。
   >* NOTEXISTS修饰符表示我们正在查找报表对象（用户）不存在的项目（小时）。


1. 单击 **保存过滤器**.

### 示例4:按多个字段过滤：按Portfolio所有者名称和Portfolio协调记分卡ID列出的任务 {#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id}

使用文本模式界面，您可以构建一个过滤器，该过滤器引用目标对象上的多个字段。 在这种情况下，引用目标字段的filter语句必须通过AND进行连接。

例如，您可以过滤任务列表，以仅显示满足以下条件的任务：

* 它们位于与其所有者是特定用户的组合关联的项目上。
* 它们位于与项目组合关联的项目上，而项目与特定的对齐记分卡未关联。

要按“Portfolio所有者名称”和“Portfolio对齐记分卡ID”过滤任务，请执行以下操作：

1. 创建任务过滤器。\
   有关创建过滤器的信息，请参阅 [过滤器Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. 单击 **切换到文本模式**.
1. 在 **为报表设置过滤器规则** 区域：
   <pre>存在:A:$$OBJCODE=PROJ<br>存在:A:ID=FIELD:projectID<br>存在:A:portfolio:ownerID=4d80ce5200000528787d57807732a33f<br>和:A:存在:A:$$EXISTSMOD=NOTEXISTS<br>和:A:存在:A:$$OBJCODE=PROJ<br>和:A:存在:A:ID=FIELD:projectID<br>和:A:存在:A:portfolio:alignmentScoreCardID=4da387b00001cbc732bb259355c33dad</pre>

   >[!NOTE]
   >
   >* “原始对象”(Original Object)是过滤器的对象：任务。
   >* 目标对象为Portfolio。
   >* 第一个目标字段是ownerID。
   >* 第二个目标字段是“对齐记分卡ID”。
   >* 链接对象为项目。
   >* 链接对象的对象代码为PROJ。
   >* 目标对象的链接字段是(Portfolio的ID)。
   >* “原始对象”(Original Object)中显示的“链接”(Linking)字段为projectID。
   >* 将ownerID替换为您环境中的用户ID。


1. 单击 **保存过滤器**.
