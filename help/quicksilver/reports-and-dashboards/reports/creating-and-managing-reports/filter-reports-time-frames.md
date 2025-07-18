---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 按时间范围筛选报表
description: 您可以按对象中存在的日期的时间范围过滤报表。 例如，您可以为输入小时数的特定时间范围过滤小时报告。
author: Courtney
feature: Reports and Dashboards
exl-id: 7dea484c-d38e-4786-85d0-f4c106cfa46f
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 4%

---

# 按时间范围筛选报表

<!-- Audited: 4/2025 -->

您可以按对象中存在的日期的时间范围过滤报表。 例如，您可以为输入小时数的特定时间范围过滤小时报告。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

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
      <td> 
      <p>新增：标准</p>
       <p> 或</p>
      <p>当前：计划</p>
   </td>

</tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限</p> <p>编辑对筛选器、视图、分组的访问权限</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p></td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

必须先创建报告，然后才能筛选其结果。

有关创建报告的详细信息，请参阅[创建报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)。

## 按日期的时间范围过滤报表 {#filter-a-report-by-the-timeframe-of-a-date}

{{step1-to-reports}}

1. 单击左上角的&#x200B;**新建报告**，然后选择要创建的报告类型。

1. 在&#x200B;**新报表**&#x200B;页面上，选择&#x200B;**筛选器**&#x200B;选项卡。

1. 单击&#x200B;**添加筛选器规则**，然后单击&#x200B;**选择字段**。

1. 在&#x200B;**选择字段**&#x200B;对话框中，选择&#x200B;**小时**，然后选择&#x200B;**输入日期**。
   ![按时间范围过滤小时报告](assets/qs-filtering-hour-report-by-timeframe-350x357.png)

1. 在显示的下拉菜单中，选择以下选项之一：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">等于</td> 
      <td>选择此修改量后，请指定输入小时数的日期。</td> 
     </tr>

   <tr> 
      <td role="rowheader">不等于</td> 
      <td>选择此修改量后，请指定输入小时数的日期，以将此日期从报表中排除。 报表显示在指定日期以外的所有日期记录的小时数。</td> 
     </tr>

   <tr> 
      <td role="rowheader">小于</td> 
      <td>选择此修改量后，请指定输入小时数的日期。 该报告显示在指定日期（不包括指定日期）之前输入的小时数。</td> 
     </tr>

   <tr> 
      <td role="rowheader">小于和等于</td> 
      <td>选择此修改量后，请指定输入小时数的日期。 此报表显示在指定日期（包括指定日期）之前输入的小时数。</td> 
     </tr>

   <tr> 
      <td role="rowheader">大于</td> 
      <td>选择此修改量后，请指定输入小时数的日期。 报表显示在指定日期（不包括指定日期）后输入的小时数。</td> 
     </tr>

   <tr> 
      <td role="rowheader">大于或等于</td> 
      <td> 选择此修改量后，请指定输入小时数的日期。 报表显示在指定日期（包括指定日期）之后输入的小时数。 </td> 
     </tr>

   <tr> 
      <td role="rowheader">介于</td> 
      <td>选择此修改量后，请指定输入小时数的日期范围。 此报表显示指定日期之间输入的小时数。</td> 
     </tr>

   <tr> 
      <td role="rowheader">空</td> 
      <td>选择此修改量可仅显示缺少输入日期的小时。</td> 
     </tr>

   <tr> 
      <td role="rowheader">非空</td> 
      <td>选择此修改量可仅显示输入日期具有值的小时。</td> 
     </tr>

   </tbody> 
   </table>

1. 单击&#x200B;**保存+关闭**。

## 内置时间范围修饰符 {#built-in-timeframe-modifiers}

Adobe Workfront具有内置的时间范围修饰符，您无需定义特定日期即可使用。 这些修饰符可用于过滤器中的任何日期字段或任何报表中的提示。

例如，如果您正在构建小时报表，并希望显示在特定时间范围内输入的小时数，则可以从以下内置时间范围过滤器选项中进行选择：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">今天</td> 
   <td>显示输入日期为今天的小时数。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">本周</td> 
   <td>显示输入日期为本周中日期的小时，其中周从星期日开始到星期六结束。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">下周</td> 
   <td>显示以下小时：其中输入日期是本周后一周中的日期，该周从星期日开始，到星期六结束。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">上周</td> 
   <td>显示以下小时，其中输入日期是本周之前一周中的日期，其中一周从星期日开始，到星期六结束。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">本月</td> 
   <td>显示输入日期为当月日期的小时。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">下个月</td> 
   <td>显示输入日期为当月下一个月中日期的小时。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">上个月</td> 
   <td>显示输入日期为当月前一个月中日期的小时</td> 
  </tr> 
  <tr> 
   <td role="rowheader">本季度</td> 
   <td> <p>显示输入日期为本季度日期的小时，其中季度定义为：</p> 
    <ul> 
     <li>第一季度：1月1日至3月30日</li> 
     <li>第二季度：4月1日至6月30日</li> 
     <li>第三季度：7月1日至9月30日</li> 
     <li>第四季度：10月1日至12月31日</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">下个季度</td> 
   <td>显示输入日期为当前季度（上面定义了季度）后某个季度中的日期的小时数。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">上个季度</td> 
   <td> <p>显示其输入日期为当前季度前一个季度中的日期的小时，其中季度在上面定义。</p> <p>注意：如果您的Workfront管理员为系统启用并定义了自定义季度，则季度的内置过滤器将被替换为自定义季度信息。 有关启用自定义季度的详细信息，请参阅<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref">启用自定义季度</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">今年</td> 
   <td>显示输入日期为当前年份中日期的小时数，其中当前年份从1月1日开始，到12月31日结束。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">往年</td> 
   <td>显示输入日期为上一年中的日期的小时数，其中上一年始于当前日期之前的12个月。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">去年</td> 
   <td> <p>显示输入日期为上一年中的日期的小时数，其中上一年从1月1日开始，到本年度之前一年的12月31日结束。</p> <p>注：会计年度没有内置时间期。 您可以创建一个报表，并使用在组织中定义的会计年度日期范围的自定义修改量按日期筛选信息。 如果要当场为某个财政年度选择时间范围，则应当使用提示而不是过滤器。 </p> </td> 
  </tr> 
 </tbody> 
</table>
