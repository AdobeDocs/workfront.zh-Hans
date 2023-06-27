---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: 网格模块
description: 在 [!DNL Adobe Workfront Fusion] 方案，您可以自动执行使用Trello的工作流，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: 60630b23-e057-4ecf-a014-6e63b6d69b48
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '5087'
ht-degree: 0%

---

# [!UICONTROL 特雷洛] 模块

在 [!DNL Adobe Workfront Fusion] 场景，您可以自动执行使用 [!UICONTROL 特雷洛]，并将其连接到多个第三方应用程序和服务。

如果您需要有关创建方案的说明，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

有关模块的信息，请参见 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

使用 [!DNL Trello] 模块，您必须具有 [!UICONTROL 特雷洛] 帐户。

## Connect [!UICONTROL 特雷洛] 到 [!DNL Workfront Fusion]

有关连接 [!UICONTROL 特雷洛] 目标帐户 [!DNL Workfront Fusion]，请参见 [创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!UICONTROL 特雷洛] 模块及其字段

配置时 [!UICONTROL 特雷洛] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除此以外，还有 [!UICONTROL 特雷洛] 可能会显示字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [展示板](#boards)
* [列表](#lists)
* [信息卡](#cards)
* [成员](#members)
* [核对清单](#checklists)
* [标签](#labels)
* [注释](#comments)

### 展示板

+++ **[!UICONTROL 观看讨论区]**

此触发器模块在添加新展示板后开始执行场景。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关将您的[！UICONTROL Trello]帐户连接到 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td> <p>展示板的最大数量 [!DNL Workfront Fusion] 将在一个执行周期内返回。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 创建展示板]**

此操作模块使用选定的设置创建一个新展示板。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关将您的[！UICONTROL Trello]帐户连接到 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL名称] </td> 
   <td> <p>输入或映射新讨论区的名称。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL描述]</td> 
   <td> <p>根据需要输入或映射展示板描述。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL组织ID]</p> </td> 
   <td> <p>输入或映射组织的ID。 组织ID可通过使用其他模块（如“观看活动”模块）进行检索。</p> <p> <img src="assets/id-of-org.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL权限级别]</p> </td> 
   <td> <p>董事会对每个权限级别有不同的投票和注释规则。 例如：如果您的讨论区是[！UICONTROL Private]，并且您将投票和注释规则设置为[！UICONTROL All]，则会收到错误。 </p> <p>每个权限级别的投票和评论仅限于以下组：</p> 
    <ul> 
     <li><strong>[！UICONTROL专用]</strong>：—&gt;成员、成员和观察者</li> 
     <li><strong>[！UICONTROL For Organization]</strong>：—&gt;成员、成员和观察员、组织成员</li> 
     <li><strong>[！UICONTROL公共]</strong>：—&gt;成员、成员和观察者、组织成员、全部</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Voting]</p> </td> 
   <td> <p>选择一个选项，以指定可以在该讨论区投票的人员。 有关权限级别的投票限制，请参阅[！UICONTROL权限级别]字段。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL注释]</p> </td> 
   <td> <p>选择一个选项，以指定可以对此讨论区的信息卡进行评论的人员。 有关对权限级别的限制的注释，请参阅[！UICONTROL权限级别]字段。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL邀请]</p> </td> 
   <td> <p>选择谁可以邀请其他人加入此讨论区。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL自连接]</p> </td> 
   <td> <p>选择团队成员是否可以自己加入讨论区，或者必须邀请他们。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL默认标签]</p> </td> 
   <td> <p>选择是否为新展示板使用默认标签集。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL默认列表]</p> </td> 
   <td> <p>选择是否将默认列表集添加到展示板（[！UICONTROL待办事项]、[！UICONTROL正在办事项]、[！UICONTROL已完成]）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL展示板源ID]</p> </td> 
   <td> <p>选择或映射要复制到新展示板中的展示板ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL卡盖]</p> </td> 
   <td> <p>选择 <strong>[！UICONTROL是]</strong> 如果您要为主板启用卡盖。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL背景]</p> </td> 
   <td> <p>选择背景或自定义背景的颜色。</p> <p>注意：自定义背景仅适用于[！UICONTROL Trello Gold and Business Class]订阅者。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL卡老化]</p> </td> 
   <td> <p>在卡片老化的两种模式之间进行选择。 </p> 
    <ul> 
     <li><strong>[！UICONTROL常规]</strong>：信息卡会随着年龄增长而逐渐变得更加透明。 </li> 
     <li><strong>[！UICONTROL海盗]</strong>：随着年龄的增长，信息卡将像旧的海盗地图一样撕裂、变黄和裂开。</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 编辑讨论区]**

