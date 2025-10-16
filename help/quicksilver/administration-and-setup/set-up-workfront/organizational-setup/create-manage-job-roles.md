---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 创建和管理职位角色
description: 作为 [!DNL Adobe Workfront] 管理员或对工作角色具有管理访问权限的用户，您可以创建可分配给用户的工作角色，并删除与您的组织无关的默认工作角色。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: 15063d937a5ba9b5285c66a0987e8deea6cc6d74
workflow-type: tm+mt
source-wordcount: '1139'
ht-degree: 0%

---

# 创建和管理工作角色

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

作为[!DNL Adobe Workfront]管理员或对工作角色具有管理访问权限的用户，您可以创建可分配给用户的工作角色，并删除与您的组织无关的默认工作角色。 有关[!DNL Workfront]中管理访问权限的信息，请参阅[授予用户对特定区域的管理访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 许可证</td> 
   <td><p>[!UICONTROL 标准版]</p>
       <p>[!UICONTROL 计划]</p></td>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>对工作角色的管理访问权限</td>
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 创建工作角色

要创建工作角色，请执行以下操作：

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**[!UICONTROL 工作角色]。**
1. 单击&#x200B;**[!UICONTROL 新建工作角色].**
1. 配置以下内容：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 名称]</td> 
      <td> <p>指示工作角色的名称。 这是[!DNL Workfront]中显示[!UICONTROL Job Role]字段的所有位置的名称。 </p> <p>提示：工作角色的名称最多可包含255个字符。 但是，较长的名称可能会在[!DNL Workfront]的某些区域中被截断。 </p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL 描述]</td> 
      <td>输入角色的描述，以指明其独特之处。 </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL 处于活动状态]</span> </td> 
      <td> 
       <ul> 
        <li> <p>如果希望角色处于活动状态并且在<b>中的所有位置都可用，以便与用户、工作项等关联，请选择</b>[!UICONTROL 是][!DNL Workfront]。 </p> </li> 
        <li> <p>如果希望停用该角色且不能将其分配给用户、工作项等，请选择<b>[!UICONTROL 否]</b>。 </p> </li> 
       </ul> <p><span>有关停用工作角色的信息，请参阅</span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">停用工作角色</a>。 </p> </td> 
     </tr>
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL 基础货币]</span> </td> 
      <td> <p><span>这是您的Workfront管理员在[!UICONTROL 设置]区域设置的[!UICONTROL 基础货币]。 有关信息，请参阅</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">设置汇率</a>。</p> <p>提示： <span>您无法编辑工作角色级别的[!UICONTROL 基本货币]。 此字段将灰显，并提醒您系统的基础货币是什么。</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 成本率]</td> 
      <td><p>这是工作角色的每小时成本率。 此值计算与角色相关的任务和问题的计划成本和实际成本，并最终计算项目的计划和实际成本。 使用[!UICONTROL 基础货币]输入汇率。</p> 
      <p>对于日期有效成本率，请单击<strong>[!UICONTROL 添加率]</strong>。 输入时间段的成本/小时值，并根据需要分配[!UICONTROL 开始日期]和[!UICONTROL 结束日期]。 第一个成本费率没有起始日期，最后一个成本费率没有终止日期。</p> <p>某些日期会自动添加。 例如，如果第一个成本费率没有结束日期，并且您添加了一个起始日期为2023年5月1日的第二个成本费率，则结束日期为2023年4月30日的成本费率将添加到第一个成本费率中，这样就不会出现任何差距。</p> <p>提示：编辑现有工作角色时，您可以选择<strong>按开始日期排序</strong>以在费率列表顶部查看最近的开始日期。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 记帐费率] </td> 
      <td><p>这是工作角色的每小时记帐费率。 此值计算与角色相关的任务和问题的计划收入和实际收入，最终计算项目的计划收入和实际收入。 使用[!UICONTROL 基础货币]输入汇率。</p> <p>对于生效日期记帐费率，请单击<strong>[!UICONTROL 添加费率]</strong>。 输入时间段的记帐/小时值，并根据需要分配[!UICONTROL 开始日期]和[!UICONTROL 结束日期]。 第一个记帐费率没有开始日期，最后一个记帐费率没有结束日期。</p> <p>某些日期会自动添加。 例如，如果第一个记帐费率没有结束日期，而您添加第二个记帐费率的开始日期为2023年5月1日，则结束日期为2023年4月30日将添加到第一个记帐费率，这样就不会存在任何间隔。</p> <p>提示：编辑现有工作角色时，您可以选择<strong>按开始日期排序</strong>以在费率列表顶部查看最近的开始日期。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL 覆盖货币]</span> </td> 
      <td>
        <p>选择与此工作角色关联的货币。 这是[!DNL Workfront]用于计算与此工作角色关联的成本和收入的货币。 </p> 
        <p><span>这不同于[!DNL Workfront]管理员在[!UICONTROL 设置]区域中设置的[!UICONTROL 基本货币]，并且可能不同于与项目关联的货币。</span> </p> 
        <p>提示：此字段仅提供系统中可在[!UICONTROL 汇率]区域中使用的货币。 如果只设置了一个货币，则不会显示此字段。</p> 
       <p><span>有关在[!DNL Workfront]中设置[!UICONTROL 基础货币]的信息，请参阅</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">设置汇率</a>。</p> <p><span>有关更改项目货币的信息，请参阅</span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">更改项目货币</a>。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL 覆盖货币成本率]</span> </td> 
      <td>
        <p>这是使用选定[!UICONTROL 覆盖货币]的工作角色的每小时成本费率。 [!DNL Workfront]使用此值计算与工作角色相关的任务和问题的计划成本和实际成本。 </p> 
        <p><span>以上面指定的[!UICONTROL Override Currency]输入比率。 当使用[!UICONTROL 基础货币]时，这也会更新此工作角色的成本率。</span> </p> 
        <p>有关[!DNL Workfront]如何计算成本的信息，请参阅<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">跟踪成本</a>。</p> 
       <p>提示：更新已具有关联的成本率的现有工作角色时，[!DNL Workfront]会根据系统中的转换率计算[!UICONTROL 覆盖货币]费率。 如果更新[!UICONTROL 覆盖货币成本费率]，工作角色的成本费率也会自动更新。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL 覆盖货币记帐费率]</span> </td> 
      <td>
        <p>这是使用选定[!UICONTROL 覆盖货币]的工作角色的每小时计费率。 [!DNL Workfront]使用此值计算与工作角色关联的任务和问题的计划收入和实际收入。 </p>
        <p><span>以上面指定的[!UICONTROL Override Currency]输入比率。 当使用[!UICONTROL 基本货币]时，这也会更新此工作角色的计费率。</span> </p>
        <p>有关[!DNL Workfront]如何计算收入的信息，请参阅<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">帐单和收入概览</a>。</p>
        <p>提示：更新已关联记帐费率的现有工作角色时，[!DNL Workfront]会根据系统中的兑换率计算覆盖货币费率。 如果更新“改写货币开单费率”，则工作角色的开单费率也会自动更新。 </p>
       </td>
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >工作角色是管理资源的组成部分。 要使用资源计划工具，工作角色需要与其关联的成本和记帐费率。 有关信息，请参阅[资源管理入门](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md)。

1. 单击&#x200B;**[!UICONTROL 创建工作角色]**。 工作角色现在可以分配给任务、问题、批准，或者您可以与其共享布局模板或其他对象。 有关[!DNL Workfront]中所有工作角色用途的信息，请参阅[工作角色概述](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md)。 有关删除工作角色的信息，请参阅[删除工作角色](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md)。

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
