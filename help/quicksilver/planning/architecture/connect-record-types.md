---
title: 连接记录类型
description: 指示各个记录类型如何相互关联的一种方法是连接它们。 此外，您可以将Adobe Workfront Planning记录类型与其他应用程序中的对象类型连接起来，以增强用户体验并将它们的焦点集中在一个应用程序中。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: f252140e4fec01c7bb8092804532d79954cef618
workflow-type: tm+mt
source-wordcount: '2507'
ht-degree: 0%

---

<!-----
title: Connect record types
description: A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Adobe Workfront Planning record types with object types from other applications to enhance your users' experience and keep their focus in one application.
hidefromtoc: yes
hide: yes
feature: Work management
role: User
author: Alina
--->

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->
<!--************ THIS MIGHT NO LONGER BE A 'RELATIONSHIP' TYPE FIELD, BECAUSE THEY WILL SHOW IT IN THE CONNECTION TAB*****************************-->


# 连接记录类型

{{planning-important-intro}}

<!--
You can use Adobe Workfront Planning to design fully-customizable workspaces that contain record types needed in your organization. A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Workfront Planning record types with object types from other applications to enhance your users' experience and keep their focus in one application. -->

您可以将记录类型相互连接或用其它应用程序的对象类型来记录类型。

本文介绍了如何将两个Workfront Planning记录类型(一个Workfront Planning记录类型)与另一个应用程序中的对象连接起来。

在记录或对象类型之间建立连接后，可以将各个记录相互连接，并在Workfront Planning记录上显示链接记录或对象类型中的字段。

<!-- uncomment out for the release close to GA: For general information about connection types, see [Connection record types overview](/help/quicksilver/planning/architecture/connect-record-types-overview.md).-->

有关将Workfront Planning记录连接到其他应用程序中的对象的信息，请参阅[连接记录](/help/quicksilver/planning/records/connect-records.md)。

有关连接记录类型和记录的示例，请参阅[连接记录类型和记录的示例](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md)。

<!--ensure this last linked article is right; the title and the link should have changed-->

## 访问要求

+++ 展开以查看Workfront Planning的访问要求。

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
   <p> Adobe Workfront</p> <p>要将Adobe Workfront Planning记录类型与Experience Manager Assets连接，您必须具有Adobe Experience Manager Assets许可证，并且贵组织的Workfront实例必须载入到AdobeUnified Experience。 有关信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">AdobeWorkfront的Unified Experience</a>。</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront协议</p></td>
   <td>
<p>您的组织必须注册到Workfront Planning的早期访问阶段 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront计划</p></td>
   <td>
<p>任何</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td>
   <td>
   <p>新增：标准</p> 
   <p>当前：计划</p>
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>访问级别配置</p></td>
   <td> <p>Adobe Workfront Planning没有访问级别控制</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>您的Workfront或组管理员必须在布局模板中添加Planning区域。 有关信息，请参阅<a href="/help/quicksilver/planning/access/access-overview.md">访问概述</a>。 </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>权限</p></td>
   <td> <p>管理工作区</a>的权限 </p>  
   <p>系统管理员有权访问所有工作区，包括他们未创建的工作区。
</td>
  </tr>
 </tbody>
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Maybe enable this at GA - but planing is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->


## 有关连接记录类型的注意事项

<!--DELETE THE CONTENT BELOW WHEN YOU MAKE "CONNECT RECORD TYPE OVERVIEW" ARTICLE PUBLIC-->

* 您可以在Adobe Workfront Planning中连接以下实体：

   * 两种记录类型

     记录类型必须属于同一工作区。
   * 来自另一个应用程序的记录类型和对象类型。

* 您可以将Workfront Planning记录类型与以下应用程序中的以下对象类型连接起来：

   * Adobe Workfront：

      * 项目
      * 项目组合
      * 项目群
      * 公司
      * 组

   * Adobe Experience Manager Assets：

      * 图像
      * 文件夹

     >[!IMPORTANT]
     >
     >您必须拥有Adobe Experience Manager Assets许可证，并且贵组织的Workfront实例必须载入Adobe业务平台或Adobe Admin Console，才能将Workfront Planning记录连接到Adobe Experience Manager Assets。
     >
     >如果您对加入Adobe Admin Console有任何疑问，请参阅[AdobeUnified Experience常见问题解答](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md)。

* 为记录类型创建单个记录后，您可以从链接的记录类型字段中选择连接到的记录。 有关信息，请参阅[连接记录](/help/quicksilver/planning/records/connect-records.md)。

