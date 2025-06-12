---
title: 配置Adobe Workfront Planning自动化
description: 您可以在Adobe Workfront Planning中配置自动化操作，在激活时，可在Workfront中创建对象或Workfront Planning中的记录。 创建的对象和记录会自动连接到现有Planning记录。 本文介绍了如何管理自动化，包括如何编辑、禁用或删除自动化。
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: cde20e5a-15a2-413a-8de4-ccf6eeb4395f
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '1796'
ht-degree: 3%

---

# 配置Adobe Workfront Planning自动化

<!--add screen shots when UI is finalized AND redo all the steps - some things got changed and moved around-->

<!--you might need to add something about notifications and emails?!-->
<!--add a new section to this article to mention a new way to create objects: help/quicksilver/planning/records/create-records.md-->
<!-- add a new section to this article to mention a new way to create WF objects from Planning: help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md-->

<!-- if they give access to use the automation to people with LESS than Manage permissions to a workspace, split this article in two: the Configure section should be for admins and the "Use a Workfront Planning automation to create an object" should be for all other users-->

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

您可以在Adobe Workfront Planning中配置自动处理，激活自动处理后，可在从Planning记录触发时，在Workfront中创建对象，或在Workfront Planning中创建记录。 创建的对象或记录会自动连接到从中触发自动化的记录。

您可以在Workfront Planning的记录类型页面中配置和激活自动化。

例如，您可以创建一个接受Workfront Planning营销活动的自动化功能，并在Workfront中创建一个项目以跟踪该营销活动的进度。

本文介绍如何管理自动化，包括如何编辑、禁用、删除和触发它们以创建对象和记录。

有关如何使用现有自动化创建记录或对象的信息，请参阅[使用Adobe Workfront Planning记录自动化创建对象](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md)。

## 访问要求

+++ 展开以查看访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> 产品</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront规划<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront计划*</p></td> 
   <td> 
<p>以下任意Workfront计划：</p> 
<ul><li>选择</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning不适用于旧版Workfront计划</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront规划包*</p></td> 
   <td> 
<p>任何 </p> 
<p>有关每个Workfront计划中包括的内容的更多信息，请联系您的Workfront客户经理。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>贵组织的Workfront实例必须载入Adobe Unified Experience才能访问Workfront Planning。</p> 
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">适用于Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td> 
   <td> 标准
   <p>Workfront计划不适用于旧版Workfront许可证</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td> <p>Adobe Workfront Planning没有访问级别控制</p> 
   <p>编辑访问权限，访问权限：在Workfront中为要创建的对象类型（项目、项目组合、项目群）创建对象。 </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td> <p>管理工作区<span class="preview">和要创建自动操作的记录类型</span>的权限。 </p>
   <p>系统管理员对所有工作区具有管理权限，包括他们未创建的工作区</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面模板</p></td> 
   <td> <p>在生产环境中，必须将所有用户（包括系统管理员）分配到包含Planning的布局模板。</p>
<p><span class="preview">在“预览”环境中，标准用户和系统管理员默认启用Planning。</span></p> </td> 
  </tr> 
</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在Workfront Planning中配置自动化

您必须先在Workfront Planning中为记录类型配置自动化，然后才能使用它创建对象。

{{step1-to-planning}}

1. 单击记录类型卡片，然后单击记录名称。

   此时将打开记录类型页面。
1. 单击记录类型名称右侧的&#x200B;**更多**&#x200B;菜单![更多菜单](assets/more-menu.png)，然后单击&#x200B;**管理自动化**。

   将打开所选记录类型的可用自动化列表。

1. 单击屏幕右上角的&#x200B;**新建自动化**。 将打开&#x200B;**新自动化**&#x200B;框。
1. 更新以下字段：

   * 将&#x200B;**无标题的自动化**&#x200B;替换为要显示在自动化按钮上的文本。 使用自动化创建Workfront对象或Planning记录时，用户将单击此按钮。
   * **描述**：添加描述以标识自动化的目的。
