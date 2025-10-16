---
user-type: administrator
product-area: system-administration
keywords: kickstart，kick-start，kickstarts，kick-starts
navigation-topic: use-kick-starts
title: 使用快速启动模板将数据导入Workfront
description: Kick-Start是经过特殊格式设置的Excel工作簿，您可以用要导入Workfront的数据填充这些工作簿。 Adobe Workfront提供了一个快速启动模板，您可以使用它来执行此操作，如Kick-Starts数据导入程序中所述。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 25813946-e338-4dd9-b02c-d20fa18c539c
source-git-commit: 156341072c291b5c03432da399a509d9772b73ea
workflow-type: tm+mt
source-wordcount: '2828'
ht-degree: 6%

---

# 使用快速启动模板将数据导入Workfront

<!--Audited: 12/2023-->

Kick-Start是经过特殊格式设置的Excel工作簿，您可以用要导入Workfront的数据填充这些工作簿。 Adobe Workfront提供了一个快速启动模板，您可以使用它来执行此操作，如[快速启动数据导入器](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-data-importer.md)中所述。

此过程分为3个主要任务：

* 首先，将快速启动模板导出为电子表格文件
* 其次，使用您的数据填充电子表格
* 最后，将填充后的电子表格导入Workfront

本文按照适当的顺序概述了其中的每个过程。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p>
       <p>规划</p></td>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>系统管理员</td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 限制

您可以使用快速启动模板将大量对象导入Workfront。 但是，请考虑以下限制：

* 以这种方式导入数据不会更新Workfront中已存在的记录的信息。
* 您只能导入新记录及其信息。
* 一次导入不超过2,000条记录，以确保导入不会超时

## 将快速启动模板导出为电子表格文件

在导出快速启动模板时，您将收到一个空白的Excel电子表格工作簿。 在将电子表格下载到您的计算机后，您可以使用该电子表格填充您的信息，然后将其导入回Workfront。

要导出快速启动模板，请执行以下操作：

{{step-1-to-setup}}

<!--
1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).  -->

1. 单击&#x200B;**系统** > **导入数据(Kick-Start)**。

