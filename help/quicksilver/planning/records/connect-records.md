---
title: 连接记录
description: 在记录类型之间创建连接后，可以将各个记录彼此连接。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 17796cdc-6de8-4209-a5af-b255dc64d70a
source-git-commit: a2062658110792689c0a15dd1c616c58ebf7e07a
workflow-type: tm+mt
source-wordcount: '2281'
ht-degree: 1%

---

<!--when you make this live, update the metadata above to this: 
---
title: Connect records and objects
description: In addition to connecting records to one another, you can also connect records to objects from other applications.  
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->
<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--if you change steps here, also update steps in the "Connect records" article-->

# 连接记录

{{planning-important-intro}}

您可以将Adobe Workfront Planning记录相互连接或与其他应用程序中的对象连接。

本文介绍了如何连接记录。 有关连接记录的更多常规信息，请参阅[连接的记录概述](/help/quicksilver/planning/records/connected-records-overview.md)。

必须首先将两个记录类型相互连接，或者将记录类型从另一个应用程序连接到对象类型。 这将创建链接的记录字段。 然后，可以使用链接的记录字段将记录彼此连接，或将记录与其他应用程序中的其他对象连接。

连接记录与将记录从另一个应用程序连接到对象类似。

有关将记录类型相互连接或从其他应用程序连接到对象类型的信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。

有关连接记录类型的示例，请参阅[连接记录类型和记录的示例](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md)。

您可以连接以下各项：

* Adobe Workfront Planning记录
* Adobe Workfront Planning记录包含来自其他应用程序的对象。

  您可以从以下应用程序将记录连接到下列类型的对象：

   * Adobe Workfront

      * 项目
      * 项目组合
      * 项目群
      * 公司
      * 组

   * Adobe Experience Manager Assets

      * 图像文件
      * 文件夹

  <!--when you add more objects, fix the Access Requirements below which right now refer only to projects-->

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
<td>产品</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p>要将Adobe Workfront Planning记录与Experience Manager Assets连接，您必须具有Adobe Experience Manager Assets许可证，并且贵组织的Workfront实例必须载入到AdobeUnified Experience。 有关信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">AdobeWorkfront的Unified Experience</a>。</p>
   </td>
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
   <td> <p>Workfront Planning没有访问级别控制</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>权限</p></td>
   <td> <p>管理工作区权限以连接记录 </p>  
   <p>查看工作区或更高权限，以查看与其他应用程序中的对象和字段的所有连接，无论您对其他应用程序的访问权限如何。 </p>
   <p>查看要从Workfront或Experience Manager Assets链接的对象或授予对这些对象的更高权限。 </p>
   <p>系统管理员有权访问所有工作区，包括他们未创建的工作区。</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>您的Workfront或组管理员必须在布局模板中添加Planning区域。 有关信息，请参阅<a href="/help/quicksilver/planning/access/access-overview.md">访问概述</a>。 </p>  
</td>
  </tr>

</tbody>
</table>

*有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 连接记录的先决条件

要将记录与其他记录或对象连接，您必须具备以下条件：

* 至少一个工作区、记录类型和记录。

  有关更多信息，请参阅以下文章：

   * [创建工作区](/help/quicksilver/planning/architecture/create-workspaces.md)
   * [创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)
   * [创建记录](/help/quicksilver/planning/records/create-records.md)

* 记录类型之间的连接，或记录类型与其他应用程序的对象之间的连接。 有关信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。

## 从Workfront Planning连接记录

您可以从Workfront Planning在以下方面连接记录：

* 从Workfront Planning中的Planning记录，在表视图的已连接字段中。
* 从Workfront Planning中的Planning记录（记录预览或连接的记录字段中的页面）。
  <!--
  * From a Planning record in Workfront Planning in the record preview or page in the connected record fields on the Details tab.
  * From a Planning record in the record's preview or page on the Connections tab.  -->

### 从表视图或<!--Details tab of the-->记录页面连接Adobe Workfront Planning记录

{{step1-to-planning}}

1. 单击要连接其记录的工作区

   工作区将打开，记录类型显示为卡片。
1. 单击记录类型的卡以打开记录类型页面。
1. 单击&#x200B;**表**&#x200B;视图的名称以将其打开。
1. （可选）通过向表中添加新行，将记录添加到您选择的记录类型。 有关信息，请参阅[创建记录](/help/quicksilver/planning/records/create-records.md)。
1. （视情况而定）将所选记录类型与其他记录类型连接后，转到链接的记录列，并双击要与其他记录链接的记录对应的单元格。

   ![](assets/connect-other-records-smaller-box-in-table-view.png)

