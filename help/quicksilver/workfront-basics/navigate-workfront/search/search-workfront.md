---
navigation-topic: search
title: 搜索 [!DNL Adobe Workfront]
description: 您可以轻松地在 [!DNL Adobe Workfront] 在无法记住其确切位置时搜索它们。
feature: Get Started with Workfront
author: Lisa
exl-id: 7c856349-c79f-40d8-9c96-b32bfb6d5417
source-git-commit: 073e6c7d4e830dfd2b8920a20e1490c5524d71bd
workflow-type: tm+mt
source-wordcount: '1667'
ht-degree: 1%

---

# 搜索 [!DNL Adobe Workfront]

您可以轻松地在 [!DNL Adobe Workfront] 在无法记住其确切位置时搜索它们。

您可以看到 [!UICONTROL 搜索] 框中的任意页面的右上角 [!DNL Workfront].

![](assets/search-globalnavigationbar-350x62.png)

您必须拥有查看对象的权限，然后才能在搜索中查找对象。 因此，搜索结果因用户而异。

## 访问要求

+++ 展开此部分可查看执行本文中的步骤所需的访问权限。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>请求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>[!UICONTROL视图]对对象类型的访问 </p> <p>注意：如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>您必须拥有查看对象的权限，然后才能在搜索中查找对象。</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

+++

## 了解搜索

