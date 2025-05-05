---
product-area: programs
navigation-topic: create and manage programs
title: 创建项目
description: 项目群表示共享跨项目边界的共同策略、目标或目标的项目集合。 项目是项目组合的一个细分，它们不能存在于项目组合之外。 项目通常与同一项目组合中的其他项目共享相同的资源。 您可以创建项目群，以便在项目组合变得太大时对其进行整理。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 6ec353c2-2241-47c2-8c59-1d8ddc43781e
source-git-commit: 594504c6a7acc9341471371ca279379042a45457
workflow-type: tm+mt
source-wordcount: '1288'
ht-degree: 0%

---

# 创建项目

<!-- Audited: 1/2024 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

项目群表示共享跨项目边界的共同策略、目标或目标的项目集合。
项目是项目组合的一个细分，它们不能存在于项目组合之外。 项目通常与同一项目组合中的其他项目共享相同的资源。

您可以创建项目群，以便在项目组合变得太大时对其进行整理。

例如，您可以有一个包含营销部门所有项目的2024年营销财政年度Portfolio。 您可能需要考虑进一步将您的项目整理到财务季度中，并在2024年营销财政年度Portfolio中添加2024年营销财政季度1-4计划。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td>

<td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td> <p>新文档： [!UICONTROL Standard] </p><p>或 </p><p>当前： [!UICONTROL 计划] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>[!UICONTROL Edit]对项目组合和程序的访问权限 </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>项目组合的[!UICONTROL Manage]权限</p> <p>创建项目后，默认情况下，您拥有[!UICONTROL Manage]权限。</p>  </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 创建项目群的方法

您可以使用以下方法之一在Workfront中创建程序：

* 从头开始在主菜单的程序区域或项目组合的程序部分创建程序。 本文介绍了如何从头开始创建程序。

* 使用kick-starts导入程序。

  作为Workfront管理员，您可以使用快速启动导入程序。

  有关在Workfront中使用Kick-Start导入数据的信息，请参阅[使用Kick-Start模板将数据导入Adobe Workfront](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)。


* 在从Workfront Planning中的记录类型连接程序时添加程序。

  您必须有一个额外的Workfront Planning包。

  有关访问Workfront Planning的信息，请参阅[Adobe Workfront Planning访问概述](/help/quicksilver/planning/access/access-overview.md)。

  有关通过将项目组合添加到记录来创建项目组合的信息，请参阅[创建记录](/help/quicksilver/planning/records/create-records.md)一文中的“连接时创建记录”一节。

## 创建项目

1. 单击Adobe Workfront右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon.png)，或（如果可用）单击左上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png)。

1. 执行以下操作之一。

   * 从[!UICONTROL 程序]区域创建程序：

      1. 在主菜单中单击&#x200B;**[!UICONTROL 程序]**。
      1. 单击&#x200B;**[!UICONTROL 新建项目]**。
      1. 在显示的框中，在&#x200B;**[!UICONTROL 选择Portfolio]**&#x200B;字段中键入现有Portfolio的名称。
      1. 在&#x200B;**[!UICONTROL 名称]**&#x200B;字段中键入新项目的名称。
      1. 单击&#x200B;**[!UICONTROL 保存]**。
   * 从[!UICONTROL 项目组合]区域创建项目：

      1. 在[!UICONTROL 主菜单]中单击&#x200B;**[!UICONTROL 项目组合]**，然后打开一个项目组合。
      1. 在左侧面板中，单击&#x200B;**[!UICONTROL 程序]**。
      1. 单击&#x200B;**[!UICONTROL 新建项目]**&#x200B;下拉菜单，然后单击&#x200B;**[!UICONTROL 新建项目]**。


1. （视情况而定）如果您是从项目组合创建项目群，请在&#x200B;**[!UICONTROL 无标题项目群]**&#x200B;字段中指定项目群的名称。

   名称最多可包含255个字符。

1. （可选）单击程序标题中的&#x200B;**[!UICONTROL 程序管理器]**&#x200B;以更新程序。

   >[!TIP]
   >
   >作为项目的创建者，默认情况下您被设置为“项目管理员”。

1. 单击左侧面板中的&#x200B;**[!UICONTROL 项目详细信息]**。
1. 双击任何字段以更新&#x200B;**[!UICONTROL 概述]**&#x200B;区域中的信息。

