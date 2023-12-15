---
title: 连接记录类型
description: 指示各个记录类型如何相互关联的一种方法是连接它们。 此外，您可以将Maestro记录类型与其他应用程序中的对象类型连接起来，以增强用户体验并将它们的焦点集中在一个应用程序中。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: 6f026590f0030b564f0d110afead9ade1acd7896
workflow-type: tm+mt
source-wordcount: '2020'
ht-degree: 0%

---

<!-----
title: Connect record types
description: A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Maestro record types with object types from other applications to enhance your users' experience and keep their focus in one application.
hidefromtoc: yes
hide: yes
feature: Work management
role: User
author: Alina
--->

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->
<!--************ THIS MIGHT NO LONGER BE A 'RELATIONSHIP' TYPE FIELD, BECAUSE THEY WILL SHOW IT IN THE CONNECTION TAB*****************************-->


# 连接记录类型

>[!IMPORTANT]
>
>本文中的信息是指AdobeMaestro，它是Adobe Workfront提供的新产品。
>
>目前，AdobeMaestro是测试版计划的一部分，该计划对有限数量的客户开放。 您必须是Workfront客户才能使用Maestro功能。
>
>有关加入Maestro测试版计划的更多信息，请与您的客户代表联系。
>
>有关信息，请参阅 [Adobe大师概述](../maestro-overview.md).

Adobe您可以使用Maestro来设计完全可自定义的工作区，其中包含组织所需的记录类型。 指示各个记录类型如何相互关联的一种方法是连接它们。 此外，您可以将Maestro记录类型与其他应用程序中的对象类型连接起来，以增强用户体验并将它们的焦点集中在一个应用程序中。

您可以连接以下各项：

* 将主要操作记录类型相互转换
* 相互间的主要分类
* 将主要操作记录类型和分类相互关联
* Maestro操作记录类型和分类与其他应用程序的对象类型相同。

这样，您便可以在另一个Maestro记录中显示链接记录或对象类型中的字段。

本文介绍了如何将两个Maestro记录类型或Maestro记录类型与另一个应用程序中的对象连接起来。

建立记录或对象类型之间的连接后，可以将各个记录相互连接。

有关将Maestro记录连接到另一个应用程序的对象的信息，请参见 [连接记录](../records/connect-records.md).

有关连接记录类型的示例，请参见 [连接记录类型和记录的示例](../architecture/example-connect-record-types-and-records.md).

<!--ensure this last linked article is right; the title and the link should have changed-->

## 访问要求

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
   <p> Adobe产品</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p><b>注释</b></p>
   <p>要将Maestro记录类型与Experience Manager Assets连接，您必须具有Adobe Experience Manager Assets许可证，并且贵组织的Workfront实例必须载入Adobe业务平台或Adobe Admin Console。 </p>
   </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront协议</p></td>
   <td>
<p>贵公司必须注册AdobeMaestro封闭测试版计划。 请联系您的客户代表以查询此新产品/服务。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront计划</p></td>
   <td>
<p>任何</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront许可证</p></td>
   <td>
   <p>任何</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">访问级别</td>
   <td> <p>任何</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">布局模板</td>
   <td> <p>系统管理员必须在布局模板中添加Maestro区域。 有关信息，请参阅 <a href="../access/grant-access.md">授予对Adobe大师的访问权限</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> <p>To connect Maestro record types with Experience Manager Assets, you must have an Adobe Experience Manager Assets license and your organization's instance of Workfront must be onboarded to the Adobe Business Platform or the Adobe Admin Console.</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create
</td>
  </tr>
 </tbody>
</table>

-->

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->


## 有关连接记录类型的注意事项

请考虑以下事项：

* 可以在Maestro中连接以下实体：

   * 两种操作记录类型
   * 两种分类
   * 操作记录类型和分类
   * 操作记录类型或分类以及来自其他应用程序的对象类型。

