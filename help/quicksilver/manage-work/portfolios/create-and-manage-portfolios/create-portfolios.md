---
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: 创建项目组合
description: Portfolio是争夺相同资源、预算和计划的项目集合。 Portfolio中的项目非常相似，以至于它们会使用相同的资源池并根据相同的记分卡进行衡量。
author: Alina
feature: Work Management, Strategic Planning
exl-id: fdaed68d-d9cc-4514-8f80-b169cdd739bd
source-git-commit: 2bfb6d03f3d0f792180a67ade8a704e4c899a671
workflow-type: tm+mt
source-wordcount: '668'
ht-degree: 1%

---

# 创建项目组合

<!--Audited: 7/2024-->

Portfolio是争夺相同资源、预算和计划的项目集合。 Portfolio中的项目非常相似，以至于它们会使用相同的资源池并根据相同的记分卡进行衡量。

您可以使用Portfolio对属于同一产品线、部门、部门、公司或其他业务部门的项目进行分组。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>任何</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>新文档： [！UICONTROL Standard]</p>
   <p>当前：[！UICONTROL计划] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>[！UICONTROL Edit]对Portfolio的访问权限</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>创建项目组合后，默认情况下，您拥有其管理权限</p>  </td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 创建项目组合的方法

您可以使用以下方法之一在Workfront中创建项目组合：

* 从主菜单的Portfolio区域开始从头开始创建项目组合。 本文介绍了如何从头开始创建项目组合。

* 使用kick-start导入项目组合。

  作为Workfront管理员，您可以使用快速启动导入项目组合。

  有关在Workfront中使用Kick-Start导入数据的信息，请参阅[使用Kick-Start模板将数据导入Adobe Workfront](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)。

* 在从Workfront Planning中的记录类型连接项目组合时添加项目组合。

  您必须拥有新的Workfront许可证和附加的Workfront Planning许可证，才能使用Workfront Planning。

  有关访问Workfront Planning的信息，请参阅[访问概述](/help/quicksilver/planning/access/access-overview.md)。

  有关通过将项目组合添加到记录来创建项目组合的信息，请参阅[创建记录](/help/quicksilver/planning/records/create-records.md)一文中的“连接时创建记录”一节。


## 创建项目组合

{{step1-click-main-menu}}

1. 单击&#x200B;**[!UICONTROL Portfolio]**。
1. 单击&#x200B;**[!UICONTROL 新建Portfolio]**。
1. 将&#x200B;**[!UICONTROL 无标题Portfolio]**&#x200B;替换为您要为项目组合指定的名称。

   名称最多可包含255个字符。

1. （可选）单击页面顶部标题中&#x200B;**[!UICONTROL Portfolio管理器]**&#x200B;下的名称，为该项目组合分配其他管理器。

   ![](assets/portfolio-manager-name-350x51.jpg)

   作为项目组合的创建者，默认情况下您被分配为项目组合经理。

1. 单击左侧面板中的&#x200B;**[!UICONTROL Portfolio详细信息]**。
1. 在&#x200B;**[!UICONTROL 概述]**&#x200B;区域中，更改以下任何信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL描述]</td> 
      <td> <p>键入Portfolio的描述以指示其独特之处。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROLPortfolio管理器]</td> 
      <td> <p>开始键入要指定为项目组合经理的用户名称，然后当该用户出现在列表中时将其选定。 这与[！UICONTROLPortfolio所有者]相同。 他可以监督项目组合中定义的工作并批准业务案例。</p> <p>重要信息：当您指定某个人作为[！UICONTROLPortfolio管理员]时，该人员会自动获得对项目组合、项目和项目组合中的项目的[！UICONTROL管理]权限。 </p> <p>提示：您还可以更新页面顶部标题中的[！UICONTROLPortfolio管理器]。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">组 </td> 
      <td> <p>添加单个组的名称（如果该组拥有项目组合或负责完成它）。 </p> <p>您可以通过将鼠标悬停在该组上并单击其旁边显示的[！UICONTROL信息]图标<img src="assets/info-icon.png">来确保选择正确的组。 这将显示一个工具提示，其中列出了有关组的信息，例如组及其上各组的层次结构。</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/group-details-widget-portfolios-350x250.png" style="width: 350;height: 250;"> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可选）在[!UICONTROL Portfolio详细信息]页面右上角的&#x200B;**[!UICONTROL 添加自定义表单]**&#x200B;框中单击，为项目组合选择自定义表单并更新自定义字段。

   >[!TIP]
   >
   >必须先创建项目组合自定义表单，然后才能将其附加到项目组合。

1. 单击&#x200B;**[!UICONTROL 保存更改]**。
1. （可选）单击左侧面板中的&#x200B;**[!UICONTROL 程序]**，然后单击&#x200B;**[!UICONTROL 添加程序]**&#x200B;以将程序添加到项目组合。

   有关创建程序的详细信息，请参阅[创建程序](../../../manage-work/portfolios/create-and-manage-programs/create-program.md)。

1. （可选）单击左侧面板中的&#x200B;**[!UICONTROL 项目]**，然后单击&#x200B;**[!UICONTROL 添加项目]**&#x200B;以将项目添加到项目组合。

   有关将项目添加到Portfolio的详细信息，请参阅[将项目添加到项目组合](../../../manage-work/portfolios/create-and-manage-portfolios/add-projects-to-portfolios.md)。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Deactivate a portfolio</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted this and moved it to their own article: delete-deactivate-portfolios)</p>
<p>When you deactivate a portfolio, you can still access it from the Portfolios area, but it no longer displays in the list of portfolios when users try to add it to a project.</p>
<ol>
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.</li>
<li value="2">Click <strong>Portfolios</strong> .</li>
<li value="3"> <p>Click the name of the portfolio.</p> </li>
<li value="4" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the More menu <img src="assets/more-icon.png"> to the right of the portfolio name, then click <strong>Deactivate Portfolio</strong>.</li>
</ol>
<h2>Delete a portfolio</h2>
<ol>
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.</li>
<li value="2"> <p>Click <strong>Portfolios</strong> .</p> </li>
<li value="3"> <p>Select the portfolio, then click the Delete icon <img src="assets/delete.png">.</p> </li>
<li value="4"> <p>In the box that appears, click <strong>Yes, Delete It</strong> to confirm.</p> </li>
</ol>
</div>
-->