您可以指定以下信息：

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>字段</th> 
      <th>描述</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 描述]</td> 
      <td> <p>指定程序的描述。</p> <p>该描述将显示在项目的登陆页面上。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 项目管理器]</td> 
      <td> <p>开始键入要充当项目管理员的用户名，然后在用户名出现在下拉列表中时单击该用户名。 这与[!UICONTROL 项目所有者]相同。 </p> <p>提示：您也可以在项目标题中更新项目管理器。 </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 组] </td> 
      <td> <p>添加单个组的名称（如果该组拥有项目或负责完成项目）。 </p> <p>您可以通过将鼠标悬停在该组上并单击其旁边显示的[!UICONTROL 信息]图标<img src="assets/info-icon.png">来确保选择正确的组。 这将显示一个工具提示，其中列出了有关组的信息，例如组及其上各组的层次结构。</p> 
       <div data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
        <img src="assets/group-details-widget-programs-350x268.png" style="width: 350;height: 268;"> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可选且有条件）单击&#x200B;**[!UICONTROL 添加自定义表单]**&#x200B;框中的，为项目组合选择自定义表单并更新自定义字段。

   >[!TIP]
   >
   >必须先创建程序自定义表单，然后才能将其附加到程序。

1. （可选且视情况而定）如果要添加自定义表单，请单击自定义表单上的任意字段以更新该字段中的信息。
1. 单击&#x200B;**[!UICONTROL 保存更改]**。
1. 单击左侧面板中的&#x200B;**[!UICONTROL 项目]**，然后单击&#x200B;**[!UICONTROL 添加项目]**&#x200B;以将项目添加到程序。

   有关将项目添加到程序的信息，请参阅[将项目添加到程序](../../../manage-work/portfolios/create-and-manage-programs/add-project-to-program.md)。

1. 单击&#x200B;**[!UICONTROL 保存更改]**。
1. （可选）单击程序名称旁边的&#x200B;**[!UICONTROL 更多菜单]** ![更多菜单](assets/more-icon.png)，然后单击&#x200B;**[!UICONTROL 停用程序]**。

   停用项目群时，当用户尝试将项目群添加到项目时，项目群不再显示在项目群列表中。 您仍然可以从[!UICONTROL 程序]区域访问该程序。

## 项目标题概述

您可以在其标题中找到有关程序的一些信息。

以下信息显示在项目的标题中：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">标题信息</td> 
   <td> <strong>备注</strong> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">包含项目组合名称的痕迹导航</td> 
   <td>您可以从项目群标题访问项目群所属的项目组合。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">项目的名称</td> 
   <td>您可以在标题中编辑项目名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象类型和激活状态的名称</td> 
   <td>当您查看项目时，“项目”一词会显示一个橙色图标。 单词“[!UICONTROL 已停用]”显示在旁边，如果程序未标记为[!UICONTROL 活动]，则大纲为灰色。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">计划的操作区域 </td> 
   <td> <p>单击以下任一选项以访问程序的更多信息或编辑选项：</p> 
    <ul> 
     <li>星形图标，用于将程序添加到收藏夹列表</li> 
     <li> <p>[!UICONTROL More]菜单<img src="assets/qs-more-menu.png">用于执行以下操作之一： </p> 
      <ul> 
       <li>编辑项目</li> 
       <li>取消激活它。 停用项目群时，您无法再将其与项目级别的项目关联。 </li> 
       <li> <p>删除它。 删除项目群不会删除项目群中的项目。 它删除项目与项目的关联。 </p> </li> 
       <li>与其他人共享</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 完成百分比]</td> 
   <td> <p>您无法在标题中编辑项目的[!UICONTROL 完成百分比]。 将从项目群的项目中更新此信息。 默认情况下，项目的完成百分比是属于该项目且处于[!UICONTROL 当前]或[!UICONTROL 已批准]状态的项目的平均完成百分比值。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 项目管理器]</td> 
   <td> <p>您可以在标题中编辑项目管理器。 这与[!UICONTROL 项目所有者]相同。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 计划完成日期]</td> 
   <td>您无法在标题中编辑项目的规划完成日期。 将从项目群的项目中更新此信息。 项目群中最新项目的计划完成日期变为项目的计划完成日期。  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 活动项目条件]</td> 
   <td>这是计算在项目群中，将[!UICONTROL Condition]设置为[!UICONTROL On Target]、[!UICONTROL At Risk]或[!UICONTROL In Trouble]的项目所占的百分比。 此处表示的项目是状态为[!UICONTROL 当前]和[!UICONTROL 已批准]的项目。 </td> 
  </tr> 
 </tbody> 
</table>

## 移动项目

您可以将现有项目添加到项目组合。 由于程序不能存在于两个不同的项目组合中，因此添加现有程序会将其从一个项目组合永久移动到另一个项目组合。

有关详细信息，请参阅[将现有项目添加到项目组合](../../../manage-work/portfolios/create-and-manage-programs/move-program.md)。
