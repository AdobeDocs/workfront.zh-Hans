---
title: 连接记录类型和记录的示例
description: 本文介绍了如何在AdobeMaestro记录类型与Workfront项目对象类型之间创建连接的示例。 它还介绍了如何将Maestro记录与连接到单个项目。
hidefromtoc: true
hide: true
source-git-commit: f058c369bdb3b991910d3a820895de73ea4709f0
workflow-type: tm+mt
source-wordcount: '1742'
ht-degree: 0%

---


# 连接记录类型和记录的示例

>[!IMPORTANT]
>
>目前，AdobeMaestro是测试版计划的一部分，该计划对有限数量的客户开放。
>
>有关加入Maestro测试版计划的更多信息，请与您的客户代表联系。
>
>有关信息，请参阅 [Adobe大师概述](../maestro-overview.md).

本文描述了以下示例：

* 如何创建两个Maestro记录类型与两个Maestro记录之间的连接。

* 如何在AdobeMaestro记录类型与Workfront项目对象类型之间创建连接，以及在Maestro记录与项目之间创建连接。

有关更多信息，另请参阅以下文章：

* [连接记录类型](../architecture-and-fields/connect-record-types.md)
* [连接记录](../records/connect-records.md)

## 连接两个Maestro记录类型和记录（示例）

例如，您有一个名为Campaign的记录类型作为原始记录类型。

您还有另一种记录类型，称为Product，它有一个货币字段，称为Budget。

您要创建一个记录类型“促销活动”的字段，以便显示记录类型“产品”中“预算”字段的值。

为此，请执行以下操作：

1. 打开营销活动记录类型的表视图。
1. 单击 **+** 图标来添加新字段，然后单击 **新建连接**.
1. 添加以下信息，例如：

   * **记录类型**：产品 <!--did they change the casing here?-->
   * **名称**：产品信息。 这是链接的记录字段的名称。
   * **描述**：这些是我希望与我的营销活动关联的产品。
   * **允许多条记录**：如果保留选中此选项，则在原始记录（营销活动）上显示链接的记录类型字段（产品信息）时，允许用户选择多个记录。 在本例中，他们能够选择要连接到一个营销活动的多个产品。
   * **选择查找字段**：如果您保留选中此选项，则 **添加查找字段** 框，以允许您链接产品字段与促销活动记录类型。 您可以跳过此步骤，稍后再添加产品字段。

   ![](assets/new-connection-with-product-record-type.png)

1. （视情况而定）如果您选择 **选择查找字段选项** 在上一步中，从与 **产品** 记录类型，请单击 **+** 图标 **预算** 字段，然后单击 **添加字段**. 这将创建一个名为的字段 **预算（来自产品信息）**，即链接字段的名称。 产品预算的任何信息都将显示在此字段中以供Campaign记录使用。

   ![](assets/add-fields-for-budget-field-for-connector-with-record-type.png)

   >[!TIP]
   >
   >    如果要将所有选定产品的预算作为一个总数查看，请选择 **SUM** 字段名称右侧的下拉菜单中。 当用户在 **产品信息** 链接的记录字段， **预算（来自产品信息）** 字段将其所有预算值相加并显示总计。 <!-- check the shot below - added a bug with a couple of UI changes here-->
   >
   > 如果您选择 **无**，而不是 **SUM**&#x200B;中，个别预算将以逗号分隔。

   这将生成以下字段：

   * 在Campaign记录表视图和营销活动的“详细信息”页面中：

      * **产品信息** （链接的记录字段）：这将显示产品的名称或名称。
      * **预算（来自产品信息）** （链接字段）：这将显示在产品信息字段中选择的产品的预算。

   * 在“产品记录”表格视图和产品的“详细信息”页面中：

      * **营销活动**：这表示产品记录类型链接自Campaign记录类型。

     ![](assets/example-campaign-information-relationship-fields-from-product-record-table.png)

   >[!TIP]
   >
   >    链接的记录字段前面有关系图标 ![](assets/relationship-field-icon.png).

1. 要填充 **产品信息** 字段，从 **营销活动** 记录类型表视图，通过在“促销活动”记录类型页面的表中添加新行来创建促销活动。
1. 单击 **+** 中的图标  **产品信息** 列来显示新营销活动。 此 **连接对象** 框显示。 要链接到的记录类型（产品）的名称将显示在框的左上角。

   ![](assets/connect-objects-box-to-select-other-maestro-records-example-for-product-record.png)

1. 选择要与Campaign记录连接的产品记录，然后单击 **连接对象**.

   以下列在Campaign记录类型表中填充：
   * 此 **产品信息** 字段将填充所选产品的促销活动记录。
   * **预算（来自产品信息）** 使用每个所选产品的预算值或所选产品的所有预算的总计填充字段。

   ![](assets/example-product-information-and-budget-relationship-fields-for-campaign-record-table.png)

   >[!TIP]
   >
   >如果不为多个值选择聚合器，则所有值将以逗号分隔。

1. 要填充 **营销活动** 中的字段 **产品** 表格视图，从“产品记录类型”表格视图开始重复步骤5-7并选择促销活动信息。 这还将更新Campaign记录类型页面表格中的Product information字段。 <!--ensure the step numbers remain correct-->


## 将Maestro记录类型与Workfront项目对象类型连接，并将记录与单个项目连接

例如，您有一个名为Campaign的记录类型作为原始记录类型。

您在Workfront中还有名为“计划收入”的项目。

