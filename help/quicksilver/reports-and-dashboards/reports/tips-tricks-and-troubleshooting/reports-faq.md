---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 报表常见问题解答
description: 报表常见问题解答
author: Nolan
feature: Reports and Dashboards
exl-id: 5e267d45-7922-4c0f-8530-59a8c152f625
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '1500'
ht-degree: 0%

---

# 报表常见问题解答

<!--Audited: 05/2025-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is the ONE anchor article for all FAQs about Reporting. Add a new FAQ in the TOC at the top first, then add the answer as a section at the bottom.)</p>
-->

以下是有关报表的常见问题解答。

## 访问要求

+++ 展开以查看访问要求。 

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>标准</p> 
   <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p>  </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 为什么我的小时差自定义计算没有在列中显示正确结果？

<!--this section is linked from the Actual Hours article for Tasks in the Task Information folder; edit the links or do not delete or change this section-->

在项目报告中，我有一个计算从计划小时数中减去实际小时数。

我得到的结果不正确。

<!--this changed with this issue in May 2025; Actual Hours changed from actualWorkRequired to actualWorkRequiredDouble: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/task/68108e860000120e90a79cb82e5811c2/updates : On a project report I have a calculation that subtracts Actual Hours (2) from Planned Hours (4). The result I am getting is 120 when it should be 2.  -->

我的计算是：

`valueexpression=SUB(workRequired,actualWorkRequired)`

### 答案

在Workfront中，大多数使用小时数的字段都以分钟为单位存储。 在计算中使用这些字段时，结果通常以分钟为单位。 要获得以小时为单位的结果，必须将计算结果或所引用的字段除以60。

计划小时数以分钟为单位存储。

根据计算时要使用的“实际小时数”字段，正确的公式包括：

* 对于以分钟为单位存储的旧版实际小时数：

  `valueexpression=SUB(workRequired,actualWorkRequired)/60`

* 对于以小时存储的实际小时：

  `valueexpression=SUB(workRequired/60,actualWorkRequiredDouble)`

有关详细信息，请参阅[查看实际小时数](/help/quicksilver/manage-work/tasks/task-information/actual-hours.md)。

## 为什么报表中我的每个图表元素的值都没有显示在图表上？

### 答案

如果报表图中有超过50个图表元素，则图表不会显示每个元素的值。

当图表中的元素少于50个时，每个元素的值都会显示在图表中。 请考虑添加过滤器或修改报告中的分组，以限制您在图表每个元素中显示的项目数。

## 为什么我的报告返回的结果太多，无法显示图表？

运行带有图表的报告时，我看到错误消息“哇……此报表返回了大量数据，因此图表不可读。 考虑通过添加过滤器或更改图表中的分组来缩小结果范围。”

### 答案

此错误意味着您的图表最多包含618个不同的结果，例如，条形图中有超过618个条形。 要解决显示问题，您需要通过修改当前过滤器和分组选择来优化结果。

有关修改筛选器和分组的信息，请参阅Adobe Workfront中的文章[筛选器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)和[分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)。

## 为什么当我作为同事访问同一报表（或日历）时，我看到我的任务（或问题），而他们却看到其任务？

### 答案

报告或日历可能具有指向已登录用户的通配符筛选器变量。 在这种情况下，报表会根据登录的用户显示信息。 调整筛选器以删除指向已登录用户的通配符。\
![用户ID筛选器变量](assets/qs--user.id-filter-variable-350x79.png)

有关基于用户的通配符筛选器变量概述的完整列表，请参阅[通配符筛选器变量概述](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)。

## 为什么我的报告中的数据不完整？

### 答案

大多数情况下，如果您的访问权限有限，导致无法查看系统中的项目，就会发生这种情况。 此外，您想要查看的项目不会与您共享。

报告的创建者可以编辑报告，以使用系统管理员或有权查看数据的任何“计划”用户的访问权限运行报告。

有关详细信息，请参阅[以其他用户的访问权限运行并交付报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md)。

## 我如何报告分配到的任务（或问题），无论我是否为这些任务的所有者？

### 答案

要查看分配给您的所有任务或问题，无论您是否是所有者（或主要受让人），请在任务或问题报表中使用以下过滤器：

1. 访问任务或问题报告。
1. 在&#x200B;**筛选器**&#x200B;选项卡上，单击&#x200B;**添加筛选器规则**。

1. 在&#x200B;**开始键入字段名称……**&#x200B;字段中，开始键入&#x200B;**任务用户名**，然后当它出现在列表中时将其选定。

   >[!NOTE]
   >
   >请勿使用&#x200B;**分配给名称**&#x200B;字段，因为此筛选器仅适用于您为主要被分配人或所有者的任务和问题。

