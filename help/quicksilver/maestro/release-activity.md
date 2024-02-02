---
title: AdobeMaestro发布活动
description: Adobe大师目前可供选定Workfront客户使用。 请经常阅读本文以了解最近为AdobeMaestro发布的功能。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 53911aa3-74fd-4747-9008-f86a521ffba6
source-git-commit: 16db6e7fedbea7a95e8e0356c523409db1f78199
workflow-type: tm+mt
source-wordcount: '3730'
ht-degree: 0%

---

# AdobeMaestro发布活动

{{maestro-important-intro}}

本文列出了在2023年5月22日Maestro闭门Beta计划启动后已发布的功能。

已发布功能按其发布的顺序列出，最新的功能排在首位。 参与Maestro封闭测试版计划的客户可以访问其生产环境中的所有功能。

>[!IMPORTANT]
>
>在2023年5月至2023年12月期间，本文中的所有功能均已发布到“预览”和“生产”环境。 自2024年1月起，Maestro功能已暂时从预览和沙盒环境中移除。 此日期之后发布的所有功能当前都可在生产环境中使用。

本文列出了自2023年5月22日Maestro封闭测试版计划启动以来发布的功能和修补程序。

这些功能每周发布一次，并按照其发布的顺序列出，最新的顺序列出。 参与Maestro封闭测试版计划的客户可以访问其“预览”和“生产”环境中的所有功能。

>[!IMPORTANT]
>
>在将功能发布到生产环境后的某个时间，将可以使用以下部分中引用的文档。


## 2024年1月29日起一周

### 改进了视图和工作区的共享

生产： 2024年1月30日

预览：待定

我们通过以下增强功能改进了工作区和视图的共享体验：

* 为了进一步明确每个权限级别允许用户执行的操作，我们在共享工作区和视图时添加了每个权限级别的详细信息。

* 您现在可以将链接复制到工作区或查看并与他人共享。 用户必须至少具有工作区或视图的查看权限，才能从复制的链接访问它们。

有关更多信息，请参阅以下文章：

* [共享工作区](/help/quicksilver/maestro/access/share-workspaces.md)
* [共享视图](/help/quicksilver/maestro/access/share-views.md)

### 将缩略图添加到记录

生产： 2024年2月1日

预览：待定

您现在可以向每个记录添加单个缩略图，以便在视图中区分它们。 在表格视图中，您可以添加以前保存在计算机上的图像文件作为缩略图。 缩略图对于每个记录可能是唯一的，并且会同时显示在记录类型页面的表格和时间线视图中。

有关更多信息，请参阅 [将缩略图添加到记录](/help/quicksilver/maestro/records/add-thumbnails-to-records.md).

### 删除连接的记录类型卡片

生产： 2024年2月1日

预览：待定

为避免混淆并简化工作流，我们已从工作区中删除了在将Maestro记录与来自第三方应用程序的对象连接后创建的记录类型卡片。 <!-- Now, when you connect Workfront objects with Maestro records, for example, you can navigate to Workfront to manage the linked objects. You can no longer find the read-only Workfront object record type page in Maestro. This simplifies the number of objects and places you manage information for your objects.  -->

有关更多信息，请参阅 [连接记录](/help/quicksilver/maestro/records/connect-records.md).

## 2024年1月22日起一周

### 新的历史记录部分显示Maestro记录的系统活动

生产： 2024年1月25日

预览：待定

为了提高审核能力，我们在记录的右侧面板中引入了新部分，您可以在其中查看对系统记录的记录所做的更改。

Maestro将在新的“历史记录”部分中记录以下信息：

* 任何字段更改

* 字段的旧值和新值（当值更改时）

* 进行更改的用户的全名

* 更改发生的日期和时间戳。

有关更多信息，请参阅 [“历史记录”部分概述](/help/quicksilver/maestro/records/history-section-overview.md).

### 新记录链接的新标签

