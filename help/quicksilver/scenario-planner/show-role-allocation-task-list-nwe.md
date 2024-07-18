---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 在任务列表中显示项目和计划的角色分配
description: 连接项目和计划后，您可以并排管理其资源分配以确保它们相匹配。 这样可避免过度分配或过度利用它们。
author: Alina
feature: Workfront Scenario Planner
exl-id: 77152e46-0b7b-4937-9d16-1a20c2a7fdf1
source-git-commit: 82a5102d28700368a094502dcd6026462c149eb1
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 0%

---

# 在任务列表中显示项目和计划的角色分配

>[!IMPORTANT]
>
>您的组织必须为[!DNL Adobe Workfront Scenario Planner]购买额外的许可证，以便您可以查看项目的计划信息。 有关获取[!DNL Workfront Scenario Planner]的信息，请参阅[使用 [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md)所需的访问权限。

连接项目和计划后，您可以并排管理其资源分配以确保它们相匹配。 这样可避免过度分配或过度利用它们。

本文介绍了如何使用项目任务列表中的[!UICONTROL 角色分配]面板协调资源。

有关在项目和计划之间协调资源的一般信息，包括先决条件，请参阅[在项目和计划之间协调资源分配概述](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md)。

## 访问要求

您需要执行以下操作：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b>计划*</b> </p> </td> 
   <td>[！UICONTROL Business]或更高版本</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b>许可证*</b> </p> </td> 
   <td> <p>[！UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td><b>产品</b> </td> 
   <td> <p>您必须为[!DNL Adobe Workfront Scenario Planner]购买额外的许可证才能访问本文中介绍的功能。</p> <p>有关获取[!DNL Workfront Scenario Planner]的信息，请参阅<a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用[!DNL Scenario Planner]</a>所需的访问权限。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>访问级别配置*</strong> </td> 
   <td> <p>[！UICONTROL视图]或更高项目访问权限 </p> <p>注意：如果您仍然没有访问权限，请咨询您的[！UICONTROL Workfront]管理员，了解他们是否对您的访问级别设置了其他限制。 有关[！UICONTROL Workfront]管理员如何更改访问级别的信息，请参阅<a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>对象权限</strong> </p> </td> 
   <td> <p>项目的[！UICONTROL视图]或更高权限</p> <p>有关请求对计划的附加访问权限的信息，请参阅<a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">在[!DNL Scenario Planner]</a>中请求对计划的访问权限。</p> <p>有关请求对项目的附加访问权限的信息，请参阅<a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象</a>的访问权限。 </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

## 在任务列表中显示项目和计划的角色分配

如果贵公司已购买[!DNL Workfront Scenario Planner]许可证，则可以在项目的[!UICONTROL 任务]部分中协调计划与链接到该计划的项目之间的资源分配。

1. （视情况而定）使用本文的任务列表](#Connect)中的[显示项目和计划的角色分配中所述的方法之一，将项目与计划连接起来。

   >[!IMPORTANT]
   >
   >如果对计划中的资源进行了更改，则必须重新发布计划所属的方案，以便计划中的最新资源信息能够更新项目。

1. 转到要在其中查看项目和相关计划的工作角色分配情况的项目。
1. 单击左侧面板中的&#x200B;**[!UICONTROL 任务]**。
1. 单击工具栏右上角的&#x200B;**[!UICONTROL 显示角色分配]**&#x200B;图标![](assets/show-role-allocation-icon.png)。

   此时将显示[!UICONTROL 角色分配]面板。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. 查看[!UICONTROL 角色分配]面板的&#x200B;**[!UICONTROL 项目总计]**&#x200B;区域中的以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL Job Role]</td> 
      <td> <p>与以下任何一项关联的工作角色的名称：</p> 
       <ul> 
        <li> <p>项目中的任务</p> </li> 
        <li> <p>项目问题</p> </li> 
        <li> <p>链接到项目的计划</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL计划小时数]</td> 
      <td>计划总持续时间内与计划上每个工作角色关联的所需小时数。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL已计划小时数]</td> 
      <td>在项目总持续时间内，与项目任务或问题中的每个工作角色关联的已计划小时数。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL变量]</td> 
      <td> <p>计划所需的小时数与项目工作相关的计划小时数之间的差额。 [!DNL Workfront]使用以下公式计算[！UICONTROL方差]：</p> <p><code>Role Allocation Variance = Initiative Hours - Planned Hours</code> </p> <p>当计划的资源时间超过计划所需的小时数时，[！UICONTROL差异]为负数并显示为红色。 这意味着您的资源被过度分配。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >项目中的计划小时数未显示在以下方案中：
   >
   >   
   >   
   >   * 未将任务或问题分配给工作角色或与其关联的工作角色的用户。
   >   * 当任务或问题的持续时间为零时。
   >   
   >



1. （可选）如果[!UICONTROL Variance]列显示您的资源分配过量，请调整以下选项之一：

   * 减少显示过度分配的一个工作角色的计划小时数，或向任务添加更多资源，并向新资源分配更多计划小时数。 您可以在编辑任务或问题时更新分配或计划小时数。 有关更多信息，请参阅以下文章：

      * [编辑任务](../manage-work/tasks/manage-tasks/edit-tasks.md)
      * [编辑问题](../manage-work/issues/manage-issues/edit-issues.md)

     >[!NOTE]
     >
     >您必须具有其他访问权限才能编辑任务和问题。

   * 增加显示计划过度分配的角色所需的小时数。 有关详细信息，请参阅[在 [!DNL Adobe Workfront Scenario Planner]](create-and-edit-initiatives.md)中创建和编辑计划。

     >[!NOTE]
     >
     >您必须具有其他访问权限才能编辑计划。


