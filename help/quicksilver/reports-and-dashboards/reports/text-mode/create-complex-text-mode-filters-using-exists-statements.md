---
product-area: reporting
navigation-topic: text-mode-reporting
title: 使用EXISTS语句创建复杂的文本模式筛选器
description: 您可以使用EXISTS语句创建复杂的文本模式过滤器。 本文需要彻底了解Adobe Workfront API和文本模式报表界面。
author: Nolan
feature: Reports and Dashboards
exl-id: 106f7c9d-46cc-46c5-ae34-93fd13a36c14
source-git-commit: af4a82ad11b57c7a7457d5d7ee74ee18494a1dc0
workflow-type: tm+mt
source-wordcount: '2668'
ht-degree: 0%

---

# 使用EXISTS语句创建复杂的文本模式筛选器

<!-- Audited: 01/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: do not EVER&nbsp;delete this article as long as Text Mode still exists in the system.&nbsp;Google ordered this article to be written and we wrote it with the help of consultants, so the use case is very complex and very hard to understand without this. It is also very much used by many customers)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;Alina: **~ Replace screen shot of icons when list/ reporting UI changes)</p>
-->

>[!IMPORTANT]
>
>本文需要彻底了解Adobe Workfront API和文本模式报表界面。 有关Workfront API的信息，请参阅[API基础知识](../../../wf-api/general/api-basics.md)。\
>有关使用文本模式的信息，请参阅[文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)。

## Workfront中的对象关系概述

所有对象都链接到Workfront数据库中的其他对象。

了解对象的层次和相互依赖关系有助于您了解哪些对象可以在报表中引用。

有关Workfront中的对象及其层次结构和相互依赖性的信息，请参阅[Adobe Workfront对象概述](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)。

构建过滤器时，您可以使用标准报表界面在最多2个级别的关系中引用连接到过滤器对象的其他对象。

例如，您可以使用标准界面在问题筛选器中引用PortfolioID以仅显示与特定项目组合相关联的项目中的问题。 在这种情况下，项目组合与问题相差2级。

但是，您不能使用标准界面在问题过滤器中引用Portfolio所有者，以仅显示与所有者为特定用户的项目组合相关联的项目中的问题。 您必须使用文本模式来访问“Portfolio所有者名称”字段，该字段与问题相差三个级别。

![问题到项目组合所有者图标](assets/issue-to-portfolio-owner-sraight-line-icons-350x83.png)

有关Workfront中对象的完整列表，请参阅[API资源管理器](../../../wf-api/general/api-explorer.md)。

有关如何导航API资源管理器并查找对象的信息，请参阅[使用API资源管理器](../../../wf-api/general/using-api-explorer.md)。

构建过滤器时，必须在文本模式界面中构建复杂的语句以引用这些类型的对象。