生产： 2024年1月25日

预览：待定

为了在创建记录时创建一致性，我们为用于创建记录的“+新建”链接重新添加了“+新记录”标签。  在此更新之前，链接包含记录类型的名称。 现在，在创建操作和分类记录时，可以使用新链接。 有关信息，请参阅 [创建记录](/help/quicksilver/maestro/records/create-records.md).

## 2024年1月8日起一周

### Maestro功能将从预览和沙盒环境中删除

预览和沙盒：2024年1月11日

Maestro区域和所有Maestro功能已暂时从“预览”和“沙盒”环境中删除。 之后，会将Maestro添加到这些环境中，我们将在发行活动说明中介绍该步骤。

### 工作区和视图的Maestro权限

生产： 2024年1月11日

预览：待定

您现在可以将工作区或视图与用户和组共享。 您可以根据用户需要查看或编辑的信息，将其权限设置为不同的级别。

共享工作区时，用户有权访问该空间中的记录类型、记录和字段。

共享工作区时，用户不会收到与工作区的记录类型关联的视图的共享权限。 您必须向视图授予单独的权限。

以下是Maestro工作区的权限级别：

* 查看：用户可以查看与其共享的工作区。 他们还可以从共享工作区查看记录类型和记录。

* 参与：用户可以在与其共享的工作区中创建、编辑或删除记录。  他们无法创建或编辑与其共享的记录类型或工作区。

* 管理：用户可以创建、编辑和删除工作区、记录类型、记录以及与其共享的工作区中的字段。

以下是记录视图的权限级别：

* 视图：用户可以从记录类型页面的“视图”下拉菜单中选择视图。
* 管理：用户可以编辑、共享和删除视图。

有关更多信息，请参阅 [访问概述](/help/quicksilver/maestro/access/access-overview.md) 和 [在Adobe大师中共享权限概述](../maestro/access/sharing-permissions-overview.md).

### 新建公式字段类型

生产： 2024年1月11日

预览：待定

您现在可以向记录类型添加公式类型字段。

公式字段使用记录类型中其他字段的现有值以及指示应如何计算现有值的函数来生成新值。

在公式计算中，不能使用来自链接记录类型的查找字段。 此功能将在以后提供。

有关信息，请参阅 [公式字段概述](/help/quicksilver/maestro/fields/formula-fields.md).

### 在表视图中管理记录时撤消/重做操作

生产： 2024年1月11日

预览：待定

现在，在表视图中执行以下操作时，可以撤消或重做更改：

* 复制/粘贴数据
* 编辑记录
* 添加记录
* 删除记录

您可以使用以下按键来撤消或重做操作：

* 撤消：CTRL/ CMD + Z
* 重做：CTRL/CMD + Shift+Z

有关更多信息，请参阅以下文章：

* [编辑记录](/help/quicksilver/maestro/records/edit-records.md)

* [删除记录](/help/quicksilver/maestro/records/delete-records.md)

* [创建记录](/help/quicksilver/maestro/records/create-records.md)

## 2023年12月25日起一周

### 在时间轴视图中搜索

预览和生产： 2023年12月27日

您现在可以搜索关键字，以便在时间轴视图中快速查找记录。 您可以使用屏幕上可见的任何字段中的关键字和特殊字符来查找记录。 有关信息，请参阅 [管理时间线视图](../maestro/views/manage-the-timeline-view.md).

## 2023年12月18日起一周

### 从“详细信息”页面添加有关记录的注释

适用于所有客户的预览和生产： 2023年12月18日

>[!NOTE]
>
>以下功能将在2024年1月版本的生产中可用：
>
>* 搜索注释
>
>* 复制并粘贴图像
>
>* 拖放图像
>
>有关更多信息，请参阅 [2024年第一季度发行版概述](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).

现在，您可以在详细信息页面中查看记录时，通过添加注释或回复他人来与他人协作处理单个记录。

