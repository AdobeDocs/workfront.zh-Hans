---
title: 使用Workfront Planning记录自动化创建Adobe Workfront对象
description: 您可以在Workfront Planning中配置自动化，以便在激活后在Workfront中创建对象。
hide: true
hidefromtoc: true
exl-id: c669217a-40e2-471f-951d-93157a34f1ee
source-git-commit: 00e58ea9a207037b701e1be010c2c4c2995d60e0
workflow-type: tm+mt
source-wordcount: '1252'
ht-degree: 3%

---

# 使用Adobe Workfront Planning记录自动化创建对象

<!--add screen shots when UI is finalized AND redo all the steps - some things got changed and moved around-->
<!--when you make this public, add this to the metadata above (and take the "hide" tags out):

feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog

-->

<!-- if they give access to use the automation to people with LESS than Manage permissions to a workspace, split this article in two: the Configure section should be for admins and the "Use a Workfront Planning automation to create an object" should be for all other users-->

您可以在Adobe Workfront Planning中配置自动操作，激活自动操作后，可在Workfront或Workfront Planning中创建对象。

您可以在记录的页面中配置和激活自动化。 创建的对象连接到Planning记录，并放置在自动化中指定的字段中。

例如，您可以创建一个接受Workfront Planning营销活动的自动化功能，并在Workfront中创建一个项目以跟踪该营销活动的进度。 该项目将连接到Workfront规划活动。

有关已连接记录的详细信息，请参阅[已连接记录概述](/help/quicksilver/planning/records/connected-records-overview.md)。

## 访问要求

+++ 展开以查看Workfront Planning的访问要求。

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
<p>贵组织的Workfront实例必须载入AdobeUnified Experience，才能访问Workfront Planning的所有功能。</p> 
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">AdobeWorkfront的Unified Experience</a>。 </p> 
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
   <p>在Workfront中编辑要创建的对象类型（项目、项目组合、项目群）的访问权限。 </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td> <p>管理要向其中添加记录的工作区的权限。 </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>
   <p>管理Workfront对象（项目组合）的权限以添加子对象（项目）。</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>布局模板</p></td> 
   <td> <p>必须为所有用户(包括Workfront管理员)分配一个布局模板，该模板应包括主菜单中的Planning区域 </p> </td> 
  </tr> 
</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


## 有关使用自动化创建对象和记录的注意事项

* 新对象或记录名称与从中创建该对象的记录名称相同。
* 如果用于的自动化记录已连接了您选择向其中添加新对象的字段中的相同类型的对象，则新对象将添加到连接字段中，而现有对象也保持连接状态。

## 在Workfront Planning中配置自动化

您必须先在Workfront Planning中配置自动化，然后才能使用它创建对象。

{{step1-to-planning}}

1. 单击记录类型卡片，然后单击记录名称。

   此时将打开记录类型页面。
1. 单击记录类型名称右侧的&#x200B;**更多**&#x200B;菜单![](assets/more-menu.png)，然后单击&#x200B;**管理自动化**。

   将打开可用自动化列表。

1. 单击屏幕右上角的&#x200B;**新建自动化**。 将打开&#x200B;**新自动化**&#x200B;框。
1. 更新以下字段：

   * 将&#x200B;**无标题的自动化**&#x200B;替换为要显示在自动化按钮上的文本。 使用自动化创建Workfront对象时，用户将单击此按钮。
   * **描述**：添加描述以标识自动化的目的。

1. 在自动化的详细信息页面上，更新&#x200B;**触发器**&#x200B;部分中的以下字段：

   * **触发器**：选择将触发自动化的操作。 例如，选择&#x200B;**按钮单击**。<!--update this step with a list of all possible triggers; right not only Button click is available-->

1. 更新&#x200B;**操作**&#x200B;部分中的以下字段：
   * **对象类型**：选择要自动创建的对象。 这是必填字段。

     您可以从Workfront Planning记录创建以下对象：

      * 项目
      * 项目组合
      * 项目群
      * 组
      * 记录
