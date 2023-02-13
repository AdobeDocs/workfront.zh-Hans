---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: 滞后类型概述
description: 滞后是在完成强制前置任务之后，在从属任务开始之前必须经过的时间量（正滞后），或者从属任务在前置任务开始之前可以开始的时间量（负滞后）。
author: Alina
feature: Work Management
exl-id: 9b3cac9a-1b8d-4697-b5d4-a2d669c790a9
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '1385'
ht-degree: 0%

---

# 滞后类型概述

滞后是在完成强制前置任务之后，在从属任务开始之前必须经过的时间量（正滞后），或者从属任务在前置任务开始之前可以开始的时间量（负滞后）。

后续任务的计划日期、预计日期和预计日期的计算考虑了前置任务的延迟日期和计划日期、预计日期和预计开始（完成）日期。

## 访问要求

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
   <td> <p>编辑对任务和项目的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理任务和项目的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 指示任务的滞后和滞后类型

在定义任务的前置关系时，可以指示任务的滞后类型。

* [在任务的“前置任务”部分中指示滞后类型](#indicate-lag-types-in-the-predecessors-section-of-a-task)
* [在任务列表中指示延迟类型](#indicate-lag-types-in-a-task-list)

### 在任务的“前置任务”部分中指示滞后类型 {#indicate-lag-types-in-the-predecessors-section-of-a-task}

1. 转到要定义前置任务和延迟类型的任务。
1. 单击 **前置任务** 中。 您可能需要单击 **显示更多**，然后 **前置任务**.
1. 单击 **添加前置项**.
1. （可选）如果要添加跨项目前置项，请将 **父项目** 名称。
1. 开始键入前置任务的名称，然后在该名称显示在列表中时将其选中。
1. 选择 **依赖关系类型**.

   有关前置依赖关系类型的详细信息，请参阅 [任务依赖关系类型概述](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. 指定 **滞后** 数量。 您可以指定负数来表示负滞后。
1. 从以下选项中进行选择，以确定您希望为上一代指明的延迟类型：

   * **天数**
   * **日历日**
   * **百分比**
   * **每周时间**
   * **每周时间（非零）**

      有关这些滞后类型及其计算方式的详细信息，请参阅部分 [滞后类型概述](#lag-types-overview) 在本文中。

1. 单击&#x200B;**保存**。

### 在任务列表中指示延迟类型  {#indicate-lag-types-in-a-task-list}

1. 转到任务列表，然后选择 **标准** 从 **查看** 下拉菜单。

1. 在 **前置任务** 列。
1. 输入以下内容，不带空格：

   * 要指示为所选任务的前置任务的任务数
   * 要在任务之间指示的依赖关系类型的缩写

      有关依赖关系类型缩写的详细信息，请参阅 [任务依赖关系类型概述](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

   * a **+** 表示正滞后或 **-** 负滞后

   * 滞后的量
   * 要使用的Lag Type的缩写。

      有关Lag Types缩写的详细信息，请参阅部分 [滞后类型概述](#lag-types-overview) 在本文中。
   例如，要指示某任务具有前置任务，且正滞后时间为2天，您可以输入

   ```
   1fs+2d
   ```

   在“前置项”列中。

1. 单击键盘上的Enter以保存对任务所做的更改。

## 滞后类型概述 {#lag-types-overview}

需要一段滞后时间的任务的一个示例可能是将树木锯成木材。 如果新切的木头必须干燥一段时间才能切割，那么在切割树木和锯成木材之间会有一段时间。

下表说明了滞后类型以及如何指示每种滞后类型的时间量：

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
   <td> <p>天数(d)</p> </td> 
   <td> <p>依赖关系链接的两个任务之间的延迟以工作天为单位进行测量。 这是默认的滞后类型。 </p> <p>例如，如果完成开始依赖项具有2个工作日延迟，而上一任务在星期五完成，则从属任务将在星期三开始。 周末的天数不算作滞后的一部分。 </p> <p>注意：天数的最大滞后限制为366。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>日历天数(c)</p> </td> 
   <td> <p>两项任务之间的延迟以日历天（包括节假日和周末）衡量。 </p> <p>注意：尽管此滞后类型将非工作日计为滞后的一部分，但从属任务永远不能在非工作日开始。 如果此滞后类型使从属任务在非工作日开始，则从属任务的“计划起始日期”将计划在下一个工作日开始。 </p> <p>例如，如果完成开始依赖项具有2个日历日延迟，而上一任务在星期四完成，则从属任务从星期一开始，而不是从星期日开始。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>百分比（p或pe）</p> </td> 
   <td> <p>延迟以完成前置任务的估计时间的百分比表示。 </p> <p>例如，如果在10天的前置任务上存在20%的延迟的完成开始依赖项，则系统将计算多少天是前置任务持续时间的20%，并将其用作滞后。 在这种情况下，任务完成后2天。 </p> <p>注意：百分比的最大滞后限制为2000%。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>每周时间(w) </p> </td> 
   <td> <p>两个任务之间的延迟通过指示一周中包含前置任务计划完成日期的天数来衡量。</p> <p>对于此滞后类型，一周中的每一天都与一个数字关联：</p> 
    <ul> 
     <li>星期日=1</li> 
     <li>星期一=2</li> 
     <li>星期二=3</li> 
     <li>星期三=4</li> 
     <li>星期四=5</li> 
     <li>星期五=6</li> 
     <li>星期六=7</li> 
    </ul> <p>如果要指明继任者的计划起始日期应位于当前周的星期二，并且星期二在前任的计划完成日期之前，您应使用以下公式对您的继任者进行编码： </p> <p><code style="font-style: normal;">4fs-3w</code> </p> <p>注意：如果在前一任务的计划完成日期的周内星期二过去，则后续任务的计划开始日期是该周的第一个可用工作日。 </p> <p>如果要指示滞后时间应在当周的星期六，并且星期六在上一代的计划完成日期之后，您应使用以下公式对您的继任者进行编码：</p> <p><code style="font-style: normal;">4fs+7w</code> </p> <p>如果星期六为非工作日，则选择星期六之后的下一个可用日期（以表示正滞后）作为后续计划的开始日期。 </p> <p>要指示过去或未来的周数，您可以在延迟类型的日数之前添加一个数字。 </p> <p>例如，要指示10周前的星期一，您可以使用此代码指示您的继任者的前身：</p> <p><code>4fs-102w</code> </p> <p>10表示10周前，2表示分配给星期一的编号。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>每周时间非零(k)</p> </td> 
   <td> <p>两个任务之间的延迟与“周”延迟类型的“日”相同，除非前一任务的时间在指定周的同一天结束。 然后，将滞后时间计算到相邻周(+/-)。 </p> <p>在这种情况下，滞后时间永远不能为0。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 负滞后概述

您可以使用负滞后指示任务需要或能力在前置任务结束之前开始。

使用负滞后时，请考虑以下规则：

* 负滞后不能强制任务的开始/结束日期在项目的计划开始/完成日期之前或之后。 这些日期在项目的“计划自”字段中指定。

   在这种情况下，请考虑以下事项：

   * 计划项目的完成日期。
   * 项目上的最后一个任务应使用任务约束上必须完成。 建议为任务指定足够长的持续时间，以便考虑项目上的所有任务。 其余任务在“尽快”约束下工作正常。

* 在任务中使用“完成 — 开始”前置任务关系可能会生成错误消息。

   在这种情况下，请考虑以下事项：

   * 在任务之间设置“完成 — 完成”前置关系。
   * 后续任务的持续时间应等于或超过任务之间预期的延迟天数。
