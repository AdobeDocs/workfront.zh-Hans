---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 删除方案计划员中的计划
description: 您可以删除已创建的计划。 您无法删除与您共享的计划。
author: Alina
feature: Workfront Scenario Planner
exl-id: 74515723-3822-425a-aa9e-970af63f9189
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 1%

---

# 删除 [!DNL Scenario Planner]

您可以删除已创建的计划。 您无法删除与您共享的计划。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> 计划*</b> </p> </td> 
   <td>[!UICONTROL Business]或更高版本</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> 许可证*</b> </p> </td> 
   <td> <p>[!UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td><b>产品</b> </td> 
   <td> <p>您必须为 [!DNL Adobe Workfront Scenario Planner] ，以访问本文中描述的功能。</p> <p>有关获取 [!DNL Workfront Scenario Planner]，请参阅 <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用所需的访问权限 [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>访问级别配置*</strong> </td> 
   <td> <p>[!UICONTROL Edit]对 [!DNL Scenario Planner]</p> <p>注意：如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>对象权限</strong> </p> </td> 
   <td> <p>[!UICONTROL管理]计划的权限</p> <p>有关请求对计划进行额外访问的信息，请参阅 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">请求对 [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 删除计划

>[!IMPORTANT]
>
>您无法恢复已删除的计划。

您可以删除计划，也可以删除计划中的一个方案。

* [删除计划](#delete-plans)
* [删除方案](#delete-scenarios)

### 删除计划

>[!IMPORTANT]
>
>删除计划时请考虑以下事项：
>
>* 与计划相关的所有信息也将被删除。 这包括与计划相关的所有设想方案和倡议，包括关于工作角色和成本的信息。 无法恢复此信息。
>* 如果计划包含已发布的方案，则链接到已删除方案的项目将保留，并且 [!DNL Scenario Planner] 区域仍在 [!UICONTROL 项目详细信息] 中。
>
>  有关将方案发布到项目的信息，请参阅 [通过在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

要删除计划，请执行以下操作：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png)，然后单击 [!UICONTROL 方案].

   此时将显示计划列表。

1. 单击计划的名称以将其打开。
1. 单击 **[!UICONTROL “更多”菜单]** ![](assets/more-menu.png) 在计划名称的右侧，单击 **[!UICONTROL 删除]** > **[!UICONTROL 是，删除它]**.

   计划将被删除，您将返回计划列表。

### 删除方案 {#delete-scenarios}

>[!IMPORTANT]
>
>删除方案时，请考虑以下事项：
>
>* 删除方案会从方案中删除所有方案及其信息。 如果这些方案被复制到其他方案，则这些方案将保留在其他方案中。
>* 删除某个方案时，后续方案将采用已删除方案的数量，并保留计数顺序。 例如，如果删除方案4，则方案5将变为方案4。
>* 如果发布了方案上的某些方案，则与方案关联的项目将保留，并且方案规划器区域将保留在链接的项目上
>* 如果已发布的倡议存在于另一种情景中，则它们仍保留在该情景中，包括它们与项目的链接。 从其他情景中发布这些计划会使用这些情景中的新信息更新链接的项目。
>
>  有关将方案发布到项目的信息，请参阅 [通过在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

要删除方案，请执行以下操作：

1. 转到要删除方案的计划。

   默认情况下，将显示初始方案。

1. 单击 **[!UICONTROL 比较方案]**.
1. 从方案卡的右上角，单击 **[!UICONTROL 更多]** 菜单 ![](assets/more-menu.png)，然后单击 **[!UICONTROL 删除]**.

   方案将被删除。

1. 单击 **[!UICONTROL 保存计划]** 以保存更改。

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