Maestro记录的注释体验与Workfront对象的新注释体验相匹配。

有关更多信息，请参阅 [管理记录注释](/help/quicksilver/maestro/records/manage-record-comments.md).

### 适用于Adobe Workfront Fusion的Maestro连接器（测试版）

生产： 2023年12月21日

>[!IMPORTANT]
>
>贵组织必须购买Adobe Workfront Fusion才能与Maestro建立连接。
>
>有关信息，请参阅 [Adobe Workfront Fusion概述](/help/quicksilver/workfront-fusion/get-started/workfront-fusion-overview.md).

现在，您可以使用Adobe Workfront Fusion连接到Maestro。 使用新的AdobeMaestro Fusion连接，您可以：

* 创建、读取、更新和删除记录

* 按记录类型获取记录列表

* 删除或获取记录类型列表

* 搜索记录

* 进行API调用

* 在Maestro中进行更改时触发方案

有关更多信息，请参阅 [AdobeMaestro模块](/help/quicksilver/workfront-fusion/apps-and-their-modules/maestro-modules.md).

## 2023年12月11日起一周

### 更新记录类型的表视图中的主字段

预览和生产： 2023年12月14日

现在，您可以选择要显示在Maestro表视图的第一列中的字段。 此字段现在称为主字段。

在此增强功能之前，记录的“名称”字段始终显示在表视图的第一列中，并且无法放置到其他位置。

经过此改进后，请注意以下事项：

* 缺省情况下，“名称”列或字段仍是表的第一列。

* 您可以选择以下任何类型的字段作为主字段，并替换第一列中的“名称”字段：

   * 单行文本

   * 数字

   * 公式

* 表视图的主字段始终冻结，不能移动，除非将其他字段设置为主字段。

* 您可以从非主列标题中更改主字段。

* 记录类型的所有表视图都具有您选择的相同主字段。

有关更多信息，请参阅 [管理表视图](/help/quicksilver/maestro/views/manage-the-table-view.md).


### 将Maestro记录与Adobe Experience Manager Assets连接

预览版本： 2023年12月14日

生产版本： 2023年12月21日

>[!IMPORTANT]
>
>贵组织的Workfront实例必须载入到Adobe业务平台或Adobe Admin Console，才能将Maestro记录连接到Adobe Experience Manager Assets。
>
>如果您对入门Adobe Admin Console有任何疑问，请参阅 [Adobe统一Experience常见问题解答](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).


现在，您可以在Maestro记录类型与Adobe Experience Manager Assets之间建立连接。

建立连接后，以下功能可用于此更新：

* 您可以将Experience Manager资源和文件夹从Experience Manager Assets中他们有权访问的特定存储库链接到Maestro记录。 在此过程中，您可以将资源字段连接到Maestro字段。

* Maestro用户可以查看Maestro中连接的资产的名称以及连接字段的值

<!--removed per PM, for now: 
* An Experience Manager Assets record type is automatically created in Maestro after you establish the connection. Connected assets are visible in the Maestro table and timeline views of this new record type.  
-->

* 您可以在Maestro记录的“已连接”记录字段中单击表格视图中的资产名称，并查看包含资产缩略图和多个关键字段的弹出窗口。 从弹出窗口中，您可以导航到Experience Manager中的资源查看器，并查看有关该查看器的所有详细信息。

有关更多信息，请参阅 [连接记录类型](/help/quicksilver/maestro/architecture/connect-record-types.md).

## 2023年12月4日起一周

### 在Maestro表视图中，为“人员类型”和链接记录字段将信息从一个字段复制并粘贴到另一个字段

预览和生产： 2023年12月5日

现在，您可以在Maestro记录类型表格视图中将一个字段中的信息复制并粘贴到另一个相同类型的字段。 以下类型的字段现在支持此功能：

* 人员
* 链接的记录字段

请考虑以下事项：

