---
title: 连接记录
description: 在记录类型之间创建连接后，可以将各个记录彼此连接。
hidefromtoc: true
hide: true
source-git-commit: f058c369bdb3b991910d3a820895de73ea4709f0
workflow-type: tm+mt
source-wordcount: '1803'
ht-degree: 0%

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
<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

<!--if you change steps here, also update steps in the "Connect records" article-->

# 连接记录

>[!IMPORTANT]
>
>目前，AdobeMaestro是测试版计划的一部分，该计划对有限数量的客户开放。
>
>有关加入Maestro测试版计划的更多信息，请与您的客户代表联系。
>
>有关信息，请参阅 [Adobe大师概述](../maestro-overview.md).

您可以将AdobeMaestro记录连接到其他应用程序或对象。

您必须先将两个记录类型连接在一起，或者将记录类型连接到另一个应用程序中的对象类型，然后可以使用记录类型的“表”视图将记录连接到另一个对象，或者将记录连接到其他对象。

有关将记录类型相互连接或从其他应用程序连接到对象类型的信息，请参见 [连接记录类型](../architecture-and-fields/connect-record-types.md).

有关连接记录类型的示例，请参见 [连接记录类型和记录的示例](../architecture-and-fields/example-connect-record-types-and-records.md).

您可以连接以下各项：

* Maestro操作记录
* 将操作记录转换为分类记录
* Maestro操作记录和来自其他应用程序的对象。

  当前支持以下应用程序和对象类型：

   * Adobe Workfront

      * 项目
      * 项目组合
      * 项目群
      * 公司
      * 组

  <!--when you add more objects, fix the Access Requirements below which right now refer only to projects-->

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto">
 <col>
<tbody>
<td>
   <p> Adobe产品</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
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
   <td><p>任意，创建Maestro记录</p> 
<p>在Workfront中查看项目的工作或更高版本</p>
  <p>有关更多信息，请参阅 <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">Adobe Workfront许可证概述</a>.</p> 
  </td>
  </tr>
  <tr>
   <td role="rowheader">访问级别</td>
   <td> <p>任意，创建Maestro记录</p>
<p>查看或更高权限的项目、Portfolio、项目群</p> 
<p>查看用户不属于的组或公司时，对组和公司的附加访问权限</p>   
</td>
  </tr>
<tr>
   <td role="rowheader"><p>对象权限</p></td>
   <td> <p>查看要与Maestro记录链接的对象或授予更高的权限  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>系统管理员必须在布局模板中添加Maestro区域。 有关信息，请参阅 <a href="../access/grant-access.md">授予对Adobe大师的访问权限</a>. </p></td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## 连接记录

### 有关连接记录的注意事项

* 建立记录类型之间的连接后，连接的记录类型在它们链接到的记录类型表中显示为链接记录字段。
* 您可以从链接的记录字段中浏览和添加链接记录的记录和对象以及对象类型。
* 您可以将链接记录类型的字段添加到要链接的记录类型的表中。
* 您无法手动更新正在链接的记录中链接字段的值。

  链接记录中链接字段的值会自动填充您正在链接的Maestro记录。

* 每个有权访问Maestro的人都可以看到您在Maestro记录之间或Maestro记录与Workfront对象之间建立的连接。 此外，您还可以查看和编辑其他所有人的连接。 <!--add that this is based on your permissions in both Maestro and Workfront (or, later, any other application)-->
* 您可以将一个Maestro记录连接到另一个应用程序的一个或多个对象。
* 不能连接分类以记录类型或从其他应用程序连接到对象。 <!-- this is temporary; there will be certain objects (teams, etc) that will be linked to taxonomies, per Lilit-->
* 目前，您只能将Maestro记录链接到Workfront对象。 要将Maestro记录与Workfront对象链接，您必须具备以下条件：

   * Workfront对象。 例如，您必须首先在Workfront中创建项目、项目组合、项目、公司或组。
   * Maestro工作区、记录类型和记录。 有关更多信息，请参阅以下文章：

      * [创建工作区](../architecture-and-fields/create-workspaces.md)
      * [创建记录类型](../architecture-and-fields/create-record-types.md)
      * [创建记录](../records/create-records.md)

   * 记录类型之间的连接，或记录类型与其他应用程序的对象之间的连接。 有关信息，请参阅 [连接记录类型](../architecture-and-fields/connect-record-types.md).

