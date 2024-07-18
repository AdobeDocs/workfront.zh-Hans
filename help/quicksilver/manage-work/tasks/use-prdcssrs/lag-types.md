---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: 滞后类型概述
description: 滞后是指在强制前置任务完成后，直到相关任务可以开始之前必须经过的时间（正滞后时间），或者相关任务在前置任务开始之前可以开始的时间（负滞后时间）。
author: Alina
feature: Work Management
exl-id: 9b3cac9a-1b8d-4697-b5d4-a2d669c790a9
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '1476'
ht-degree: 0%

---

# 滞后类型概述

<!-- Audited: 01/2024 -->

滞后是指前置任务计划完成之后必须经过多长时间，直到相关任务可以开始（正滞后时间），或者相关任务在前置任务开始之前可以开始的时间（负滞后时间）。

后续任务的计划、预计和预计日期的计算考虑到了前置任务的滞后时间和计划、预计和预计开始（完成）日期。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<!--drafted - replace table at P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

您必须具有以下权限才能执行本文中的步骤：

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
   <td><p>新增：标准</p>
       <p>或</p>
       <p>当前：计划 </p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对任务和项目的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理任务和项目的权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 指示任务的滞后和滞后类型

在定义任务的前置任务关系时，可以在任务上指示滞后类型。

### 在任务的“前置任务”部分中指示滞后类型 {#indicate-lag-types-in-the-predecessors-section-of-a-task}

1. 转到要为其定义前置任务和滞后类型的任务。
1. 单击左侧面板中的&#x200B;**前置任务**。 您可能需要单击&#x200B;**显示更多**，然后单击&#x200B;**前置任务**。
1. 单击&#x200B;**添加前置任务**。
1. （可选）如果要添加跨项目前置任务，请将&#x200B;**父项目**&#x200B;名称替换为其他项目。
1. 开始键入前置任务的名称，然后将其在列表中显示时选定。
1. 选择&#x200B;**依赖关系类型**。

   有关前置任务依赖关系类型的详细信息，请参阅[任务依赖关系类型概述](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)。