* 显示多个值的字段支持将字段值从一个字段复制和粘贴到另一个字段。

* 不能从其他源复制信息，不能从与粘贴信息的字段类型相同的Maestro字段复制。

* 您无法复制和粘贴在记录的“详细信息”区域中显示的字段的字段值。

有关更多信息，请参阅 [编辑记录](../maestro/records/edit-records.md).

有关链接字段的信息，请参阅 [连接记录类型](../maestro/architecture/connect-record-types.md).

## 2023年11月27日起一周

### 在Maestro表视图中将信息从一个字段复制并粘贴到另一个字段

预览和生产： 2023年11月28日

现在，您可以在Maestro记录类型表格视图中将一个字段中的信息复制并粘贴到另一个相同类型的字段。

请考虑以下事项：

* 不能从其他源复制信息，不能从与粘贴信息的字段类型相同的Maestro字段复制。

* 您无法复制和粘贴在记录的“详细信息”区域中显示的字段的字段值。

* 不能复制和粘贴以下字段类型的字段值：

   * 人员

   * 系统字段

   * 因连接记录而创建的链接字段

有关更多信息，请参阅 [编辑记录](../maestro/records/edit-records.md).

## 2023年11月6日起一周

### 表格视图的分组

预览和生产： 2023年11月7日

您现在可以在记录类型页面的表视图中分组记录。 您可以在Maestro界面中按三个唯一字段分组 <!--checking into this for now: and by four fields when using the API-->.

有关更多信息，请参阅 [管理表视图](../maestro/views/manage-the-table-view.md).

## 2023年10月30日起一周

### 新的用户字段类型和日期字段，用于捕获记录创建或上次修改者或日期

预览和生产： 2023年10月30日

我们为Maestro记录引入了以下字段类型：

* 创建者

* 创建日期

* 上次修改者

* 上次修改日期

根据这些字段类型创建的字段的字段值为只读，可捕获创建或上次修改记录的用户的名称，或创建或上次修改记录的日期。

有关更多信息，请参阅 [创建字段](../maestro/fields/create-fields.md).

### 从Maestro记录导航到Workfront对象

预览和生产： 2023年10月31日

现在，您可以从Maestro中的以下区域打开Workfront对象页面：

* 只读链接Workfront对象记录表视图

* 只读Workfront对象记录详细信息页面

有关更多信息，请参阅 [连接记录](../maestro/records/connect-records.md).

### 改进了表视图中的导航

预览和生产： 2023年11月2日

我们改进了记录类型页面的表视图中的导航。

以下是一些改进：

* 使用键盘上的Tab键浏览表的列和行

* 从任何列位置添加新记录。 在此改进之前，您只能从第一列添加记录。

* 使用Shift + Enter键盘组合在表中添加新记录（或行）。

有关更多信息，请参阅 [创建记录](../maestro/records/connect-records.md).

## 2023年10月16日起一周

### 新建人员字段类型

预览和生产： 2023年10月16日

您现在可以向Maestro记录类型添加人员类型字段。 您可以使用“人员”类型字段将现有用户与记录关联。 有关信息，请参阅 [创建字段](../maestro/fields/create-fields.md).

### 富文本 — 段落字段的格式

预览和生产： 2023年10月16日

我们为段落类型字段添加了富文本格式控件。 您可以在记录类型的“表”视图中或在记录的“详细信息”页中使用富文本设置段落字段的格式。 有关更多信息，请参阅 [编辑记录](../maestro/records/edit-records.md).


### 时间轴视图的记录并分组颜色编码

预览和生产： 2023年10月19日

您现在可以对时间轴视图中的记录栏和分组进行颜色编码。

下面是您可以选择在“时间轴”视图中显示的记录条和分组的颜色选项：

* 分组可以匹配以下颜色：

   * 灰色（默认）

   * 分组依据的字段的颜色

* 条形可以与以下颜色匹配：

   * 记录类型的颜色

   * 所选字段的颜色

   * 分组的颜色

   * 无颜色（默认）

