---
title: 连接记录类型
description: 指示各个记录类型如何相互关联的一种方法是连接它们。 此外，您可以将Adobe Workfront Planning记录类型与其他应用程序中的对象类型连接起来，以增强用户体验并将它们的焦点集中在一个应用程序中。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: 1eb1e919bede7e366956d8c0bd969329a641123f
workflow-type: tm+mt
source-wordcount: '2196'
ht-degree: 1%

---


# 连接记录类型

<span class="preview">此页面上的信息引用了尚未公开的功能。 它仅在“预览Sandbox”环境中可用。</span>

{{planning-important-intro}}

<!--
You can use Adobe Workfront Planning to design fully-customizable workspaces that contain record types needed in your organization. A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Workfront Planning record types with object types from other applications to enhance your users' experience and keep their focus in one application. -->

可以将记录类型相互连接或可以将记录类型与其他应用程序中的对象类型连接。

本文介绍了如何将两个Workfront Planning记录类型或Workfront Planning记录类型与另一个应用程序中的对象连接。

在记录或对象类型之间建立连接后，可以将各个记录相互连接，并在Workfront Planning记录上显示链接记录或对象类型中的字段。

有关连接类型的一般信息，请参阅[连接的记录类型概述](/help/quicksilver/planning/architecture/connect-record-types-overview.md)。

有关将记录或记录与其他应用程序中的对象连接的信息，请参阅[连接记录](/help/quicksilver/planning/records/connect-records.md)。

有关连接记录类型和记录的示例，请参阅[连接记录类型和记录的示例](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md)。

<!--ensure this last linked article is right; the title and the link should have changed-->

## 访问要求

+++ 展开以查看Workfront Planning的访问要求。

您必须具备以下条件才能访问Workfront Planning：

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
   <td role="rowheader"><p>Adobe Workfront规划计划*</p></td> 
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
   <td> <p>标准</p> 
   <p>Workfront计划不适用于旧版Workfront许可证</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td> <p>Adobe Workfront Planning没有访问级别控制</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>   <p>管理工作区</a>的权限 </p>  
   <p>系统管理员有权访问所有工作区，包括他们未创建的工作区。</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>布局模板</p></td> 
   <td> <p>必须为所有用户(包括Workfront管理员)分配一个布局模板，该模板应包括主菜单中的Planning区域 </p> </td> 
  </tr> 
</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

<!-- OLD: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p> Adobe Workfront Planning</p>
   <p>To connect Adobe Workfront Planning record types with Experience Manager Assets, you must have an Adobe Experience Manager Assets license and your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p> 
   <p>Current: Plan</p>
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create.</p>
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

+++


## 连接记录类型

<!--when changes here, also update the article for "Connect records"-->

{{step1-to-planning}}

1. 单击要连接其记录类型的工作区，

   或

   从工作区中，展开现有工作区名称右侧的向下箭头，搜索工作区，然后在工作区显示在列表中时将其选定。
1. 单击记录类型的卡以打开记录类型页面。
1. 单击表格视图右上角的&#x200B;**+**&#x200B;图标，然后单击“**新建连接**”选项卡。

   ![](assets/new-connection-tab-with-workfront-aem-options.png)

1. 在&#x200B;**记录类型**&#x200B;字段中，搜索记录类型，或选择以下选项之一：

   * 当前工作区中的其他记录类型

     <span class="preview">![](assets/many-to-many-connection-picker.png)</span>
     >[!TIP]
     >
     > 
     >如果所选工作区中没有其他记录类型，则不会显示工作区部分。


   * 另一个工作区中配置为从其他工作区连接的记录类型。 有关信息，请参阅[编辑记录类型](/help/quicksilver/planning/architecture/edit-record-types.md)。

     <span class="preview">![](assets/new-connection-allow-multiple-records-box.png)</span>

     >[!TIP]
     >
     >如果没有配置为从其他工作区连接的记录类型，则不会显示工作区部分。


   * 来自&#x200B;**Workfront对象类型**&#x200B;部分的&#x200B;**项目、Portfolio、项目群、公司**&#x200B;或&#x200B;**组**。

     ![](assets/workfront-project-connection-selection.png)

   * 来自&#x200B;**Adobe应用程序**&#x200B;部分的&#x200B;**Experience Manager Assets**。

     <span class="preview">![](assets/aem-assets-connection-selection.png)</span>