1. 使用数值指定&#x200B;**Lag**&#x200B;值。 您可以指定负数来指示负延迟。
1. 从以下选项中进行选择，以确定要为前置任务指定的滞后类型：

   * **天**
   * **日历日**
   * **百分比**
   * 一周中的&#x200B;**天**
   * 每周的&#x200B;**天（非零）**

     有关这些Lag类型及其计算方式的更多信息，请参阅本文中的[Lag类型](#lag-types)部分。

1. 单击&#x200B;**保存**。

### 在任务列表中指示滞后类型  {#indicate-lag-types-in-a-task-list}

1. 转到任务列表，然后选择&#x200B;**标准**&#x200B;视图。

1. 单击与要为其指定前置任务和延迟量的任务对应的&#x200B;**前置任务**&#x200B;列。
1. 输入以下内容（不含空格）：

   * 要指定为所选任务的前置任务的任务编号
   * 要在任务之间指示的依赖关系类型的缩写

     有关依赖项类型缩写的详细信息，请参阅[任务依赖项类型概述](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)。

   * 正滞后为&#x200B;**+**&#x200B;或负滞后为&#x200B;**-**

   * 滞后时间
   * 要使用的Lag类型的缩写

     有关Lag类型的缩写的详细信息，请参阅本文中的[Lag类型](#lag-types)部分。

   例如，要指示某个任务具有前置任务且正滞后时间为2天，您应在“前置任务”列中输入`1fs+2d`。

1. 按键盘上的Enter键保存对任务所做的更改。

## 滞后类型 {#lag-types}

例如，一项需要延迟时间的任务可能会将树锯成木材。 如果新砍的木头在砍伐之前必须干燥一段时间，那么从砍伐树木到把它们锯成木头之间就会有一个滞后时间。

下表说明了滞后类型以及如何指示每种滞后类型的时间：

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <td> <p><strong>值</strong> </p> </td> 
   <td> <p><strong>描述</strong> </p> </td> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>天数（d或de）</p> </td> 
   <td> <p>通过依赖关系链接的两个任务之间的延迟以工作日计算。 这是默认的Lag类型。 </p> <p>例如，如果有一个滞后时间为2个工作日的完成 — 开始依赖项，而前置任务在星期五结束，则依赖项任务在星期三开始。 周末的天数不算滞后时间。 </p> <p>注意：最大滞后天数为366。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>日历日（c或ce）</p> </td> 
   <td> <p>两项任务之间的延迟以日历日衡量，包括假日和周末。 </p> <p>注意：尽管此滞后类型将非工作日计为滞后的一部分，但相关任务绝对不能在非工作日开始。 如果此滞后类型使相关任务在非工作日开始，则相关任务的计划起始日期安排在下一个工作日。 </p> <p>例如，如果某个具有2天日历延迟的完成 — 开始依赖关系，而前置任务在星期四结束，则依赖任务在星期一而不是星期日开始。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>百分比（p或pe）</p> </td> 
   <td> <p>延迟以估计完成前置任务所需时间的百分比表示。 </p> <p>例如，如果某个完成 — 开始相关性在10天的前置任务上有20%的延迟，则系统将计算多少天表示前置任务任务任务持续时间的20%，并将其用作延迟。 在这种情况下，它将在任务完成后2天后执行。 </p>

<p><b>注释</b></p> 百分比的最大滞后时间限制为2000%。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>每周时间（w或we） </p> </td> 
   <td> <p>通过指定包含前置任务计划完成日期的一周中某天，可以测量两个任务之间的延迟。</p> <p>对于此滞后类型，一周中的每一天都与一个数字关联：</p> 
    <ul> 
     <li>星期日=1</li> 
     <li>星期一=2</li> 
     <li>星期二=3</li> 
     <li>星期三=4</li> 
     <li>星期四=5</li> 
     <li>星期五=6</li> 
     <li>星期六=7</li> 
    </ul> <p>如果要指明接替者的计划开始日期应位于本周的星期二，并且星期二早于前身的计划完成日期，则可以使用以下公式为接替者编码： </p> <p><code style="font-style: normal;">4fs-3w</code> </p>

<p><b>注释</b></p>

如果后续任务的开始日期计算为某一星期的某一星期二，并且过去一周的某一天，则后续任务的计划开始日期为下周的同一天（星期二）（如果可用）。 </p> <p>如果要指示滞后时间应位于本周的某个星期六，并且该星期六在前置任务的计划完成日期之后，则可以使用以下公式为后置任务编码：</p> <p><code>4fs+7w</code> </p> <p>如果星期六是非工作日，则选择星期六之后的下一个可用日（以指示正滞后时间）作为接替者的计划开始日期。 </p>

<p>这不适用于计划例外。 如果日期也是计划例外，并且后续任务的开始日期计算为当天，则系统会尝试查找最近的可用日期，即前置任务表达式中指定的周中某日。</p>

<p>例如，如果“开始日期”计算为某个星期二，并且该日期为计划例外，且前置任务的滞后时间为正，则它会选择以下星期二（如果该日期也是工作日）作为后置任务的开始日期。 如果滞后时间为负，则系统会选择前一个星期二作为开始日期。</p>

<p>要指示过去或未来周，您可以在滞后类型的天数字前添加一个数字。 </p> <p>例如，要指示10周前的星期一，您可以使用此代码指示后继者的前置任务：</p> <p><code>4fs-102w</code> </p> <p>10表示10周前，2是分配给星期一的数字。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>非零周中的日（k或ke）</p> </td> 
   <td> <p>两个任务之间的延迟的度量方式与“星期”延迟类型相同，但如果前置任务的时间在指定周的同一天结束，则不在此限。 然后计算到相邻周的滞后时间(+/-)。 </p> <p>在这种情况下，滞后时间不能为0。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 负滞后时间

您可以使用负滞后时间指示任务在前置任务结束之前开始的必要性或能力。

使用负滞后时，请考虑以下规则：

* 负滞后不能强制任务的开始/完成日期早于或晚于项目的计划开始/完成日期。 这些日期在项目的“时间表开始日期”字段中指定。

  在这种情况下，请考虑以下事项：

   * 从完成日期开始计划项目。
   * 项目的最后一个任务应使用“必须完成任务限制”。 建议为任务指定足够的持续时间，以便考虑项目中的所有任务。 剩余的任务与“尽快”限制配合使用。

* 将“完成 — 开始”前置任务关系与任务结合使用可能会产生错误消息。

  在这种情况下，请考虑以下事项：

   * 在任务之间设置“完成 — 完成”前置任务关系。
   * 后续任务的持续时间应等于或超过任务之间预期滞后天数。