有关生成复杂过滤器的信息，请参阅本文的[使用EXISTS语句的复杂文本模式过滤器概述](#overview-of-complex-text-mode-filters-that-use-exists-statements)部分。

## 使用EXISTS语句的复杂文本模式过滤器概述 {#overview-of-complex-text-mode-filters-that-use-exists-statements}

创建跨越对象层次结构中多个级别的过滤器或过滤缺少的对象时，请考虑以下事项：

* 如果要引用未直接连接到滤镜对象的对象，则必须创建复杂的滤镜。
* 必须使用EXISTS语句执行以下操作：

   * 创建跨多个级别的过滤器。
   * 创建筛选器以查找缺少的对象。\
     例如，在构建用户报告时，您可以筛选在特定时间段内未记录时间的用户。

在过滤器中使用EXISTS语句时，请考虑以下规则：

* 在EXISTS过滤器中，您可以引用三个对象：

   * 滤镜的对象（原始对象）。
   * 要引用其字段的对象（目标对象）。
   * 连接“原始”对象和“目标”对象的对象（链接对象），以防它们彼此不直接连接。

* 使用EXISTS的过滤器包含两个由等号链接的单独语句：

   * 等号之前的语句是指您引用的对象（链接对象或目标对象）。
   * 等号后面的语句是指您引用的对象（原始对象）。

* 必须使用链接对象的对象代码来连接语句。\
  您可以在API Explorer中找到所有对象的对象代码。\
  有关API Explorer的信息，请参阅[API Explorer](../../../wf-api/general/api-explorer.md)。

* 当由于原始对象和目标对象直接连接而缺少链接对象时，您可以使用目标对象的对象代码而不是链接对象。
* 您可以引用同一对象（目标对象）上的多个字段（目标字段），在这种情况下，必须通过AND连接引用这些字段的行。\
  有关筛选属于Target对象的多个字段的示例，请参阅本文中的[示例4：按多个字段筛选：按Portfolio所有者名称和Portfolio对齐记分卡ID筛选任务](#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id)部分。

* EXISTS语句唯一支持的修饰符是NOTEXISTS。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
      <p>新增：</p>
         <ul>
         <li><p>标准</p></li>
         </ul>
      <p>当前：</p>
         <ul>
         <li><p>计划</p></li>
         </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对筛选器、视图、分组的访问权限</p> <p>编辑对报告、功能板、日历的访问权限以编辑报告中的筛选器</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理对报告的权限以编辑报告中的筛选器</p> <p>管理筛选器权限以编辑它</p></td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 创建跨对象层次结构中多个级别的复杂文本模式筛选器

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***[This information is somewhat duplicated from the section below: Create Text-Mode Filters for Missing Objects])</p>
-->

您可以构建一个筛选器，该筛选器在对象层次结构的多个级别中引用对象，筛选器对象存在于对象层次结构中。 例如，您可以为与特定Portfolio所有者无关联的项目上的问题构建问题过滤器。

必须始终使用EXISTS语句和文本模式界面来构建此筛选器。

有关筛选器的示例，请参阅本文中的[示例1：按Portfolio所有者名称筛选问题](#example-1-filter-for-issues-by-portfolio-owner-name)部分。

要创建跨越对象层次结构中多个级别的过滤器，请执行以下操作：

1. 标识筛选器的对象。 我们将此对象称为“原始对象”。\
   例如，问题。

1. 标识要作为筛选依据的字段。 我们将此对象称为属于目标对象的目标字段。\
   例如，所有者ID字段（目标字段），它属于Portfolio（目标对象）。

1. （视情况而定）如果原始对象（问题）和目标字段（所有者ID）未直接相连，则必须找到第三个对象，即连接它们的链接对象（项目）。 链接对象必须至少有一个从原始对象的“字段”或“引用”选项卡（链接字段显示在原始对象上）中引用的字段，并且链接对象的“字段”或“引用”选项卡中还必须有一个指向目标对象的链接字段。 链接字段至链接对象上显示的目标对象（或链接对象上显示的链接字段）必须与目标字段匹配。

   例如，（项目） ID（原始对象上显示的链接字段）是从“问题”（原始对象）中引用的。 (Portfolio)ownerID（将字段链接到目标对象）显示在项目（链接对象）的“字段”选项卡中。 PortfolioownerID也是目标对象(Portfolio)中的字段。 链接对象上的链接字段与目标字段匹配。\
   ![portfolio_id_in_the_project_api_object.PNG](assets/portfolio-id-in-the-project-api-object-350x88.png)

1. 使用API资源管理器标识链接对象（项目）的&#x200B;**对象代码**。\
   例如，项目的对象代码为PROJ。\
   ![project_objCode_in_the_API.PNG](assets/project-objcode-in-the-api-350x84.png)

1. 为原始对象创建滤镜。\
   例如，创建问题过滤器。\
   有关创建筛选器的信息，请参阅[筛选器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

1. 单击&#x200B;**切换到文本模式**，然后单击&#x200B;**编辑文本模式**。
1. 将以下公式示例粘贴到新过滤器的文本模式界面中，并用正确的对象和字段替换示例文本：

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object>
   EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object>
   EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field>
   ```

   有关使用上面标识的字段的示例，请参阅本文中的[示例1：按Portfolio所有者名称筛选问题](#example-1-filter-for-issues-by-portfolio-owner-name)部分。

1. 单击&#x200B;**保存筛选器**。

## 为缺少的对象创建复杂文本模式筛选器

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: **^[This information is somewhat duplicated from the section above: Create Text-Mode Filters that Span Multiple Levels in the Object Hierarchy])</p>
-->

您可以构建一个过滤器来引用缺少的对象。 例如，您可以构建一个用户过滤器，以显示哪些用户尚未在Workfront中记录小时数。

必须始终使用&#x200B;*EXISTS*&#x200B;语句和文本模式界面来构建此筛选器。

有关缺少对象的筛选器的示例，请参阅本文中的以下部分：

* [示例2：筛选缺少的对象：未出现在任何自定义表单中的自定义字段](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms)
* [示例3：筛选缺少的对象：在特定时间段内未记录时间的用户](#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time)

要创建引用缺少对象的筛选器：

1. 标识筛选器的对象。 我们将此对象称为“原始对象”。\
   例如，参数或自定义字段。

1. 标识要作为筛选依据的字段。 我们将此对象称为属于目标对象的目标字段。\
   例如，类别ID字段（目标字段），它属于类别（目标对象）。

1. 由于原始对象（参数）和目标字段(categoryID)之间没有直接连接，因此您必须找到第三个对象，即连接它们的链接对象（类别参数）。 链接对象必须至少有一个从原始对象的“字段”或“引用”选项卡（链接字段显示在原始对象上）中引用的字段，并且链接对象的“字段”或“引用”选项卡中还必须有一个指向目标对象的链接字段。 链接字段至链接对象上显示的目标对象（或链接对象上显示的链接字段）必须与目标字段匹配。

   例如，类别参数（显示在原始对象上的链接字段）的ID是从参数（原始对象）中引用的。 parameterID（将字段链接到目标对象）显示在类别参数（链接对象）的“字段”选项卡中。 链接对象上显示的指向目标对象的链接字段与目标字段匹配。

1. 使用API资源管理器标识链接对象的&#x200B;**对象代码**（类别参数）。\
   例如，类别参数的对象代码为CTGYPA。\
   ![category_parameter_objcode_in_api.PNG](assets/category-parameter-objcode-in-api-350x79.png)

1. 为原始对象创建滤镜。\
   例如，创建一个“参数”筛选器。\
   有关创建筛选器的信息，请参阅[筛选器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

1. 单击&#x200B;**切换到文本模式**，然后单击&#x200B;**编辑文本模式**。
1. （视情况而定）如果要过滤缺少的对象，请将以下公式示例粘贴到新过滤器的文本模式界面中，并用正确的对象和字段替换示例文本：

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object>
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object>
   EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

   有关未与自定义Forms关联的自定义字段的报表示例，请参阅本文中的[示例2：筛选缺少的对象：未出现在任何自定义表单中的自定义字段](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms)部分。

1. 单击&#x200B;**保存筛选器**。

## 跨对象层次结构中多个级别的文本模式筛选器的示例

使用这些示例使用EXISTS语句构建文本模式过滤器。

### 示例1：按Portfolio所有者名称筛选问题 {#example-1-filter-for-issues-by-portfolio-owner-name}

使用文本模式界面，您可以构建问题列表的过滤器，以仅显示与项目组合（其所有者为特定用户）相关的项目上的问题。

要按Portfolio所有者名称筛选问题，请执行以下操作：

1. 创建问题过滤器。\
   有关创建筛选器的信息，请参阅[筛选器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

1. 单击&#x200B;**切换到文本模式**，然后单击&#x200B;**编辑文本模式**。
1. 请参阅以下通用代码：

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object>
   EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object>
   EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field>
   ```

1. 将以下代码粘贴到&#x200B;**为报表**&#x200B;设置筛选规则区域以替换上面的通用代码：

   ```
   EXISTS:A:$$OBJCODE=PROJ
   EXISTS:A:ID=FIELD:projectID
   EXISTS:A:portfolio:ownerID=4d94d7da001699b19edf50de15682221
   ```

   >[!NOTE]
   >
   >* 原始对象是报告的对象：问题
   >* 目标对象Portfolio。
   >* 链接对象为“项目”。
   >* 目标字段和链接到从链接对象引用的目标对象的链接字段是ownerID。
   >* 此处链接对象的对象代码为PROJ。
   >* 原始对象上显示的链接字段为projectID，链接字段为ID。

1. 将上一语句中目标字段(ownerID)的值替换为您环境中的用户ID。
1. 单击&#x200B;**保存筛选器**。

### 示例2：筛选缺少的对象：未在任何自定义表单中显示的自定义字段 {#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms}

利用文本模式界面，您可以构建过滤器以查看与自定义Forms（类别）无关联的自定义字段（参数）。 此过滤器将参数链接到通过另一个对象“类别参数”连接的类别。 由于这两个字段之间没有直接连接，并且您正在过滤缺少的信息，因此您必须使用EXISTS语句。

>[!IMPORTANT]
>
>参数是指在自定义表单中引用的字段库中存在的字段。 类别参数是显示在特定表单上的字段版本。 例如，如果在5个表单中显示相同的字段，则Workfront数据库中将有1个参数和5个类别参数。

要筛选未与自定义表单关联的自定义字段，请执行以下操作：

1. 创建参数或自定义字段过滤器。\
   有关创建筛选器的信息，请参阅[筛选器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

1. 单击&#x200B;**切换到文本模式**，然后单击&#x200B;**编辑文本模式**。
1. 请参阅以下通用代码：

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object>
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object>
   EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

1. 将以下代码粘贴到&#x200B;**为报表**&#x200B;设置筛选规则区域以替换上面的通用代码：

   ```
   EXISTS:A:$$OBJCODE=CTGYPA
   EXISTS:A:parameterID=FIELD:ID
   EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

   >[!NOTE]
   >
   >* 原始对象是报表的对象：参数。
   >* 目标对象为“类别”。
   >* 链接对象是类别参数。
   >* 链接对象的对象代码为CTGYPA。
   >* 与目标对象的链接字段为parameterID，因为parameterID同时存在于链接对象表和目标对象表中。
   >* 在原始对象上显示的链接字段是（类别参数的）ID。

1. 单击&#x200B;**保存筛选器**。

### 示例3：筛选缺少的对象：在特定时间段内未记录时间的用户 {#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time}

使用文本模式界面，您可以构建过滤器以查看在特定时间段内未记录时间的用户。 此过滤器将用户链接到小时，这些小时彼此直接相连。 但是，必须使用EXISTS语句和文本模式界面才能过滤缺少的信息。

要筛选上周未记录时间的用户，请执行以下操作：

1. 创建用户过滤器。\
   有关创建筛选器的信息，请参阅[筛选器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

1. 单击&#x200B;**切换到文本模式**，然后单击&#x200B;**编辑文本模式**。
1. 请参阅以下通用代码：

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object>
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object>
   EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

1. 将以下代码粘贴到&#x200B;**为报表**&#x200B;设置筛选规则区域以替换上面的通用代码：

   ```
   EXISTS:A:$$OBJCODE=HOUR
   EXISTS:A:ownerID=FIELD:ID
   EXISTS:A:entryDate=$$TODAYb-1w
   EXISTS:A:entryDate_Range=$$TODAYe-1w
   EXISTS:A:entryDate_Mod=between
   EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

   >[!NOTE]
   >
   >* 原始对象是报表的对象：用户。
   >* 目标对象是小时。
   >* 在本例中，您不需要链接对象，因为“用户”和“小时”直接连接到Workfront数据库。
   >* 由于没有链接对象，因此必须使用目标对象的对象代码：HOUR。
   >* 目标对象的链接字段是ownerID（显示在原始对象上；缺少链接对象）。
   >* 在原始对象上显示的链接字段是ID（小时）（显示在目标对象上；缺少链接对象）。
   >* EXISTS:A:entryDate语句引用定义Target对象(Hour)的字段，并使用与常规筛选语句相同的语法。 这样可以确保只显示那些在特定时间段（在本例中是上一周）未记录时间的用户。
   >* NOTEXISTS修饰符指示我们正在查找报表对象（用户）不存在的项目（小时）。

1. 单击&#x200B;**保存筛选器**。

### 示例4：按多个字段筛选：按Portfolio所有者名称和Portfolio对齐记分卡ID列出的任务 {#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id}

使用文本模式界面，您可以构建一个引用Target对象上多个字段的筛选器。 在这种情况下，引用目标字段的filter语句必须通过AND连接。

例如，您可以筛选任务列表，以仅显示满足以下条件的任务：

* 他们位于与项目组合（其所有者为特定用户）关联的项目上。
* 它们位于与项目组合关联的项目上，而该项目与特定一致性记分卡无关。

要按Portfolio所有者名称和Portfolio对齐计分卡ID筛选任务，请执行以下操作：

1. 创建任务过滤器。\
   有关创建筛选器的信息，请参阅[筛选器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

1. 单击&#x200B;**切换到文本模式**，然后单击&#x200B;**编辑文本模式**。
1. 将以下代码粘贴到&#x200B;**为报表**&#x200B;设置筛选规则区域：

   ```
   EXISTS:A:$$OBJCODE=PROJ
   EXISTS:A:ID=FIELD:projectID
   EXISTS:A:portfolio:ownerID=4d80ce5200000528787d57807732a33f
   AND:A:EXISTS:A:$$EXISTSMOD=NOTEXISTS
   AND:A:EXISTS:A:$$OBJCODE=PROJ
   AND:A:EXISTS:A:ID=FIELD:projectID
   AND:A:EXISTS:A:portfolio:alignmentScoreCardID=4da387b00001cbc732bb259355c33dad
   ```

   >[!NOTE]
   >
   >* “原始对象”是滤镜：“任务”的对象。
   >* 目标对象Portfolio。
   >* 第一个目标字段是ownerID。
   >* 第二个目标字段是“对齐计分卡ID”。
   >* 链接对象为“项目”。
   >* 链接对象的对象代码为PROJ。
   >* “与目标对象关联”字段是Portfolio的ID。
   >* 原始对象上显示的链接字段为projectID。
   >* 使用您环境中的用户ID替换ownerID。

1. 单击&#x200B;**保存筛选器**。