此操作模块编辑现有展示板的设置。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关将您的[！UICONTROL Trello]帐户连接到 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL展示板ID]</p> </td> 
   <td> <p>输入或映射您希望模块创建的展示板的唯一[！UICONTROL Trello] ID。 您可以使用其他模块（如监视板模块）检索展示板ID</p> <p> <img src="assets/watch-boards.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL新名称]</td> 
   <td> <p> 输入或映射展示板的新名称。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL新描述]</td> 
   <td> <p> 根据需要输入或映射新的展示板描述。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL组织ID]</p> </td> 
   <td> <p>输入或映射您希望模块编辑的展示板的唯一[！UICONTROL网格] ID。 您可以使用其他模块(例如 [!DNL Watch Activities] 模块。</p> <p> <img src="assets/org-id.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL订阅] </td> 
   <td> <p>选择一个选项，以指定代理用户是否已订阅展示板。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL权限级别]</p> </td> 
   <td> <p>董事会对每个权限级别有不同的投票和注释规则。 例如：如果您的讨论区是[！UICONTROL Private]，并且您将投票和注释规则设置为[！UICONTROL All]，则会收到错误。 </p> <p>每个权限级别的投票和评论仅限于以下组：</p> 
    <ul> 
     <li><strong>[！UICONTROL专用]</strong>：—&gt;成员、成员和观察者</li> 
     <li><strong>[！UICONTROL For Organization]</strong>：—&gt;成员、成员和观察员、组织成员</li> 
     <li><strong>[！UICONTROL公共]</strong>：—&gt;成员、成员和观察者、组织成员、全部</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Voting]</p> </td> 
   <td> <p>选择一个选项，以指定可以在该讨论区投票的人员。 有关权限级别的投票限制，请参阅[！UICONTROL权限级别]字段。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL注释]</p> </td> 
   <td> <p>选择一个选项，以指定可以对此讨论区的信息卡进行评论的人员。 有关对权限级别的限制的注释，请参阅[！UICONTROL权限级别]字段。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL邀请] </td> 
   <td> <p>选择谁可以邀请人员加入此讨论区。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL自连接]</td> 
   <td> <p> 选择团队成员是否可以自己加入讨论区，或者必须邀请他们。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL卡盖]</td> 
   <td> <p> 选择此主板上是否应显示卡盖。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL背景] </td> 
   <td> <p>选择背景或自定义背景的颜色。</p> <p>注意：自定义背景仅适用于[！UICONTROL Trello Gold and Business Class]订阅者。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL背景ID]</td> 
   <td> <p> 如果已在[！UICONTROL背景]字段中选择使用自定义背景，请输入或映射要使用的背景的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL卡老化]</p> </td> 
   <td> <p>在卡片老化的两种模式之间进行选择。 </p> 
    <ul> 
     <li><strong>[！UICONTROL常规]</strong>：信息卡会随着年龄增长而逐渐变得更加透明。 </li> 
     <li><strong>[！UICONTROL海盗]</strong>：随着年龄的增长，信息卡将像旧的海盗地图一样撕裂、变黄和裂开。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL日历信息源已启用]</td> 
   <td> <p> 选择是否启用日历馈送。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL &lt;color&gt; 标签名称]</td> 
   <td> <p> 为所需的颜色标签指定名称。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL存档] </td> 
   <td> <p>选择一个选项以指示是否要存档（关闭）展示板。 </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 获取讨论区]**

此操作模块可检索讨论区的详细信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关将您的[！UICONTROL Trello]帐户连接到 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL展示板ID]</p> </td> 
   <td> <p>输入或映射要检索相关信息的展示板的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!DNL Search for Boards]**

