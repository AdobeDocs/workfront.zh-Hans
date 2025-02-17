---
title: 使用Workfront Planning记录自动化创建Adobe Workfront对象
description: 您可以在Adobe Workfront Planning中配置自动化操作，在激活时，可在Workfront中创建对象或Workfront Planning中的记录。 创建的对象和记录会自动连接到现有Planning记录。 本文介绍如何管理自动化，包括如何编辑、禁用、删除和触发它们以创建对象和记录。
hide: true
hidefromtoc: true
exl-id: c669217a-40e2-471f-951d-93157a34f1ee
source-git-commit: 0a7bb953e7e02e24857bfb7ff671538e184bda17
workflow-type: tm+mt
source-wordcount: '1479'
ht-degree: 2%

---

# 使用Adobe Workfront Planning记录自动化创建对象

<!--add screen shots when UI is finalized AND redo all the steps - some things got changed and moved around-->
<!--when you make this public, add this to the metadata above (and take the "hide" tags out):

feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog

-->

<!--add a new section to this article to mention a new way to create objects: help/quicksilver/planning/records/create-records.md-->
<!-- add a new section to this article to mention a new way to create WF objects from Planning: help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md-->

<!-- if they give access to use the automation to people with LESS than Manage permissions to a workspace, split this article in two: the Configure section should be for admins and the "Use a Workfront Planning automation to create an object" should be for all other users-->

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

您可以在Adobe Workfront Planning中配置自动处理，激活自动处理后，可在从Planning记录触发时，在Workfront中创建对象，或在Workfront Planning中创建记录。 创建的对象或记录会自动连接到从中触发自动化的记录。

您可以在Workfront Planning的记录页面中配置和激活自动化。 创建的连接对象将放置在运行自动化时所用的记录类型的连接字段中。

例如，您可以创建一个接受Workfront Planning营销活动的自动化功能，并在Workfront中创建一个项目以跟踪该营销活动的进度。 该项目将连接到营销策划上“连接的项目”字段中的Workfront规划营销策划。

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
<p>贵组织的Workfront实例必须载入Adobe Unified Experience，才能访问Workfront Planning的所有功能。</p> 
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

* 对于新Workfront对象，新对象名称与从中创建该对象的记录名称相同。
* 对于新的Planning记录，您可以指明应该使用哪个原始记录字段来确定新记录的名称。
* 新对象或记录不会覆盖同一字段中的现有对象或记录。 为同一记录多次触发相同的自动化操作时，除了之前创建的那些之外，还会将新对象或记录添加到原始记录的同一已连接字段中。
* 该自动化仅在“多对多连接类型”或“一对多连接类型”字段中添加其他对象。 在所有其他情况下，自动化会创建对象，但不会将其连接到触发自动化的原始记录。

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

   * **触发器**：选择将触发自动化的操作。 例如，选择&#x200B;**按钮单击**。<!--update this step with a list of all possible triggers; right not only Button click is available-->

1. 更新&#x200B;**操作**&#x200B;部分中的以下字段： <!--submitted bugs for these fields - see if they need changing here-->
   * **对象类型**：选择要自动创建的对象。 这是必填字段。

     您可以从Workfront Planning记录创建以下对象：

      * 项目
      * 项目组合
      * 项目群
      * 组
      * 记录

     >[!TIP]
     >
     >保存自动化后，无法再更改此字段中的对象类型。