### 连接Maestro记录

1. 单击 **主菜单** 图标 ![](assets/main-menu-workfront.png) 在Workfront的右上角， <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> 然后单击 **大师** ![](assets/maestro-icon.png).

   默认情况下应打开上次访问的工作区。

1. （可选）展开现有工作区名称右侧的向下箭头，然后选择要从中连接记录的工作区。
1. 单击记录类型的卡以打开记录类型页面。
1. 从中选择表视图 **视图** 记录类型页面右上角的下拉菜单
1. 从所选记录类型添加与另一记录或对象类型的连接。 有关信息，请参阅 [连接记录类型](../architecture-and-fields/connect-record-types.md).

新列将添加到表中以显示链接的记录类型。

1. 通过向表添加新行将记录添加到您选择的记录类型。 有关信息，请参阅 [创建记录](../../maestro/records/create-records.md).
1. 从表视图中列出的记录，转到链接的记录列，将鼠标悬停在与要与其他Maestro记录链接的记录对应的单元格上，然后单击 **+** 图标。

   此 **连接对象** 框显示。

   ![](assets/connected-objects-table-for-records.png)

1. 在搜索框中开始键入记录的名称，然后当它显示在列表中时将其选定

   或

   在框中选择一个或多个记录的名称，然后单击 **连接对象** “连接对象”框右上角的。

   添加了以下内容：

   * 链接的记录显示在您在步骤3中选择的记录的链接记录字段中。 更新链接的记录会自动更新您正在链接的记录的链接记录字段。 <!--ensure the number of the step stays accurate-->
   * 属于链接记录的链接字段会自动填充原始链接记录中的信息。 您无法手动编辑链接的字段。

     >[!TIP]
     >
     >* 我们交替使用“链接字段”和“查找字段”。
     >
     >* 如果在连接记录类型时启用了“允许多条记录”设置，则多个选定对象的字段值要么以逗号分隔，要么根据您选择的聚合器聚合。

1. （可选）关闭“Maestro记录类型”页面，然后转到您选择的工作区。
1. 单击链接到的记录类型的卡。

   例如，如果您已将Campaign记录与产品记录连接，请单击 **产品** 卡片。

   记录类型卡片应在“表”视图中打开。

   请注意，Campaign链接记录字段显示您在产品记录类型页面中链接到产品的营销活动的名称。 更新促销活动信息会自动更新产品记录类型的促销活动链接记录字段。

### 将Maestro记录连接到Workfront对象

<!--when we will have more applications to link to from Maestro, change the title to soemthing like: Connect Maestro records to objects from other applications-->

在Maestro记录类型和Workfront对象类型之间创建连接后，可以将单个Maestro记录连接到Workfront中的对象。 您还可以将字段从Workfront对象连接到Maestro记录类型。

1. 单击 **主菜单** 图标 ![](assets/main-menu-workfront.png) 在Workfront的右上角， <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> 然后单击 **大师** ![](assets/maestro-icon.png).

   默认情况下应打开上次访问的工作区。

1. （可选）展开现有工作区名称右侧的向下箭头，然后选择要从中连接记录的工作区。
1. 单击记录类型的卡以打开记录类型页面。
1. 从中选择表视图 **视图** 记录类型页面右上角的下拉菜单
1. 从Workfront中为选定记录类型添加与对象类型的新连接。 从Workfront部分下的以下对象中进行选择：

   * 项目
   * 项目组合
   * 项目群
   * 公司
   * 组

   有关更多信息，请参阅 [连接记录类型](../architecture-and-fields/connect-record-types.md).

   新列将添加到表中以显示链接对象类型。