此搜索模块检索有关您指定的主板的信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关将您的[！UICONTROL Trello]帐户连接到 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查询] </td> 
   <td> <p>输入或映射要获取相关信息的展示板名称（或部分名称）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL返回展示板的最大数量]</td> 
   <td> <p> 输入展示板的最大数量 [!DNL Workfront Fusion] 将在一个执行周期内返回。 该值必须小于或等于1000。</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Partial] </p> </td> 
   <td> <p>默认情况下，此模块会搜索成员内容，以查找查询中每个单词的完全匹配项。 启用[！UICONTROL Partial]后，模块会查找以查询中任意单词开头的内容。</p> <p> 例如，如果您使用单词“development”来查找标题为“My Development Status Report”的展示板，则默认情况下您需要搜索整个单词。 如果您启用了[！UICONTROL Partial]，则可以搜索“dev”，但不能搜索“velopment”。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL展示板] </td> 
   <td> <p>输入“我的”或映射以逗号分隔的展示板ID列表。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 存档或取消存档展示板]**

此操作模块可关闭或重新打开您指定的展示板。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关将您的[！UICONTROL Trello]帐户连接到 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL展示板ID]</td> 
   <td> <p> 输入或映射要关闭或重新打开的主板的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL存档或取消存档]</td> 
   <td> <p> 选择要关闭（存档）还是重新打开（取消存档）展示板。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 将成员分配给讨论区]**

此操作模块将成员分配给您指定的展示板。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关将您的[！UICONTROL Trello]帐户连接到 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL展示板ID]</td> 
   <td> <p> 选择要添加成员的展示板。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL电子邮件地址]</td> 
   <td> <p> 输入或映射要添加到讨论区的成员的电子邮件地址。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL成员类型]</p> </td> 
   <td> <p>选择要添加到讨论区的成员类型。</p> 
    <ul> 
     <li><strong>[！UICONTROL管理员]</strong>：主板管理员可以对主板执行任何主板操作。</li> 
     <li><strong>[！UICONTROL正常]</strong>：普通成员只是董事会成员。</li> 
     <li><strong>[！UICONTROL观察者]</strong>：观察者是对讨论区具有只读访问权限的成员。 <br>观察者仅适用于具有[！UICONTROL Trello Business Class]的团队。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL全名]</td> 
   <td> <p> 输入要添加到展示板的用户的全名。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 从讨论区中取消分配成员]**

此操作模块从展示板中移除成员。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关将您的[！UICONTROL Trello]帐户连接到 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL展示板ID]</td> 
   <td> <p> 输入（映射或选择）要从其中移除用户的展示板的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL成员] </td> 
   <td> <p>选择要从展示板中移除的成员。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### 列表

+++ **[!UICONTROL 观看卡片移至列表]**

将信息卡移动到特定列表时，此触发器模块将激活。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关将您的[！UICONTROL Trello]帐户连接到 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Board]</td> 
   <td>选择包含您要观看卡片列表的展示板。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL列表]</td> 
   <td>选择要观察卡片的列表。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td> <p>卡片的最大数量 [!DNL Workfront Fusion] 将在一个执行周期内返回。</p>  </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 创建列表]**

此操作模块会在您指定的展示板上创建一个列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关将您的[！UICONTROL Trello]帐户连接到 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL展示板ID]</td> 
   <td> <p> 输入或映射要创建列表的展示板的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL名称] </td> 
   <td> <p>输入或映射新列表的名称。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL位置] </td> 
   <td> <p>选择是将列表添加到卡片顶部还是将其附加到卡片底部。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL复制列表]</td> 
   <td> <p> 选择您要如何输入要复制的列表的ID。</p> 
    <ul> 
     <li> <p><strong>手动输入</strong> </p> <p>在 <strong>[！UICONTROL列表ID]</strong> 字段，输入或映射要复制的列表的ID。<br></p> </li> 
     <li> <p><strong>选择</strong> </p> <p>选择包含要复制的列表的主板，然后选择列表。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 编辑列表]**

