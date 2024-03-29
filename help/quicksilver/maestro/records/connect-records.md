---
title: 连接记录
description: 在记录类型之间创建连接后，可以将各个记录彼此连接。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 17796cdc-6de8-4209-a5af-b255dc64d70a
source-git-commit: a0f12a016ae8ac73136f05bf3255f9882e2ce6d4
workflow-type: tm+mt
source-wordcount: '2372'
ht-degree: 1%

---

<!--when you make this live, update the metadata above to this: 
---
title: Connect records and objects
description: In addition to connecting Maestro records to one another, you can also connect Maestro records to objects from other applications.  
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->
<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--if you change steps here, also update steps in the "Connect records" article-->

# 连接记录

{{maestro-important-intro}}

您可以将Adobe Workfront Planning记录连接到其他应用程序或对象。

必须首先将两个记录类型相互连接，或者将记录类型从另一个应用程序连接到对象类型。 这将创建链接的记录字段。 然后，可以使用链接的记录字段将记录彼此连接，或将记录与其他应用程序中的其他对象连接。

连接记录与将记录从另一个应用程序连接到对象类似。

有关将记录类型相互连接或从其他应用程序连接到对象类型的信息，请参见 [连接记录类型](../architecture/connect-record-types.md).

有关连接记录类型的示例，请参见 [连接记录类型和记录的示例](../architecture/example-connect-record-types-and-records.md).

您可以连接以下各项：

* Adobe Workfront规划记录
* Adobe Workfront计划记录包含来自其他应用程序的对象。

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

您必须具有以下权限才能执行本文中的步骤：

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
   <p>要将Adobe Workfront规划记录与Experience Manager Assets连接，您必须具有Adobe Experience Manager Assets许可证，并且贵组织的Workfront实例必须载入到Adobe业务平台或Adobe Admin Console。</p>
   </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront协议</p></td>
   <td>
<p>贵组织必须注册Adobe Workfront计划封闭测试版计划。 请联系您的客户代表以查询此新产品/服务。 </p>
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
   <td role="rowheader"><p>访问级别配置</p></td>
   <td> <p>Workfront规划没有访问级别控制</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>权限</p></td>
   <td> <p>管理工作区权限以连接记录 </p>  
   <p>查看工作区或更高权限以查看与其他应用程序中的对象和字段的所有连接，无论您对其他应用程序的访问权限如何。 </p>
   <p>系统管理员有权访问所有工作区，包括他们未创建的工作区。</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>您的Workfront或组管理员必须在布局模板中添加Planning区域。 有关信息，请参阅 <a href="../access/access-overview.md">访问概述</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 连接记录

### 有关连接记录的注意事项

* 连接记录类型后，连接的记录类型会在链接它们的记录类型表格中以及链接它们的记录的“详细信息”页面中显示为链接记录字段。
* 您可以从链接的记录字段中浏览和添加链接记录的记录和对象以及对象类型。
* 您可以将链接记录类型的字段添加到要链接的记录类型的表中。
* 您无法手动更新正在链接的记录中链接字段的值。

  链接记录的链接字段的值会自动从原始记录或对象中填充您正在链接的Workfront计划记录。

* 有权访问Workfront规划和视图或者对工作区具有更高权限的每个人，都可以查看您在记录之间或记录与其他应用程序的对象之间建立的连接。 他们可以查看连接的记录和对象，无论他们在您连接的应用程序中的权限如何。
* 如果您对连接记录所在的工作区具有管理权限，则可以查看和编辑其他人的连接。
* 您可以将一个记录连接到另一个应用程序的一个或多个对象。
* 要将记录与其他记录或对象链接，您必须具备以下各项：

   * 至少一个工作区、记录类型和记录。

     有关更多信息，请参阅以下文章：

      * [创建工作区](../architecture/create-workspaces.md)
      * [创建记录类型](../architecture/create-record-types.md)
      * [创建记录](../records/create-records.md)

   * 记录类型之间的连接，或记录类型与其他应用程序的对象之间的连接。 有关信息，请参阅 [连接记录类型](../architecture/connect-record-types.md)

### 连接Adobe Workfront规划记录

{{step1-to-maestro}}

默认情况下应打开上次访问的工作区。

1. （可选）展开现有工作区名称右侧的向下箭头，然后选择要从中连接记录的工作区。
1. 单击记录类型的卡以打开记录类型页面。
1. 选择 **表** 从查看 **视图** 记录类型页面右上角的下拉菜单
1. （可选）通过向表中添加新行，将记录添加到您选择的记录类型。 有关信息，请参阅 [创建记录](../../maestro/records/create-records.md).
1. （视情况而定）将所选记录类型与其他记录类型连接后，转到链接的记录列，并双击要与其他记录链接的记录对应的单元格。

   ![](assets/connect-other-records-smaller-box-in-table-view.png)

