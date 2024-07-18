---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '分组：指示应使用文本模式折叠或展开分组的结果'
description: '分组：指示应使用文本模式折叠或展开分组的结果'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2880e06f-34f3-47b1-9462-5a15a20d6fee
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 0%

---

# 分组：指示应使用文本模式折叠或展开分组的结果

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this article: NWE only; not possible in classic) </p>
-->

您可以使用标准Report Builder指示分组中的结果在列表或报表中是应折叠还是展开。 默认情况下，分组中的结果显示为展开状态。 有关创建分组的信息，请参阅[在Adobe Workfront中创建分组](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Understanding text mode, Edit groupings to organize reports, Create a Custom Report; create a snippet when convenient)</p>
-->

>[!TIP]
>
>* 当您在查看列表时手动调整分组时，Adobe Workfront会记住您的手动首选项，直到您注销。 重新登录时，将根据此设置显示列表。
>* 从图表元素访问分组结果后，这些结果始终以展开形式显示。
>

您还可以指定使用文本模式显示的分组是展开还是折叠。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>请求修改分组 </p>
   <p>计划修改报告</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限以修改报告</p> <p>编辑对筛选器、视图和分组的访问权限以修改分组</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 指示应使用文本模式折叠还是展开分组结果

1. 转到对象列表。
1. 从&#x200B;**分组**&#x200B;下拉菜单中，选择&#x200B;**新建分组**。

1. 添加分组，然后单击&#x200B;**切换到文本模式**。

   或

   如果分组已处于文本模式，请将以下代码添加到要折叠显示的分组级别：

   ```
   group.0.iscollapsed=true
   ```

1. （可选）如果要展开分组显示，请将以下代码添加到相应的分组级别：

   ```
   group.0.iscollapsed=false
   ```

1. 单击&#x200B;**完成**，然后单击&#x200B;**保存分组**。