此操作模块编辑现有列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关将您的[！UICONTROL Trello]帐户连接到 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL列表ID]</td> 
   <td> <p> 输入或映射要更新的列表的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL名称] </td> 
   <td> <p>输入或映射列表的新名称。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL展示板ID]</td> 
   <td> <p> 映射或选择要将列表移动到的展示板。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL位置] </td> 
   <td> <p>选择是将列表添加到卡片顶部还是将其附加到卡片底部。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL已订阅]</td> 
   <td> <p>如果要将活动成员订阅到该列表，请启用此选项。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 获取列表]**

此操作模块可检索有关特定列表的详细信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关将您的[！UICONTROL Trello]帐户连接到 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL列表ID]</p> </td> 
   <td> <p>输入或映射要检索相关信息的列表的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### 信息卡

+++ **[!UICONTROL 关注卡]**

在添加新信息卡时，此触发器模块处于激活状态。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关将您的[！UICONTROL Trello]帐户连接到 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL观察对象]</td> 
   <td> <p>选择要监视卡的位置。</p> 
    <ul> 
     <li><strong>[！UICONTROL所有卡片]</strong> </li> 
     <li> <p><strong>特定展示板上的信息卡</strong> </p> <p>选择要观察卡片的展示板</p> </li> 
     <li> <p><strong>[！UICONTROL卡特定列表]</strong> </p> <p>选择包含要监视卡片列表的展示板，然后选择列表。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td> <p>卡片的最大数量 [!DNL Workfront Fusion] 将在一个执行周期内返回。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 创建信息卡]**

此操作模块在选定列表中创建一个信息卡。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关将您的[！UICONTROL Trello]帐户连接到 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输入列表ID]</td> 
   <td> <p> 选择您希望如何输入要添加信息卡的列表的ID。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>在 <strong>[！UICONTROL列表ID]</strong> 字段中，输入或映射要添加信息卡的列表的ID。<br></p> </li> 
     <li> <p><strong>[！UICONTROL选择]</strong> </p> <p>选择包含要复制的列表的主板，然后选择列表。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL标签] </td> 
   <td> <p>对于要添加到卡片的每个标签，输入标签的ID。 例如，可以使用[！UICONTROL Retrieve Labels]模块检索ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL成员]</td> 
   <td>对于要添加到卡片中的每个成员，输入成员的ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL名称] </td> 
   <td> <p>输入新卡的名称。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL描述]</p> </td> 
   <td> <p>输入卡的说明。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL位置] </td> 
   <td> <p>选择是将信息卡添加到列表顶部还是将信息卡附加到列表底部。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL到期日期]</td> 
   <td> <p> 输入卡的到期日期。 有关支持的日期和时间格式的列表，请参阅 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">键入强制 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL到期结束]</td> 
   <td> <p> 启用此选项以在到期日标记卡已完成。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件URL]</td> 
   <td> <p>输入或映射要作为附件添加到信息卡的文件的URL。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL源文件]</p> </td> 
   <td> <p>为要作为附件添加到信息卡的文件输入或映射信息。</p> 
    <ul> 
     <li>[！UICONTROL文件名]：输入或映射文件名，包括文件扩展名。</li> 
     <li> 
     <p>从上一个模块中选择一个文件，或映射文件的名称和数据</p> 
     <p>注意：每个附件有10 MB的文件上传限制。 但是，[！UICONTROL Business Class]和[！UICONTROL Trello Gold]成员在每个附件中具有250 MB的文件上传限制。</p> 
     </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL复制卡]</td> 
   <td> <p> 选择您要如何输入要复制的卡片ID。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>在 <strong>[！UICONTROL卡ID]</strong> 字段中，输入或映射要复制的卡的ID。<br></p> </li> 
     <li> <p><strong>[！UICONTROL选择]</strong> </p> <p>选择包含要复制的卡的主板，然后选择包含该卡的列表，然后选择该卡。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 编辑信息卡]**