将颜色与特定字段匹配时，您只能选择具有颜色编码选项的字段。

有关更多信息，请参阅 [管理时间线视图](../maestro/views/manage-the-timeline-view.md).

## 2023年10月9日起一周

### 在表格视图中搜索

预览和生产： 2023年10月9日

您现在可以搜索关键字，以便在表格视图中快速查找记录。 您可以使用屏幕上可见的任何字段中的关键字和特殊字符来查找记录。 有关信息，请参阅 [管理表视图](../maestro/views/manage-the-table-view.md).

## 2023年9月18日起一周

### 重新排列行

预览和生产： 2023年9月20日

现在，您可以在记录类型页面的“表”视图中重新排列一个或多个行（或记录）。 有关信息，请参阅 [管理表视图](../maestro/views/manage-the-table-view.md).

## 2023年9月4日起一周

### 将Maestro记录与Workfront公司和组连接起来

预览和生产： 2023年9月5日

您现在可以将Maestro记录与Workfront公司和集团连接起来。 您必须首先在Maestro记录类型与Workfront公司和组对象类型之间创建连接。 然后，您可以将所选记录类型的单个Maestro记录连接到单独的Workfront公司和组。

请考虑以下事项：

* 必须在每个Workspace的Maestro记录类型与Workfront公司和组对象类型之间创建连接。

* 您无法将分类记录类型与Workfront对象类型连接。

* 您可以将多个Maestro记录连接到同一个Workfront公司或组，将多个公司或组连接到同一个Maestro记录。

* 您不能在Maestro中编辑公司或组。 在查看Maestro链接记录时，在Workfront中执行的所有公司或组更改都将显示在Maestro中。

  有关更多信息，请参阅以下文章：

   * [连接记录类型](../maestro/architecture/connect-record-types.md)
   * [连接记录](../maestro/records/connect-records.md)

### 单行文本字段支持URL

预览和生产： 2023年9月7日

为了在表格视图中使用链接时提高可见性，我们在单行文本字段中增加了对URL的支持。 在更新单行文本字段时使用指向其他网站或外部驱动器的URL，现在可将其标识为链接，并允许您从表中单击它们。 在此增强功能之前，链接显示为文本。

## 2023年8月28日起一周

### 表格视图工具栏的字段可见性菜单

预览和生产： 2023年8月31日

要显示关于给定记录集的正确信息，特别是如果您要与必须查看某个记录类型的某些而非所有字段的其他人共享视图，您现在可以选择显示哪些字段（或列）以及隐藏哪些字段或列。

您可以从字段列的每个标题中隐藏或显示单个字段，也可以从表格视图工具栏中的设置管理记录类型的所有字段。

有关更多信息，请参阅 [管理表视图](../maestro/views/manage-the-table-view.md).

## 2023年8月21日起一周

### 将Maestro记录连接到项目和项目组合

预览和生产： 2023年8月24日

您现在可以将Maestro记录与Workfront项目和项目组合连接。 您必须在Maestro记录类型与创建连接字段的程序或项目组合之间创建连接。 然后，您可以将同一工作区中所有其它记录类型的任何Maestro记录连接到特定程序和项目组合，这些程序和项目组合在同一工作区中创建只读Workfront程序或WorkfrontPortfolio记录类型。 请考虑以下事项：

* Workfront连接器记录类型对于每个工作区都是唯一的。
* 您可以将多个Maestro记录连接到同一个Workfront项目或组合，将多个项目和组合连接到同一个Maestro记录。
* 您不能在Maestro中编辑项目和项目组合。 查看链接记录时，在Workfront中执行的所有项目和项目组合更改在Maestro中均可见。

### 表格视图的新排序功能

预览和生产： 2023年8月24日

您现在可以对记录类型页面的表视图中的记录进行排序。
以下功能现已可用：

