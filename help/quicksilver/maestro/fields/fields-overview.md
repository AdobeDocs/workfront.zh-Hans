---
title: 字段概述
description: 您可以在AdobeMaestro中添加反映组织生命周期的新字段。 字段是记录类型的属性。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: a1ad5ada-5010-4dec-934e-a49a3e28aa5f
source-git-commit: ce015eba8291995eec1611917896a0e797f820cc
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 1%

---

# 字段概述

<!--
title: Field overview
description: You can add new fields in Adobe Maestro that reflect your organization's lifecycle. Fields are attributes of record types. 
hidefromtoc: yes
author: Alina
feature: Work Management (***************WE NEED A NEW ONE HERE***********)
role: User, Admin
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

>[!IMPORTANT]
>
>本文中的信息是指AdobeMaestro，它是Adobe Workfront提供的新产品。
>
>目前，AdobeMaestro是测试版计划的一部分，该计划对有限数量的客户开放。 您必须是Workfront客户才能使用Maestro功能。
>
>有关加入Maestro测试版计划的更多信息，请与您的客户代表联系。
>
>有关信息，请参阅 [Adobe大师概述](../maestro-overview.md).

您可以在AdobeMaestro中添加反映组织生命周期的新字段。 字段是记录类型的属性。


## 有关Maestro字段的注意事项

* 您只能从记录类型页面的表视图创建字段。 字段在表格视图中显示为列。 与记录类型关联的所有字段也会显示在该类型每个记录的“详细信息”页面中。

  有关管理表列（或记录字段）的信息，请参见 [管理表视图](../views/manage-the-table-view.md).

  有关管理字段的信息，另请参阅以下文章：

   * [编辑字段](../fields/edit-fields.md)
   * [删除字段](../fields/delete-fields.md)

* 与记录类型关联的字段可用于与该类型的所有记录相关联。 <!--will this change and will the fields be available for other record types, too?! Also, the next bullet might need to change too if this one changes -->

* 无法将与记录类型关联的字段添加到其他记录类型。 <!-- this will change when they open the Field library tab when creating a field-->

* 您可以通过以下方式手动或自动创建字段：

   * 手动：

      * 通过在记录类型页面的表视图中添加列。 表的列是与记录类型关联的字段。 这些是在记录的“详细信息”页面上显示的相同字段。

        不能从记录的详细信息页面创建字段。

        本文介绍了如何手动创建字段。

      * 连接记录类型。 在两个Maestro记录类型之间添加新的连接时，或者从其它应用程序添加记录类型和对象类型时，您可以创建链接记录字段。

        <!--* Importing record types with fields using a CSV or an Excel file. - this is not available yet-->

        有关连接Maestro记录类型的详细信息，请参见 [连接记录类型](../architecture/connect-record-types.md).

      * 通过使用Excel或CSV文件导入记录类型。 有关更多信息，请参阅 [创建记录类型](../architecture/create-record-types.md).

   * 自动：

      * 默认情况下，每次创建记录类型时。

        以下是默认为每个新操作记录类型创建的标准字段：

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

        以下是默认情况下，为每个新分类记录类型创建的标准字段：

         * 名称 <!--will more be added? If not, consider rephrasing this bullet-->

      * 从模板创建工作区时。 从模板创建工作区时，Maestro会为操作记录类型和分类创建字段。 有关信息，请参阅 [创建工作区](../architecture/create-workspaces.md).

* 无法从Workfront访问Maestro字段。

* 仅当您将Workfront记录类型与Workfront对象类型连接并添加来自Workfront对象的链接或查找字段时，才能从Maestro访问字段。 有关信息，请参阅 [连接记录类型](../architecture/connect-record-types.md).

* 如果您对字段所属的工作区具有“管理”权限，则可以查看和更新您或任何其他用户创建的字段的设置。

* 一个记录类型最多可以有500个字段。

* 字段名称最多可包含250个字符。

* 删除操作记录类型、分类或工作区时，与它们关联的所有字段以及字段的值也会被删除，并且无法恢复。 <!-- this might change with a possible recycle bin solution?!-->