1. 执行下列操作之一：

   * 从列表中单击已连接记录的名称以将其添加到所选记录。 记录会自动添加。
   * 开始键入记录的名称，并在该记录显示在列表中时单击它。 记录会自动添加。
   * 单击 **查看全部** 以显示所有记录。

1. （视情况而定）如果您单击 **全选** 在上一步中， **连接对象** 框显示。

   ![](assets/connected-objects-table-for-records.png)

1. 在搜索框中开始键入记录的名称，然后当它显示在列表中时将其选定

   或

   在框中选择一个或多个记录的名称，然后单击 **连接对象** “连接对象”框右上角的。

   >[!TIP]
   >
   >    您可以打开记录的详细信息页面，找到链接的记录字段，然后单击 **+** 图标以添加来自连接的记录或对象类型的记录。

   添加了以下内容：

   * 链接的记录显示在您在步骤6中选择的记录的链接记录字段中。 <!--accurate?-->
   * 如果您在连接记录类型时添加了链接的查找字段，则链接字段会填充有链接记录中的信息。

   更新链接的记录会自动更新您正在链接的记录的链接字段。 您无法手动编辑链接的字段。

   >[!TIP]
   >
   >* 我们交替使用“链接字段”和“查找字段”。
   >
   >* 如果您已启用 **允许多条记录** 设置连接记录类型时，多个选定对象的字段值显示时用逗号分隔，或根据您选择的聚合器聚合。

1. （可选）关闭记录类型页面，然后转到您选择的工作区。
1. 单击链接到的记录类型的卡。

   例如，如果您已连接 **营销活动** 包含产品记录的记录，单击 **产品** 卡片。

   记录类型卡片应在“表”视图中打开。 如果没有，请选择表格视图。

   请注意 **营销活动** 链接记录字段显示您在产品记录类型页面中链接到产品的营销活动的名称。 更新促销活动信息会自动更新产品记录类型的促销活动链接记录字段。

### 将Adobe Workfront计划记录连接到Workfront对象

<!--when we will have more applications to link to from Maestro, change the title to something like: Connect Maestro records to objects from other applications-->

在记录类型和Workfront对象类型之间创建连接后，可以将单个记录连接到Workfront中的对象。 您连接的Workfront字段会自动填充到链接对象的记录中。

>[!NOTE]
>
>您无法将Workfront对象与Workfront中的Workfront规划记录相关联。


{{step1-to-maestro}}

默认情况下应打开上次访问的工作区。

1. （可选）展开现有工作区名称右侧的向下箭头，然后选择要从中连接记录的工作区。
1. 单击记录类型的卡以打开记录类型页面。
1. 选择 **表** 从查看 **视图** 下拉菜单。

1. 单击 **新记录**  将单个记录添加到您选择的记录类型。 有关信息，请参阅 [创建记录](../../maestro/records/create-records.md).
1. （视情况而定）将选定的记录类型与Workfront对象类型连接后，转到链接对象列，并双击与要与Workfront对象链接的记录对应的单元格。

   ![](assets/connect-projects-smaller-box-in-table-view.png)

1. 执行下列操作之一：

   * 单击列表中的对象以将其添加到所选记录。 对象按字母顺序列出。 对象将自动添加。
   * 开始键入对象的名称，并在该对象显示在列表中时单击它。 对象将自动添加。
   * 单击 **查看全部** 显示您至少具有查看权限的所有对象。

1. （视情况而定）如果您单击 **查看全部** 在上一步中， **连接对象** 框显示。

   ![](assets/connect-objects-box-to-select-projects.png)

1. 开始在搜索框中键入Workfront对象的名称，然后当该对象显示在列表中时将其选定

   或

   在框中选择一个或多个对象的名称，然后单击 **连接对象** “连接对象”框右上角的。

   >[!IMPORTANT]
   >
   >* 您只能添加您有权查看的Workfront对象。
   >
   >* 添加Workfront对象后，每个对工作区具有“查看”或更高权限的用户都可以查看Workfront对象及其字段信息，无论他们在Workfront中的权限或访问权限如何。

   添加了以下内容：

   * 选定的Workfront对象将添加到链接的记录字段。
   * 如果您在通过Workfront连接记录类型时添加了它们，则Workfront对象的链接字段（或查找字段）会自动填充Workfront中的信息。

   >[!TIP]
   >
   >您可以打开记录的详细信息页面，找到链接的记录字段，然后单击 **+** 图标，以从连接的对象类型添加对象。

   有关将记录类型与来自其他应用程序的对象连接的详细信息，请参见 [连接记录类型](../architecture/connect-record-types.md).

1. （可选）单击表视图的链接字段或表的链接字段中连接到Workfront计划记录的Workfront对象的名称。 **详细信息** 记录页。

   这将打开只读的Workfront规划 **详细信息** 页面中显示的链接Workfront对象。 将记录类型与Workfront对象连接后，您选择作为查找字段的字段会显示在Workfront计划记录的详细信息页面中。

   >[!TIP]
   >
   >* 启用“允许多条记录”设置时，查找字段的值显示时用逗号分隔，或者根据您选择的聚合器聚合。
   >
   >* 在Workfront中，不会为链接的Workfront对象创建链接记录字段。