此操作模块编辑现有信息卡。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关将您的[！UICONTROL Trello]帐户连接到 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输入卡片ID]</td> 
   <td> <p> 选择您要如何输入要编辑的卡片ID。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>在 <strong>[！UICONTROL卡ID]</strong> 字段中，输入或映射要编辑的卡片ID。<br></p> </li> 
     <li> <p><strong>[！UICONTROL选择]</strong> </p> <p>选择包含要编辑的卡片的展示板，然后选择包含该卡片的列表，然后选择该卡片。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL新名称]</td> 
   <td> <p>输入或映射卡的新名称。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL新描述]</p> </td> 
   <td> <p>输入或映射信息卡的新描述。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL移动信息卡]</p> </td> 
   <td> <p>选择主板或主板，并列出您要移动卡的位置。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL标签] </td> 
   <td> <p>添加您要添加到卡片的任何标签的ID。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL位置] </td> 
   <td> <p>选择是将信息卡添加到列表顶部还是将信息卡附加到列表底部。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL到期日期]</td> 
   <td> <p> 输入卡的到期日期。 有关支持的日期和时间格式的列表，请参阅 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">键入强制 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL到期结束]</td> 
   <td> <p> 如果启用此选项，则卡在到期日期被标记为“完成”。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL成员] </td> 
   <td> <p>添加或映射要添加到卡片的任何成员的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL附件封面ID]</p> </td> 
   <td> <p>输入或映射您希望卡用作封面的图像附件的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL订阅] </td> 
   <td> <p>选择是否应订阅该会员卡。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL存档] </td> 
   <td> <p>选择一个选项以指示是否要存档（关闭）卡片。 </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 获取信息卡]**

此操作模块可检索选定信息卡的详细信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关将您的[！UICONTROL Trello]帐户连接到 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL展示板ID]</td> 
   <td> <p>输入包含要检索其详细信息的信息卡的主板的ID。 这允许您查看展示板的自定义字段的名称。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输入卡片ID]</td> 
   <td> <p> 选择您要如何输入检索其详细信息的卡的ID。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>在 <strong>[！UICONTROL卡ID]</strong> 字段，输入或映射要检索其详细信息的卡的ID。<br></p> </li> 
     <li> <p><strong>[！UICONTROL选择]</strong> </p> <p>选择包含要检索其详细信息的信息卡的主板，然后选择包含该信息卡的列表，然后选择该信息卡。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 搜索卡片]**

此操作模块返回与搜索查询匹配的卡片。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关将您的[！UICONTROL Trello]帐户连接到 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Board] </td> 
   <td> <p>选择要搜索的主板。 如果未选择展示板，则将搜索所有展示板。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL查询]</p> </td> 
   <td> <p>输入搜索查询。 您可以使用以下搜索运算符优化搜索：</p> 
    <ul> 
     <li><code><strong>-operator</strong></code> <p>您可以将“ — ”添加到任何运算符以进行负面搜索，例如 <code>[!UICONTROL -has:members]</code> 以搜索未分配任何成员的卡片。</p> </li> 
     <li><code><strong>@name</strong></code> <p>返回分配给成员的卡片。 您还可以使用 <code>member:</code>. 使用 <code>@me</code> 只包括你的卡片。</p> </li> 
     <li><code><strong>#label</strong></code> <p>返回标记的卡片。 您还可以使用 <code>label:</code>. 例如， <code>label:"FIX IT"</code> 将返回标签为“FIX IT”的卡。</p> </li> 
     <li><code><strong>board:id</strong></code> <p>返回特定展示板中的卡片。 例如， <code>board:Trello</code> 将返回展示板名称中带有[！UICONTROL Trello]的展示板上的卡片。</p> </li> 
     <li><code><strong>list:name</strong></code> <p>返回列表中名为“name”的卡片。</p> </li> 
     <li><code><strong>has:attachments</strong></code> <p>返回带有附件的卡片。 此 <code>has</code>：运算符也可以与其他属性一起使用，例如 <code>has:description</code>， <code>has:cover</code>， <code>has:members</code>，或 <code>has:stickers</code>.</p> </li> 
     <li><code><strong>due:day</strong></code> <p>返回24小时内到期的卡片。 此 <code>due:</code> 运算符也可以与其他时间范围一起使用，例如 <code>due:week</code>， <code>due:month</code>，或 <code>due:overdue</code>. 您还可以搜索特定的日期范围。 例如，添加 <code>due:14</code> 搜索包括未来14天内到期的卡。</p> </li> 
     <li><code><strong>created:day</strong></code> <p>返回过去24小时内创建的信息卡。 此<code> created:</code> 运算符也可以与其他时间范围一起使用，例如 <code>created:week</code> 或 <code>created:month</code>. 您还可以搜索特定的日期范围。 例如，添加 <code>created:14</code> 至搜索，包含过去14天中创建的信息卡。</p> </li> 
     <li><code><strong>edited:day</strong></code> <p>返回过去24小时内编辑的卡片。 此 <code>edited:</code> 运算符也可以与其他时间范围一起使用，例如 <code>edited:week</code> 或 <code>edited:month</code>. 您还可以搜索特定的日期范围。 例如，添加 <code>edited:21</code> 至搜索包含过去21天内编辑的卡片。</p> </li> 
     <li><code><strong>description:</strong>, <strong>checklist:</strong>, <strong>comment:</strong>, and <strong>name:</strong></code> <p>返回与信息卡描述、核对清单、注释或名称文本匹配的信息卡。 例如，评论：“FIX IT”将在评论中返回带有“FIX IT”的卡片。</p> </li> 
     <li><code><strong>is:open</strong> and <strong>is:archived</strong></code> <p>返回已打开或已存档的卡片。 如果未指定，则[！UICONTROL Trello]会返回这两种类型。</p> </li> 
     <li><code><strong>is:starred</strong> </code> <p>仅包括星型展示板上的信息卡。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL返回卡片的最大数量]</td> 
   <td> <p> 卡片的最大数量 [!DNL Workfront Fusion] 将在一个执行周期内返回。 该值必须小于或等于1000。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Partial] </td> 
   <td> <p>默认情况下，此模块会搜索成员内容，以查找查询中每个单词的完全匹配项。 启用[！UICONTROL Partial]后，模块会查找以查询中任意单词开头的内容。</p> <p> 例如，如果您使用单词“development”来查找标题为“My Development Status Report”的展示板，则默认情况下您需要搜索整个单词。 如果您启用了[！UICONTROL Partial]，则可以搜索“dev”，但不能搜索“velopment”。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL卡] </td> 
   <td> <p>添加要专门搜索的任何卡片。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 存档或取消存档信息卡]**

