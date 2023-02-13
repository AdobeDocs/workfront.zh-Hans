---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: GitHub模块
description: 在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用GitHub的工作流，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: 5e520aab-8307-4a52-96b6-13b284f9cb53
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1796'
ht-degree: 0%

---

# [!DNL GitHub] 模块

在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!UICONTROL GitHub]，并将其连接到多个第三方应用程序和服务。

## 访问要求

您必须具有以下访问权限才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td>
  <td> <p>[!UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td>
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 先决条件

使用 [!DNL GitHub] 模块，你必须得 [!DNL GitHub] 帐户。

## 连接 [!DNL GitHub] to [!DNL Workfront Fusion]

有关连接 [!DNL GitHub] 帐户 [!UICONTROL Workfront Fusion]，请参阅 [创建连接 [!UICONTROL Adobe Workfront Fusion]  — 基本说明](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL GitHub] 模块及其字段。

配置 [!DNL GitHub] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!DNL GitHub] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [触发器](#triggers)
* [操作](#actions)

### 触发器

* [[!UICONTROL 监视问题]](#watch-issues)
* [[!UICONTROL 监视存储库]](#watch-repositories)
* [[!UICONTROL 观看福克斯]](#watch-forks)
* [[!UICONTROL 观看评论]](#watch-comments)
* [[!UICONTROL 观看拉取请求]](#watch-pull-requests)

#### [!UICONTROL 监视问题]

添加新问题或修改现有问题时，将触发此模块。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL GitHub] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL，我要观看]</td> 
   <td>选择是要监视所有存储库，还是只监视一个存储库。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL存储库]</td> 
   <td>如果您选择仅在一个存储库中监视问题，请选择要监视的存储库。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL返回问题的最大数量]</td> 
   <td>设置 [!DNL Workfront Fusion] 可在一个周期内使用。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>选择您是希望仅关注新问题，还是希望关注新问题和所有更改。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL过滤器]</td> 
   <td> <p>您可以按与要关注的问题的关联方式过滤这些问题。</p> 
    <ul> 
     <li>[!UICONTROL所有问题]</li> 
     <li>[!UICONTROL仅分配给我的问题]</li> 
     <li>[!UICONTROL仅由我创建的问题]</li> 
     <li>[!UICONTROL仅提及我的问题]</li> 
     <li>[!UICONTROL仅我订阅了更新的问题]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td>选择是仅观看未解决的问题，还是仅观看已解决的问题。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标签]</td> 
   <td>添加标记。 模块会监控此标记存在的问题。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 监视存储库]

创建或修改存储库时，将触发此模块。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL GitHub] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL返回存储库的最大数]</td> 
   <td>设置 [!DNL Workfront Fusion] 可在一个周期内使用。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>选择您是要关注新存储库和所有更改，还是仅关注新存储库。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 观看福克斯]

创建新分支时，将触发此模块。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL GitHub] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL存储库]</td> 
   <td>选择要监视分叉的存储库。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL返回分叉的最大数]</td> 
   <td>设置 [!DNL Workfront Fusion] 可在一个周期内使用。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 观看评论]

添加新注释或修改现有注释时，将触发此模块。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL GitHub] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL存储库]</td> 
   <td>选择要监视的存储库。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL问题编号]</td> 
   <td>如果要仅通过搜索针对特定问题做出的新评论来限制搜索，请输入问题编号。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL返回问题的最大数量]</td> 
   <td>设置 [!DNL Workfront Fusion] 可在一个周期内使用。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>选择是仅监视新注释，还是仅监视注释和所有更改。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 观看拉取请求]

添加新拉取请求或修改现有拉取请求时，将触发此模块。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL GitHub] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL存储库]</td> 
   <td>选择要监视的存储库。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL返回拉取请求的最大数量]</td> 
   <td>设置 [!DNL Workfront Fusion] 可在一个周期内使用。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td>选择您是要观看[!UICONTROL only open pull]请求、[!UICONTROL only closed ones]请求，还是所有拉取请求。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>选择是仅监视新拉取请求，还是要监视新拉取请求和所有更改。</td> 
  </tr> 
 </tbody> 
</table>

### 操作

