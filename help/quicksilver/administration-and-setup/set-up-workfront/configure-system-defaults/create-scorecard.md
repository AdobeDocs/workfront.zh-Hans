---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: 创建记分卡
description: 评分卡衡量项目与之前已确立的项目组合标准的一致性。 评分卡通常反映组织的使命、价值和战略目标。Portfolio经理通常定义评分卡问题和答案，以确保它们在项目优先级和选择期间有意义且有价值。 安 [!DNL Adobe Workfront] 管理员基于组合管理器中的建议来构建记分卡。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 89c9b450-72a6-4b72-98d1-22956696543a
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# 创建记分卡

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

评分卡衡量项目与之前已确立的项目组合标准的一致性。 评分卡通常反映组织的使命、价值和战略目标。

Portfolio经理通常会定义评分卡问题和答案，以确保它们在项目优先级排序和选择期间有意义且有价值。 安 [!DNL Adobe Workfront] 管理员基于组合管理器中的建议来构建记分卡。

为评分卡选择的问题和答案必须可以量化，以便提供比较不同项目的对齐值。

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td> <p>[!UICONTROL Business]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td>[!UICONTROL计划]</td> 
  </tr> 
 </tbody> 
</table>

## 创建记分卡

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 单击 **[!UICONTROL 记分卡]**，然后单击 **[!UICONTROL 新建记分卡]** 创建新记分卡并启动记分卡生成器。

1. 指定 **[!UICONTROL 记分卡名称]** 和 **[!UICONTROL 描述]**.

   在将记分卡与项目关联时，会显示该名称。 描述显示在记分卡列表中记分卡名称旁边。

1. 单击 **[!UICONTROL 添加问题]** 用于打开 [!UICONTROL 记分卡问题] ，然后为问题指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL问题]</td> 
      <td>键入要包含在记分卡中的问题。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL点]</td> 
      <td>键入此问题可能的最大点数。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL负点]</td> 
      <td>选择此选项可指示 [!DNL Workfront] 应从可能的总分中减去。 负分数无法添加到记分卡的最大可能点数。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL显示类型]</td> 
      <td>选择 <strong>[!UICONTROL值(0-100)]</strong> 如果要在评分卡中显示数字字段，用户可以在其中指定0到100之间的任何值。<p>或者，选择 <strong>[!UICONTROL下拉列表]</strong> 或 <strong>[!UICONTROL单选按钮]</strong> 要创建答案，用户可以使用该控件指定。 单击 <strong>[!UICONTROL添加答案]</strong>，然后键入 <strong>[!UICONTROL值]</strong> 以百分点表示，以防此答案得到满足。 如果选择100%，则为此问题分配的分数将完全实现。 如果要指明此答案仅包含分配给此问题的总分数的一部分，请选择一个较低的百分比值。 例如，如果您的问题的值为10点，并且您希望此答案包含其中5点，则为您的值选择50%。</p>
      <p>选择 <strong>[!UICONTROL默认]</strong> 如果您指明此答案为默认答案，则。</strong></p>
     </tr> 
    </tbody> 
   </table>

1. 单击 **[!UICONTROL 添加问题]** 要向记分卡添加更多问题和答案，请执行相同的步骤。

   >[!NOTE]
   >
   >您可以通过按正确顺序拖放问题来重新排序记分卡中的问题。

1. 单击 **[!UICONTROL 保存]** 完成输入数据时。

## 将记分卡应用于项目

具有 [!UICONTROL 管理] 对项目的权限，可在记分卡创建后将记分卡应用到项目 [!DNL Workfront] 管理员。

在为项目创建业务案例时，会向项目添加记分卡。 有关向项目添加记分卡的更多信息，请参阅 [将记分卡应用于项目并生成对齐分数](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

有关创建记分卡的更多信息，请参阅 [创建记分卡](#create-a-scorecard).

有关项目权限的更多信息，请参阅 [在中共享项目 [!DNL Adobe Workfront]](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