* 将记录类型与另一个记录类型或另一个应用程序中的对象类型连接后，将出现以下情况：

   * **当您连接两个记录类型时**：在您连接的记录类型上创建链接记录字段。 在要连接的记录类型上创建类似的链接记录字段。

     例如，如果将“Campaign”记录类型与“Product”记录类型连接，则将在“Campaign”记录类型上创建名为“链接的产品”的链接记录字段，并在“Product”记录类型上创建自动名为“Campaign”的链接记录类型。

   * **当您将记录类型与另一个应用程序的对象类型连接时**：

      * 链接记录字段是在您连接的记录类型上创建的。 不会在其他应用程序的对象类型上自动创建链接记录字段。

      * 无法从Workfront对象访问Planning记录字段。
      * 当Workfront管理员通过Workfront与Adobe Experience Manager Assets之间的集成配置Experience Manager映射时，可从Metadata Assets访问规划记录字段。 有关详细信息，请参阅[配置Adobe Workfront和Experience Manager Assets之间的资源元数据映射](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en)。

   * **当您添加所连接的记录或对象的链接（或查找）字段时**：您可以将其他应用程序的对象中的字段连接到Workfront Planning记录类型。 链接字段是只读的，当您连接记录或对象时，它们会自动显示连接记录或对象中的信息。

     例如，如果您将“促销活动”记录类型与Workfront项目连接并选择将该项目的“计划完成日期”字段引入Workfront计划记录，则将自动为促销活动创建一个名为“计划完成日期”（来自项目）的链接字段。 您无法手动编辑此链接的字段。 计划完成日期（来自项目）字段显示链接项目的计划完成日期。

     >[!IMPORTANT]
     >
     >    对工作区具有“查看”或更高权限的每个人都可以查看链接字段中的信息，无论其在链接对象类型应用程序中的权限或访问级别如何。

* 链接的记录字段前面有关系图标![](assets/relationship-field-icon.png)。

  链接的字段前面有标识该字段类型的图标。 例如，链接（或查找）字段前面有图标，指示字段是数字、段落或日期。


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

   * 所选工作区中的其他记录类型

     <!--replace screen shot below-->

     ![](assets/new-connection-tab-fields-with-another-record-selected.png)

     >[!TIP]
     >
     >只有来自所选工作区的记录类型可供连接。
     > 
     >如果所选工作区中没有其他记录类型，则不会显示工作区部分。

     <!--remove the first sentence in the tip above at GA-->

     <!--FORMAT THE TIP BELOW AT RELEASE: * A record type from another workspace that was configured to connect from other workspaces. For information, see [Edit record types](/help/quicksilver/planning/architecture/edit-record-types.md). (*****add screen shot****)
        [!TIP]
         If there are no record types that are configured to connect from other workspace, the workspace section does not display.-->

   * 来自&#x200B;**Workfront对象类型**&#x200B;部分的&#x200B;**项目、Portfolio、项目群、公司**&#x200B;或&#x200B;**组**。

     <!--replace screen shot below-->

     ![](assets/workfront-project-connection-selection.png)

   * 来自&#x200B;**Adobe应用程序**&#x200B;部分的&#x200B;**Experience Manager Assets**。

     ![](assets/aem-assets-connection-selection.png)

1. 更新以下信息：

   * **名称**：已连接字段的名称，它将显示在原始记录类型的表视图或记录页中。 这会在原始记录类型的表视图或原始记录的链接记录字段中创建链接记录列。 默认情况下，字段的名称是您连接到的记录或对象的名称。

   >[!TIP]
   >
   >您可以有多个与同一记录或对象类型的连接。 如果不编辑已连接的字段名称，Workfront会在已连接记录的名称后添加一个数字，以指示使用相同名称连接的记录类型的数量。

   * **描述**：有关连接的记录字段的其他信息。 当您将鼠标悬停在表中的字段列上时，将显示字段的描述。
   * **允许多条记录**：选择此选项可指示当链接记录类型字段显示在原始记录上时，允许用户添加多条记录。 默认情况下，该选项处于选中状态。<!--This option is available only when connecting records from two different workspaces or a record and an AEM asset object type.-->
   <!--* **Connection type**: This option is available only when connecting records from the same workspace or a record and a Workfront object type. Choose from the following connection types:
        * One to one
        * One to many
        * Many to one
        * Many to many
        
        For information about connection types, see [Connect record types overview](/help/quicksilver/planning/architecture/connect-record-types-overview.md). -->
   * **选择查找字段**：选择此选项可从所选记录类型添加字段。 查找字段是与要链接到的记录或对象类型关联的字段。 链接它们将显示您链接到的记录或对象中的信息，以及您从中链接的记录的信息。 默认情况下，该选项处于选中状态。

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