* [[!UICONTROL 搜索问题]](#search-for-an-issue)
* [[!UICONTROL 创建问题]](#create-an-issue)
* [[!UICONTROL 更新问题]](#update-an-issue)
* [[!UICONTROL 获取问题]](#get-an-issue)
* [[!UICONTROL 添加受分配人]](#add-assignees)
* [[!UICONTROL 删除受分配人]](#remove-assignees)
* [[!UICONTROL 向问题添加标签]](#add-labels-to-an-issue)
* [[!UICONTROL 从问题中删除标签]](#remove-a-label-from-an-issue)
* [[!UICONTROL 创建评论]](#create-a-comment)
* [[!UICONTROL 列出注释]](#list-comments)

#### [!UICONTROL 搜索问题]

此模块会搜索与您的搜索标准匹配的问题。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL GitHub] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL返回问题的最大数量]</td> 
   <td>设置 [!DNL Workfront Fusion] 将在一个周期内使用（每个方案运行的重复次数）。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL排序依据]</td> 
   <td> <p>选择要对搜索结果排序的方式。</p> 
    <ul> 
     <li> <p>[!UICONTROL最佳匹配] </p> </li> 
     <li>[!UICONTROL创建日期]</li> 
     <li>[!UICONTROL更新日期]</li> 
     <li>[!UICONTROL注释数]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL排序方向]</td> 
   <td> <p>选择升序或降序。 </p> <p>对于日期，选择 <strong>[!UICONTROL降序]</strong> 将首先返回最近的日期。 </p> <p>对于[!UICONTROL注释数]，选择 <strong>[!UICONTROL降序]</strong> 将首先返回评论数最多的问题。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查询]</td> 
   <td>输入或映射搜索查询。 有关搜索选项的详细说明，请参阅 <a href="https://docs.github.com/en/github/searching-for-information-on-github/searching-issues-and-pull-requests">搜索问题和拉取请求</a> 在 [!DNL GitHub] 帮助站点。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建问题]

此模块在选定的存储库中创建新问题。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL GitHub] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL存储库]</td> 
   <td>选择要在中创建问题的存储库。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assignee]</td> 
   <td>选择要分配给问题的人员。 可用的受分配者包括对存储库具有写入权限的任何人，以及对存储库具有读取权限的组织成员。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL里程碑]</td> 
   <td>选择要与新问题关联的里程碑。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标签]</td> 
   <td>选择要应用于新问题的任何标签。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标题]</td> 
   <td>输入或映射新期的标题。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主体]</td> 
   <td>输入或映射问题正文，如说明或其他信息</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新问题]

此模块会更新现有 [!DNL GitHub] 问题。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL GitHub] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL存储库]</td> 
   <td>选择要在中更新问题的存储库。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assignee]</td> 
   <td>选择要分配给问题的人员。 可用的受分配者包括对存储库具有写入权限的任何人和对存储库具有读取权限的组织成员。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL里程碑]</td> 
   <td>选择要与问题关联的里程碑。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标签]</td> 
   <td>选择要应用于问题的任何标签。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>输入或映射要更新的问题的问题编号。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td>选择要将问题更新到的状态。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标题]</td> 
   <td>输入或映射问题的标题。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主体]</td> 
   <td>输入或映射问题正文，如说明或其他信息</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取问题]

此模块检索有关指定问题的详细信息

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL GitHub] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL存储库]</td> 
   <td>选择包含要检索相关详细信息的问题的存储库。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>输入或映射要检索相关详细信息的问题的问题编号。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 添加受分配人]

此模块将受分配者添加到指定的问题

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL GitHub] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL存储库]</td> 
   <td>选择包含要向其添加任务的问题的存储库。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assignee]</td> 
   <td>选择要分配给问题的人员。 可用的受分配者包括对存储库具有写入权限的任何人和对存储库具有读取权限的组织成员。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>输入或映射要向其添加受分配者的问题的问题编号。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除受分配人]

此模块会从指定的问题中删除受分配者。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL GitHub] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL存储库]</td> 
   <td>选择包含要从中删除受分配者的问题的存储库。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assignee]</td> 
   <td>选择要从问题中删除的人员。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>输入或映射要从中删除受分配者的问题的问题编号。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 向问题添加标签]

此模块会向问题添加标签。 标签是在存储库级别定义的，并且只能由对存储库具有写入权限的人员创建。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL GitHub] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL存储库]</td> 
   <td>选择包含要向其添加标签的问题的存储库。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标签]</td> 
   <td>选择要添加到问题的标签。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>输入或映射要向其添加标签的问题的问题编号。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 从问题中删除标签]

此模块会从问题中删除单个标签。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL GitHub] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL存储库]</td> 
   <td>选择包含要从中删除标签的问题的存储库。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标签]</td> 
   <td>选择要从问题中删除的标签。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>输入或映射要从中删除标签的问题的问题编号。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建评论]

此模块会针对指定的问题创建评论。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL GitHub] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL存储库]</td> 
   <td>选择包含要创建评论的问题的存储库。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>输入或映射要创建评论的问题的问题编号。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主体]</td> 
   <td>输入或映射评论的内容。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出注释]

此模块列出了对指定问题的所有评论。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL GitHub] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL存储库]</td> 
   <td>选择包含要列出评论的问题的存储库。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>输入或映射要列出评论的问题的问题编号。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Since]</td> 
   <td>模块将返回在此日期之后创建的注释。 有关支持的日期格式列表，请参阅 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在中键入强制 [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL返回评论的最大数量]</td> 
   <td>设置 [!DNL Workfront Fusion] 可在一个周期内使用。 </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Troubleshooting</h2>
-->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Module does not receive any events</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">If a module does not receive any events, check the webhook settings in Github and make sure that:</p>
-->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You have set the correct type of event that the chosen module should receive</p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You have entered the correct Payload URL</p>
  -->