该操作模块将信息卡存档或发送回展示板。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关将您的[！UICONTROL Trello]帐户连接到 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL卡ID]</td> 
   <td> <p> 输入或映射要存档或发回展示板的卡片ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL存档或取消存档]</td> 
   <td> <p> 选择是要关闭卡片（存档）还是将其发送回展示板（取消存档）。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 添加附件]**

此操作模块将一个附件添加到选定的信息卡。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关将您的[！UICONTROL Trello]帐户连接到 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输入卡片ID]</td> 
   <td> <p> 选择您要如何输入检索其详细信息的卡的ID。</p> 
    <ul> 
     <li> <p><strong>手动输入</strong> </p> <p>在 <strong>[！UICONTROL卡ID]</strong> 字段，输入或映射要检索其详细信息的卡的ID。<br></p> </li> 
     <li> <p><strong>[！UICONTROL选择]</strong> </p> <p>选择包含要检索其详细信息的信息卡的主板，然后选择包含该信息卡的列表，然后选择该信息卡。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL附件类型]</p> </td> 
   <td> <p>选择是要直接上载文件，还是要提供文件的URL。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL文件]</strong> </p> <p>从上一个模块中选择一个源文件，或映射源文件的名称和数据。</p> </li> 
     <li> <p><strong>[！UICONTROL URL]</strong> </p> <p>输入文件的URL，并提供附件的名称。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

### 成员

+++ **[!UICONTROL 将成员分配给讨论区]**

参见“[!UICONTROL 将成员分配给讨论区]“，在 [讨论区](#boards).

+++

+++ **[!UICONTROL 从讨论区中取消分配成员]**

参见“[!UICONTROL 从讨论区中取消分配成员]“，在 [讨论区](#boards).

+++

+++ **[!UICONTROL 向信息卡添加成员]**

此操作模块将指定的成员添加到指定的信息卡。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关将您的[！UICONTROL Trello]帐户连接到 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL输入卡片ID和成员ID]</p> </td> 
   <td> <p>选择您希望如何输入卡片ID和成员ID。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>输入或映射 <strong>[！UICONTROL卡ID]</strong> 和 <strong>[！UICONTROL成员ID]</strong>.</p> </li> 
     <li> <p><strong>[！UICONTROL选择]</strong> </p> <p>选择包含要向其添加成员的卡片的展示板，然后选择包含该卡片的列表、卡片本身以及要添加到卡片的成员。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 搜索成员]**