1. （视情况而定）如果您已选择连接到Experience Manager Assets或Workfront Planning记录类型，并且不想在链接的字段中显示连接的记录或资源的标题，请取消选中&#x200B;**记录外观**&#x200B;区域中的&#x200B;**标题**&#x200B;切换开关。 取消选择后，链接的字段中仅显示记录的缩略图。 没有缩略图图像的记录改为显示图像图标。 默认情况下，该切换处于选中状态。 在&#x200B;**记录外观**&#x200B;区域中显示已连接记录的显示方式示例。

   >[!TIP]
   >
   >    当允许链接多个记录时，仅显示缩略图可能会节省较小区域（如记录视图）的空间。
   >
   >记录的标题是记录的主字段。 有关详细信息，请参阅[主字段概述](/help/quicksilver/planning/fields/primary-field-overview.md)。

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


1. （可选）单击&#x200B;**跳过**&#x200B;以跳过添加链接记录或对象类型的字段。 链接记录的&#x200B;**Name**&#x200B;或&#x200B;**Title**&#x200B;是您连接到的记录类型的表视图中唯一可见的字段。

1. （可选且视情况而定）如果选择链接数字、货币、百分比或日期类型字段，则还应选择汇总值以汇总多个值。 当用户在链接的记录字段中选择多个链接记录时，链接字段的值会根据您选择的聚合器显示为逗号分隔的或汇总值。

   如果查找字段包含多个未汇总的值，则在视图中对字段进行排序或分组时，请考虑以下事项：

   * 排序由第一个值完成

   * 记录按字段值的每个唯一组合进行分组

   * 时间线视图基于第一个日期值构建。

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
   >例如，您可以从Campaign记录（原始记录）中链接产品记录（链接记录），并将其命名为“产品字段”。 您还可以选择从营销活动记录中链接产品记录的“预算”字段，并将其称为“产品预算”。 如果您允许在“产品字段”中选择多个记录，则可以选择预算为$100,000的产品1和预算为$110,000的产品2，以及预算为$100,000的产品3。 您可以在链接字段中查看原始记录的以下预算信息，具体取决于您选择的汇总：
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

   * 要链接的记录类型上的链接记录字段。 手动添加链接记录后，链接记录字段将显示来自链接记录类型的单个记录。 有关添加记录的信息，请参阅[连接记录](/help/quicksilver/planning/records/connect-records.md)。 链接记录字段的名称是您在步骤7中选择的名称。<!--accurate-->

   * 链接（或查找）字段（或字段），在您手动添加链接记录字段中的记录或对象后，显示有关链接记录或对象类型的信息。 仅在创建连接时选择了&#x200B;**Select lookup fields**&#x200B;设置时才创建查找字段。 查找字段会根据以下模式自动命名：

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

     例如，如果您链接了某个“促销活动”记录类型与“项目”记录类型，并将该“项目”链接记录字段命名为“项目群信息”，然后选择还在该促销活动的表格视图中显示该“项目”的“预算”字段，则该链接字段在该促销活动的表格视图中自动命名为`Budget (from Program information)`。

   * 当您将记录类型链接到另一个记录类型时，链接记录字段也会添加到要链接的记录类型上。 链接记录类型中链接的记录字段的名称是您链接来源的记录类型的名称。

     例如，如果您从“Campaign”记录类型中链接“Product”记录类型，并将营销活动的连接字段命名为“链接的产品”，则会为“Product”记录类型创建“Campaign”链接记录字段。

     >[!TIP]
     >
     > 不会为对象创建链接记录字段，这些对象从另一个应用程序链接到您在Workfront Planning中链接的记录类型。

1. （可选，视情况而定）在原始记录类型或链接记录类型表格视图中，单击链接记录字段标题中的向下箭头，然后单击以下任一项：

   * **编辑字段**：您可以更新该字段的&#x200B;**名称**&#x200B;和&#x200B;**描述**&#x200B;信息。
   * **编辑查找字段**：添加或删除链接记录的任何字段。

   ![](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   要添加或移除查找字段，请按照上述步骤10-14中的说明操作。<!--ensure these step numbers stay accurate-->

   >[!NOTE]
   >
   > 不能添加属于从另一应用程序链接到对象类型的记录类型的查找字段。
   >
   > 例如，无法将“Campaign Status”的查找字段添加到要从营销活动链接到的Workfront项目。

1. （可选）单击链接记录字段标题中的向下箭头，或者单击链接记录类型中的查找字段标题，然后单击&#x200B;**删除**。

   删除记录字段或查找字段。 如果删除记录字段，则与链接记录关联的任何查找字段也会被删除。
