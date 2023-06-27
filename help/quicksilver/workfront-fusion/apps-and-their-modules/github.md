---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: GitHub模块
description: 在 [!DNL Adobe Workfront Fusion] 方案，您可以自动执行使用GitHub的工作流，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: 5e520aab-8307-4a52-96b6-13b284f9cb53
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1844'
ht-degree: 0%

---

# [!DNL GitHub] 模块

在 [!DNL Adobe Workfront Fusion] 场景，您可以自动执行使用 [!UICONTROL GitHub]，并将其连接到多个第三方应用程序和服务。

## 访问要求

您必须具有以下权限才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td>
  <td> <p>[！UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td>
   <td> <p>[！UICONTROL计划]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td> 
   <td>
   <p>当前许可证要求：否 [!DNL Workfront Fusion] 许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] 用于工作自动化和集成] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 计划，您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 计划。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关以下项的信息 [!DNL Adobe Workfront Fusion] 许可证，请参见 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 先决条件

使用 [!DNL GitHub] 模块，您必须拥有 [!DNL GitHub] 帐户。

## Connect [!DNL GitHub] 到 [!DNL Workfront Fusion]

有关连接 [!DNL GitHub] 目标帐户 [!UICONTROL Workfront Fusion]，请参见 [创建连接 [!UICONTROL Adobe Workfront Fusion]  — 基本说明](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL GitHub] 模块及其字段。

配置时 [!DNL GitHub] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除此以外，还有 [!DNL GitHub] 可能会显示字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [触发器](#triggers)
* [操作](#actions)

### 触发器

* [[!UICONTROL Watch问题]](#watch-issues)
* [[!UICONTROL 监视存储库]](#watch-repositories)
* [[!UICONTROL Watch Forks]](#watch-forks)
* [[!UICONTROL 关注评论]](#watch-comments)
* [[!UICONTROL Watch拉取请求]](#watch-pull-requests)

#### [!UICONTROL Watch问题]

添加新问题或修改现有问题时触发此模块。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL GitHub] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL我要观看]</td> 
   <td>选择是要监视所有存储库，还是只监视一个存储库。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL存储库]</td> 
   <td>如果您已选择仅在一个存储库中监视问题，请选择要监视的存储库。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL返回的最大问题数]</td> 
   <td>设置满足以下条件的最大结果数 [!DNL Workfront Fusion] 在一个周期内使用。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL监视]</td> 
   <td>选择您是只想查看新问题，还是想查看新问题和所有更改。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL筛选器]</td> 
   <td> <p>您可以根据与问题的关联方式筛选要关注的问题。</p> 
    <ul> 
     <li>[！UICONTROL所有问题]</li> 
     <li>[！UICONTROL Only issues assigned to me]</li> 
     <li>[！UICONTROL仅我创建的问题]</li> 
     <li>[！UICONTROL仅问题提及我]</li> 
     <li>[！UICONTROL仅我订阅的更新问题]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL状态]</td> 
   <td>选择是只查看未完成的问题，还是只查看已关闭的问题。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL标签]</td> 
   <td>添加标记。 模块会监视此标记是否存在问题。</td> 
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
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL GitHub] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL返回存储库的最大数量]</td> 
   <td>设置满足以下条件的最大结果数 [!DNL Workfront Fusion] 在一个周期内使用。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL监视]</td> 
   <td>选择是要监视新存储库和所有更改，还是只监视新存储库。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Watch Forks]

创建新分支时，将触发此模块。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL GitHub] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL存储库]</td> 
   <td>选择要监视分支的存储库。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL返回的分叉最大数量]</td> 
   <td>设置满足以下条件的最大结果数 [!DNL Workfront Fusion] 在一个周期内使用。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 关注评论]

添加新评论或修改现有评论时，将触发此模块。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL GitHub] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL存储库]</td> 
   <td>选择要监视的存储库。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL问题编号]</td> 
   <td>如果要通过仅搜索针对特定问题提出的新注释来限制搜索，请输入问题编号。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL返回的最大问题数]</td> 
   <td>设置满足以下条件的最大结果数 [!DNL Workfront Fusion] 在一个周期内使用。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL监视]</td> 
   <td>选择是要只查看新注释，还是要查看注释及所有更改。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Watch拉取请求]

添加新拉取请求或修改现有拉取请求时，将触发此模块。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL GitHub] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL存储库]</td> 
   <td>选择要监视的存储库。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL返回的最大拉取请求数]</td> 
   <td>设置满足以下条件的最大结果数 [!DNL Workfront Fusion] 在一个周期内使用。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL状态]</td> 
   <td>选择您是要监视[！UICONTROL仅打开拉取]请求，还是要监视[！UICONTROL仅关闭的拉取]请求，还是要监视所有拉取请求。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL监视]</td> 
   <td>选择您是只想查看新的拉取请求，还是想查看新的拉取请求和所有更改。</td> 
  </tr> 
 </tbody> 
</table>

### 操作