1. 通过将新行添加到表，将单个记录添加到您选择的记录类型。 有关信息，请参阅 [创建记录](../../maestro/records/create-records.md).
1. 从表格视图中列出的记录，转到链接对象列，将鼠标悬停在与要与Workfront中的其他对象链接的记录对应的单元格上，然后单击 **+** 图标。 <!--change Workfront to other applications, when this will be possible-->

   此 **连接对象** 框显示。

   ![](assets/connect-objects-box-to-select-projects.png)

1. 开始在搜索框中键入Workfront对象的名称，然后当该对象显示在列表中时将其选定

   或

   在框中选择一个或多个对象的名称，然后单击 **连接对象** “连接对象”框右上角的。

   向Maestro中添加了以下内容：

   * 选定的Workfront对象将添加到链接的记录字段。
   * 将字段添加到链接记录时，将为您选择的每个链接字段创建新的链接字段（或查找字段）。
   * 名为“Workfront对象”的新记录类型将在与链接的Maestro记录相同的工作区中创建。 对象的名称是此记录类型名称的一部分。 例如，链接到Workfront项目会在Maestro中创建Workfront项目记录类型。

     这是只读记录类型，它显示在您从Maestro记录创建的新链接对象字段中选择的Workfront对象。 链接的对象的链接字段也会显示在只读链接的Workfront记录中。

     >[!IMPORTANT]
     >
     > 仅当单个项目添加到Maestro记录时，才会创建只读Workfront对象记录类型。 仅仅在Maestro记录类型和Workfront对象类型之间创建连接不会创建Workfront记录类型。

     Workfront对象字段中的任何现有信息都显示在链接或查找字段中。

     >[!TIP]
     >
     >
     >* 如果启用了“允许多条记录”设置，则多个对象的值要么以逗号分隔，要么根据您选择的聚合器聚合。
     >
     >* 不会为链接的Workfront对象创建指向Maestro链接记录的链接记录字段。


1. （可选）关闭“Maestro记录类型”页面，然后转到您选择的工作区。
1. 单击Workfront对象记录类型的卡片。 例如，单击 **Workfront项目** 信息卡(如果链接到Workfront项目)。 只读Workfront记录类型卡片应在“表”视图中打开。

   >[!NOTE]
   >
   >    * Workfront记录类型页面中列出的记录是只读Workfront对象。 从Workfront记录类型链接的字段也显示为只读列，在Workfront中填充这些字段时，会自动填充这些字段。
   >    * 您不能在Maestro中手动更新Workfront字段。 Workfront对象字段必须在Workfront中填充，并且字段值会自动显示在Maestro的Workfront记录中。
   >
   >    * 要在“时间线”视图中显示Workfront对象记录类型，您必须至少有两个日期字段显示在只读Workfront记录类型页面的“表”视图中。

1. （可选）单击 **更多** 菜单 ![](assets/more-menu.png) 在页面标题中，位于Workfront对象记录类型名称旁边，然后单击 **重命名** 以编辑记录名称。

   >[!NOTE]
   >
   >    您无法从Workfront记录类型页面中删除链接的Workfront记录类型或任何对象。

1. （可选）单击 **添加字段** 图标 ![](assets/add-fields-icon.png) 表视图右上角的Workfront记录类型页面，用于从Workfront记录类型中添加或删除Workfront字段。

   >[!NOTE]
   >
   >  您在Workfront对象记录类型页面中添加或删除的字段不会从链接到Workfront对象类型的Maestro记录类型中添加或删除。 这些字段仅在只读Workfront记录类型页面上可见，因此您可以在Maestro中查看它们。

1. （可选）从“Workfront对象记录类型”页面上的“视图”下拉菜单中，选择“时间轴”视图，以在时间轴视图中显示Workfront链接对象。