1. 选择要包括的信息类型。

   您选择的每个选项都表示导出电子表格中多个选项卡的集合。 例如，如果选择&#x200B;**报表**&#x200B;选项，则创建报表所需的所有对象都将包含在电子表格中（视图、筛选器、分组、报表）。

   您可以使用下面列出的所有对象类型将数据导入Workfront。 (唯一的例外是访问级别选项。 导出中的“访问级别”数据表仅供参考 — 允许您按ID为新用户帐户分配访问级别。)

   每种对象类型的模板都可以以下列文件格式导出，并包含以下工作表：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong>对象</strong> </p> </th> 
      <th> <p><strong>导出为</strong> </p> </th> 
      <th> <p>导出电子表格中的<strong>工作表</strong> </p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col"> <p>功能板</p> <p>系统中所有公开共享的报告面板都可以导出。 无法在系统范围内导出非共享功能板。 在一次导出中，最多可以选择100个特定仪表板。</p> </td> 
      <td scope="col">导出为ZIP文件</td> 
      <td scope="col"> <p>参数</p> <p>说明文本</p><p>参数选项</p> <p>参数组</p> <p>类别参数</p> <p>类别</p> <p>报表</p> <p>门户选项卡部分</p> <p>功能板</p> <p>首选项</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>报表</p> <p>系统中的所有报告都可导出。 在单个导出中，最多可以选择100个特定报告。</p> <p>Kick-Starts不支持文本模式过滤器或分组。 为了成功导出，必须将报表过滤器和分组切换到“标准模式”。</p> </td> 
      <td scope="col">导出为ZIP文件 </td> 
      <td scope="col"> <p scope="col">参数</p> <p scope="col">说明文本</p> <p scope="col">参数选项</p> <p scope="col">参数组</p> <p scope="col">类别参数</p> <p scope="col">类别</p> <p scope="col">报表</p> <p scope="col">首选项</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>审批</p> </td> 
      <td scope="col"> <p>导出为Excel文件</p> </td> 
      <td scope="col"> <p>阶段审批者</p> <p>审批阶段</p> <p>审批</p> <p>审批流程</p> <p>首选项</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>自定义数据</p> </td> 
      <td scope="col"> <p>导出为Excel文件</p> </td> 
      <td scope="col"> <p>参数</p> <p>说明文本</p>  <p>参数选项</p> <p>参数组</p> <p>类别参数</p> <p>类别</p> <p>首选项</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>费用类型</p> </td> 
      <td scope="col"> <p>导出为Excel文件</p> </td> 
      <td> <p>费用类型</p> <p>首选项</p> </td> 
     </tr> 
     <tr> 
      <td> <p>小时数类型</p> </td> 
      <td scope="col"> <p>导出为Excel文件</p> </td> 
      <td> <p>小时数类型</p> <p>首选项</p> </td> 
     </tr> 
     <tr> 
      <td> <p>团队</p> </td> 
      <td scope="col"> <p>导出为Excel文件</p> </td> 
      <td> <p> 团队成员</p> <p>团队</p> <p>首选项 </p> </td> 
     </tr> 
     <tr> 
      <td> <p>用户</p> </td> 
      <td> <p>导出为Excel文件。 要查看完整的选项列表，请单击<strong>更多选项</strong>。</p> </td> 
      <td> <p>用户</p> <p>首选项</p> </td> 
     </tr> 
     <tr> 
      <td>访问级别</td> 
      <td>导出为Excel文件</td> 
      <td> <p>访问级别</p> <p>首选项</p> </td> 
     </tr> 
     <tr> 
      <td>任务分配</td> 
      <td>导出为Excel文件</td> 
      <td> <p>任务分配</p> <p>首选项</p> </td> 
     </tr> 
     <tr> 
      <td>公司</td> 
      <td>导出为Excel文件</td> 
      <td> <p> 公司</p> <p>首选项 </p> </td> 
     </tr> 
     <tr> 
      <td>电子邮件模板</td> 
      <td>导出为Excel文件</td> 
      <td> <p>电子邮件模板</p> <p>首选项 </p> </td> 
     </tr> 
     <tr> 
      <td>费用</td> 
      <td>导出为Excel文件</td> 
      <td> <p> 费用'</p> <p>首选项 </p> </td> 
     </tr> 
     <tr> 
      <td>外部页面</td> 
      <td>导出为Excel文件</td> 
      <td> <p> 外部页面</p> <p>首选项 </p> </td> 
     </tr> 
     <tr> 
      <td>筛选条件</td> 
      <td>导出为ZIP文件</td> 
      <td> <p> 筛选条件</p> <p>首选项 </p> </td> 
     </tr> 
     <tr> 
      <td>组</td> 
      <td>导出为Excel文件</td> 
      <td> <p> 组</p> <p>首选项 </p> </td> 
     </tr> 
     <tr> 
      <td>分组</td> 
      <td>导出为ZIP文件</td> 
      <td> <p> 分组</p> <p>首选项 </p> </td> 
     </tr> 
     <tr> 
      <td>Hour</td> 
      <td>导出为Excel文件</td> 
      <td> <p> Hour</p> <p>首选项 </p> </td> 
     </tr> 
     <tr> 
      <td>问题</td> 
      <td>导出为Excel文件</td> 
      <td> <p> 问题</p> <p>首选项 </p> </td> 
     </tr> 
     <tr> 
      <td>工作角色</td> 
      <td>导出为Excel文件</td> 
      <td> <p> 工作角色</p> <p>首选项 </p> </td> 
     </tr>

   <tr> 
      <td>里程碑路径</td> 
      <td> 导出为Excel文件</td> 
      <td> <p> 里程碑</p> <p>里程碑路径</p> <p>首选项 </p> </td> 
     </tr>

   <tr> 
      <td>注释</td> 
      <td>导出为Excel文件</td> 
      <td> <p> 注释</p> <p>首选项 </p> </td> 
     </tr> 
     <tr> 
      <td>组合</td> 
      <td>导出为Excel文件</td> 
      <td> <p> 组合</p> <p>首选项 </p> </td> 
     </tr> 
     <tr> 
      <td>项目</td> 
      <td>导出为Excel文件</td> 
      <td> <p> 队列</p> <p>项目</p> <p>路由规则</p> <p>队列主题</p> <p>首选项 </p> </td> 
     </tr> 
     <tr> 
      <td>资源评估</td> 
      <td>导出为Excel文件</td> 
      <td> <p> 资源评估</p> <p>首选项 </p> </td> 
     </tr> 
     <tr> 
      <td>风险</td> 
      <td>导出为Excel文件</td> 
      <td> <p> 风险</p> <p>首选项 </p> </td> 
     </tr> 
     <tr> 
      <td>风险类型</td> 
      <td> 导出为Excel文件</td> 
      <td> <p> 风险类型</p> <p>首选项</p> </td> 
     </tr> 
     <tr> 
      <td>记分卡</td> 
      <td>导出为Excel文件</td> 
      <td> <p>记分卡问题</p> <p>计分卡选项</p> <p>记分卡</p> <p>首选项 </p> </td> 
     </tr> 
     <tr> 
      <td>任务</td> 
      <td>导出为Excel文件</td> 
      <td> <p> 任务</p> <p>首选项 </p> </td> 
     </tr> 
     <tr> 
      <td>模板</td> 
      <td> 导出为Excel文件</td> 
      <td> <p> 队列</p> <p>模板</p> <p>路由规则</p> <p>队列主题</p> <p>首选项 </p> </td> 
     </tr> 
     <tr> 
      <td>模板分派</td> 
      <td>导出为Excel文件</td> 
      <td> <p> 模板分派</p> <p>首选项 </p> </td> 
     </tr> 
     <tr> 
      <td>模板任务</td> 
      <td>导出为Excel文件</td> 
      <td> <p> 模板任务</p> <p>首选项 </p> </td> 
     </tr> 
     <tr> 
      <td>时间表</td> 
      <td> 导出为Excel文件</td> 
      <td> <p> 时间表配置文件</p> <p>时间表</p> <p>首选项 </p> </td> 
     </tr> 
     <tr> 
      <td>视图 </td> 
      <td> <p>导出为ZIP文件</p> </td> 
      <td> <p> 视图</p> <p>首选项 </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**下载**。
