---
user-type: administrator
product-area: system-administration;projects
keywords: kickstart，kick-start，kickstarts，kick-starts
navigation-topic: use-kick-starts
title: Kick-Starts方案：简单的项目和任务导入准备
description: 详细描述使用Kick Start方法导入基本项目和任务时可用的设置和控件。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c095ce9d-b189-449b-bd13-2633837697ed
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '1493'
ht-degree: 8%

---

# 快速启动方案：简单的项目和任务导入准备

详细描述了使用Kick-Start方法导入基本项目和任务时可用的设置和控件。

## 方案

实施团队宁愿导入活动项目的项目和任务信息，而不是手动将此数据输入到系统中。

* [项目](#projects)
* [任务列表](#task-list)

### 项目 {#projects}

下表显示了四个项目及其需要映射到Kick Start文件格式的基本详细信息。

此方案假定用户已导入Adobe Workfront。 如果用户尚未在Workfront中，请将其他名称替换为此方案，或者在此方案之前使用用户完成快速启动方案。

1. 实施Workfront。

   | 计划开始日期 | 今天 |
   |---|---|
   | 项目经理 | 詹妮弗·坎贝尔 |
   | 项目赞助者 | 马克·刘易斯 |
   | 组 | 营销 |
   | 公司 | *您的公司* |

   {style="table-layout:auto"}

1. 实施人力资源系统。

   | 计划开始日期 | 20xx年7月14日 |
   |---|---|
   | 项目经理 | 帕姆·雷诺兹 |
   | 项目赞助者 | 马克·刘易斯 |
   | 组 | 营销 |
   | 公司 | *您的公司* |

   {style="table-layout:auto"}

1. 实施文档管理系统。

   | 计划开始日期 | 20xx年8月22日 |
   |---|---|
   | 项目经理 | 詹妮弗·坎贝尔 |
   | 项目赞助者 | 雷·安德鲁 |
   | 组 | IT |
   | 公司 | *您的公司* |

   {style="table-layout:auto"}

1. 实施新的日历系统。

   | 计划开始日期 | 20xx年9月6日 |
   |---|---|
   | 项目经理 | 帕姆·雷诺兹 |
   | 项目赞助者 | 雷·安德鲁 |
   | 组 | IT |
   | 公司 | *您的公司* |

   {style="table-layout:auto"}

### 任务列表 {#task-list}

以下任务列表显示了项目过于简化的任务列表。 项目之间的唯一区别是每个项目的开始日期和进度。

父任务继承子任务的持续时间、工作和完成百分比。 无需为将成为摘要任务的设置这些值。

>[!NOTE]
>
>此方案中提供的说明没有在[Kick-Starts方案](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-company-group-role-user-prep.md)中提供的分步说明那样明确：公司、组、角色和用户快速启动准备。 假设您已了解如何从公司和组表中查找和复制值，因此将提到这些步骤，但并未具体说明。

1. 配置。
1. 导入用户。

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">任务负责人</td> 
      <td>雷·安德鲁</td> 
     </tr> 
     <tr> 
      <td role="rowheader">父任务</td> 
      <td>1</td> 
     </tr> 
     <tr> 
      <td role="rowheader">持续时间</td> 
      <td>1 小时</td> 
     </tr> 
     <tr> 
      <td role="rowheader">工作</td> 
      <td>1 小时</td> 
     </tr> 
     <tr> 
      <td role="rowheader">完成百分比</td> 
      <td> <p>Workfront： 0%</p> <p>HR： 100%</p> <p>文档： 100%</p> <p>日历：100%</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 设置权限。

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">任务负责人</td> 
      <td>雷·安德鲁</td> 
     </tr> 
     <tr> 
      <td role="rowheader">父任务</td> 
      <td>1</td> 
     </tr> 
     <tr> 
      <td role="rowheader">前置任务</td> 
      <td>2</td> 
     </tr> 
     <tr> 
      <td role="rowheader">持续时间</td> 
      <td>1 小时</td> 
     </tr> 
     <tr> 
      <td role="rowheader">工作</td> 
      <td>1 小时</td> 
     </tr> 
     <tr> 
      <td role="rowheader">完成百分比</td> 
      <td> <p>Workfront： 0%</p> <p>HR： 100%</p> <p>文档： 100%</p> <p>日历：100%</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 构建组。

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">任务负责人</td> 
      <td>雷·安德鲁</td> 
     </tr> 
     <tr> 
      <td role="rowheader">父任务</td> 
      <td>1</td> 
     </tr> 
     <tr> 
      <td role="rowheader">前置任务</td> 
      <td>4</td> 
     </tr> 
     <tr> 
      <td role="rowheader">持续时间</td> 
      <td>2 天</td> 
     </tr> 
     <tr> 
      <td role="rowheader">工作</td> 
      <td>4小时</td> 
     </tr> 
     <tr> 
      <td role="rowheader">完成百分比</td> 
      <td> <p>Workfront： 0%</p> <p>HR： 100%</p> <p>文档： 100%</p> <p>日历：25%</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 准备培训。

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">任务负责人</td> 
      <td>克里斯·曼宁</td> 
     </tr> 
     <tr> 
      <td role="rowheader">持续时间</td> 
      <td>2 天</td> 
     </tr> 
     <tr> 
      <td role="rowheader">工作</td> 
      <td>4小时</td> 
     </tr> 
     <tr> 
      <td role="rowheader">完成百分比</td> 
      <td> <p>Workfront： 0%</p> <p>HR： 100%</p> <p>文档：50%</p> <p>日历：100%</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 构建持续的支持策略。

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">任务负责人</td> 
      <td>克里斯·曼宁</td> 
     </tr> 
     <tr> 
      <td role="rowheader">持续时间</td> 
      <td>2 天</td> 
     </tr> 
     <tr> 
      <td role="rowheader">工作</td> 
      <td>4小时</td> 
     </tr> 
     <tr> 
      <td role="rowheader">完成百分比</td> 
      <td> <p>Workfront： 0%</p> <p>HR： 100%</p> <p>文档：50%</p> <p>日历： 0%</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 转出。

   | 前置任务 | 1， 6， 7 |
   |---|---|

   {style="table-layout:auto"}

1. 培训用户。

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">任务负责人</td> 
      <td>克里斯·曼宁</td> 
     </tr> 
     <tr> 
      <td role="rowheader">父任务</td> 
      <td>8</td> 
     </tr> 
     <tr> 
      <td role="rowheader">持续时间</td> 
      <td>1 天</td> 
     </tr> 
     <tr> 
      <td role="rowheader">工作</td> 
      <td>2 小时</td> 
     </tr> 
     <tr> 
      <td role="rowheader">完成百分比</td> 
      <td> <p>Workfront： 0%</p> <p>HR： 0%</p> <p>文档： 0%</p> <p>日历： 0%</p> </td> 
     </tr> 
    </tbody> 
   </table>

## 下载模板

转到Kick-Starts页面。 选择公司、组、项目、任务和用户对象。 选中包括现有数据复选框（执行此操作可快速引用公司、组和用户ID）。 单击“Download（下载）”按钮。

## 输入项目详细信息

打开您刚刚下载的Workfront.xlsx文件。 转到“项目项目”工作表。

![项目项目集](assets/im2.png)
除非您已经在Workfront中创建项目，否则它应为空。

![空项目表](assets/im10.png)

设置以下项目字段的值：

* **设置isNew列**
将isNew列的TRUE输入到第3行到第6行中。
* **设置唯一ID**
在ID列的每行中输入一个唯一的ID — 通常，创建新记录时，从1开始的整数可正常工作。
* **设置项目名称**
将每个项目的名称输入到setName列中。
* **设置项目计划**

  在setScheduleID字段中输入您希望项目使用的计划ID

* **设置项目计划开始日期**

  在setPlannedStartDate列中输入日期和时间以及您希望项目开始的时间和日期。 如果留空，Workfront将根据浏览器的时区导入项目，其中包含当天的日期和当天午夜的时间戳。

* **设置任务编号**
将值输入到setTaskNumber列中，以控制任务在项目计划中的显示顺序。
* **提供项目日期。**
在setPlannedStartDate列中为每个项目输入计划开始日期。
* **设置其他所需的详细信息。**
根据需要填写其他详细信息，例如描述或当前状态。 在“组ID”工作表中查找每个项目的组ID，并将其输入各个项目的setGroupID列。 在CMPY公司页上查找项目的公司ID，并将其输入到setCompanyID列中。 在“用户用户”工作表中查找每个项目所有者的用户ID，并将其输入到setOwnerID列中。 在用户用户工作表中查找每个项目发起人的用户ID，并将其输入到setSponsiderID列中。

![设置值](assets/im9.png)

>[!NOTE]
>
>通过查看Workfront的“工作流设置”区域中每个对象的状态和优先级首选项，可以找到“状态”和“优先级”字段的可接受值。

## 输入任务详细信息

在使用kick-starts导入项目时，您可以添加有关项目任务的信息。

打开您刚刚下载的Workfront.xlsx文件。 **转到“任务”工作表。**

除非您已在Workfront中创建任务，否则此工作表应为空。

![任务表](assets/im8.png)

![空任务表](assets/im7.png)

![任务表列](assets/im6.png)

映射任务的最简单方法是一次映射一个项目（尤其是当每个项目中的任务相同时）。 然后，您可以复制第一个项目的任务计划，并对后续项目的任务计划进行细微调整。 其余步骤将假定您仅为实施Workfront项目创建任务。 根据此方案，您将为每个项目导入9个任务，因此请将TRUE输入到isNew列的第3行至第11行中。

设置以下任务字段的值：

* **设置ID**
在ID列的每一行中输入一个唯一的ID。
* **设置名称**
将任务名称输入到setName列中。
* **确认项目ID**
输入您为实施Workfront项目设置的ID；查看PROJ项目表以确保该ID正确无误。
* **设置用户**
转到“用户”工作表查找分配给每个任务的用户的ID，并在setAssignedToID列的相应单元格中输入这些值。
* **识别任务关系**
对于任务2至5，在setParentID列中输入1。 对于任务9，在setParentID列中输入8。 在setPrecedousString列中，输入每个前置任务的任务编号。 如果一个任务有多个前置任务，例如此场景中的任务8，您需要使用逗号分隔每个前置任务ID。 通过使用创建前置任务关系一文中所述的简写，可以在非完成 — 开始关系上使用滞后来定义前置任务。
* **设置持续时间**
通过在setDuration字段中输入任务的小时数、天数、周数或月数来设置每个任务的持续时间。 然后在setDurationUnit字段中输入持续时间单位。

  |   | 可接受值 |
  |---|---|
  | 分钟 | 一 |
  | 小时 | H |
  | 天数 | D |
  | 周 | 星期- |
  | 月 | T |

  分钟数也可以表示为一小时的小数（例如，分钟数= 5小时）

* 在setWorkRequired字段中设置每个任务的工作量。 然后在setWorkUnit字段中输入工作单位。 如果“要求工作”值与duration不同，则还需要在setDurationType字段中输入A。

  | 持续时间类型 | 可接受值 |
  |---|---|
  | 计算的分配量 | A |
  | 计算的工作量 | 星期- |
  | 投入比导向 | D |
  | 简单 | S |

* 在每个任务的setPercentComplete字段中输入完成百分比的整数表示形式。 此值不应包括百分比符号(%)。
* 根据需要，为您正在创建的每个Task包括说明和其他详细信息。

  ![添加详细信息](assets/im5.png)

* setPlannedStartDate和setTaskConstraint列不用于构建此项目的时间线，因为我们依赖前置任务关系。 您可以为每个任务输入日期。 如果这样做，请确保还在setTaskConstraint列中提供了有效的任务限制。 有关此字段有效值的详细信息，请查看任务约束和相关文章。

  在此情况下，为要导入的其他项目构建任务的最简单方法是复制您刚刚定义的任务并将其粘贴到下方，从第12行开始。 然后，您将：

   1. 对ID列中的值重新编号。
   1. 将setProjectID列更新为您为下一个项目设置的值。
   1. 更新setParentID和setPredictiveString值以反映分配给此项目任务的新ID。
   1. 更新任务分配和完成百分比。
   1. 对下一个项目的任务重复这些步骤。

* **导入Excel文件**

  按照[使用快速启动模板](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)将数据导入Adobe Workfront中提供的说明进行操作。
