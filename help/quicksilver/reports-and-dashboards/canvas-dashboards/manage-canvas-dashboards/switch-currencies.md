---
product-area: Canvas Dashboards
navigation-topic: report-types
title: 在画布功能板中使用货币字段
description: 您可以在画布功能板中使用货币字段。
author: Courtney
feature: Reports and Dashboards
source-git-commit: 3e4ab2dfc66efd262c0c2ad30a9c62758084f8ce
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 4%

---


# 在画布功能板中使用货币字段

>[!IMPORTANT]
>
>画布功能板目前仅适用于参与Beta测试阶段的用户。 在此阶段，部分功能可能无法完成或无法按预期工作。 请按照“画布功能板测试版”概述文章中[提供反馈](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback)部分的说明提交任何有关您体验的反馈。<br>
>如果您对可能的错误或技术问题有反馈，请向Workfront支持提交票证。 有关详细信息，请参阅[联系客户支持](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)。<br>
>请注意，以下云提供商未提供此测试版：
>
>* 自带Amazon Web Services密钥
>* Azure
>* Google Cloud Platform

## 访问要求

+++ 展开可查看本文所述功能的访问权限要求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 包</p></td> 
   <td> 
<p>任何 </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td> 
<p>标准</p> 
<p>规划</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td><p>编辑对报告、功能板和日历的访问权限</p>
   <p>查看对财务数据的访问权限</p>
  </td> 
  </tr> 
    </tr>  
        <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td><p>管理仪表板的权限</p>
  </td> 
  </tr> 
</tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。
+++

## 先决条件

1. 您必须在Workfront实例中设置多种货币类型，才能使用本文中所述的功能。 有关详细信息，请参阅[设置汇率](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)。

   >[!IMPORTANT]
   >
   >本文中介绍的功能仅适用于本机货币字段。 即将支持自定义货币字段。


## 为画布功能板设置默认货币

创建画布功能板时，您可以设置功能板的默认货币。 此货币将用于显示功能板上的报告中的所有本机货币字段，除非已在报告级别锁定了“货币”字段。

1. 在左侧面板中，单击&#x200B;**画布功能板**。

1. 单击右上角的&#x200B;**新建仪表板**。

1. 在&#x200B;**创建仪表板**&#x200B;框中，

1. 指定以下内容：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>名称</strong></td>
      <td><p>输入仪表板的名称。 我们建议仅使用UTF-8字符以避免兼容性问题。</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>描述（可选）</strong></td>
      <td>输入仪表板的说明。</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>货币</strong></td>
      <td>选择仪表板的默认货币类型。 <br>
      <br>用户可在筛选仪表板时切换不同的货币类型。</td>
     </tr>
    </tbody>
   </table>


## 在画布功能板上的货币之间切换

您可以在仪表板级别在不同货币类型之间切换。 包含货币字段的报表将更新以反映所选的货币类型。

可以在报表级别锁定货币字段。 如果货币字段已锁定，则当您更改仪表板的货币类型时，该报表的货币类型将不会更改。

要更改仪表板的货币类型，

1. 单击功能板详细信息页面右上角的货币下拉菜单。
1. 从列表中选择所需的货币类型。

   ![更改货币下拉框](assets/filter-by-currency.png)


## 限制

下表概述了在“设置”的“汇率”区域中定义货币时的限制。

<table> 
<tr>
<td></td>
<td>用户可以</td>
<td>用户无法</td>
</tr>
<tr> 
<td>已定义单一货币</td>
<td>
<ul>
<li>在画布图表、KPI和表报表中使用本机货币字段</li>
<li>在画布图表、KPI和图表报表中使用自定义货币字段</li>
</ul>
</td>
<td>
<ul>
<li>为仪表板分配默认货币（在创建或编辑仪表板时）</li>
<li>查看并使用功能板级别的货币切换</li>
<li>锁定特定货币以在画布图表、KPI或表格报表中查看</li>
<li>在画布图、KPI和表格报表中使用“计划”币种字段</li>
</ul>
</td> 
</tr>
</td> 
</tr> 
<tr>
<td>定义了多种货币</td>
<td>
<ul>
  <li>在画布图表、KPI和表报表中使用本机货币字段</li>
  <li>为仪表板设置默认货币（在创建或编辑仪表板时）</li>
  <li>查看并使用功能板级别的货币切换</li>
  <li>锁定特定货币以在画布图表、KPI或表格报表中查看，以忽略功能板货币切换首选项</li>
</ul>
</td>
<td><ul>
  <li>在画布图表、KPI和表格报表中使用自定义数据货币字段</li>
  <li>在画布图、KPI和表格报表中使用“计划”币种字段</li>
</ul>
</td>
</tr></table>





