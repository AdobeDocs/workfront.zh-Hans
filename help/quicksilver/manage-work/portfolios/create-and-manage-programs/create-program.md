---
product-area: programs
navigation-topic: create and manage programs
title: 创建项目
description: 项目表示一组项目，这些项目共享跨项目边界的共同策略、目标或目标。 程序不能存在于组合之外。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 6ec353c2-2241-47c2-8c59-1d8ddc43781e
source-git-commit: 93c36a87667097729e89a61f68cc17e9c861d547
workflow-type: tm+mt
source-wordcount: '1025'
ht-degree: 0%

---

# 创建项目

项目表示一组项目，这些项目共享跨项目边界的共同策略、目标或目标。 程序不能存在于组合之外。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[!UICONTROL Business]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[!UICONTROL计划] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>[!UICONTROL Edit]对Portfolio和程序的访问 </p> <p>注意：如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以更改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>[!UICONTROL管理]对产品组合的权限</p> <p>创建程序后，默认情况下，您拥有该程序的[!UICONTROL管理]权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 创建项目

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 执行以下操作之一。

   * 从 [!UICONTROL 程序] 区域：

      1. 单击 **[!UICONTROL 程序]** 中。
      1. 单击 **[!UICONTROL 新计划]**.
      1. 在显示的框中，键入现有Portfolio的名称(位于 **[!UICONTROL 选择Portfolio]** 字段。
      1. 在 **[!UICONTROL 名称]** 字段。
      1. 单击&#x200B;**[!UICONTROL 保存]**。
   * 从 [!UICONTROL Portfolio] 区域：

      1. 单击 **[!UICONTROL Portfolio]** 在 [!UICONTROL 主菜单]，然后单击一个项目组合。
      1. 在左侧面板中，单击 **[!UICONTROL 程序]**.
      1. 单击 **[!UICONTROL 新计划]** 下拉菜单，然后 **[!UICONTROL 新计划]**.


1. 在 **[!UICONTROL 无标题程序]** 字段。

   名称最多可包含255个字符。

1. （可选）单击 **[!UICONTROL 项目经理]** 在程序标题中更新它。

   >[!TIP]
   >
   >作为程序的创建者，默认情况下将您设置为“程序管理器”。

1. 单击 **[!UICONTROL 计划详细信息]** 中。
1. 双击任意字段以更新 **[!UICONTROL 概述]** 的上界。
1. 指定以下信息：

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
      <td role="rowheader">[!UICONTROL描述]</td> 
      <td> <p>指定程序的描述。</p> <p>描述将显示在项目的登陆页面上。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Program Manager]</td> 
      <td> <p>开始键入要充当项目管理器的用户名称，然后在下拉列表中显示该用户名称时，单击该用户名称。 这与[!UICONTROL程序所有者]相同。 </p> <p>提示：您还可以在程序标题中更新程序管理器。 </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL组] </td> 
      <td> <p>如果某个组拥有程序或有责任完成该程序，请添加该组的名称。 </p> <p>您可以确保选择正确的组，方法是将鼠标悬停在该组上，然后单击[!UICONTROL信息]图标 <img src="assets/info-icon.png"> 显示在其旁边的。 此时会显示工具提示，其中列出了有关群组的信息，例如群组上的群组层次结构及其管理员。</p> 
       <div data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
        <img src="assets/group-details-widget-programs-350x268.png" style="width: 350;height: 268;"> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可选和视情况而定）在 **[!UICONTROL 添加自定义表单]** 框中，选择组合的自定义表单并更新自定义字段。

   >[!TIP]
   >
   >必须先创建程序自定义表单，然后才能将其附加到程序。

1. （可选）双击任意字段以更新自定义表单的信息。
1. 单击 **[!UICONTROL 项目]** 在左侧面板中，然后 **[!UICONTROL 添加项目]** 向项目添加项目。

   有关将项目添加到项目群的信息，请参阅 [将项目添加到项目群](../../../manage-work/portfolios/create-and-manage-programs/add-project-to-program.md).

1. 单击 **[!UICONTROL 保存更改]**.
1. （可选）单击 **[!UICONTROL “更多”菜单]** ![](assets/more-icon.png) 在项目名称旁边，单击 **[!UICONTROL 停用程序]**.

   当您停用某个项目时，当用户尝试将该项目添加到项目时，该项目将不再显示在项目列表中。 您仍可以从 [!UICONTROL 程序] 的上界。

## 项目标题概述

您可以在其标题中找到有关程序的有限信息。

程序标题中显示以下信息：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">标题信息</td> 
   <td> <p><strong>注释</strong> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">具有组合名称的痕迹导航</td> 
   <td>您可以从项目的标题中访问项目所属的项目组合。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">项目的名称</td> 
   <td>您可以在标题中编辑程序名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象类型的名称和激活状态</td> 
   <td>当您查看程序时，“程序”一词会显示在绿色大纲中。 单词“[!UICONTROL Devalited]”旁会显示，如果程序未标记为[!UICONTROL Active]，则大纲将灰色。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">方案的操作区域 </td> 
   <td> <p>单击以下任一选项可访问程序的更多信息或编辑选项：</p> 
    <ul> 
     <li>将程序添加到收藏夹列表的星形图标</li> 
     <li> <p>[!UICONTROL More]菜单 <img src="assets/qs-more-menu.png"> 要执行以下操作之一： </p> 
      <ul> 
       <li>编辑程序</li> 
       <li>停用它。 停用某个项目后，您无法再将其与项目级别的项目关联。 </li> 
       <li> <p>删除它。 删除程序不会删除程序中的项目。 它会删除项目与项目的关联。 </p> </li> 
       <li>与他人共享</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL完成百分比]</td> 
   <td> <p>您无法编辑标头中程序的[!UICONTROL Percent Complete]。 此信息将从项目中更新。 默认情况下，程序的完成百分比是属于程序的[!UICONTROL Current]和[!UICONTROL Approved]状态中项目完成百分比值的平均值。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Program Manager]</td> 
   <td> <p>您可以在标题中编辑项目管理器。 这与[!UICONTROL程序所有者]相同。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL计划完成日期]</td> 
   <td>您无法编辑标题中程序的完成百分比。 计划完成百分比是标题中项目完成百分比的平均值。 此处表示的项目是状态为[!UICONTROL Current]和[!UICONTROL Approved]的项目。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Active Projects Condition]</td> 
   <td>这是计算程序中将[!UICONTROL条件]设置为[!UICONTROL On Target]、[!UICONTROL At Risk]或[!UICONTROL In Foure]的项目百分比。 此处表示的项目是状态为[!UICONTROL Current]和[!UICONTROL Approved]的项目。 </td> 
  </tr> 
 </tbody> 
</table>

## 移动程序

您可以将现有项目添加到项目组合中。 由于程序不能存在于两个不同的组合中，因此添加现有程序会将其从一个组合永久移动到另一个组合。

有关更多信息，请参阅 [将现有项目添加到项目组合](../../../manage-work/portfolios/create-and-manage-programs/move-program.md).