1. 单击&#x200B;**保存**。
自动化详细信息页面将打开。

1. 在自动化的详细信息页面上，更新&#x200B;**触发器**&#x200B;部分中的以下字段：

   * **触发器**：选择将触发自动化的操作。 例如，选择&#x200B;**按钮单击**。<!--update this step with a list of all possible triggers; right now only Button click is available-->

1. 更新&#x200B;**操作**&#x200B;部分中的以下字段： <!--submitted bugs for these fields - see if they need changing here-->
   * **操作**：选择在触发自动操作时希望Workfront执行的操作。 这是必填字段。
选择以下操作之一：

      * 创建多个项目
      * 创建单个项目
      * 创建项目
      * 创建记录
      * 创建程序
      * 创建项目组合
      * 创建组

     >[!TIP]
     >
     >保存自动化后，无法再更改在此字段中选择的操作。

1. （视情况而定）根据您选择的操作，更新以下字段：

   * **创建单个项目**： <!--replace to the left: Create a single project-->
      * **创建项目的已连接字段**：这是将显示新项目的已连接字段。 这是必填字段。
      * **项目模板**：选择Workfront将用于创建项目的项目模板。

   * 创建多个项目：
      * **创建项目的已连接字段**：这是将显示新项目的已连接字段。 这是必填字段。
      * **其选择将创建记录的字段**：从所选记录类型中选择多选或单选字段。 Workfront会为当前在记录中选定的每个字段选项创建一个项目，您将从该记录中触发自动化。

     >[!TIP]
     >
     >项目仅针对运行自动化的记录的多选或单选字段上当前选定的选项创建，而不是针对该字段的所有可能选项创建。
     >

      * **使用相同的模板**：选择此选项可针对每个新项目使用相同的模板。 如果取消选择该选项，请为每个字段选择一个&#x200B;**项目模板**。
      * **项目模板**：如果您选择了&#x200B;**使用同一模板**&#x200B;选项，请选择Workfront将用于创建项目的项目模板。

   * **创建项目组合**：
      * **在其中创建项目组合的已连接字段**：这是将显示新项目组合的已连接字段。 这是必填字段。
      * **要附加到新项目组合的自定义表单**：选择要附加到新项目组合的自定义表单。 您必须先创建项目组合自定义表单，然后才能选择它。
   * **创建程序**：
      * **在其中创建程序的已连接字段**：这是将显示新程序的已连接字段。 这是必填字段。
      * **项目组合**：选择将添加新项目的项目组合。 这是必填字段。
      * **要附加到新程序的自定义表单**：选择要附加到新程序的自定义表单。 您必须先创建程序自定义表单，然后才能选择它。
   * **创建组**：
      * **在其中创建组的已连接字段**：这是将显示新组的已连接字段。 这是必填字段。
      * **要附加到新组的自定义表单**：选择要附加到新程序的自定义表单。 您必须先创建程序自定义表单，然后才能选择它。
   * **创建记录**：
      * **记录类型**：选择要创建的记录类型。

        将显示&#x200B;**设置**&#x200B;子部分。 更新&#x200B;**设置**&#x200B;子部分中的以下字段：

         * **将显示当前记录的已连接记录类型上的字段**：这是为将显示当前记录的操作选择的记录类型上的已连接字段。

        例如，如果您正在创建用于连接产品记录的营销活动的自动化，则在使用自动化创建产品后，这是产品记录类型上将显示营销活动的已连接字段。

        这是必填字段。

        <!--submitted a change in functionality and UI text for this - revise??-->