* [[!UICONTROL 可搜索的对象]](#objects-available-for-search)
* [[!UICONTROL 可供搜索的字段]](#fields-available-for-search)

### 可搜索的对象

您可以在Workfront中搜索以下对象：

* 项目
* 任务
* 问题
* 报告
* 用户
* 模板
* 文档
* 项目组合
* 项目群
* 仪表板
* 公司
* 注释

### 可供搜索的字段

可搜索的字段基于搜索类型：基本或 [!UICONTROL 高级搜索].

* **基本搜索**:在基本搜索中搜索对象时， [!DNL Workfront] 在以下字段中查找可能包含关键词的文本：

   * 对象名称
   * 描述
   * 自定义数据字段
   * 更新
   * 文档名称（在特定文档搜索和基本搜索中）

   有关基本搜索的详细信息，请参阅 [!DNL Workfront]，请参阅 [基本搜索](#basic-search) 在本文中。

* **[!UICONTROL 高级搜索]**:在 [!UICONTROL 高级搜索]，则可以将过滤器设置为基本搜索中不可用的搜索字段。 因此， [!UICONTROL 高级搜索] 用于搜索对象中的任意字段。

   有关 [!UICONTROL 高级搜索]，请参阅 [高级搜索](#advanced-search) 在本文中。

>[!NOTE]
>
>执行 [!UICONTROL 高级搜索]，则必须选择 [!UICONTROL 高级搜索] 选项。 您无法将基本搜索细化为 [!UICONTROL 高级搜索].

## 了解 [!DNL Workfront] 搜索

使用 [!UICONTROL 搜索] in [!DNL Workfront]:

* 搜索不区分大小写
* [!DNL Workfront] 不正确或理解拼写错误
* 正在搜索 [!DNL Workfront] 不支持通配符
* 正在搜索 [!DNL Workfront] 支持部分字搜索，但不支持子字符串搜索。\
   例如，搜索关键词“stand”将返回包含“standard”一词的结果，但不返回包含“inderant”一词的结果。

## 搜索多个词

当您在搜索中包含多个词时，并且希望仅查找与“搜索”框中所有词匹配的对象时，可以按任意顺序键入这些词。

例如，搜索“营销演示”（不带引号）时，会查找具有以下名称的对象：

* 营销演示
* 演示营销
* 1月市场分析演示

它还会查找名称中可能包含“营销”且描述中包含“演示”的对象。

但是，您可以在 [!UICONTROL 搜索] 框来调整显示的搜索结果：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>包括引号</td> 
   <td> <p>在双引号内以正确顺序输入单词，可仅查找精确匹配的对象。<br>例如，搜索“营销演示”（带引号）时，会查找具有以下名称的对象：</p> 
    <ul> 
     <li> 营销演示</li> 
     <li> 1月营销演示</li> 
     <li>营销演示计划</li> 
    </ul> <p>但是，此搜索未找到名为“演示营销”的对象。</p> </td> 
  </tr> 
  <tr> 
   <td>包含或</td> 
   <td> <p>通过“OR”（不带引号）连接单词允许您仅查找与[!UICONTROL Search]框中至少一个单词匹配的对象。 这些词可以按任意顺序输入。<br>例如，搜索“营销或演示”（不带引号）时，会查找具有以下名称的对象：</p> 
    <ul> 
     <li> 市场分析演示</li> 
     <li>1月市场分析演示</li> 
     <li>演示</li> 
     <li>市场分析</li> 
    </ul> <p>注意：“OR”必须全部大写。 否则，它会被解释为您正在搜索的短语中的另一个词。</p> </td> 
  </tr> 
  <tr> 
   <td>包含和</td> 
   <td> <p>通过“AND”（不带引号）连接单词允许您仅查找与[!UICONTROL Search]框中的所有单词匹配的对象。 这些词可以按任意顺序输入。<br>例如，搜索“营销和演示”（不带引号）时，会查找具有以下名称的对象：</p> 
    <ul> 
     <li>营销演示</li> 
     <li>演示营销</li> 
     <li>1月市场分析演示</li> 
    </ul> <p>注意：“AND”必须全部大写。 否则，它会被解释为您正在搜索的短语中的另一个词。 同样，包括“&amp;”（不带引号）仅搜索包含与号的对象。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 在中使用搜索 [!DNL Workfront]

[!DNL Workfront] 具有两种搜索类型：基本和高级。 如果要在常用对象字段（如名称或描述）中查找关键字，请使用基本搜索。 使用 [!UICONTROL 高级搜索] 如果要使用过滤器搜索其他对象字段，请执行以下操作：

* [基本搜索](#basic-search)
* [高级搜索](#advanced-search)

### 基本搜索

基本搜索允许您在系统中的所有对象中搜索关键字，或一次只搜索一个对象（如项目）。 [!DNL Workfront] 然后在几个特定字段中搜索这些关键词。 然后，您可以根据所选的其他特定对象字段来优化搜索结果 [!DNL Workfront].

有关在基本搜索中搜索的特定字段的列表，请参阅 [可供搜索的字段](#fields-available-for-search) 在本文中。

>[!NOTE]
>
>执行 [!UICONTROL 高级搜索]，则必须选择 [!UICONTROL 高级搜索] 选项。 您无法将基本搜索细化为 [!UICONTROL 高级搜索].

* [执行基本搜索](#perform-a-basic-search)
* [优化基本搜索](#refine-a-basic-search)

#### 执行基本搜索

您可以通过以下任一方式执行基本搜索：

* 在系统中的所有对象之间（常规搜索）。
* 一次只对一个对象（特定于对象的搜索）。

要执行基本搜索，请执行以下操作：

1. 单击放大镜 ![](assets/search-icon.png) 的双曲余切值。 您还可以键入 **[!UICONTROL ALT + /]** 或 **[!UICONTROL 选项+ /]** 打开 [!UICONTROL 搜索] 菜单。

1. （可选）要搜索特定对象，请单击 **[!UICONTROL 全部]** 下拉菜单，然后选择要搜索的对象。

   ![](assets/search-objecttype.png)

1. 在 **[!UICONTROL 搜索]** 框中，开始键入您正在搜索的信息。\
   有关搜索字段的信息 [!DNL Workfront]，请参阅 [了解搜索](#understand-search).\
   ![](assets/qs-search-drop-down-highlighted-350x234.png)\
   在搜索栏中开始输入时， [!DNL Workfront] 根据您的查看历史记录提供推荐，并以蓝色突出显示您正在搜索的关键词。

1. 如果要查找的项目显示在 [!UICONTROL typeaid] 菜单，单击它。

   或

   按 **[!UICONTROL 输入]** 进行全面搜索。 此搜索会查询整个数据库，而不是您最近查看的项目。

   的 [!UICONTROL 搜索结果] 从左侧打开的页面幻灯片包含上一页的大部分内容。

   如果您执行了常规搜索， [!DNL Workfront] 返回与搜索的任何字段中的搜索词匹配的任何对象的结果，如 [了解搜索](#understand-search). 与您的搜索匹配的对象将显示在列表中。

   >[!NOTE]
   >
   >有时，单词的变体会显示在找到的项目列表中。\
   >例如，搜索“营销”时，会在名称中显示包含“营销”或“市场”的对象。

1. （可选）如果搜索生成的结果过多，请按照 [优化基本搜索](#refine-a-basic-search).
1. （可选）要返回搜索前所在的页面，请单击 **[!UICONTROL 关闭]** 中。

>[!NOTE]
>
>的 [!UICONTROL 搜索结果] 仅当页面处于焦点时，页面才会保持打开状态。 单击离开页面或打开其他页面可关闭 [!UICONTROL 搜索结果] 页面。

#### 优化基本搜索

执行基本搜索后 — 如 [[!UICONTROL 执行基本搜索]](#perform-a-basic-search) — 您可以优化搜索。

使用搜索结果左侧的工具栏可缩小要查找的信息范围。

要优化搜索，请执行以下操作：

1. （视情况而定）如果您执行了常规搜索，请在结果左上角的对象列表中选择要搜索的对象。
1. 在结果左侧的工具栏中，找到搜索中显示的对象可用的字段。\
   每个字段的值会按计数排序，每个字段最多显示10个值。
1. 在可用于缩短结果列表的任意字段内单击。\
   您所做的选择将以蓝色突出显示，并且未选择的字段值将被隐藏。\
   选择每个新值后，右侧的结果会动态更新。\
   ![](assets/qs-refine-search-350x175.png)

1. （可选）单击选定的值以取消选择它们，然后再次显示每个字段的所有值。

### [!UICONTROL 高级搜索]

[!UICONTROL 高级搜索] 允许您使用基本搜索不可用的字段和过滤器进行搜索。 例如，您可以搜索具有特定优先级或文档所有者名称的项目。

>[!NOTE]
>
>执行 [!UICONTROL 高级搜索]，则必须选择 [!UICONTROL 高级搜索] 选项。 您无法将基本搜索细化为 [!UICONTROL 高级搜索].

* [使用 [!UICONTROL 高级搜索]](#use-advanced-search)

#### 使用 [!UICONTROL 高级搜索]

您可以使用 [!UICONTROL 高级搜索] ，以根据特定条件筛选搜索。\
当您无法记住与某个对象关联的关键字，但您知道有关该对象的某些特定信息(例如：项目优先级、文档所有者名称等)。

要执行高级搜索，请执行以下操作：

1. 位于 [!DNL Workfront]，请单击 **[!UICONTROL 搜索]** 图标 ![](assets/search-icon.png). 的 [!DNL Search] 菜单。

1. 在 [!UICONTROL 搜索] 菜单，单击 **[!UICONTROL 高级搜索]**.\
   ![](assets/qs-advanced-search-350x224.png)\
   的 [!UICONTROL 高级搜索] 页面幻灯片从右侧打开，其中涵盖上一页的大部分内容。

1. 选择要搜索的对象类型。\
   **[!UICONTROL 项目]** 默认情况下，处于选中状态。

   ![](assets/advanced-search-objects-qs-remove-after-prod-release.png)

1. （可选）在列表顶部的字段中键入关键词。
1. （可选）单击 **[!UICONTROL 筛选结果]** 要根据特定的字段类型过滤搜索结果，请从列表中选择一个字段。 如有必要，还请为字段选择一个值。\
   或\
   添加新过滤器。

1. 单击 **[!UICONTROL 搜索]**.\
   与您的搜索匹配的项目列表将显示在 [!UICONTROL 高级搜索] 工具栏。

1. （可选）要返回搜索前所在的页面，请单击 **[!UICONTROL 关闭]** 在右上角。

>[!NOTE]
>
>的 [!UICONTROL 搜索结果] 仅当页面处于焦点时，页面才会保持打开状态。 单击离开页面或打开其他页面可关闭 [!UICONTROL 搜索结果] 页面。