您想对活动的记录类型创建一个连接字段，以便在Workfront中显示特定活动的项目上计划收入字段的值。

为此，请执行以下操作：

1. 转到要将Campaign记录类型与Workfront项目连接的工作区。
1. 在所选工作区中打开Campaign记录类型的表视图。
1. 单击 **+** 图标来添加新字段，然后单击 **新建连接**.
1. 添加以下信息，例如：

   * **记录类型**：Workfront项目(来自Workfront子部分) <!--did they change the casing here for the field label and did they take "Workfront" out of the name of the object?-->
   * **名称**：项目信息。 这是链接对象字段的名称。
   * **描述**：这些是我希望与营销活动关联的项目。
   * 
      * **允许多条记录**：如果保留选中此选项，则当用户将链接对象类型字段（项目信息）显示在原始记录（营销活动）上时，用户可以选择多个对象。
   * **选择查找字段**：如果您保留选中此选项，则 **添加查找字段** 框打开，允许您链接具有Campaign记录类型的项目字段。 您可以跳过此步骤，稍后添加项目字段。

   ![](assets/new-connection-tab-with-workfront-option.png)

1. （视情况而定）如果您选择 **选择查找字段选项** 在上一步中，从与 **项目** 对象类型，单击 **+** 图标 **计划收入** 字段，然后单击 **添加字段**. 这将创建一个名为的字段 **计划收入（来自项目信息）**，即链接字段的名称。 “项目收入”字段中的任何信息均会在此字段中显示促销活动记录。

   >[!TIP]
   >
   >    如果要将所有选定项目的计划收入查看为一个总数，请选择 **SUM** 字段名称右侧的下拉菜单中。 当用户在 **项目信息** 链接对象字段， **计划收入（来自产品信息）** 字段将其所有值相加并显示总计。 <!-- check the shot below - added a bug with a couple of UI changes here-->
   >
   > 如果您选择 **无**，而不是 **SUM**，则各个计划收入以逗号分隔。

   ![](assets/add-planned-revenue-project-field-to-new-connection.png)

   这将生成以下字段：

   * 在Campaign记录表视图和营销活动的“详细信息”页面中：

      * **项目信息** （链接对象字段）：这将显示项目的名称或名称。
      * **计划收入（来自项目信息）** （链接的字段）：这将显示在项目信息字段中选择的项目计划收入。

   >[!TIP]
   >
   >    链接对象字段前面有关系图标 ![](assets/relationship-field-icon.png).

1. 要填充 **项目信息** 字段，从 **营销活动** 记录类型表视图，通过在表中添加新行来创建营销活动。
1. 单击 **+** 中的图标  **项目信息** 列来显示新营销活动。 此 **连接对象** 框显示。 要链接到的对象类型(Workfront项目)的名称将显示在框的左上角。

   ![](assets/connect-objects-box-to-select-projects.png)

1. 选择要与Campaign记录连接的一个或多个项目，然后单击 **连接对象**.

   以下内容将添加到所选工作区：

   * 在Campaign记录类型表中：
      * 此 **项目信息** 字段将填充所选项目的营销活动记录。
      * 此 **计划收入（来自产品信息）** 字段用每个所选产品的预算值填充。 这是只读字段。

   ![](assets/project-linked-field-and-planned-revenue-in-campaign-table-highlighted.png)

   >[!TIP]
   >
   >如果不为多个值选择聚合器，并在对象链接字段中选择多个对象，则所有值将以逗号分隔。

   * 所选工作区的只读Workfront项目记录类型。

1. 单击页面标题中记录名称左侧的后指箭头，以转到要更新的工作区。
1. 打开 **Workfront项目** 记录类型卡以打开记录类型页面。

   请注意以下有关Workfront项目记录类型页面的信息：

   * 这是只读的Maestro记录类型，不能删除或更新。
   * 您选择连接到营销活动的项目在Workfront项目记录类型页面中显示为单独的记录。 项目记录也是只读的，当项目在Workfront中更新时，其信息会自动更新。 您必须从所连接的Maestro记录添加更多项目，以便在Workfront项目记录类型中查看它们。
   * 营销活动链接的记录字段使用从营销活动记录类型页面连接到项目的营销活动名称进行填充。

1. （可选）单击 **更多** 图标 ![](assets/more-menu.png) Workfront项目记录类型名称的右侧，然后单击 **重命名** 以重命名记录类型。

   >[!TIP]
   >
   >您可以通过单击记录类型标题中的名称来重命名记录类型名称。

1. 单击添加字段图标 ![](assets/add-fields-icon.png) 将更多项目字段添加到WorkfrontWorkfront项目经理记录类型中。
1. 单击 **+** 图标，以将其添加到中的Workfront项目经理记录 **未选择的字段** 部分。
1. 单击 **-** 图标来显示要从Workfront项目经理记录中移除的任何项目字段。 **选定的字段** 部分。
1. 单击&#x200B;**保存**。

   >[!TIP]
   >
   >    您添加到Workfront项目Maestro记录的字段仅添加到“Workfront项目”页面上，并未添加到“Campaign记录类型”页面，如链接字段。 您必须从营销活动记录类型的项目信息连接对象字段添加项目字段，才能查看营销活动。

1. （可选且视情况而定）如果您选择为项目显示至少两个日期字段，请单击 **视图** Workfront项目记录类型表中的下拉菜单，然后 **创建视图** > **时间线** > **创建** 以创建时间线视图并在时间线中显示项目。