1. （视情况而定）根据要创建的对象类型，更新以下字段：


   * **项目**：
      * **创建对象的已连接字段**：这是将显示新项目的已连接字段。 这是必填字段。
      * **从中创建项目的模板**：选择Workfront将用于创建项目的项目模板。
   * **Portfolio**：
      * **创建对象的已连接字段**：这是将显示新项目组合的已连接字段。 这是必填字段。
      * **要附加到新项目组合的自定义表单**：选择要附加到新项目组合的自定义表单。 您必须先创建项目组合自定义表单，然后才能选择它。
   * **计划**：
      * **创建对象的已连接字段**：这是将显示新程序的已连接字段。 这是必填字段。
      * **项目组合**：选择将添加新项目的项目组合。 这是必填字段。
      * **要附加到新程序的自定义表单**：选择要附加到新程序的自定义表单。 您必须先创建程序自定义表单，然后才能选择它。
   * **组**：
      * **创建对象的已连接字段**：这是将显示新组的已连接字段。 这是必填字段。
      * **要附加到新组的自定义表单**：选择要附加到新程序的自定义表单。 您必须先创建程序自定义表单，然后才能选择它。
   * **记录**：
      * **连接的记录类型**：选择要创建的记录类型。
      * **创建记录的已连接字段**：这是将显示新记录的已连接字段。 这是必填字段。<!--this might need revision as right now it shows the field on the connected record table where the current record will display; submitted a bug to correct this label-->
      * **映射字段**
         * **传输自**：从创建自动化的记录类型中选择字段，以将其映射到连接的记录类型的字段。
      * **传输到**：从新创建的记录中选择将使用您运行自动化的记录中的信息填充的字段。
1. （可选且有条件）如果您选择创建记录，请单击&#x200B;**添加字段**&#x200B;以将其他查找字段从一个记录映射到另一个记录。
1. （可选且有条件）如果您没有Workfront对象类型的连接字段，请单击&#x200B;**创建连接字段**&#x200B;图标![创建连接字段图标](assets/create-a-connection-field-icon.png)以添加字段。

   新字段自动创建并命名为&#x200B;**连接的&lt; Workfront对象名称>**。 例如，当为记录创建已连接项目组合字段时，将其命名为“已连接项目组合”。

1. 单击自动化详细信息页面右上角的&#x200B;**保存**。

   自动化显示在自动化列表中，并可用于记录。
1. （可选）要编辑、禁用或删除自动化，请执行以下操作：

   1. 在自动化列表中，将鼠标悬停在已保存自动化的名称上，然后单击&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)。

   1. 单击&#x200B;**编辑**&#x200B;以更新有关自动机的信息并配置字段。
   1. 单击&#x200B;**禁用**&#x200B;可从表视图中删除自动化并阻止用户使用它创建记录或对象。 若要使其再次可用，请再次单击&#x200B;**更多**&#x200B;菜单![更多菜单](assets/more-menu.png)，然后单击&#x200B;**激活**。
   1. 单击&#x200B;**删除**&#x200B;以删除自动化。 无法恢复已删除的自动化。 使用自动化创建的记录仍与最初选择的记录保持连接。

## 使用Workfront Planning自动化功能创建对象或记录

1. 在Workfront Planning中，打开记录类型页面，其中包含要用于创建Workfront对象或Planning记录的记录。
1. 打开表格视图。
1. 选择一个或多个记录。

   表格底部会显示一个蓝色条状栏，其中包含其他按钮，包括自动化按钮。
1. 单击屏幕右下角附近的自动化按钮。

   ![自动化按钮](assets/automation-custom-button.png)

   如果自动化成功创建了对象或记录，则屏幕底部会显示确认消息。

   新对象将显示在自动按钮的设置中指示的已连接字段中。 在查看新对象之前，您可能需要刷新页面。

   >[!NOTE]
   >
   >我们建议检查对象是否已按预期创建和连接。

1. （可选）单击已连接字段中的新对象。 “对象”页面随即打开，您可以对新对象进行其他更改。

<!--you might need to add something about notifications and emails?!-->


<!--****************************************FUTURE ARTICLE AFTER THE RELEASE TO PREVIEW ON FEBRUARY 20:*****************************************************  

You can configure automations in Adobe Workfront Planning that, when activated, create objects in Workfront or records in Workfront Planning when triggered from a Planning record. The created objects or records are automatically connected to the records you are triggering the automation from. 

