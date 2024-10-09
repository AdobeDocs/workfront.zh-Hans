---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: 查看Workfront Data Connect使用情况量度
description: 使用Workfront Data Connect Metrics选项卡，您可以根据每月使用的计算小时数和执行的查询数查看组织的使用量度。
author: Nolan
feature: Reports and Dashboards
source-git-commit: 4c8b7e7f33ec593b2942725eb9160f7fbe2962e3
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 1%

---

# 查看[!DNL Workfront Data Connect]使用情况量度

使用[!DNL Workfront Data Connect] [!UICONTROL 指标]选项卡，您可以根据使用的计算小时数和执行的查询数查看组织的使用情况指标。 组织根据其许可证类型和Data Connect附加组件购买提供的每月计算小时数有限。 [!UICONTROL 量度]选项卡显示与已使用量度相关的可用每月计算小时数信息。

## 访问要求

+++ 展开以查看访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td><p>包括在以下计划中：</p>
    <ul>
        <li>Ultimate</li> 
    </ul>    
   <p>可作为以下计划的附加组件购买：</p> 
    <ul>
        <li>选择</li> 
        <li>Prime</li>
    </ul> 
    <p>Workfront Data Connect不适用于旧版Workfront计划。</p> 
   </td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p></td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 查看使用情况量度和可用的计算小时数

1. 单击Adobe Workfront右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon.png)，或（如果可用）单击左上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png)，然后单击&#x200B;[!UICONTROL **设置**]。

1. 在左侧面板中，单击&#x200B;[!UICONTROL **系统**] > [!UICONTROL **数据访问**]。

1. 单击&#x200B;[!UICONTROL **指标**]&#x200B;选项卡。 您的使用情况量度显示在&#x200B;**计算使用情况**&#x200B;图形中，而执行的查询次数显示在&#x200B;**查询计数**&#x200B;图形中。

   ![Data Connect使用量度](/help/quicksilver/reports-and-dashboards/data-lake/assets/data-connect-usage-metrics.png)

1. （可选）您可以使用&#x200B;[!UICONTROL **选择视图**]&#x200B;下拉菜单更改两个图形中包含的信息的时间范围。

1. （可选）您可以使用&#x200B;**计算使用情况**&#x200B;图形上方的复选框来显示或隐藏：
   * [!UICONTROL **每日计算小时数**] — 您的组织每天使用的计算小时数。
   * [!UICONTROL **每月累计计算小时数**] — 贵组织在一个月内使用的计算小时总数。 每月重置为零。
   * [!UICONTROL **每月计算小时津贴**] — 贵组织根据许可证和/或附加购买提供的计算小时数。