1. 继续[用您的数据填充电子表格模板](#populate-the-spreadsheet-template-with-your-data)，用您的信息填充空白模板电子表格。

## 使用您的数据填充电子表格模板 {#populate-the-spreadsheet-template-with-your-data}

* [电子表格中包含的选项卡（数据表）概述](#overview-of-the-tabs-data-sheets-included-in-the-spreadsheet)
* [导入记录](#import-a-record)
* [包含日期](#include-dates)
* [使用通配符](#use-wildcards)
* [ID的属性名称替换](#attribute-name-substitution-for-ids)

### 电子表格中包含的选项卡（数据表）概述

>[!TIP]
>
>要更好地了解在填充Kick-Start模板时如何需要格式化每列中的信息，请考虑执行一个练习，即在您尝试导入的对象上使用现有Workfront数据导出Kick-Start。 有关说明，请参阅[通过Kick-Starts从Adobe Workfront导出数据](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md)。

打开空白的快速启动模板时，许多选项卡（数据表）可用。 它们取决于您选择下载的对象。 每一个都表示应用程序中的一个对象，如项目、任务、小时、功能板和用户：

打开其中一个选项卡时，第2行将显示导入期间可以设置的每个对象的字段。 在列标题中，字段“set”一词后面的名称与数据库中显示的名称相同。 这些字段用作列标题。

>[!IMPORTANT]
>
>要避免出现错误，请确保以下各项：
>
>* 请勿删除快速启动电子表格的第一行空白。
>* 请勿删除、修改或重新排列这些字段（列标题）。 例如，请勿更改其顺序或名称。
>* 向列标题中以粗体显示的每个字段添加值。 这些表示必填字段。
>
>     但是，如果必填字段包含系统首选项中设置的默认值，则无需填充该字段。
>
>     例如，在&#x200B;**PROJ项目**&#x200B;选项卡上，**setCondition**&#x200B;和&#x200B;**setConditionType**&#x200B;字段可以留空，但&#x200B;**setGroupID**&#x200B;和&#x200B;**setName**&#x200B;列不能留空。
>
>* 系统会自动生成某些字段，包括&#x200B;**setResourceRevenue**&#x200B;和&#x200B;**setEnteredByID**。 如果在电子表格中输入这些字段的数据，则在上传电子表格时，快速启动过程将覆盖该数据。

### 导入记录  {#import-a-record}

工作表的每一行对应于一个唯一对象。

1. 在&#x200B;**isNew**&#x200B;列中添加信息：

   * 如果要导入的对象是新对象，请键入&#x200B;**TRUE**&#x200B;以导入行中的数据。 此值区分大小写，且必须始终为全大写字母
   * 如果该对象已在Workfront中，请在&#x200B;**isNew**&#x200B;列中键入&#x200B;**FALSE**&#x200B;以忽略该行。 此值区分大小写，且必须始终为全大写字母

      * Workfront中已存在的记录不会更新。
      * 如果您从Workfront下载了包含数据的模板，则现有对象已标记为&#x200B;**FALSE**。
      * 如果下载了空白模板，则不需要为现有对象添加新行。

1. 通过以下方式之一在&#x200B;**ID**&#x200B;列中添加信息：

   * 如果要导入的对象是新的（并且您在&#x200B;**isNew**&#x200B;列中键入了&#x200B;**TRUE**），请为ID键入任意数字。 此数字在电子表格中必须是唯一的。 例如，如果导入三个对象，则可分别为其指定ID 1、2、3。

   * 如果该对象在Workfront中已存在（且&#x200B;**FALSE**&#x200B;位于&#x200B;**isNew**&#x200B;列中），并且您正在导入有关现有对象的新信息，则ID必须是该对象在Workfront中存在的字母数字GUID。

   >[!TIP]
   >
   > 要在Workfront中查找对象的唯一GUID，您可以为该对象创建一个报表，并在该报表中添加ID列。 该列中每个对象的值是这些对象的GUID。

   * Workfront中已存在的记录不会更新。
   * 如果您下载了包含数据的模板，则现有对象已包含GUID作为ID。
   * 您可以基于现有对象导入新对象，方法是：在&#x200B;**isNew**&#x200B;列中将&#x200B;**FALSE**&#x200B;更改为&#x200B;**TRUE**，更改ID，并在导入之前进行必要的数据调整。

   ![组ID示例](assets/kick-start-group-example.png)

   * 导入项目时，必须指明组ID。

      * 如果该组已存在于Workfront中，则必须将其唯一ID添加到项目的&#x200B;**setGroupID**&#x200B;字段中。
      * 如果Workfront中不存在该组，您可以将&#x200B;**GROUP**&#x200B;工作表添加到导入文件，将“组”工作表中的&#x200B;**isNew**&#x200B;字段设置为&#x200B;**TRUE**，并在&#x200B;**ID**&#x200B;列中指明新组的数字ID。 新项目的&#x200B;**setGroupID**&#x200B;字段必须与新组的数字&#x200B;**ID**&#x200B;匹配。

     **示例：**&#x200B;对于项目，**setGroupID**&#x200B;列中显示的值必须是以下值之一：

      * Workfront实例中现有组的GUID
      * 导入期间创建新组时&#x200B;**组**&#x200B;工作表上ID列中的值（数字）

1. 输入导入期间要填充的必填字段和任何其他字段的值。
1. （可选）要添加自定义数据，请执行以下操作：

   * 为要包含在导入流程中的每个自定义字段创建新列。
   * 按如下方式命名其相应自定义字段的每个新列： **DE：[自定义字段在Workfront中显示的名称]**。 例如，您可以创建以下自定义字段：“DE： Departments”。
   * 在列&#x200B;**setCategoryID**&#x200B;中，键入此自定义字段所在的现有自定义表单的GUID。 导入自定义数据时需要此字段。
   * 如果您需要在自定义字段中添加多个数据值（如单选按钮、复选框或列表），请使用首选项选项卡中列出的垂直条自定义数据分隔符“|”来分隔这些值。

     **示例：**&#x200B;在DE:Departments列下键入A|D以填充自定义表单中的部门A和部门D。

     >[!NOTE]
     >
     >仅使用分隔符“|”分隔自定义字段值。 您无法在任何其他电子表格列（包括&#x200B;**setCategoryID**）中使用它。

### 包括日期  {#include-dates}

Workfront可以处理大多数日期格式。 但是，必须确保电子表格中的日期列设置为日期的格式。 如果该列的格式为常规、数字或文本，则导入将失败。

>[!TIP]
>
>最常用的格式为YYYY/MM/DD格式。
>
>例如：07/10/2023。

Workfront还接受时间值作为日期的一部分。

例如：07/10/2022 01:30或07/10/2022 1:00 PM。

如果忽略日期中的时间，Workfront会执行以下操作之一：

* 假定时间为12:00 AM。 要查看预期的日期结果，系统时区必须与您的时区匹配。
* 如果它位于与调度关联的对象上，则时间将推迟到调度允许的最早时间。

>[!NOTE]
>
>使用UNIX时间戳时，必须在值的末尾加上三个额外的零。
>
>例如，如果您的时间戳为7336899000，则会在单元格中输入7336899000000。

### 使用通配符 {#use-wildcards}

在填充快速启动模板电子表格时，您可以使用以下通配符：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>通配符</strong> </p> </th> 
   <th> <p><strong>行为</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>$$今天</p> </td> 
   <td> <p>在<strong>setDate</strong>字段上使用时，此通配符将日期设置为导入Kick-Start当天的午夜。</p> <p>您可以使用过滤器上允许通配符使用的标准语法来修改通配符。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span>如果希望项目在导入当周的星期一开始，而不考虑实际执行导入的日期，则可以使用<strong>$$TODAYbw</strong>。 这会将您项目的计划开始日期设置为星期日凌晨12:00。 由于当时项目时间表可能不允许工作，因此将于星期一上午9点开始。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$NOW</p> </td> 
   <td> <p>在<strong>setDate</strong>字段上使用时，此通配符根据您在Kick-Start导入期间创建记录的时间设置日期。</p> <p>您可以使用过滤器上允许通配符使用的标准语法来修改通配符。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span>如果希望项目在导入后3小时开始，则可以使用<strong>$$NOW+3h</strong>。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$USER.ID</p> </td> 
   <td> <p>在<strong>setAssignedToID</strong>或其他基于用户ID的字段上使用时，此通配符将分配工作或以其他方式将记录与执行导入的个人相关联。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$CUSTOMER</p> </td> 
   <td> <p>此通配符是专门为快速启动用户导入添加的。 创建Workfront帐户后，将创建具有系统管理员访问权限级别的用户。 在帐户中创建其他用户时，分配给默认管理员的用户名可用作前缀。</p> <p>由于用户名在所有客户中必须是唯一的，因此，如果您有多个人的用户名非常常见，例如John Smith，他的用户名可能是“jsmith”，那么这个选项会很有用。 通过在默认管理员用户名前面加上用户名分配，您可以保证每个用户名都是唯一的（例如：<strong>$$CUSTOMER.jsmith</strong>）。</p> <p>提示：要确保用户名在系统范围内是唯一的，一种更轻松的方式是在<strong>setUsername</strong>字段中输入个人的电子邮件地址。</p> </td> 
  </tr> 
 </tbody> 
</table>

### ID的属性名称替换  {#attribute-name-substitution-for-ids}

尽管最佳做法是尽可能使用ID，但在设置&#x200B;**setAttributeID**&#x200B;值时，有时不便于将ID从一个工作表交叉引用到另一个工作表。 只需更改列标题即可按名称引用值。

**示例：**

* **项目导入**

  导入项目时，请转到&#x200B;**组组**&#x200B;工作表设置项目的&#x200B;**setGroupID**，记下各自的组ID，并将其粘贴到&#x200B;**项目项目**&#x200B;工作表的正确单元格（**setGroupID**&#x200B;列）中。

  当仅处理几个组和项目时，这是可行的，但如果您处理的是每个组和项目的多个组，则它是不实用的。

  若要对上述示例进行属性名称替换，请将&#x200B;**setGroupID**&#x200B;列标题更改为&#x200B;**#setGroupID组名称**。 然后，您可以按名称引用每个项目的组。

  >[!NOTE]
  >
  >使用“属性名称替换”的选项仅限于现有记录的引用。 不能对在同一导入中创建的对象使用名称替换。

* **用户导入**

  导入用户时，从&#x200B;**ROLE Role**&#x200B;选项卡上的角色列表中填写&#x200B;**setRoleID**。

  一些角色ID用于帐户中已存在的记录，而其他角色ID则在导入期间创建。

  对于分配给现有角色的新用户记录，可以使用名称替换。 对于分配给新导入角色的新用户记录，您无法执行此操作。

  以下是在同一导入文件上使用这两种方法的方法：

   * 在电子表格中向&#x200B;**setRoleID**&#x200B;列的左侧添加一列。
   * 为新列&#x200B;**命名#setRoleID角色名称**。
   * 若要将角色分配给现有记录，请在&#x200B;**#setRoleID ROLE name**&#x200B;列中输入角色名称。

     对于新角色记录的角色分配，请在setRoleID中输入您在“角色角色”工作表中分配的ID。

     ![用户的角色ID](assets/set-role-id.png)

## 将电子表格数据导入Workfront

使用数据填充Excel模板后，可将其数据上传到Workfront。

Kick-Start导入支持以下文件类型：

* Excel (.xls或.xlsx)
* 压缩的(.ZIP)文件（仅包含.xlsx或.xls文件）

  >[!NOTE]
  >
  >在导入引用以下对象的Excel电子表格时，必须使用.ZIP文件：
  >
  >* 报告
  >* 文档
  >* 头像
  >* 查看、筛选或分组属性文件
  >
  >使用压缩的导入文件时，.ZIP文件必须与.xlsx或.xls文件同名，并且所有文件都必须处于同一结构级别（没有文件夹）。

要将模板电子表格数据导入Workfront，请执行以下操作：

<!--1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).-->

{{step-1-to-setup}}

1. 单击&#x200B;**系统** > **导入数据(Kick-Start)**。

1. 在&#x200B;**使用快速启动电子表格上载数据**&#x200B;部分中，单击&#x200B;**选择文件**，然后浏览并选择填充的电子表格。

   文件会自动上传，并显示已成功导入的通知。

   如果Excel文件上传到Workfront需要5分钟以上的时间，则应用程序会超时，并且Workfront无法上传该文件。 尝试以较小的对象批次导入数据。

1. （视情况而定）如果导入失败，您将收到一条错误消息，说明问题所在。 尝试确定出现问题的字段、工作表和行号，并更正Excel文件中的信息。 然后，再次尝试导入文件。
1. （视情况而定）如果您使用的是Workfront Fusion，则现在可以在导入完成后打开FLO或场景。