You can configure and activate the automation in the record's page in Workfront Planning. The connected object that is created is placed in the connected field of the record type you run the automation from. 

For example, you could create an automation that takes a Workfront Planning campaign and creates a project in Workfront to track that campaign's progress. The project would be connected to the Workfront Planning campaign in the Connected Project field on the campaign.

For more information on connected records, see [Connected records overview](/help/quicksilver/planning/records/connected-records-overview.md).

## Access requirements

+++ Expand to view access requirements for Workfront Planning. 

You must have the following access to perform the steps in this article:  

 <table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access all the capabilities of Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td> Standard
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p> 
   <p>Edit access in Workfront for the object types that you want to create (projects, portfolios, programs). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Manage permissions to the workspace you want to add records to. </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Manage permissions to Workfront objects (portfolios) to add children objects (projects).</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout template</p></td> 
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu </p> </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).   

+++


## Considerations about creating objects and records using an automation

* For new Workfront objects, the new object name is the same as the record name from which you create it. 
* For new Planning records, you can indicate what original record field should be used to determine the new record's name. 
* New objects or records don't override existing ones in the same field. Triggering the same automation multiple times for the same record adds the new objects or records in the same connected field of the original record, in addition to the ones created before. 
* The automation adds additional objects only in the Many to many or One to many connection type fields. In the all other cases, the automation creates the object, but it does not connect it to the original record from which the automation is triggered. 

## Configure an automation in Workfront Planning

You must configure an automation for a record type in Workfront Planning before you can use it to create objects.

{{step1-to-planning}}

1. Click a record type card, then click the name of a record. 

   The record type page opens. 
1. Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record type name, then click **Manage automations**. 

   The list of available automations for the selected record type opens.

1. Click **New automation** in the upper-right corner of the screen. The **New automation** box opens.
1. Update the following fields:

   * Replace **Untitled automation** with the text that you want to appear on the automation button. Users will click this button when using the automation to create a Workfront object or a Planning record.
   * **Description**: Add a description to identify the purpose of the automation.
1. Click **Save**.
   The automation details page opens. 

1. On the automation's details page, update the following fields in the **Triggers** section: 

   * **Trigger**: Select the action that will trigger the automation. For example, select **Button click**. *************update this step with a list of all possible triggers; right now only Button click is available*********

1. Update the following fields in the **Actions** section: **********submitted bugs for these fields - see if they need changing here***********
   * **Actions**: Select the action that you want Workfront to perform when triggering the automation. This is a required field. 
   Select one of the following actions: 

      * Create group
      * Create program
      * Create portfolio
      * Create project
      * Create record

      >[!TIP]
      >
      >After you saved the automation, you can no longer change the action selected in this field.

1. (Conditional) Depending on what action you selected, update the following fields:

   * **Create project**: 
      * **Connected field where the object is created**: This is the connected field where the new project will display. This is a required field. 
      * **Project template**: Select a project template that Workfront will use to create the project.  
   * **Create portfolio**:
      * **Connected field where the object is created**: This is the connected field where the new portfolio will display. This is a required field.
      * **Custom form to attach to the new portfolio**: Select a custom form to attach to the new portfolio. You must create a portfolio custom form before you can select it. 
   * **Create program**: 
      * **Connected field where the object is created**: This is the connected field where the new program will display. This is a required field.
      * **Program portfolio**: Select a portfolio where the new program will be added. This is a required field.
      * **Custom form to attach to the new program**: Select a custom form to attach to the new program. You must create a program custom form before you can select it. 
   * **Create group**:
      * **Connected field where the object is created**: This is the connected field where the new group will display. This is a required field.
      * **Custom form to attach to the new group**: Select a custom form to attach to the new program. You must create a program custom form before you can select it. 
   * **Create record**: 
      * **Record type**: Select the record type you want to create. 

      The **Settings** sub-section displays. Update the following fields in the **Settings** sub-section: 

      * **Field on the connected record type where the current record will show**: This is the connected field on the record type selected for the action where the current record will display. 
      
      For example, if you are creating an automation for campaigns to connect Product records from, this is the connected field on the Product record type where the campaigns will display, after the products are created using the automation. 
      
      This is a required field. 
      
      ******submitted a change in functionality and UI text for this - revise?? *******
      * **Map fields**
         * **Transfer from**: Select fields from the record type the automation is created for to map them to the fields of the connected record type. 
      * **Transfer to**: Select fields from the newly created record that will populate with information from the record you are running the automation from. 

      >[!TIP]
      >
      >The field types from the original record type must match the field types from the newly created record type.