1. 更新以下信息：

   * **名称**：已连接字段的名称，它将显示在原始记录类型的表视图或记录页中。 这会在原始记录类型的表视图或原始记录的链接记录字段中创建链接记录列。 默认情况下，字段的名称是您连接到的记录或对象的名称。

   >[!TIP]
   >
   >您可以有多个与同一记录或对象类型的连接。 如果不编辑已连接的字段名称，Workfront会在已连接记录的名称后添加一个数字，以指示使用相同名称连接的记录类型的数量。

   * **描述**：有关连接的记录字段的其他信息。 当您将鼠标悬停在表中的字段列上时，将显示字段的描述。
   * **允许多条记录**：选择此选项可指示当链接记录类型字段显示在原始记录上时允许用户添加多条记录。 默认情况下，该选项处于选中状态。

     仅当从两个不同的工作区连接记录或连接记录和Adobe Experience Manager资源对象时，此选项才可用。

     <span class="preview">![](assets/new-connection-allow-multiple-records-box.png)</span>

   * **连接类型**：选择下列选项之一，以指示他们可以连接多少条记录，也可以连接多少条记录：

      * 多对多
      * 一对多
      * 多对一
      * 一对一

     仅当连接来自同一工作区的记录或记录和Workfront对象类型时，此选项才可用。

     <span class="preview">![](assets/many-to-many-connection-picker.png)</span>

     有关连接类型的详细信息，请参阅[连接的记录类型概述](/help/quicksilver/planning/architecture/connect-record-types-overview.md)。

   * **选择查找字段**：选择此选项可从所选记录类型添加字段。 查找字段是与要链接到的记录或对象类型关联的字段。 链接它们将显示您链接到的记录或对象中的信息，以及您链接到的记录中的信息。 默认情况下，该选项处于选中状态。

     >[!TIP]
     >
     > 不能添加以下字段类型作为查找字段：
     >
     >    * 人员
     >    * 创建者
     >    * 上次修改者
     >    * Workfront预输入字段（包括项目所有者或项目发起人等字段）

1. （有条件，可选）如果您已选择连接Workfront对象，请从&#x200B;**仅链接符合这些条件的对象**&#x200B;部分中选择&#x200B;**自定义表单**。 只有附加了所选自定义表单的对象才能链接到所选记录类型。 您可以选择多个表单。

   >[!NOTE]
   >
   > 您必须先在Workfront中为选定对象创建自定义表单，然后它们才会显示在此列表中。

1. （视情况而定）如果您已选择连接到Experience Manager Assets，请从&#x200B;**链接以下存储库中的资源**&#x200B;部分的&#x200B;**Experience Manager存储库**&#x200B;下拉菜单中选择一个存储库。 这是必填字段。 只有您在Experience Manager Assets中有权访问的存储库才会显示在此字段中。

   >[!NOTE]
   >
   >Workfront管理员可以通过Workfront中的元数据映射，将Workfront Planning字段映射到Experience Manager Assets字段。 有关详细信息，请参阅[配置Adobe Workfront和Experience Manager Assets之间的资源元数据映射](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en)。

1. （视情况而定）如果您选择连接到Experience Manager Assets或Workfront Planning记录类型，请在&#x200B;**记录外观**&#x200B;区域中选择以下选项之一：

   * <span class="preview">**名称和图像**：连接的记录的名称和缩略图或图标都会显示在连接的记录字段中。 这是默认选项。</span>
   * <span class="preview">**名称**：只有连接的记录的名称才会显示在连接的记录字段中。</span>
   * <span class="preview">**图像**：只有连接的记录的缩略图或图标将显示在连接的记录字段中。</span>

   没有缩略图图像的记录改为显示记录类型图标。 在&#x200B;**记录外观**&#x200B;区域中显示已连接记录的显示方式示例。

   >[!TIP]
   >
   >    当允许链接多个记录时，仅显示缩略图可能会节省较小区域（如记录视图）的空间。
   >
   >记录的名称是记录的主要字段。 有关详细信息，请参阅[主字段概述](/help/quicksilver/planning/fields/primary-field-overview.md)。
   >
   >选择Workfront对象类型时，无法选择记录外观。

1. 单击&#x200B;**创建**。

1. （视情况而定）如果您选择了&#x200B;**选择查找字段**&#x200B;设置，则会打开&#x200B;**添加查找字段**&#x200B;框。

   单击&#x200B;**+**&#x200B;图标可从&#x200B;**未选择的字段**&#x200B;区域添加字段。

   或

   单击&#x200B;**-**&#x200B;图标可从&#x200B;**选定字段**&#x200B;区域移除字段

   ![](assets/add-lookup-fields-for-another-maestro-record-type-box.png)

   链接记录或对象后，连接的字段的值会自动填充。

   >[!IMPORTANT]
   >
   >    对工作区具有“查看”或更高权限的每个人都可以查看链接字段中的信息，无论其在链接对象类型应用程序中的权限或访问级别如何。


1. （可选）单击&#x200B;**跳过**&#x200B;以跳过添加链接记录或对象类型的字段。 链接记录的名称或主字段是您连接到的记录类型的表视图中唯一可见的字段。