此操作模块检索有关以下项的信息 [!UICONTROL 特雷洛] 成员。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关将您的[！UICONTROL Trello]帐户连接到 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查询] </td> 
   <td> <p>输入要查找的用户的全名或用户名。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Partial] </td> 
   <td> <p>默认情况下，此模块会搜索成员内容，以查找查询中每个单词的完全匹配项。 启用[！UICONTROL Partial]后，模块会查找以查询中任意单词开头的内容。</p> <p> 例如，如果您使用单词“development”来查找标题为“My Development Status Report”的展示板，则默认情况下您需要搜索整个单词。 如果您启用了[！UICONTROL Partial]，则可以搜索“dev”，但不能搜索“velopment”。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL返回成员的最大数目]</td> 
   <td> <p> 最大成员数 [!DNL Workfront Fusion] 将在一个执行周期内返回。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### 核对清单

+++ **[!UICONTROL 创建清单]**

此操作模块在选定的信息卡上创建核对清单。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关将您的[！UICONTROL Trello]帐户连接到 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输入卡片ID]</td> 
   <td> <p> 选择您希望如何输入要在其中添加清单的卡的ID。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>在 <strong>[！UICONTROL卡ID]</strong> 字段，输入或映射要添加清单的卡ID。<br></p> </li> 
     <li> <p><strong>[！UICONTROL选择]</strong> </p> <p>选择包含要在其中添加清单的卡的主板，然后选择包含该卡的列表，然后选择该卡。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL名称] </td> 
   <td> <p>输入或映射清单的名称。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL位置] </td> 
   <td> <p>选择是将清单添加到顶部，还是将[！UICONTROL]清单附加到卡底部。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL输入清单ID]</p> </td> 
   <td> <p>输入或映射要复制到新清单中的源清单的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 创建清单项目]**

此操作模块将一个项目添加到特定核对清单。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关将您的[！UICONTROL Trello]帐户连接到 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输入清单ID]</td> 
   <td> <p> 选择您希望如何输入要添加项目的清单的ID。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>在 <strong>[！UICONTROL核对清单ID]</strong> 字段，输入或映射要添加清单的卡ID。<br></p> </li> 
     <li> <p><strong>[！UICONTROL选择]</strong> </p> <p>选择包含要在其中添加清单的卡的主板，然后选择包含该卡的列表，然后选择该卡，然后选择清单。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL项名称]</p> </td> 
   <td> <p>输入或映射新项目的名称。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL位置]</p> </td> 
   <td> <p>选择是将项目添加到清单顶部还是将[！UICONTROL append]添加到清单底部。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL已选中]</p> </td> 
   <td> <p>如果要将项目添加为已选中，请启用此选项。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 编辑清单项目]**

此操作模块编辑现有核对清单。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关将您的[！UICONTROL Trello]帐户连接到 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输入卡片ID和清单项目ID]</td> 
   <td> <p> 选择您要如何输入卡的ID以及要在其中编辑项目的核对清单。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>在 <strong>[！UICONTROL核对清单ID]</strong> 字段，输入或映射要添加清单的卡ID。</p> <p>在 <strong>[！UICONTROL清单项目ID]</strong> 字段，输入或映射清单的ID。</p> </li> 
     <li> <p><strong>[！UICONTROL选择]</strong> </p> <p>选择包含要在其中添加清单的卡的主板，然后选择包含该卡的列表，然后选择该卡，然后选择清单。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL核对清单ID]</td> 
   <td>选择或映射要将清单项目移动到的清单。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL项名称]</p> </td> 
   <td> <p>输入或映射新项目的名称。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL位置]</p> </td> 
   <td> <p>选择是将项目添加到清单顶部还是附加到清单底部。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL状态]</p> </td> 
   <td> <p>选择清单项目是完整的还是不完整的。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### 标签

+++ **[!UICONTROL 向信息卡添加标签]**