1. (Optional and conditional) If you selected to create a record, click **Add fields** to map additional lookup fields from one record to another.
1. (Conditional) If you selected to create a record and there are no connection fields between the original record type and the record type selected in the **Actions** area, click the question mark icon to the right of the **Field on the connected record type where the current record will show** field, then click the **Add** icon ![Create a connection field icon](assets/create-a-connection-field-icon.png) to add a connection field. 

   The new field is automatically created for the record type you selected in the **Actions** area, and named **Connected Record**. 
   
   A connected field for the selected record type is also created on the original record type from where you are configuring the automation. 
1. (Optional and conditional) If you selected to create a Workfront object and don't have a connection field for the selected Workfront object type, click the question mark icon to the right of the **Connected field where the < Workfront object type name > is created** field, and click the **Add** icon ![Create a connection field icon](assets/create-a-connection-field-icon.png) to add a connection field. 

   ![](assets/question-mark-icon-to-add-connected-fields-in-automations-with-workfront.png)

   The new field is automatically created and named **Connected < Workfront object name >**. For example, when a portfolio connected field is created for the record, it is named "Connected portfolio." 

1. Click **Save** in the upper-right corner of the automation details page. 

   The automation displays on the list of automations, and is available to use in records.

## Manage existing automations

{{step1-to-planning}}

1. Click a record type card, then click the name of a record. 

   The record type page opens. 
1. Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record type name, then click **Manage automations**. 

   The list of available automations for the selected record type opens.

1. (Optional) To edit, disable, or delete an automation, do one of the following:

   1. From the list of automations, hover over the name of a saved automation, then click the **More** menu ![More menu](assets/more-menu.png).

   1. Click **Edit** to update information about and configure fields on the automation.

      >[!TIP]
      >
      >   You cannot change the action you originally selected for an automation. 
   

   1. Click **Disable** to remove the automation from the record's table view and prevent users from using it to create records or objects. 

   Records that have been created using a disabled automation remain connected to the record originally selected.
   
   To make it available again, click the **More** menu ![More menu](assets/more-menu.png) again, then click **Activate**.
   1. Click **Delete** to delete the automation. A deleted automation cannot be recovered. 
   
   Records that have been created using a deleted automation remain connected to the record originally selected.  

## Use a Workfront Planning automation to create an object or a record

1. In Workfront Planning, open the record type page that contains the automation you want to use to autoamtically create and connect records or objects. 
1. Open the table view. 
1. Select one or more records.
   
   A blue bar displays at the bottom of the table with additional buttons, including automation buttons. 
1. Click the automation button near the lower-right corner of the screen. 

   ![Automation button](assets/automation-custom-button.png)

   The following things occur: 

   * A confirmation message displays at the bottom of the screen, if the automation successfully created an object or a record. 

   * The new object displays in the connected field you indicated in the setup of the automation button. You might need to refresh your page before viewing the new object. 

   * The record you are triggering the automation from is added to the connected field of the new record.

   >[!NOTE]
   >
   >We recommend checking that the objects or records were created and the connected as expected.

1. (Optional) Click the new object in the connected field. The object page opens and you can make additional changes to the new object. 

***********you might need to add something about notifications and emails?!*************

-->