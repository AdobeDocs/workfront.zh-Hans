---
title: 连接的记录类型概述
description: 指示各个记录类型如何相互关联的一种方法是连接它们。 此外，您可以将Adobe Workfront Planning记录类型与其他应用程序中的对象类型连接起来，以增强用户体验并将它们的焦点集中在一个应用程序中。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: d56a4721353f8b7db856eab5a3ae3b53396bd079
workflow-type: tm+mt
source-wordcount: '1086'
ht-degree: 1%

---


<!--update metadata at GA-->
<!--add mini TOC when live, already added to big TOC to get the link-->

# 连接的记录类型概述

<!--REMOVE THE CONTENT BELOW FROM THE "CONNECT RECORD TYPES" ARTICLE WHEN YOU TURN THIS ARTICLE LIVE- THIS IS THE SAME CONTENT AS THERE, DUPLICATED-->

通过连接各个记录类型可以指出它们彼此相关，或与来自其他应用程序的对象相关。

本文概述了记录类型连接，并介绍了您可以在记录类型和对象类型之间建立连接的类型。

有关您连接记录类型的信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。

## 有关连接记录类型的注意事项

* 您可以在Adobe Workfront Planning中连接以下实体：

   * 两种记录类型。

     默认情况下，您可以从同一工作区连接两种记录类型。 您还可以设置记录类型以与其他工作区的记录类型连接。
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

     例如，如果将“Campaign”记录类型与“Product”记录类型连接，则会在Campaign记录类型上创建名为“链接的产品”的链接记录字段。 在产品记录类型上创建一个自动命名为“Campaign”的链接记录类型。

   * **当您将记录类型与另一个应用程序的对象类型连接时**：

      * 链接记录字段是在您连接的记录类型上创建的。 不会在其他应用程序的对象类型上自动创建链接记录字段。

      * 无法从Workfront对象访问Planning记录字段。
      * 当Workfront管理员通过Workfront与Adobe Experience Manager Assets之间的集成配置Experience Manager映射时，可从Metadata Assets访问规划记录字段。 有关详细信息，请参阅[配置Adobe Workfront和Experience Manager Assets之间的资源元数据映射](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en)。

   * **当您从连接到的记录或对象添加链接（或查找）字段时**：除了创建链接记录字段之外，您还可以从连接的记录或对象类型连接到称为查找字段的字段。 链接（或查找字段）包含所连接记录中的信息，该信息显示在您连接的记录中。

     您可以将其他记录类型或其他应用程序对象中的字段连接到Workfront Planning记录类型。

     链接字段是只读的，当您连接记录或对象时，它们会自动显示连接记录或对象中的信息。

     您可以在公式、筛选器或分组中引用来自其他记录或对象类型的查找字段。

     例如，如果您将“促销活动”记录类型与Workfront项目连接并选择将该项目的“计划完成日期”字段引入Workfront计划记录，则将自动为促销活动创建一个名为“计划完成日期”（来自项目）的链接字段。 您无法手动编辑此链接的字段。 计划完成日期（来自项目）字段显示链接项目的计划完成日期。

     >[!IMPORTANT]
     >
     >对工作区具有“查看”权限或更高权限的所有人都可以查看查找字段中的信息，无论他们在链接对象类型<!--or their permissions in other workspaces-->的应用程序中的权限或访问级别如何。

<!--see the commented out text above for the release of cross-workspace connections-->

* 链接的记录字段前面有关系图标![](assets/relationship-field-icon.png)。

  链接的字段前面有标识该字段类型的图标。 例如，链接（或查找）字段前面有图标，指示字段是数字、段落或日期。


## 连接类型

在两个记录类型之间或在记录与来自另一个应用程序的对象类型之间建立连接后，可以在连接的记录字段中添加记录。

根据可添加到已连接记录字段中的记录数，在连接记录类型时可以选择以下连接类型：

* [一对多](#one-to-many-connection-type)
* [一对一](#many-to-one-connection-type)
* [多对一](#many-to-one-connection-type)
* [多对多](#many-to-many-connection-type)

>[!WARNING]
>
>在连接以下内容时，这些选项不可用：
>* 来自不同工作区的两个记录
>
>* 记录类型和AEM资源


<!-- add screen shots for each type of connection below-->

### 一对多连接类型

![](assets/one-to-many-connection-picker.png)

在记录类型之间选择一对多连接类型时，您可以稍后将一个记录与要连接的多个记录连接。

例如，如果将营销活动与项目关联，则可以将一个营销活动与多个项目关联。 但一个项目只能连接到一个营销策划。

选择此连接类型后，可以将其更改为多对多连接类型。

### 一对一连接类型

![](assets/one-to-one-connection-picker.png)

在记录类型之间选择一对一的连接类型时，您以后可以将一个记录与您正在连接的其他记录连接。

例如，如果将营销活动与项目关联，则可以将一个营销活动与一个项目关联。 一个项目只能连接到一个营销策划。

选择此连接类型后，可将其更改为任何其他连接类型。

### 多对一连接类型

![](assets/many-to-one-connection-picker.png)

在记录类型之间选择多对一连接类型时，以后可以只连接一条记录的多个记录。

例如，如果将营销活动与项目关联，则可以将多个营销活动与一个项目关联。 一个项目可以连接到多个营销策划。

选择此连接类型后，可以将其更改为多对多连接类型。

### 多对多连接类型

![](assets/many-to-many-connection-picker.png)

在记录类型之间选择多对多连接类型时，您可以稍后将多个记录与要连接的多个记录连接起来。

例如，如果将营销活动与项目关联，则可以将多个营销活动与多个项目关联。 您还可以将多个项目连接到多个营销策划。

如果选择此连接类型，则在保存后无法更改连接类型。