1. （视情况而定）根据要创建的对象类型，更新以下字段：

   * **项目**：
      * **创建对象的已连接字段**：这是将显示新项目的已连接字段。 这是必填字段
      * **从中创建项目的模板**：选择Workfront将用于创建项目的项目模板。
   * **Portfolio**：
      * **创建对象的已连接字段**：这是将显示新项目组合的已连接字段。 这是必填字段。
      * **要附加到新项目组合的自定义表单**：选择要附加到新项目组合的自定义表单。 您必须先创建项目组合自定义表单，然后才能选择它。
   * **计划**：
      * **创建对象的已连接字段**：这是将显示新程序的已连接字段。 这是必填字段。
      * **项目组合**：选择将添加新项目的项目组合。 这是必填字段。
      * 
         * **要附加到新程序的自定义表单**：选择要附加到新程序的自定义表单。 您必须先创建程序自定义表单，然后才能选择它。
   * **组**：
      * **创建对象的已连接字段**：这是将显示新组的已连接字段。 这是必填字段。
      * **要附加到新组的自定义表单**：选择要附加到新程序的自定义表单。 您必须先创建程序自定义表单，然后才能选择它。
   * **记录**：
      * **连接的记录类型**：选择要创建的记录类型。
      * **创建记录的已连接字段**：这是将显示新记录的已连接字段。 这是必填字段。
      * **映射字段**：从创建自动化的记录类型中选择字段，以将其映射到连接的记录类型的字段。
      * **至连接的记录字段**：从连接的记录中选择与创建自动化记录类型对应的字段。
1. （可选且有条件）如果您没有Workfront对象类型的连接字段，请单击&#x200B;**创建连接字段**&#x200B;图标![](assets/create-a-connection-field-icon.png)以添加字段。
1. （可选且有条件）如果您已选择添加记录，请单击&#x200B;**映射字段**&#x200B;区域中的&#x200B;**添加**&#x200B;以添加和映射其他字段，然后选择要&#x200B;**从**&#x200B;转移的字段和要&#x200B;**从**&#x200B;转移的字段以指示原始选定记录的字段应显示在连接记录的哪个字段中。
1. 单击&#x200B;**保存**。

   自动化显示在自动化列表中，并可用于记录。
1. （可选）要编辑、禁用或删除自动化，请执行以下操作：

   从自动化列表中，将鼠标悬停在已保存自动化的名称上，然后单击&#x200B;**更多**&#x200B;菜单![](assets/more-menu.png)，然后选择以下选项之一：

   * **编辑**：更新有关自动机的信息并配置字段。
   * **禁用**：自动化将不会作为选项显示在记录的表格视图的工具栏中，用户无法再使用它来创建记录或对象。 若要使其再次可用，请再次单击&#x200B;**更多**&#x200B;菜单![](assets/more-menu.png)，然后单击&#x200B;**激活**。
   * **Delete**：自动化已删除，无法恢复。 使用自动化创建的记录仍与最初选择的记录保持连接。

## 使用Workfront Planning自动化功能创建对象

1. 在Workfront Planning中，打开包含要用于创建Workfront对象的记录的记录类型页面。
1. 打开表格视图。
1. 选择一个或多个记录。

   表格底部会显示一个蓝色条状栏，其中包含其他按钮，包括自动化按钮。
1. 单击屏幕右下角附近的自动化按钮。

   ![自动化按钮](assets/automation-custom-button.png)

   新对象将显示在自动按钮的设置中指示的已连接字段中。

   >[!NOTE]
   >
   >我们建议检查对象是否已按预期创建和连接。

1. （可选）单击已连接字段中的新对象。 “对象”页面随即打开，您可以对新对象进行其他更改。

<!--you might need to add something about notifications and emails?!-->