* 在表级别排序，您可以同时按多个字段排序。
* 在列或字段级别排序，您可以一次按单个字段排序。

### 改进了时间轴视图：新增了分组和紧凑/标准视图切换的外观

预览和生产： 2023年8月24日

我们对时间线视图进行了以下改进：

* 现在，您可以按照以下模式显示时间轴视图：

   * 标准：以单独的行显示记录。
   * 紧凑：在同一行中显示其日期不相交的记录。

* 我们更改了时间轴视图中分组行的外观，以显示在它们包含记录的时间轴上方。 在此改进之前，在时间线的整个长度上显示分组线。

## 2023年8月14日起一周

### 重新排序表视图中的列

您现在可以在Maestro表视图中重新排列列。 重新排序列时，请考虑以下事项：

* “名称”字段始终是记录类型页面的表视图中的第一个字段

* 不能将“名称”字段移动到其他位置

* “名称”字段已冻结，不是水平滚动的一部分。

### 时间轴视图的水平滚动

您现在可以在记录类型的时间轴视图中水平滚动。

## 2023年8月7日起一周

### 从Excel文件导入记录类型

预览和生产： 2023年8月10日

您现在可以导入Excel文件以在工作区中创建记录类型。 文件工作表成为记录类型，文件列成为各自的字段。

### 改进了连接记录类型和项目的体验

预览和生产： 2023年8月10日

我们改进了您连接记录类型的方式，包括连接到Workfront项目。 作为此改进的一部分，我们在从表视图为记录类型添加字段时进行了以下更改：

* 从“New field”选项卡中删除了Relationship-type字段。

* 添加“新连接”选项卡，您可以在此处直接选择要连接的记录或对象类型，而无需使用“关系类型”字段。

## 2023年7月10日起一周

### 更新记录类型的外观

预览和生产： 2023年7月13日

您现在可以为记录类型选择自定义图标，并为记录类型图标选择自定义颜色。

### 新建复选框字段类型

预览和生产： 2023年7月13日

您现在可以向Maestro记录类型添加复选框字段类型。 您可以使用Checkbox-type字段将单个复选框选项添加到记录。 您可以使用此字段指明特定记录的特定属性或状态。 例如，您可以将其用作跟踪每个记录的完成、批准或任何其他二进制属性的标志。

## 2023年6月26日起一周

### 快速激活表中的上下文菜单

预览和生产： 2023年6月28日

我们启用了在查看表视图或记录类型中的记录时，通过右键单击记录行中的任何位置来激活上下文菜单的功能。 现在，当您从记录类型的表视图中的任意位置访问上下文菜单时，可以快速查看、删除或复制指向记录的“详细信息”页面的链接。 在此增强功能之前，上下文菜单只能从记录的“名称”列中的更多菜单访问。

## 2023年6月19日起一周

### 记录字段名称是唯一的

现在，我们引入了一项要求，要求Maestro记录类型的字段名称应具有唯一名称。 属于不同记录类型的字段不必具有唯一名称。

## 2023年6月5日起一周

### 将Maestro记录连接到Workfront项目

预览和生产： 2023年6月5日

您现在可以将Maestro记录连接到Workfront项目。 您必须创建连接器Maestro记录类型，以在Maestro记录与Workfront项目之间建立连接。 然后，可以使用“关系”字段将任何其他记录类型的任何Maestro记录连接到连接器记录。 请考虑以下事项：

* 每个工作区都必须具有Workfront的连接器记录类型。
* 您可以将多个Maestro记录连接到同一个Workfront项目，将多个项目连接到同一个Maestro记录。
* 无法在Maestro中编辑项目。 查看链接记录时，在Workfront中执行的所有项目更改在Maestro中均可见。

## 2023年5月29日起一周

### 创建时间线视图的两日期要求

预览和生产： 2023年5月31日

您必须至少具有两个与记录类型关联的日期字段才能创建时间线视图。