1. 执行下列操作之一：

   * 从列表中单击已连接记录的名称以将其添加到所选记录。 记录会自动添加。
   * 开始键入记录的名称，并在该记录显示在列表中时单击它。 记录会自动添加。

   <!--1. (Optional) If you cannot find a record or an object to connect, and you want to add it, click **+ Add** to add a new record. For more information, see the "Create records as you connect them" in the article [Create records](/help/quicksilver/planning/records/create-records.md).
    
    You can also create projects and portfolios by adding them to a record in the connected record field. You can create only blank projects, without a template by adding them to a record. 
    
     -->

   >[!TIP]
   >
   >    您可以打开记录的页面，方法是单击视图中的记录名称，找到链接的记录字段，然后双击该字段（如果已经连接记录），或单击&#x200B;**连接记录**（如果字段为空）以从连接的记录或对象类型添加记录。
   >
   >![](assets/connect-records-from-record-page-field.png)

1. （可选）单击&#x200B;**查看全部**&#x200B;以显示所有记录。

1. （视情况而定）如果您在上一步中单击了&#x200B;**查看所有**，则会显示&#x200B;**连接对象**&#x200B;框。

   ![](assets/connected-objects-table-for-records.png)

1. 在搜索框中开始键入记录的名称，然后当它显示在列表中时将其选定

   或

   在框中选择一个或多个记录的名称，然后单击&#x200B;**连接对象**。

   添加了以下内容：

   * 链接记录显示在您在上一步中选择的记录的链接记录字段中。
   * 如果您在连接记录类型时添加了链接的查找字段，则链接字段会填充有链接记录中的信息。

   更新链接的记录会自动更新您正在链接的记录的链接字段。 您无法手动编辑链接的字段。

   >[!TIP]
   >
   >* 我们交替使用“链接字段”和“查找字段”。
   >
   >* 如果在连接记录类型时启用了&#x200B;**允许多条记录**&#x200B;设置，则多个选定对象的字段值要么以逗号分隔，要么根据您选择的聚合器聚合。

1. （可选）关闭记录类型页面，然后转到您选择的工作区。
1. 单击链接到的记录类型的卡。

   例如，如果您已将&#x200B;**Campaign**&#x200B;记录与产品记录连接，请单击&#x200B;**Product**&#x200B;卡。

   记录类型卡片应在“表”视图中打开。 如果没有，请选择表格视图。

   请注意，**Campaign**&#x200B;链接记录字段在产品记录类型页面中显示您链接到产品的营销活动的名称。 更新促销活动信息会自动更新产品记录类型的促销活动链接记录字段。

### 将Adobe Workfront Planning记录从表视图或<!--Details tab of the-->记录页面连接到Workfront对象

<!--when we will have more applications to link to from Planning, change the title to something like: Connect Workfront Planning records to objects from other applications-->

在记录类型和Workfront对象类型之间创建连接后，可以将单个记录连接到Workfront中的对象。 您连接的Workfront字段会自动填充到链接对象的记录中。

>[!NOTE]
>
>您无法从Workfront中将Workfront对象类型与Workfront Planning记录类型连接起来。


{{step1-to-planning}}

1. 单击要连接其记录的工作区。

   工作区将打开，记录类型显示为卡片。
1. 单击记录类型的卡以打开记录类型页面。
1. 从&#x200B;**视图**&#x200B;下拉菜单中选择&#x200B;**表**&#x200B;视图。

1. 单击&#x200B;**新建记录**&#x200B;以将单个记录添加到您选择的记录类型。 有关信息，请参阅[创建记录](/help/quicksilver/planning/records/create-records.md)。
1. （视情况而定）将选定的记录类型与Workfront对象类型连接后，转到链接对象列，并双击与要与Workfront对象链接的记录对应的单元格。

   ![](assets/connect-projects-smaller-box-in-table-view.png)

1. 执行下列操作之一：

   * 单击列表中的对象以将其添加到所选记录。 对象按字母顺序列出。 对象将自动添加。
   * 开始键入对象的名称，并在该对象显示在列表中时单击它。 对象将自动添加。

   >[!TIP]
   >
   >您可以从视图中打开记录的页面，双击链接的记录字段，或单击字段中的&#x200B;**连接**&#x200B;以添加来自连接的对象类型的对象。

