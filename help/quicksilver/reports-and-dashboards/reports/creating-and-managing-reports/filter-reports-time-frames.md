---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 按时间范围过滤报表
description: 您可以按对象上存在日期的时间范围过滤报表。 例如，您可以过滤小时报表，以查看输入小时的特定时间范围。
author: Nolan
feature: Reports and Dashboards
exl-id: 7dea484c-d38e-4786-85d0-f4c106cfa46f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1046'
ht-degree: 4%

---

# 按时间范围过滤报表

您可以按对象上存在日期的时间范围过滤报表。 例如，您可以过滤小时报表，以查看输入小时的特定时间范围。

## 访问要求

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
   <td> <p>编辑对报表、功能板、日历的访问</p> <p>编辑对过滤器、视图、分组的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

必须先创建报表，然后才能过滤其结果。

有关创建报表的更多信息，请参阅 [创建报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## 按日期的时间范围过滤报表 {#filter-a-report-by-the-time-frame-of-a-date}

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png)，然后单击 **报表**.

1. 单击 **新建报表**，然后选择所需的报表类型。\
   例如，选择 **小时报表**.

1. 选择 **过滤器** 选项卡。
1. 单击 **添加过滤器规则**，然后选择 **小时录入日期**.\
   ![](assets/qs-filtering-hour-report-by-timeframe-350x357.png)

1. 在以下下拉菜单中，选择以下任意选项：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">等于</td> 
      <td>选择此修改量后，指定输入小时的日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">不等于</td> 
      <td>选择此修改量后，指定输入小时的日期，以从报表中排除此日期。 报表显示所有日期（预计在您指定的日期）的记录小时数。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">空</td> 
      <td>选择此修改量可仅显示缺少登入日期的小时。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">非空</td> 
      <td>选择此修改量可仅显示输入日期具有值的小时。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">介于</td> 
      <td>选择此修改量后，指定输入小时数的日期范围。 报表显示在指定日期之间输入的小时数。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">小于</td> 
      <td>选择此修改量后，指定输入小时数之前的日期。 报表显示在指定日期之前输入的小时数，而不包括指定日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">小于和等于</td> 
      <td>选择此修改量后，指定输入小时数之前的日期。 报表显示在指定日期（包括指定日期）之前输入的小时数。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">大于</td> 
      <td>选择此修改量后，指定输入小时数的日期。 报表显示在指定日期之后输入的小时数，而不包括指定的日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">大于或等于</td> 
      <td> <p>选择此修改量后，指定输入小时数的日期。 报表显示在指定日期（包括指定日期）之后输入的小时数。</p> <p>选择任何内置时间范围修饰符，如 <a href="#built-in-time-frame-modifiers" class="MCXref xref">内置时间范围修饰符</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 这些修饰符可用于过滤器中的任何日期字段或任何报表中的提示。
1. 单击 **保存并关闭**.

## 内置时间范围修饰符 {#built-in-time-frame-modifiers}

Adobe Workfront具有内置时间范围修饰符，您无需定义特定日期即可使用这些修饰符。 

这些修饰符可用于过滤器中的任何日期字段或任何报表中的提示。 

有关如何按与日期关联的时间范围过滤报表的详细信息，请参阅  [按日期的时间范围过滤报表](#filter-a-report-by-the-time-frame-of-a-date).

例如，如果您正在构建小时报表，并且希望显示在特定时间范围内输入的小时数，则可以从以下内置时间范围过滤器选项中进行选择：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">今天</td> 
   <td>显示登入日期为今天的小时数。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">本周</td> 
   <td>显示“登入日期”是当周日期的小时数，其中一周从星期日开始，到星期六结束。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">下周</td> 
   <td>显示“登入日期”是当周后一周中的日期的小时，其中一周从星期日开始，到星期六结束。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">上周</td> 
   <td>显示“登入日期”是当周之前一周中的日期的小时，其中一周从星期日开始，到星期六结束。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">本月</td> 
   <td>显示登入日期是当月日期的小时数。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">下个月</td> 
   <td>显示“登入日期”是当月后一个月中的日期的小时。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">上个月</td> 
   <td>显示“登入日期”是当月前一个月中某个日期的小时</td> 
  </tr> 
  <tr> 
   <td role="rowheader">本季度</td> 
   <td> <p>显示“登入日期”是当前季度中日期的小时数，其中季度定义为：</p> 
    <ul> 
     <li>第一季度：1月1日 — 3月30日</li> 
     <li>第二季度：4月1日 — 6月30日</li> 
     <li>第三季度：7月1日至9月30日</li> 
     <li>第四季度：10月1日 — 12月31日</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">下个季度</td> 
   <td>显示“登入日期”是当前季度后季度中的日期的小时数，其中季度在上面定义。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">上个季度</td> 
   <td> <p>显示“登入日期”是当前季度之前季度中某个日期的小时，其中季度在上面定义。</p> <p>注意：如果您的Workfront管理员为您的系统启用并定义了自定义季度，则季度的内置过滤器将替换为您的自定义季度信息。 有关启用自定义季度的更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref">为项目启用自定义季度</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">今年</td> 
   <td>显示“登入日期”是当年日期的小时，其中当年从1月1日开始，到12月31日结束。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">往年</td> 
   <td>显示“登入日期”是过去一年中某个日期的小时，其中过去一年从当前日期之前的12个月开始。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">去年</td> 
   <td> <p>显示“登入日期”是去年某个日期的小时，其中去年从1月1日开始，到当年前一年的12月31日结束。</p> <p>注意：财政年度没有内置时间段。 您可以使用自定义修改量创建报表并按日期过滤信息，以查看在您的组织中定义的会计年度日期范围。 如果要当场选择一个会计年度的时间范围，则应使用提示，而不是过滤器。 </p> </td> 
  </tr> 
 </tbody> 
</table>