1. 选择&#x200B;**Equal**&#x200B;修饰符。
1. 在文本框中开始键入&#x200B;*$$USER.ID*，并从显示的下拉列表中选择它。\
   这可确保您看到分配给登录用户的所有任务和问题。 您可以使用特定用户名替换通配符。\
   ![分配给我的任务](assets/qs-tasks-assigned-to-me-assignment-users-name-filter-350x63.png)

1. 单击&#x200B;**保存+关闭**。

## 为什么添加问题/添加任务链接未出现在项目中的问题和任务列表的底部？

### 答案

首先，确保您拥有将问题和任务添加到项目的正确访问和权限。 在这种情况下，您应该会在&#x200B;**问题**&#x200B;和&#x200B;**任务**&#x200B;列表的底部看到&#x200B;**添加问题**&#x200B;和&#x200B;**添加任务**&#x200B;链接。

但是，有些内容可能会阻止显示这些链接：

* 如果将快速过滤器应用于这些列表，则不会显示链接。 移除快速过滤器并显示链接，这样您就可以将问题和任务添加到项目中。\
  有关快速过滤器的信息，请参阅[开始使用Adobe Workfront中的列表](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)。

* 如果对这些列表应用了&#x200B;**分组**，则不会显示链接。 移除&#x200B;**分组**，并且应该显示链接，以便您可以将问题和任务添加到项目中。\
  有关创建分组的信息，请参阅Adobe Workfront中的[分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)。

* 如果将&#x200B;**视图**&#x200B;应用于这些列表，并且该列表选择了项目默认货币以外的货币，则不会显示链接。 将&#x200B;**视图**&#x200B;更改为&#x200B;**项目的原始货币**，将显示链接，以便您可以将问题和任务添加到项目中。\
  有关更改视图中的货币的详细信息，请参阅[创建具有唯一汇率的财务数据报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md)。

![项目货币](assets/nwe-project-original-currency-350x229.png)

## 我的报表或仪表板中的信息是否会自动刷新？

### 答案

报表或功能板中的信息不会自动刷新。

可在缓存的报表中手动刷新信息。\
有关刷新缓存报表的详细信息，请参阅[运行报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-report.md)。

信息可在缓存的仪表板中手动刷新。\
有关刷新缓存仪表板的更多信息，请参阅文章[仪表板入门](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md#running-dashboards)中的[显示仪表板](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md)部分。

## 我可以更改报告的所有者吗？

### 答案

您无法更改报告的所有者。 但是，创建报告的用户可以允许其他用户编辑报告。 允许用户编辑报告的方式取决于您所在的用户类型。

* 系统管理员可以通过将“报告”行中的“编辑”选项配置为包含创建报告的访问权限，来允许具有“计划”许可证的用户编辑报告。\
  有关详细信息，请参阅[授予对报告、功能板和日历的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)。

* 任何有权创建和共享报告的最终用户都可以通过共享报告并授予其他用户管理权限，允许其他人编辑个别报告。\
  有关详细信息，请参阅[在Adobe Workfront中共享报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)。

如果您有权查看或管理报表，则还可以创建该报表的副本，默认情况下您是报表的所有者。 要了解有关复制报告的详细信息，请参阅[创建报告副本](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md)。

## 为何无法访问已停用用户拥有的报表？

### 答案

有时，报告的所有者也是在报告上的&#x200B;**Run this report with Access Rights of：**&#x200B;字段中指定的用户。 如果停用具有&#x200B;**用户访问权限的**&#x200B;运行此报告，则与其共享报告的用户不再显示该报告。 发生这种情况时，您可以将&#x200B;**Run this Report with the Access Rights of：** blank保留为空或在字段中输入活动用户，以使报告可再次访问。

要了解有关&#x200B;**使用**&#x200B;字段的访问权限运行此报告的详细信息，请参阅[使用其他用户的访问权限运行并交付报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md)。 有关识别已停用用户拥有的所有报表的信息，请参阅[创建报表活动报表](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md)。

## 如何访问包含已删除用户所拥有报表的仪表板？

### 答案

在删除用户时，您仍然可以访问他们创建的任何报告，但是，也会删除包含该报告的任何仪表板。 这意味着您无法再访问以下内容：

* 包含报表（包括对象左侧面板中的仪表板）的仪表板

若要了解有关删除用户影响的更多信息，请参阅[删除用户](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md)。

如果您具有报表的“查看”访问权限，则可以执行以下操作：

1. 创建报告副本。\
   要了解如何创建报告副本，请参阅[创建报告副本](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md)。

1. 更新仪表板以包含复制的报告。\
   要了解如何编辑仪表板，请参阅[编辑仪表板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/edit-dashboard.md)。