1. （可选）单击&#x200B;**查看全部**&#x200B;以显示您至少具有查看权限的所有对象。

1. （视情况而定）如果您在上一步中单击了&#x200B;**查看所有**，则会显示&#x200B;**连接对象**&#x200B;框。

   ![](assets/connect-objects-box-to-select-projects.png)

1. 开始在搜索框中键入Workfront对象的名称，然后当该对象显示在列表中时将其选定

   或

   在框中选择一个或多个对象的名称，然后单击&#x200B;**连接对象**。

   >[!IMPORTANT]
   >
   >* 您只能添加您有权查看的Workfront对象。
   >
   >* 添加Workfront对象后，每个对工作区具有“查看”或更高权限的用户都可以查看Workfront对象及其字段信息，无论他们在Workfront中的权限或访问权限如何。

   添加了以下内容：

   * 选定的Workfront对象将添加到链接的记录字段。
   * 如果您在通过Workfront连接记录类型时添加了它们，则Workfront对象的链接字段（或查找字段）会自动填充Workfront中的信息。

   有关将记录类型与来自其他应用程序的对象连接的详细信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。

1. （可选）单击表视图的链接字段或记录页面中链接字段内连接到Workfront Planning记录的Workfront对象的名称。

   如果您至少具有对象的“查看”权限，此操作将在Workfront中打开Workfront对象。

   >[!TIP]
   >
   >* 启用“允许多条记录”设置时，查找字段的值显示时用逗号分隔，或者根据您选择的聚合器聚合。
   >
   >* 在Workfront中，不会为链接的Workfront对象创建链接记录字段。

1. （可选）在记录类型的表视图中，将鼠标悬停在链接Workfront对象的列标题上，单击下拉菜单，然后单击&#x200B;**编辑查找字段**。

1. 从&#x200B;**未选择的字段**&#x200B;区域添加Workfront对象字段

   或

   从&#x200B;**选定字段**&#x200B;区域删除Workfront对象字段。

   这会从Workfront Planning记录中添加或删除链接字段。 与已删除字段关联的信息仍保留在Workfront中。


### 将Workfront Planning记录从表视图或<!--Details tab of the-->记录页面连接到Adobe Experience Manager对象

<!--when we will have more applications to link to from Planning, change the title to something like: Connect Workfront Planning records to objects from other applications-->

>[!IMPORTANT]
>
>您必须拥有Adobe Experience Manager Assets许可证，并且贵组织的Workfront实例必须载入Adobe业务平台或Adobe Admin Console，才能将Workfront Planning记录连接到Adobe Experience Manager Assets。
>
>如果您对加入Adobe Admin Console有任何疑问，请参阅[AdobeUnified Experience常见问题解答](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md)。

在记录类型与Adobe Experience Manager Assets之间创建连接后，可以将单个记录连接到Experience Manager资源。 创建连接后，您从Experience Manager Assets连接的资源字段会自动填充在您链接的记录类型中。

>[!NOTE]
>
>当Workfront管理员通过Experience Manager Assets与Workfront之间的集成配置元数据映射时，可从Adobe Experience Manager Assets访问Planning记录及其字段。 有关详细信息，请参阅[配置Adobe Workfront和Experience Manager Assets之间的资源元数据映射](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en)。

要将记录与AEM Assets连接：

{{step1-to-planning}}

1. 单击要连接其记录的工作区。

   此时会打开工作区，并显示记录类型。
1. 单击记录类型的卡以打开记录类型页面。
1. 从记录类型页面右上角的&#x200B;**视图**&#x200B;下拉菜单中选择&#x200B;**表**&#x200B;视图。

1. （可选）单击&#x200B;**新记录**&#x200B;以将新记录添加到您选择的记录类型。 有关信息，请参阅[创建记录](/help/quicksilver/planning/records/create-records.md)。
1. （视情况而定）将选定的记录类型与Experience Manager Assets连接后，转到链接对象列，将鼠标悬停在与要与Experience Manager中的其他对象链接的记录对应的单元格上，然后单击&#x200B;**+**&#x200B;图标。

   >[!TIP]
   >
   >  您可以在记录页面中的链接对象字段中添加&#x200B;**+**&#x200B;图标，以将资产连接到记录。

   此时会显示&#x200B;**选择Assets**&#x200B;框。<!--we might change this to Connect assets-->

   ![](assets/select-assets-box-for-aem-record-connections.png)