1. （可选）要在Workfront中打开链接的Workfront对象，请单击 **转到源** Workfront对象的“详细信息”页面的右上角。

   ![](assets/workfront-project-maestro-details-page-with-go-to-source-link.png)

   如果您至少具有查看对象的权限，这将打开Workfront对象页面。 如果您有相应的权限，则可以编辑有关Workfront对象的信息。

1. （可选）在记录类型的表格视图中，将鼠标悬停在链接Workfront对象的列标题上，单击下拉菜单，然后单击 **编辑查找字段**.

1. 从添加Workfront对象字段 **未选择的字段** 区域

   或

   从中删除Workfront对象字段 **选定的字段** 区域。

   这会从Workfront规划记录中添加或删除链接字段。 与已删除字段关联的信息仍保留在Workfront中。


### 将Workfront计划记录连接到Adobe Experience Manager对象

<!--when we will have more applications to link to from Maestro, change the title to something like: Connect Maestro records to objects from other applications-->

>[!IMPORTANT]
>
>您必须拥有Adobe Experience Manager Assets许可证，并且贵组织的Workfront实例必须载入Adobe业务平台或Adobe Admin Console，才能将Workfront规划记录连接到Adobe Experience Manager Assets。
>
>如果您对入门Adobe Admin Console有任何疑问，请参阅 [Adobe统一Experience常见问题解答](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

在记录类型与Adobe Experience Manager Assets之间创建连接后，可以将单个记录连接到Experience Manager资源。 创建连接后，您从Experience Manager Assets连接的资源字段会自动填充在您链接的记录类型中。

{{step1-to-maestro}}

默认情况下应打开上次访问的工作区。

1. （可选）展开现有工作区名称右侧的向下箭头，然后选择要从中连接记录的工作区。
1. 单击记录类型的卡以打开记录类型页面。
1. 选择 **表** 从查看 **视图** 记录类型页面右上角的下拉菜单

1. （可选）单击 **新记录** 以将新记录添加到您选择的记录类型。 有关信息，请参阅 [创建记录](../../maestro/records/create-records.md).
1. （视情况而定）将选定的记录类型与Experience Manager Assets连接后，转到链接对象列，将鼠标悬停在与要与Experience Manager中的其他对象链接的记录对应的单元格上，然后单击 **+** 图标。

   >[!TIP]
   >
   >  您可以添加，然后单击 **+** 图标将资产连接到记录的详细信息页面中的链接对象字段。

   此 **选择资源** 框显示。 <!--we might change this to Connect assets-->

   ![](assets/select-assets-box-for-aem-record-connections.png)

1. 单击可选择以下某些类型的资产：

   * 图像
   * 文件夹

   您可以选择多个资源。

   >[!IMPORTANT]
   >
   > 您只能连接您有权在Experience Manager中查看的资源。 连接后，所有Workfront规划用户都可以在Workfront规划中查看资源，无论他们在Experience Manager Assets中是否具有访问权限。

1. 单击 **选择**. <!-- we might change this to Connect-->

   添加了以下内容：

   * 选定的Experience Manager资源将添加到链接的记录字段。
   * 链接的字段（或查找字段）会填充Experience Manager所连接资源中的信息。

     Experience Manager资源字段中的任何现有信息都会自动显示在链接或查找字段中。

     >[!TIP]
     >
     >* 如果启用了允许多条记录设置，则多个对象的值将以逗号分隔或根据您选择的聚合器聚合。
     >
     >* 没有在Experience Manager Assets应用程序中为链接的Experience Manager资源创建指向Workfront Planning链接记录的链接记录字段。

1. （可选）转到您链接到Experience Manager Assets的记录类型，然后单击链接记录字段中的资源名称。 资源的Experience Manager详细信息将显示在弹出窗口中。 <!--update screen shot with hi-rez picture-->

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

1. （可选）要在Experience Manager中打开“Experience Manager资源记录详细信息”页面，请转到要链接到的记录的记录类型页面，单击链接记录字段中的资源名称以打开弹出窗口，然后单击 **打开** 图标 ![](assets/open-asset-icon.png) 以打开资产。

   这会在Adobe Experience Manager Assets中打开Experience Manager资源。

1. （可选）在记录类型的表格视图中，将鼠标悬停在链接的Experience Manager资源的列标题上，单击下拉菜单，然后单击 **编辑查找字段**.

1. 从添加Experience Manager Assets对象字段 **未选择的字段** 区域

   或

   从中删除Workfront对象字段 **选定的字段** 区域。

   这会在记录中添加或删除链接字段。 与已删除字段关联的信息仍保留在AdobeExperience Assets中。
