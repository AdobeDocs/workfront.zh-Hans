---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 删除方案规划程序中的计划
description: 您可以删除已创建的计划。 不能删除与您共享的计划。
author: Alina
feature: Workfront Scenario Planner
exl-id: 74515723-3822-425a-aa9e-970af63f9189
source-git-commit: 7cfe82eb703e2a043c264cf86c0e5424d1e33d78
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 1%

---

# 删除[!DNL Scenario Planner]中的计划

您可以删除已创建的计划。 不能删除与您共享的计划。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 计划*</p> </td> 
   <td> <ul></li>
   <li><p>新增功能：Ultimate </p></li>
   <p>Scenario Planner不可用于新的Workfront Select或Workfront Prime计划。 </p>
   <li><p>当前： [！UICONTROL Business]或更高版本</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 许可证*</p> </td> 
   <td> <p>新增：浅色或更高</p> 
   <p>当前： [！UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td>产品* </td> 
   <td> <ul><li><p>对于新的Workfront计划：</p><p> Adobe Workfront</li></p>
   <li><p>对于当前Workfront计划： </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>

<p>有关详细信息，请参阅<a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用[!DNL Scenario Planner]</a>所需的访问权限。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>访问级别 </td> 
   <td> <p>[！UICONTROL Edit]访问 [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>对象权限 </p> </td> 
   <td> <p>[！UICONTROL Manage]对计划的权限</p> <p>有关请求对计划的附加访问权限的信息，请参阅<a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">在[!DNL Scenario Planner]</a>中请求对计划的访问权限。</p> </td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅[Workfront文档的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 删除计划

>[!IMPORTANT]
>
>无法恢复已删除的计划。

您可以删除计划，也可以删除计划中的一个方案。

* [删除计划](#delete-plans)
* [删除方案](#delete-scenarios)

### 删除计划

>[!IMPORTANT]
>
>删除计划时，请考虑以下事项：
>
>* 与计划相关的所有信息也会被删除。 这包括与该计划相关的所有方案和计划，包括有关工作角色和成本的信息。 此信息无法恢复。
>* 如果计划包含已发布的方案，则将保留链接到已删除计划的项目，并且[!DNL Scenario Planner]区域保留在[!UICONTROL 项目详细信息]部分。
>
>  有关将计划发布到项目的信息，请参阅[通过在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)中发布计划来更新或创建项目。

要删除计划，请执行以下操作：

{{step1-to-scenario-planner}}

此时将显示计划列表。

1. 单击计划的名称以将其打开。
1. 单击计划名称右侧的&#x200B;**[!UICONTROL 更多菜单]** ![更多菜单](assets/more-menu.png)，然后单击&#x200B;**[!UICONTROL 删除]** > **[!UICONTROL 是，删除它]**。

   计划将被删除，您将返回到计划列表。

### 删除方案 {#delete-scenarios}

>[!IMPORTANT]
>
>删除场景时，请考虑以下事项：
>
>* 删除方案会从方案中删除所有计划及其信息。 如果将这些计划复制到其他方案，则这些计划将保留在其他方案上。
>* 当删除场景时，后续场景接受被删除场景的个数，并且保留计数顺序。 例如，如果删除方案4，则方案5将变为方案4。
>* 如果发布了方案上的某些计划，则保留链接到计划的项目，并且“方案规划器”区域保留在链接的项目上
>* 如果发布的计划存在于另一个方案中，则它们仍存在于该方案中，包括它们与项目的链接。 从其他方案发布这些计划会使用来自这些方案的新信息更新链接的项目。
>
>  有关将计划发布到项目的信息，请参阅[通过在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)中发布计划来更新或创建项目。

要删除方案，请执行以下操作：

1. 转到要删除方案的计划。

   默认情况下，将显示初始方案。

1. 单击&#x200B;**[!UICONTROL 比较方案]**。
1. 从方案卡的右上角，单击&#x200B;**[!UICONTROL 更多]**&#x200B;菜单![更多](assets/more-menu.png)，然后单击&#x200B;**[!UICONTROL 删除]**。

   方案将被删除。

1. 单击&#x200B;**[!UICONTROL 保存计划]**&#x200B;以保存更改。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Delete initiatives</h2>
<p>(NOTE: moved this section to its own article about deleting initiatives) </p> <note type="important">
<p>Consider the following when deleting initiatives:</p>
<ul>
<li>Deleting an initiative deletes the job roles and cost information from the initiative.</li>
<li><span>When you delete an initiative that is published to a project, the initiative is removed from the scenario but the Scenario Planner area remains in the Project Details section.</span> </li>
<li> <p>If the initiative you delete is the only published initiative on the scenario, the indicator that the plan has been published is also removed. </p> <p>For information about publishing initiatives to projects, see <a href="../scenario-planner/publish-scenarios-update-projects.md" class="MCXref xref">Update or create projects by publishing initiatives in the Scenario Planner</a>.</p> </li>
</ul>
</note>
<p>To delete an initiative:</p>
<ol>
<li value="1"> <p> <p>Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png">, then click Scenarios.</p> </p> <p>A list of plans displays. </p> </li>
<li value="2">Click the name of a plan to open it, then locate the initiative you want to delete.</li>
<li value="3"> <p>Click the <strong>More menu</strong> <img src="assets/more-menu.png"> to the right of the initiative name, then click <strong>Delete</strong> > <strong>Yes, delete it</strong>. </p> <p>The initiative is deleted. </p> </li>
<li value="4">Click <strong>Save Plan</strong> to save your changes. </li>
</ol>
</div>
-->