1. 单击可选择以下某些类型的资产：

   * 图像
   * 文件夹

   您可以选择多个资源。

   >[!IMPORTANT]
   >
   > 您只能连接您有权在Experience Manager中查看的资源。 连接后，所有Workfront Planning用户都可以在Workfront Planning中查看资源，无论他们在Experience Manager Assets中是否具有访问权限。

1. 单击&#x200B;**选择**。<!-- we might change this to Connect-->

   添加了以下内容：

   * 选定的Experience Manager资源将添加到链接的记录字段。
   * 链接的字段（或查找字段）会填充Experience Manager所连接资源中的信息。

     Experience Manager资源字段中的任何现有信息都会自动显示在链接或查找字段中。

     >[!TIP]
     >
     >* 如果启用了允许多条记录设置，则多个对象的值将以逗号分隔或根据您选择的聚合器聚合。
     >
     >* 在Experience Manager Assets应用程序中，不会为链接的Experience Manager资源创建指向Workfront Planning链接记录的链接记录字段。

1. （可选）转到您链接到Experience Manager Assets的记录类型，然后单击链接记录字段中的资源名称。 资源的Experience Manager详细信息将显示在弹出窗口中。<!--update screen shot with hi-rez picture-->

   ![](assets/asset-pop-up-window-with-aem-details-and-thumbnail.png)

   为图像文件显示以下字段：

   * 图像的缩略图
   * 图像文件名
   * 维度
   * 大小
   * 描述
   * Experience Manager中的文件路径
   * 资源类型
   * 创建日期
   * 修改日期

1. （可选）要在Experience Manager中打开Experience Manager资源记录页面，请转到要链接到的记录的记录类型页面，在链接的记录字段中单击资源的名称以打开弹出窗口，然后单击&#x200B;**在AEM中打开**&#x200B;图标![](assets/open-asset-icon.png)以打开该资源。

   这会在Adobe Experience Manager Assets中打开Experience Manager资源。

1. （可选）在记录类型的表视图中，将鼠标悬停在链接的Experience Manager资源的列标题上，单击下拉菜单，然后单击&#x200B;**编辑查找字段**。

1. 从&#x200B;**未选择的字段**&#x200B;区域添加Experience Manager Assets对象字段

   或

   从&#x200B;**选定字段**&#x200B;区域删除Workfront对象字段。

   这会在记录中添加或删除链接字段。 与已删除字段关联的信息仍保留在AdobeExperience Assets中。

<!--
### Connect Workfront Planning records from the Connections tab of the record page

1. Go to any view of a record type that has been connected to other record types or object types from other applications. 
1. Follow the steps described in the previous subsections to find a record in the view that you want to connect with other records or objects. 
1. Click the name of a record. 

    The preview page opens. 
1. (Optional) Click the **Open in new tab** icon ![](assets/open-details-in-a-new-tab-icon.png) to open the record's page. 
1. Click the **Connections** tab in the record's preview or page. 

    ![](assets/connections-tab-on-record-in-workfront-planning.png)

    All record or object types that are linked to the selected record type display as sections. Connected records or objects display under their record or object type names on cards. 

1. (Optional) Click the downward-pointing arrow to the left of a section to collapse it. 

1. (Conditional) If there are records or objects connected to the selected record, click **Connect** to add more records or objects of the same type. 
    The Connect button does not display if there are no records currently connected to the selected record. 
1. Follow the steps describes in the previous sections to connect records from Workfront Planning or objects from Workfront or AEM Assets. 
    The records and objects are added immediately.
1. (Optional) Hover over the connected card of a record or object, then click the **Disconnect record** icon to disconnect it from the selected record. 

    ![](assets/disconnect-record-icon-with-tooltip-on-connections-tab.png)

    The record is immediately disconnected from all areas of Workfront Planning or from other applications where it might show as connected. Any lookup field values are also removed. 

-->

## 从Workfront对象连接记录

要从Workfront对象连接Workfront Planning记录，您必须具备以下条件：

* 在Workfront Planning中建立的记录类型与Workfort对象类型之间的连接。
* Workfront或组管理员必须将Planning部分添加到可以连接到“布局模板”中的Planning记录类型的Workfront对象类型中。

有关详细信息，请参阅Adobe Workfront对象的“规划”部分中的[管理记录](/help/quicksilver/planning/records/manage-records-in-planning-section.md)。