* 您可以连接以下具有Maestro记录类型的应用程序中的以下对象：

   * Adobe Workfront：

      * 项目
      * 项目组合
      * 项目群
      * 公司
      * 群组

   * Adobe Experience Manager Assets：

      * 图像
      * 文件夹

     >[!IMPORTANT]
     >
     >您必须具有Adobe Experience Manager Assets许可证，并且贵组织的Workfront实例必须载入Adobe业务平台或Adobe Admin Console，才能将Maestro记录连接到Adobe Experience Manager Assets。
     >
     >如果您对入门Adobe Admin Console有任何疑问，请参阅 [Adobe统一Experience常见问题解答](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

* 将记录类型与另一个记录类型或另一个应用程序中的对象类型连接后，将出现以下情况：

   * **连接两种记录类型时**：在您连接的记录类型上创建链接记录字段。 在您连接的记录类型上会创建一个类似的链接记录字段。

     例如，如果将“Campaign”记录类型与“Product”记录类型连接，则将在“Campaign”记录类型上创建名为“链接的产品”的链接记录字段，并在“Product”记录类型上创建自动名为“Campaign”的链接记录类型。

   * **将记录类型与另一个应用程序的对象类型连接时**：在您连接的记录类型上创建链接记录字段。 在第三方应用程序对象上不会自动创建任何链接的记录字段。

     仅当实际对象连接到Maestro记录时，才会为第三方应用程序对象创建新的Maestro记录类型。

     有关更多信息，请参阅 [连接记录](../records/connect-records.md).

   * **从您连接的记录或对象添加查找字段时**：链接的字段会添加到您正在连接的记录中，其中显示您选择的查找字段，这些字段将从链接的记录转到您正在链接的记录。 记录字段始终为只读，并且会自动填充第三方对象的值。

     例如，如果您将“Campaign”Maestro记录类型连接到Workfront项目，并且选择将该项目的“计划完成日期”字段引入Maestro记录，则将为您链接来源的记录自动创建一个名为“计划完成日期”（来自项目）的链接字段。

* 链接的记录字段前面有关系图标 ![](assets/relationship-field-icon.png).

  链接的字段前面有标识该字段类型的图标。 例如，指示字段是数字、段落或日期的图标。

* 为记录类型创建单个记录后，您可以从链接的记录类型字段中选择连接到的记录。 有关信息，请参阅 [连接记录](../records/connect-records.md).

## 连接记录类型

<!--when changes here, also update the article for "Connect records"-->

{{step1-to-maestro}}

默认情况下应打开上次访问的工作区。

1. （可选）展开现有工作区名称右侧的向下箭头，然后选择要从中连接记录类型的工作区。
1. 单击记录类型的卡以打开记录类型页面。
1. 单击 **+** 图标，然后单击 **新建连接** 选项卡。

   ![](assets/new-connection-tab-with-workfront-aem-options.png)

1. 在 **记录类型** 字段中，选择下列选项之一： <!--is the field name spelled right? lowercase "t"?-->

   * 所选工作区中的其他操作记录类型或分类

     >[!TIP]
     >
     >只有所选工作区中的记录类型和分类可供连接。
     > 
     >如果在所选工作区中没有其他记录类型，则不会显示工作区名称。

   * A **项目、Portfolio、计划、公司**，或 **组** 从 **Workfront对象类型** 部分。
   * **Experience Manager Assets** 从 **Adobe应用程序** 部分。

   ![](assets/new-connection-tab-fields-with-another-record-selected.png)


1. 更新以下信息：

   * **名称**：已连接字段的名称，它将显示在原始记录类型的表视图或详细信息页面中。 这会在原始记录类型的表视图或原始记录的链接记录字段中创建链接记录列。 <!--ensure they updated this; and update the screen shot: it used to be "Label"-->

   >[!TIP]
   >
   >我们建议您在连接的记录字段的名称中包含要链接到的记录名称，以捕获新字段来自的记录类型。 链接的记录的名称在新链接的记录字段或其链接的字段中不可见。

   * **描述**：有关连接的记录字段的其他信息。 当您将鼠标悬停在表中的字段列上时，将显示字段的描述。
   * **允许多条记录**：选择此选项以指示您允许用户在链接记录类型字段显示在原始记录上时添加多个记录。 默认情况下，该选项处于选中状态。
   * **选择查找字段**：选择此选项可从所选记录类型添加字段。 默认情况下，该选项处于选中状态。

1. （视情况而定，可选）如果您已选择连接Workfront对象，请选择 **自定义表单** 从 **仅链接符合这些条件的项目** 部分。 <!--this needs to be updated for each object when they fix this UI.--> 只有附加了选定自定义表单的对象才能链接到选定的Maestro记录类型。 您可以选择多个表单。

   ![](assets/workfront-project-connection-selection.png)

1. （视情况而定）如果您已选择连接到Experience Manager Assets，请从以下位置选择一个存储库： **Experience Manager存储库** 中的下拉菜单 **链接以下存储库中的资产** 部分。 这是必填字段。 只有您在Experience Manager Assets中有权访问的存储库才会显示在此字段中。

   ![](assets/aem-assets-connection-selection.png)

1. 单击 **创建**.

1. （视情况而定）如果您选择 **选择查找字段** 设置， **添加查找字段** 框打开。

   单击 **+** 图标，以添加来自的字段 **未选择的字段** 区域。

   或

   单击 **-** 图标，以从删除字段 **选定的字段** 区域

   ![](assets/add-lookup-fields-for-another-maestro-record-type-box.png)


1. （可选）单击 **跳过** 并且不要从链接的记录或对象添加任何字段。 此 **名称** 在原始记录的表格视图中，链接记录的字段是唯一可见的字段。

1. （可选且视情况而定）如果选择链接数字、货币、百分比或日期类型字段，则还应选择聚合器值。 当用户在链接的记录字段中选择多个链接记录时，链接字段的值会根据您选择的聚合器显示为逗号分隔的或聚合的值。

   ![](assets/aggregator-drop-down-for-number-linked-field.png)

   >[!NOTE]
   >
   > 将记录类型连接到Experience Manager Assets时，聚合不可用。

   从以下项中选择：

   * **无**：显示来自用逗号分隔的多个记录的值。 这是默认选项。
   * **MAX**：显示来自在链接记录字段中选择的多个记录的所有值中的最高值。
   * **MIN**：显示在链接记录字段中选择的多个记录的所有值中的最小值。
   * **SUM**：显示来自在链接的记录字段中选择的多个记录的所有值的总数。
   * **平均**：显示来自在链接的记录字段中选择的多个记录的所有值的平均值。

   >[!NOTE]
   >
   >例如，您可以从Campaign记录（原始记录）中链接产品记录（链接记录），并将其命名为“产品字段”。 您还可以选择从营销活动记录中链接产品记录的“预算”字段，并将其称为“产品预算”。 如果您允许在“产品字段”中选择多个记录，则可以选择预算为$120,000的产品1和预算为$100,000的产品2。 您可以在链接字段中查看原始记录的以下预算信息，具体取决于您选择的汇总：
   >
   >* **无**：120,000美元，100,000美元
   >* **MAX**：120,000美元
   >* **MIN**：100,000美元
   >* **SUM**：220,000美元
   >* **平均**：110,000美元
   >

1. （可选）使用 **搜索** 图标 ![](assets/search-icon.png) 以搜索字段。

1. 单击 **添加字段** 以保存更改。

   添加了以下项目：

   * 手动添加链接记录类型中的记录后，显示这些记录的链接记录字段。 链接记录字段的名称是您在步骤5中选择的名称。 <!--accurate-->

   * 在链接记录字段中手动添加记录后，显示链接记录类型字段中信息的链接字段（或字段）。 仅在以下情况下创建链接的字段： **选择查找字段** 创建连接时可选择“设置”。 链接的字段根据以下模式进行命名：

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

   * 当您将Maestro记录类型链接到彼此时，链接记录字段也会添加到要链接的记录类型上。 链接记录类型中链接的记录字段的名称是您链接来源的记录类型的名称。

     例如，如果您从“Campaign”记录类型中链接“Product”记录类型，并将营销活动的连接字段命名为“链接的产品”，则会为“Product”记录类型创建“Campaign”链接记录字段。

1. （可选）在原始记录类型或链接记录类型表格视图中，单击链接记录字段标题中的向下箭头，然后单击以下任一项：

   * **编辑字段**：您只能更新 **名称** 和 **描述** 字段的信息。
   * **编辑查找字段**：添加或删除任何链接记录的字段。

   ![](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   要添加或移除查找字段，请按照上述步骤9-13中的说明操作。 <!--ensure these step numbers stay accurate-->

   >[!NOTE]
   >
   > 您无法将链接到的记录的查找字段添加到指示第三方应用程序中对象的链接记录类型。
   >
   > 例如，在链接到Workfront项目时，您无法从“Maestro项目”记录类型中显示的“Campaign”链接记录字段中添加“Campaign”Maestro对象的查找字段。


1. （可选）在链接记录字段标题中，从要链接的记录类型单击向下箭头，然后单击 **删除**.

   记录字段和任何其他链接的查找字段将被删除，并且这些字段及其信息将无法恢复。

   >[!TIP]
   >
   >    您链接到的记录类型中的链接记录字段不会被删除。 <!-- is this still accurate?! -->