在&#x200B;**映射字段**&#x200B;区域中，更新以下信息：

         * **传输自**：从创建自动化的记录类型中选择字段，以将其映射到连接的记录类型的字段。
         * **传输到**：从新创建的记录中选择将使用您运行自动化的记录中的信息填充的字段。

        >[!TIP]
        >
        >* 原始记录类型中的字段类型必须与新创建的记录类型中的字段类型匹配。
        >* 如果未选择任何字段，则新记录的名称将为&#x200B;**无标题记录**。

1. （可选且有条件）如果您选择创建记录，请单击&#x200B;**添加字段**&#x200B;以将其他查找字段从一个记录映射到另一个记录。
1. （视情况而定）如果原始记录类型与在&#x200B;**记录类型**&#x200B;字段中选择的记录类型之间没有连接字段，请单击&#x200B;**添加连接字段**。

   ![创建记录的自动化设置](assets/automation-setup-create-record.png)

   将创建以下两个字段：

   * 已为您在&#x200B;**记录类型**&#x200B;字段中指示的记录类型创建名为&#x200B;**连接的记录**&#x200B;的新连接字段。
   * 将为您配置自动化的记录类型创建一个与&#x200B;**记录类型**&#x200B;字段中指示的名称相同的新连接字段。

     例如，如果您正在配置营销活动的自动化以自动创建另一个名为Brands的记录类型，然后单击&#x200B;**添加连接的字段**，则会创建以下字段：

      * 已为&#x200B;**品牌**&#x200B;记录类型创建&#x200B;**连接的记录**&#x200B;连接字段。
      * 已为&#x200B;**营销活动**&#x200B;记录类型创建&#x200B;**品牌**&#x200B;连接字段。

1. （可选）如果原始记录类型与在“操作”区域中选择的Workfront对象之间没有连接字段，请单击&#x200B;**添加连接的字段**。

   ![自动设置以创建多个项目](assets/automation-setup-create-multiple-projects.png)

   将创建以下内容：

   * 将为您为其构建自动操作的记录类型创建一个名为&#x200B;**已连接&lt; Workfront对象名称>**&#x200B;的新连接字段。 例如，当您选择自动创建项目时，将为您正在为其构建自动化的记录类型创建一个&#x200B;**连接的项目**&#x200B;字段。
   * 新的记录类型信息卡会添加到Workfront中Workfront项目的“计划”部分，其中包含您正在为其配置自动化的记录类型的名称。

1. 单击自动化详细信息页面右上角的&#x200B;**保存**。

   自动化显示在自动化列表中，并可用于记录。

## 管理现有自动化

{{step1-to-planning}}

1. 单击记录类型卡片，然后单击记录名称。

   此时将打开记录类型页面。
1. 单击记录类型名称右侧的&#x200B;**更多**&#x200B;菜单![更多菜单](assets/more-menu.png)，然后单击&#x200B;**管理自动化**。

   将打开所选记录类型的可用自动化列表。

1. （可选）要编辑、禁用或删除自动化，请执行下列操作之一：

   1. 在自动化列表中，将鼠标悬停在已保存自动化的名称上，然后单击&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)。

   1. 单击&#x200B;**编辑**&#x200B;可更新以下信息：

      * 单击自动化名称右侧的&#x200B;**更多**&#x200B;菜单![更多菜单](assets/more-menu.png)，然后单击&#x200B;**编辑**&#x200B;以更改自动化名称。
      * 自动化中的任何字段，**操作**&#x200B;字段除外。

        >[!TIP]
        >
        >您无法更改最初为自动化选择的操作。


   1. 单击“**禁用**”可从记录的表视图中删除自动化并阻止用户使用它来创建记录或对象。

      已使用禁用的自动化创建的记录仍与最初选择的记录保持连接。

      若要使其再次可用，请再次单击&#x200B;**更多**&#x200B;菜单![更多菜单](assets/more-menu.png)，然后单击&#x200B;**激活**。
   1. 单击&#x200B;**删除**&#x200B;以删除自动化。 无法恢复已删除的自动化。

      使用已删除的自动化创建的记录仍与最初选择的记录保持连接。
