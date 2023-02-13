---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 创建和管理作业角色
description: 作为 [!DNL Adobe Workfront] 管理员或具有“作业角色”管理访问权限的用户，可以创建可分配给用户的作业角色，并删除与您的组织无关的默认作业角色。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '917'
ht-degree: 0%

---

# 创建和管理作业角色

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

作为 [!DNL Adobe Workfront] 管理员或具有“作业角色”管理访问权限的用户，可以创建可分配给用户的作业角色，并删除与您的组织无关的默认作业角色。 有关中的管理访问权限的信息 [!DNL Workfront]，请参阅 [授予用户对特定区域的管理访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td>[!UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>对作业角色的管理访问权限</p> <p><b>注意</b>:如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 创建作业角色

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe] Workfront，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单&#x200B;击 **[!UICONTROL 作业角色].**
1. 单击 **[!UICONTROL 新工作角色].**
1. 配置以下内容：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL名称]</td> 
      <td> <p>指示作业角色的名称。 此名称会显示在 [!DNL Workfront] 其中，显示[!UICONTROL作业角色]字段。 </p> <p>提示：作业角色的名称最多可包含255个字符。 但是，较长的名称可能会在 [!DNL Workfront]. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL处于活动状态]</span> </td> 
      <td> 
       <ul> 
        <li> <p>选择 <b>[!UICONTROL Yes]</b> 如果您希望角色处于活动状态，并且可在 [!DNL Workfront] 与用户、工作项等关联。 </p> </li> 
        <li> <p>选择 <b>[!UICONTROL No]</b>，但是您希望停用角色，并且无法将角色分配给用户、工作项目等。 </p> </li> 
       </ul> <p><span>有关取消激活作业角色的信息，请参阅</span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">停用作业角色</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL描述]</td> 
      <td>输入角色的描述，以指示角色的唯一性。 </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL基本货币]</span> </td> 
      <td> <p><span>这是[!UICONTROL基本货币]，由您的Workfront管理员在[!UICONTROL设置]区域中设置。 有关信息，请参阅</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">设置汇率</a> .</p> <p>提示： <span>您无法在作业角色级别编辑[!UICONTROL基本货币]。 此字段灰显，用于提醒系统的基本货币。</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL成本/Hr.]</td> 
      <td>这是作业角色的每小时成本率。 此值计算与职责相关的任务和问题的计划成本和实际成本，以及最终的项目计划成本和实际成本。 <span>使用[!UICONTROL基本货币]输入汇率。</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Bill/Hr.] </td> 
      <td>这是作业角色的每小时费率。 此值计算与角色相关的任务和问题的计划收入和实际收入，以及最终项目的计划收入和实际收入。 使用[!UICONTROL基本货币]输入汇率。 </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL覆盖货币]</span> </td> 
      <td> 
       <div> 
        <p>选择与此作业角色关联的货币。 这是 [!DNL Workfront] 用于计算与此职务角色关联的成本和收入。 </p> 
        <p><span>这与由 [!DNL Workfront] 管理员（位于[!UICONTROL设置]区域），并且可以与与项目关联的货币不同。</span> </p> 
        <p>提示：只有您系统的[!UICONTROL Exchange Rates]区域中可用的货币才可在此字段中使用。</p> 
       </div> <p><span>有关在中设置[!UICONTROL基本货币]的信息 [!DNL Workfront]，请参阅</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">设置汇率</a>.</p> <p><span>有关更改项目货币的信息，请参阅</span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">更改项目货币</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL覆盖货币成本/小时]</span> </td> 
      <td> 
       <div> 
        <p>这是使用选定的[!UICONTROL改写货币]的任务角色的每小时成本费率。 [!DNL Workfront] 使用此值计算与任务职责关联的任务和问题的计划成本和实际成本。 </p> 
        <p><span>在上面指定的[!UICONTROL覆盖货币]中输入汇率。 此外，在使用[!UICONTROL基本货币]时，还会更新此作业角色的成本/小时费率。</span> </p> 
        <p>有关如何 [!DNL Workfront] 计算成本，请参阅 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">跟踪成本</a>.</p> 
       </div> <p>提示：更新已与其关联成本/小时费率的现有作业角色时， [!DNL Workfront] 根据系统中的兑换率计算[!UICONTROL覆盖货币]汇率。 如果更新[!UICONTROL改写货币成本/小时]，则任务角色的成本/小时也会自动更新。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL覆盖货币帐单/小时]</span> </td> 
      <td> 
       <div> 
        <p>这是使用选定的[!UICONTROL覆盖货币]的作业角色每小时计费费率。 [!DNL Workfront] 使用此值计算与任务职责相关的任务和问题的计划收入和实际收入。 </p> 
        <p><span>在上面指定的[!UICONTROL覆盖货币]中输入汇率。 此外，在使用[!UICONTROL基本货币]时，还会更新此作业角色的帐单/小时费率。</span> </p> 
        <p>有关如何 [!DNL Workfront] 计算收入，请参阅 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">账单和收入概述</a>.</p> 
       </div> <p>提示：更新已与其关联开单/小时费率的现有作业角色时， [!DNL Workfront] 根据系统中的兑换率计算“覆盖货币”汇率。 如果您更新“改写货币开单/小时”，则作业角色的开单/小时也会自动更新。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >工作角色是管理资源的一个组成部分。 要使用资源规划工具，任务角色需要与它们关联的成本和开单费率。 有关信息，请参阅 [资源管理入门](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

1. 单击 **[!UICONTROL 创建作业角色]**. 作业角色现在可分配给任务、问题、审批，或者您可以与其共享布局模板或其他对象。 有关中作业角色的所有用法的信息 [!DNL Workfront]，请参阅 [作业角色概述](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). 有关删除作业角色的信息，请参阅 [删除作业角色](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Delete a job role</h2>
<ol data-mc-continue="false">
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <strong>Setup</strong> <img src="assets/gear-icon-settings.png">.</li>
<li value="2">Click<strong>Job Roles.</strong></li>
<li value="3">Select the job role that you want to delete, then click <strong>Delete.</strong></li>
<li value="4">If there are any objects (users, tasks, issues) that are assigned to the job role, do one of the following:<br>
<ul>
<li><p><strong>Replace the job role with a different job role:</strong> Select the new job role from the drop-down list.</p><p>Any current and past resource allocations that are associated with the deleted job role are transferred to the job role that you select.</p><p>Users who have only one job role assigned to them are reassigned to the job role that you select; users who have a secondary job role assigned to them are not reassigned to the job role that you select.</p></li>
<li><p><strong>Delete the job role and its resource allocation:</strong> Select<strong>None</strong> from the drop-down list.</p><note type="important">
Deleting a job role deletes all current and past resource allocation related to that job role for all projects.
</note><p>​For example, if a task or issue is assigned to only that job role, the task or issue is unassigned after the job role is deleted.</p></li>
</ul></li>
<li value="5">Click  <strong>Yes, Delete It</strong>. </li>
</ol>
</div>
-->