1. （可选且视情况而定）如果选择链接数字、货币、百分比或日期类型字段，则还应选择汇总值以汇总多个值。 当用户在链接的记录字段中选择多个链接记录时，链接字段的值会根据您选择的聚合器显示为逗号分隔的或汇总值。

   如果查找字段包含多个未汇总的值，则在视图中对字段进行排序或分组时，请考虑以下事项：

   * 排序由第一个值完成

   * 记录按字段值的每个唯一组合进行分组

   * 时间线视图基于第一个日期值构建

   >[!IMPORTANT]
   >
   >    如果希望字段可用作时间轴和日历视图的开始日期和结束日期，则在添加查找日期字段时必须选择一个聚合器值。 例如，您可以为查找日期字段选择MAX或MIN汇总。

   ![](assets/aggregator-drop-down-for-number-linked-field.png)

   >[!NOTE]
   >
   > 将记录类型连接到Experience Manager Assets时，聚合不可用。

   从以下项中选择：

   * **无**：显示来自多个记录的值，这些记录用逗号分隔。 这是默认选项。
   * **MAX**：显示在链接记录字段中选择的多个记录的所有值中的最大值。
   * **MIN**：显示在链接记录字段中选择的多个记录的所有值中的最小值。
   * **SUM**：显示在链接记录字段中选择的多个记录的所有值的总数。
   * **AVG**：显示在链接记录字段中选择的多个记录的所有值的平均值。
   * **UNIQUE**：从查找字段值中删除重复项，并仅显示唯一值。 这对于以下字段类型不可用：
      * 段落
      * 复选框
      * 人员

   >[!NOTE]
   >
   >例如，您可以从Campaign记录（原始记录）中链接产品记录（链接记录），并将其命名为“产品字段”。 您还可以选择从营销活动记录中链接产品记录的Budget字段，并将其称为“Product Budget”。 如果您允许在“产品字段”中选择多个记录，则可以选择预算为$100,000的产品1和预算为$110,000的产品2，以及预算为$100,000的产品3。 您可以在链接字段中查看原始记录的以下预算信息，具体取决于您选择的汇总：
   >
   >* **无**：$100,000，$110,000，$100,000
   >* **MAX**： $110,000
   >* **分钟**： $100,000
   >* **总和**：$310,000
   >* **平均**： $103,000.33
   >* **唯一**： $100,000
   >

1. （可选）使用&#x200B;**搜索**&#x200B;图标![](assets/search-icon.png)搜索字段。

1. 单击&#x200B;**添加字段**&#x200B;以保存更改。

   添加了以下项目：

   * 要链接的记录类型上的链接记录字段。 手动添加链接记录后，链接记录字段将显示来自链接记录类型的单个记录。 有关添加记录的信息，请参阅[连接记录](/help/quicksilver/planning/records/connect-records.md)。 链接记录字段的名称是您在步骤6中选择的名称。<!--accurate-->

   * 链接（或查找）字段（或字段），在您手动添加链接记录字段中的记录或对象后，显示有关链接记录或对象类型的信息。 仅在创建连接时选择了&#x200B;**Select lookup fields**&#x200B;设置时才创建查找字段。 查找字段会根据以下模式自动命名：

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

     例如，如果您链接了促销活动记录类型与项目群记录类型，并将项目群链接记录字段命名为“项目群信息”，然后选择还在Campaign表格视图中显示项目群预算字段，则链接字段在促销活动表格视图中自动命名为`Budget (from Program information)`。

   * 当您将记录类型链接到另一个记录类型时，链接记录字段也会添加到要链接的记录类型上。 链接记录类型中链接的记录字段的名称是您链接来源的记录类型的名称。

     例如，如果您从“Campaign”记录类型中链接“Product”记录类型，并命名了Campaign“链接的产品”的已连接字段，则会为“Product”记录类型创建“Campaign”链接记录字段。

     >[!TIP]
     >
     > 不会为对象创建链接记录字段，这些对象从另一个应用程序链接到您在Workfront Planning中链接的记录类型。

1. （可选，视情况而定）在原始记录类型或链接记录类型表格视图中，单击链接记录字段标题中的向下箭头，然后单击以下任一项：

   * **编辑字段**：更新该字段的&#x200B;**名称**&#x200B;和&#x200B;**描述**&#x200B;信息。
   * **编辑查找字段**：添加或删除链接记录的任何字段。

   ![](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   要添加或移除查找字段，请按照上述步骤16-17中的说明操作。<!--ensure these step numbers stay accurate-->

   >[!NOTE]
   >
   > 不能添加属于从另一应用程序链接到对象类型的记录类型的查找字段。
   >
   > 例如，无法将“Campaign Status”的查找字段添加到要从营销活动链接到的Workfront项目。

1. （可选）单击链接记录字段标题中的向下箭头，或者单击链接记录类型中的查找字段标题，然后单击&#x200B;**删除**。

   删除记录字段或查找字段。 如果删除记录字段，则与链接记录关联的任何查找字段也会被删除。
