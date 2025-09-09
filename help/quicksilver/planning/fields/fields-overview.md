---
title: 字段概述
description: 您可以在Adobe Workfront Planning中添加反映组织生命周期的新字段。 字段是记录类型的属性。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: a1ad5ada-5010-4dec-934e-a49a3e28aa5f
source-git-commit: 3667359ba2c6ea0aab3ce6845f1a537183f304ec
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 2%

---


# 字段概述

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

您可以在Adobe Workfront Planning中添加反映组织生命周期的新字段。 字段是记录类型的属性。


## 关于Adobe Workfront Planning字段的注意事项

* 您只能从记录类型页面的表视图创建字段。 字段在表格视图中显示为列。 与记录类型关联的所有字段也会显示在记录页面中。

  有关管理表列（或记录字段）的信息，请参阅[管理表视图](/help/quicksilver/planning/views/manage-the-table-view.md)。

  有关管理字段的信息，另请参阅以下文章：

   * [编辑字段设置](/help/quicksilver/planning/fields/edit-fields.md)
   * [删除字段](/help/quicksilver/planning/fields/delete-fields.md)

* 与记录类型关联的字段可用于与该类型的所有记录相关联。<!--will this change and will the fields be available for other record types, too?! Also, the next bullet might need to change too if this one changes -->

* 无法将与记录类型关联的字段添加到其他记录类型。<!-- this will change when they open the Field library tab when creating a field-->

* 您可以通过以下方式手动或自动创建字段：

   * 手动：

      * 在记录类型页面的表视图中添加列时。 表的列是与记录类型关联的字段。 它们是显示在记录页面上的相同字段。

        您无法从记录的页面创建字段。

      * 连接记录类型时。 在两种记录类型之间添加新连接，或者从其它应用程序添加记录类型和对象类型时，可以创建链接记录字段。

        有关连接记录类型的详细信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。

      * 从Workfront导入现有字段时。

        有关信息，请参阅[从Adobe Workfront导入字段](/help/quicksilver/planning/fields/import-fields-from-workfront.md)。


   * 自动：

      * 在创建记录类型时：

         * 名称
         * 描述
         * 开始日期
         * 结束日期
         * 状态。 记录状态的默认值是：
            * 开发
            * 计划
            * 活动
            * 已完成
            * 暂停

        您可以添加更多值或重命名现有值。

      * 从模板创建工作区时。

        有关信息，请参阅[创建工作区](/help/quicksilver/planning/architecture/create-workspaces.md)。

      * 使用Excel或CSV文件导入记录类型时。

        有关详细信息，请参阅[创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)。

* 无法从Workfront访问Workfront Planning字段。

* 只有在将记录类型与Workfront对象类型连接并从Workfront对象添加链接或查找字段时，才能从Workfront Planning访问Workfront字段。 有关信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。

* 如果您拥有工作区的“管理”权限以及该字段所属的记录类型，则可以查看和更新您或任何其他用户创建的字段的设置。

* 一个记录类型最多可以有500个字段。

* 字段名称最多可包含250个字符。

* 删除记录类型或工作区时，与其关联的所有字段以及字段值也会被删除，并且无法恢复。<!-- this might change with a possible recycle bin solution?!-->
* 当您删除属于公式表达式一部分的字段时，公式字段会发生变化。
* 当更改公式表达式并且该公式字段在其他公式字段中被引用时，其他公式也会受到影响。