此操作模块向选定的信息卡添加标签。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关将您的[！UICONTROL Trello]帐户连接到 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输入卡片ID]</td> 
   <td> <p> 选择您希望如何输入要在其中添加清单的卡的ID。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>在 <strong>[！UICONTROL卡ID]</strong> 字段，输入或映射要添加清单的卡ID。 在<strong>[！UICONTROL标签ID]</strong> 字段中，输入或映射要添加标签的ID。<br></p> </li> 
     <li> <p><strong>[！UICONTROL选择]</strong> </p> <p>选择包含要在其中添加清单的卡的主板，然后选择包含该卡的列表，然后选择该卡。 </p> <p>选择要添加到信息卡的标签。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

### 注释

+++ **[!UICONTROL 关注评论]**

当指定位置中有新评论时检索评论详细信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关将您的[！UICONTROL Trello]帐户连接到 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL观察对象]</td> 
   <td> <p>选择要监视备注的位置。</p> 
    <ul> 
     <li><strong>到处都是[！UICONTROL所有卡]</strong> </li> 
     <li> <p><strong>[！UICONTROL Board]</strong> </p> <p>选择要观察评论的讨论区</p> </li> 
     <li> <p><strong>[！UICONTROL列表]</strong> </p> <p>选择包含要监视其注释的列表的展示板，然后选择该列表。</p> </li> 
     <li><strong>[！UICONTROL卡]</strong> </li> 
     <li>选择包含要监视其注释的信息卡的主板，然后选择包含该信息卡的列表，然后选择该信息卡。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td> <p>评论的最大数量 [!DNL Workfront Fusion] 将在一个执行周期内返回。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 在信息卡中创建评论]**

此操作模块向选定的信息卡添加评论。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关将您的[！UICONTROL Trello]帐户连接到 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输入卡片ID]</td> 
   <td> <p> 选择您希望如何输入要在其中添加评论的卡片ID。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>在 <strong>[！UICONTROL卡ID]</strong> 字段中，输入或映射要添加评论的卡片ID。<br></p> </li> 
     <li> <p><strong>[！UICONTROL选择]</strong> </p> <p>选择包含要在其中添加注释的卡片的展示板，然后选择包含该卡片的列表，然后选择该卡片。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL注释] </td> 
   <td> <p>输入要添加到选定信息卡的注释。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 在信息卡中列出注释]**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关将您的[！UICONTROL Trello]帐户连接到 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输入卡片ID]</td> 
   <td> <p> 选择您希望如何输入要在其中添加评论的卡片ID。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>在 <strong>[！UICONTROL卡ID]</strong> 字段中，输入或映射要添加评论的卡片ID。<br></p> </li> 
     <li> <p><strong>[！UICONTROL选择]</strong> </p> <p>选择包含要在其中添加注释的卡片的展示板，然后选择包含该卡片的列表，然后选择该卡片。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL返回评论的最大数量]</td> 
   <td> <p> 输入最大评论数 [!DNL Workfront Fusion] 将在一个执行周期内返回。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL始自] </td> 
   <td> <p>设置创建评论时段的开始日期。 有关支持的日期和时间格式的列表，请参阅 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">键入强制 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Before] </td> 
   <td> <p>设置创建评论时段的结束日期。 有关支持的日期和时间格式的列表，请参阅 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">键入强制 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## [!UICONTROL 特雷洛] 对象Id

* [如何在中查找信息卡的ID或短链接 [!DNL Trello]](#how-to-find-the-id-or-the-shortlink-of-a-card-in-trello)
* [如何在中查找其他对象的ID [!DNL Trello]](#how-to-find-ids-of-other-objects-in-trello)

### 如何在中查找信息卡的ID或短链接 [!DNL Trello]

如果要编辑信息卡或创建新评论，您需要知道信息卡或其短链接的ID。 您可以从 [!UICONTROL 新信息卡] 触发器。 也可以通过打开信息卡并单击 [!UICONTROL 共享] 按钮。 可以在以下位置找到短链接： [!UICONTROL 链接至此信息卡] 框，在URL末尾的 `https://trello.com/c/`.

![](assets/share-and-more-350x575.png)

### 如何在中查找其他对象的ID [!DNL Trello]

讨论区、列表和评论ID只能使用触发器获取。 此 [!DNL trello.com] 网站不显示这些ID。