* [[!UICONTROL 搜索问题]](#search-for-an-issue)
* [[!UICONTROL 创建问题]](#create-an-issue)
* [[!UICONTROL 更新问题]](#update-an-issue)
* [[!UICONTROL 获取问题]](#get-an-issue)
* [[!UICONTROL 添加被分派人]](#add-assignees)
* [[!UICONTROL 移除被分派人]](#remove-assignees)
* [[!UICONTROL 向问题添加标签]](#add-labels-to-an-issue)
* [[!UICONTROL 从问题中删除标签]](#remove-a-label-from-an-issue)
* [[!UICONTROL 创建评论]](#create-a-comment)
* [[!UICONTROL 列出注释]](#list-comments)

#### [!UICONTROL 搜索问题]

此模块搜索与您的搜索条件匹配的问题。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL GitHub] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL返回的最大问题数]</td> 
   <td>设置满足以下条件的最大结果数 [!DNL Workfront Fusion] 将在一个周期内使用（每个方案运行的重复次数）。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL排序方式]</td> 
   <td> <p>选择您希望对搜索结果进行排序的方式。</p> 
    <ul> 
     <li> <p>[！UICONTROL最佳匹配] </p> </li> 
     <li>[！UICONTROL创建日期]</li> 
     <li>[！UICONTROL更新日期]</li> 
     <li>[！UICONTROL评论数]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL排序方向]</td> 
   <td> <p>选择升序或降序。 </p> <p>对于日期，选择 <strong>[！UICONTROL降序]</strong> 将首先返回最近的日期。 </p> <p>对于[！UICONTROL评论数]，选择 <strong>[！UICONTROL降序]</strong> 将首先返回评论数量最多的问题。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查询]</td> 
   <td>输入或映射您的搜索查询。 有关搜索选项的详细说明，请参阅 <a href="https://docs.github.com/en/github/searching-for-information-on-github/searching-issues-and-pull-requests">搜索问题和拉取请求</a> 在 [!DNL GitHub] 帮助站点。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建问题]

此模块在选定的存储库中创建一个新问题。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL GitHub] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL存储库]</td> 
   <td>选择要在其中创建问题的存储库。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL被分派人]</td> 
   <td>选择要分配给问题的人员。 可用的被分配者包括拥有存储库写入权限的任何人，以及拥有存储库读取权限的组织成员。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL里程碑]</td> 
   <td>选择要与新问题关联的里程碑。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL标签]</td> 
   <td>选择要应用于新问题的任何标签。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL标题]</td> 
   <td>输入或映射新问题的标题。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL主体]</td> 
   <td>输入或映射问题的正文，如描述或附加信息</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新问题]

此模块更新现有的 [!DNL GitHub] 问题。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL GitHub] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL存储库]</td> 
   <td>选择要更新问题的存储库。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL被分派人]</td> 
   <td>选择要分配给问题的人员。 可用的被分配者包括拥有存储库写入权限的任何人和拥有存储库读取权限的组织成员。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL里程碑]</td> 
   <td>选择要与问题关联的里程碑。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL标签]</td> 
   <td>选择要应用于问题的任何标签。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL编号]</td> 
   <td>输入或映射要更新的问题的问题编号。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL状态]</td> 
   <td>选择要将问题更新到的状态。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL标题]</td> 
   <td>输入或映射问题的标题。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL主体]</td> 
   <td>输入或映射问题的正文，如描述或附加信息</td> 
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
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL GitHub] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL存储库]</td> 
   <td>选择包含您要检索其详细信息的问题的存储库。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL编号]</td> 
   <td>输入或映射要检索其详细信息的问题编号。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 添加被分派人]

此模块向指定问题添加被分派人

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL GitHub] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL存储库]</td> 
   <td>选择包含要添加被分配人的问题的存储库。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL被分派人]</td> 
   <td>选择要分配给问题的人员。 可用的被分配者包括拥有存储库写入权限的任何人和拥有存储库读取权限的组织成员。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL编号]</td> 
   <td>输入或映射要添加被分配人的问题的问题编号。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 移除被分派人]

此模块从指定问题中删除被分配人。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL GitHub] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL存储库]</td> 
   <td>选择包含要从其中移除被分配人的问题的存储库。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL被分派人]</td> 
   <td>选择要从问题中删除的人员。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL编号]</td> 
   <td>输入或映射要从其中移除被分配人的问题的问题编号。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 向问题添加标签]

此模块向问题添加标签。 标签在存储库级别定义，并且只能由对存储库具有写入权限的用户创建。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL GitHub] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL存储库]</td> 
   <td>选择包含您要将标签添加到其中的问题的存储库。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL标签]</td> 
   <td>选择要添加到问题的标签。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL编号]</td> 
   <td>输入或映射要添加标签的问题编号。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 从问题中删除标签]

此模块从问题中删除单个标签。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL GitHub] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL存储库]</td> 
   <td>选择包含要从其中移除标签的问题存储库。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL标签]</td> 
   <td>选择要从问题中删除的标签。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL编号]</td> 
   <td>输入或映射要从其中移除标签的问题编号。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建评论]

此模块创建指定问题的评论。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL GitHub] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL存储库]</td> 
   <td>选择包含您要为其创建评论的问题的存储库。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL编号]</td> 
   <td>输入或映射您要创建评论的问题编号。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL主体]</td> 
   <td>输入或映射注释的内容。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出注释]

此模块列出有关指定问题的所有注释。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL GitHub] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL存储库]</td> 
   <td>选择包含您要从中列出注释的问题的存储库。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL编号]</td> 
   <td>输入或映射要从中列出注释的问题编号。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL始自]</td> 
   <td>模块将返回在此日期之后创建的注释。 有关支持的日期格式的列表，请参阅 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">键入强制 [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL返回评论的最大数量]</td> 
   <td>设置满足以下条件的最大结果数 [!DNL Workfront Fusion] 在一个周期内使用。 </td> 
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
