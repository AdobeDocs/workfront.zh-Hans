---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 创建和管理职位角色
description: 作为 [!DNL Adobe Workfront] 管理员或对工作角色具有管理访问权限的用户，您可以创建可分配给用户的工作角色，并删除与您的组织无关的默认工作角色。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: fda9c07ee43cc4e6ba1a26ea937ca820367800a8
workflow-type: tm+mt
source-wordcount: '1173'
ht-degree: 0%

---

# 创建和管理职位角色

{{highlighted-preview}}

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

作为 [!DNL Adobe Workfront] 管理员或对工作角色具有管理访问权限的用户，您可以创建可分配给用户的工作角色，并删除与您的组织无关的默认工作角色。 有关中管理访问权限的信息 [!DNL Workfront]，请参见 [授予用户对特定区域的管理访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

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
   <td>[！UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>对工作角色的管理访问权限</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询 [!DNL Workfront] 管理员（如果他们在您的访问级别设置了其他限制）。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参见 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

## 创建工作角色

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) （位于的右上角） [!DNL Adobe] Workfront，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击&#x200B;。 **[!UICONTROL 职位角色].**
1. 单击 **[!UICONTROL 新建工作角色].**
1. 配置以下内容：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL名称]</td> 
      <td> <p>指示工作角色的名称。 此名称在中显示 [!DNL Workfront] 其中[！UICONTROL Job Role]字段显示。 </p> <p>提示：工作角色的名称最多可包含255个字符。 但是，较长的名称可能会被截断在某些区域 [!DNL Workfront]. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[！UICONTROL处于活动状态]</span> </td> 
      <td> 
       <ul> 
        <li> <p>选择 <b>[！UICONTROL是]</b> 如果您希望角色在中任何位置都处于活动状态且可用 [!DNL Workfront] ，以与用户、工作项等关联。 </p> </li> 
        <li> <p>选择 <b>[！UICONTROL否]</b>，如果您希望停用角色且不能将其分配给用户、工作项等。 </p> </li> 
       </ul> <p><span>有关停用工作角色的信息，请参阅</span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">取消激活工作角色</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL描述]</td> 
      <td>输入角色的描述，以指示该角色的独特之处。 </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[！UICONTROL基本货币]</span> </td> 
      <td> <p><span>这是[！UICONTROL基本货币]，由Workfront管理员在[！UICONTROL设置]区域设置。 有关信息，请参阅</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">设置汇率</a> .</p> <p>提示： <span>无法在工作角色级别编辑[！UICONTROL基本货币]。 该字段呈灰显状态，提醒您系统的基本货币是什么。</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL成本/小时]</td> 
      <td><p>这是工作角色的每小时成本率。 此值计算与角色相关的任务和问题的计划成本和实际成本，并最终计算项目的计划和实际成本。 使用[！UICONTROL基本货币]输入汇率。</p> 
      <p><span class="preview">对于日期有效成本率，请单击 <strong>[！UICONTROL添加率]</strong>. 输入时间段的成本/小时值，并根据需要分配[！UICONTROL开始日期]和[！UICONTROL结束日期]。 第一个成本费率没有起始日期，最后一个成本费率没有终止日期。</span></p> <p><span class="preview">某些日期会自动添加。 例如，如果第一个成本费率没有终止日期，并且您添加了一个起始日期为2023年5月1日的第二个成本费率，则终止日期为2023年4月30日将添加到第一个成本费率，这样就不会存在任何间隔。</span></p> <p><span class="preview">提示：编辑现有工作角色时，您可以选择 <strong>按开始日期排序</strong> 在费率列表顶部查看最近的开始日期。 </span></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL账单/小时] </td> 
      <td><p>这是工作角色的每小时记帐费率。 此值计算与角色相关的任务和问题的计划收入和实际收入，最终计算项目的计划收入和实际收入。 使用[！UICONTROL基本货币]输入汇率。</p> <p><span class="preview">要了解生效日期记帐费率，请单击 <strong>[！UICONTROL添加率]</strong>. 输入时间段的计费/小时值，并根据需要分配[！UICONTROL开始日期]和[！UICONTROL结束日期]。 第一个记帐费率没有开始日期，最后一个记帐费率没有结束日期。</span></p> <p><span class="preview">某些日期会自动添加。 例如，如果第一个记帐费率没有结束日期，而您添加的第二个记帐费率的开始日期为2023年5月1日，则结束日期为2023年4月30日将添加到第一个记帐费率，因此不存在间隔。</span></p> <p><span class="preview">提示：编辑现有工作角色时，您可以选择 <strong>按开始日期排序</strong> 在费率列表顶部查看最近的开始日期。 </span></p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[！UICONTROL替代货币]</span> </td> 
      <td> 
       <div> 
        <p>选择与此工作角色关联的货币。 这就是那种货币 [!DNL Workfront] 使用计算与此工作角色关联的成本和收入。 </p> 
        <p><span>这与您设置的[！UICONTROL基础货币]不同 [!DNL Workfront] 管理员（位于[！UICONTROL设置]区域），并且可以不同于与项目关联的货币。</span> </p> 
        <p>提示：此字段仅系统中在[！UICONTROL汇率]区域可用的货币。</p> 
       </div> <p><span>有关在中设置[！UICONTROL基本货币]的信息 [!DNL Workfront]，请参见</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">设置汇率</a>.</p> <p><span>有关更改项目货币的信息，请参见</span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">更改项目货币</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[！UICONTROL覆盖货币成本/小时]</span> </td> 
      <td> 
       <div> 
        <p>这是使用选定[！UICONTROL覆盖货币]的工作角色的每小时成本费率。 [!DNL Workfront] 使用此值计算与工作角色相关联的任务和问题的计划成本和实际成本。 </p> 
        <p><span>以上面指定的[！UICONTROL覆盖货币]输入比率。 当使用[！UICONTROL基本货币]时，这也会更新此工作角色的成本/小时率。</span> </p> 
        <p>有关如何 [!DNL Workfront] 计算成本，请参阅 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">跟踪成本</a>.</p> 
       </div> <p>提示：更新已具有关联的成本/小时费率的现有工作角色时， [!DNL Workfront] 根据您系统中的兑换率计算[！UICONTROL覆盖货币]兑换率。 如果更新[！UICONTROL覆盖货币成本/小时]，工作角色的成本/小时也会自动更新。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[！UICONTROL覆盖货币计费/小时]</span> </td> 
      <td> 
       <div> 
        <p>这是使用选定[！UICONTROL覆盖货币]的工作角色的每小时记帐费率。 [!DNL Workfront] 使用此值计算与工作角色相关联的任务和问题的计划收入和实际收入。 </p> 
        <p><span>以上面指定的[！UICONTROL覆盖货币]输入比率。 当使用[！UICONTROL基本货币]时，这也会更新此工作角色的计费/小时费率。</span> </p> 
        <p>有关如何 [!DNL Workfront] 计算收入，请参阅 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">开单和收入概览</a>.</p> 
       </div> <p>提示：更新已具有关联的计费/小时费率的现有工作角色时， [!DNL Workfront] 根据系统中的折换率计算改写币种汇率。 如果您更新覆盖货币计费/小时，则工作角色的计费/小时也会自动更新。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >工作角色是管理资源的一个组成部分。 要使用资源计划工具，工作角色需要与其关联的成本和记帐费率。 有关信息，请参阅 [资源管理入门](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

1. 单击 **[!UICONTROL 创建工作角色]**. 工作角色现在可以分配给任务、问题、批准，或者您可以与其共享布局模板或其他对象。 有关中工作角色的所有用途的信息 [!DNL Workfront]，请参见 [工作角色概述](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). 有关删除工作角色的信息，请参阅 [删除工作角色](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

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
