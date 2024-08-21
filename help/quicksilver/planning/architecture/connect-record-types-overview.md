---
title: 连接的记录类型概述
description: 指示各个记录类型如何相互关联的一种方法是连接它们。 此外，您可以将Adobe Workfront Planning记录类型与其他应用程序中的对象类型连接起来，以增强用户体验并将它们的焦点集中在一个应用程序中。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 1ad86cd55459d92650ac7a24c41765e579f8bb94
workflow-type: tm+mt
source-wordcount: '830'
ht-degree: 0%

---


<!--update metadata at GA-->
<!--add mini TOC when live, already added to big TOC to get the link-->

# 连接的记录类型概述

<!--REMOVE THE CONTENT BELOW FROM THE "CONNECT RECORD TYPES" ARTICLE WHEN YOU TURN THIS ARTICLE LIVE- THIS IS THE SAME CONTENT AS THERE, DUPLICATED-->

通过连接各个记录类型可以指出它们彼此相关，或与来自其他应用程序的对象相关。

本文概述了记录类型连接，并介绍了您可以在记录类型和对象类型之间建立连接的类型。

有关您连接记录类型的信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。

## 有关连接记录类型的注意事项

在Workfront Planning中连接需执行以下两个步骤：

1. 首先，必须在两个记录类型或记录类型与来自另一个应用程序的对象类型之间建立连接。 有关如何连接记录类型的信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。
1. 其次，在连接一种类型的单个记录与另一种类型的记录之后，可以连接这两种记录类型。 有关连接记录的信息，请参阅[连接记录](/help/quicksilver/planning/records/connect-records.md)。

有关连接记录类型，请考虑以下事项：

* 您可以在Adobe Workfront Planning中连接以下实体：

   * 两种记录类型。

     默认情况下，您可以从同一工作区连接两种记录类型。 您还可以设置记录类型以与其他工作区的记录类型连接。 有关信息，请参阅[编辑记录类型](/help/quicksilver/planning/architecture/edit-record-types.md)。
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

* 为连接的记录类型创建记录后，可通过“连接的记录”字段将它们链接在一起。  有关信息，请参阅[连接记录](/help/quicksilver/planning/records/connect-records.md)。

* 将记录类型与另一个记录类型或另一个应用程序中的对象类型连接后，将出现以下情况：

   * **当您连接两个Planning记录类型时**：在您要连接的记录类型上创建一个链接记录字段。 在要连接的记录类型上创建类似的链接记录字段。

     例如，如果将“Campaign”记录类型与“Product”记录类型连接，则会在Campaign记录类型上创建名为“链接的产品”的链接记录字段（连接字段）。 在产品记录类型上创建一个自动命名为“Campaign”的链接记录类型。

   * **当您将记录类型与另一个应用程序的对象类型连接时**：

      * 链接记录字段是在您连接的记录类型上创建的。 不会在其他应用程序的对象类型上自动创建链接记录字段。
      * 无法从Workfront对象访问Planning记录字段。
      * 当Workfront管理员通过Workfront与Adobe Experience Manager Assets之间的集成配置Experience Manager映射时，可从Metadata Assets访问规划记录字段。 有关详细信息，请参阅[配置Adobe Workfront和Experience Manager Assets之间的资源元数据映射](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en)。
      * Planning记录在Workfront对象的Planning选项卡中可见。 有关信息，请参阅Adobe Workfront对象的“规划”部分中的[管理记录](/help/quicksilver/planning/records/manage-records-in-planning-section.md)。

   * **从您连接的记录或对象添加查找字段时**：除了创建链接记录字段外，您还可以从连接的记录或对象类型连接到称为查找字段的字段。 链接（或查找字段）包含所连接记录中的信息，该信息显示在您连接的记录中。

     您可以将其他记录类型或其他应用程序对象中的字段连接到Workfront Planning记录类型。

     链接字段为只读，它们自动显示已连接记录的信息。

     您可以在公式、筛选器或分组中引用来自其他记录或对象类型的查找字段。

     例如，如果您将“促销活动”记录类型与Workfront项目连接并选择将该项目的“计划完成日期”字段引入Workfront计划记录，则将自动为促销活动创建一个名为“计划完成日期”（来自项目）的链接字段。 您无法手动编辑此链接的字段。 计划完成日期（来自项目）字段显示链接项目的计划完成日期。

     >[!IMPORTANT]
     >
     >对工作区具有“查看”权限或更高权限的每个人都可以查看查找字段中的信息，无论他们在链接对象类型应用程序中的权限或访问级别，或者他们在其他工作区中的权限如何。

     链接的记录字段前面有关系图标![](assets/relationship-field-icon.png)。

     链接的字段前面有标识该字段类型的图标。 例如，链接（或查找）字段前面有图标，指示字段是数字、段落或日期。

<!--## Connection types

After you establish a connection between two record types or between a record and an object type from another application, you can add records in the connected record fields. 

Depending on how many records you can add to a connected record field, the following are the connection types you can choose from when connecting record types: 

* [Many to many](#many-to-many-connection-type)
* [One to many](#one-to-many-connection-type)
* [Many to one](#many-to-one-connection-type)
* [One to one](#many-to-one-connection-type)

>[!WARNING]
>
>These options are not available when connecting the following: 
>* Two records from different workspaces
>
>* A record type and Experience Manager assets

### Many-to-many connection type

![](assets/many-to-many-connection-picker.png)

When you create a many-to-many connection between record types, you can then select multiple records in the connection field from both record types. 

For example, if you create a many-to-many connection between campaigns and projects, you can select multiple projects for each campaign, and multiple campaigns for each project. 

A real-life example of a many-to-many relationship type is the relationship between movies and actors. Each movie can have multiple actors, and each actor can play in multiple movies. 

When you select this connection type, you cannot change the connection type after you save it. 

### One-to-many connection type

![](assets/one-to-many-connection-picker.png)


When you create a one-to-many connection between record types, you can then select multiple records in the connection field in the current record type, but the corresponding connection field in the record type you connect to will allow selecting only one record. The connected record field that is automatically created on the second record type is automatically set to a many-to-one relationship type. 

For example, if you create a one-to-many connection between campaigns and projects, you can select multiple projects for each campaign, but each project can be connected to only one campaign.

A real-life example of a one-to-many relationship type is the relationship between libraries and books: a library has many books in its inventory; but one particular book can only be in one library at a given point in time. 

When you select this connection type, you can later change it only to a many-to-many connection type. 

### Many-to-one connection type

![](assets/many-to-one-connection-picker.png)


When you create a many-to-one connection between record types, you can then connect each record in the current record type with only one record from the connected record type. The connected record field that is automatically created on the second record type is automatically set to a one-to-many relationship type. 

For example, if you connect campaigns with projects and you choose this type of connection, you can add only one project to a campaign. But you can add multiple campaigns to one project. 

A real-life example of a many-to-one relationship type is the relationship between many movies and one actor: one actor can be in many movies, but each movie can only have a specific actor once in its cast. 

When you select this connection type, you can later change it only to a many-to-many connection type.

### One-to-one connection type

![](assets/one-to-one-connection-picker.png)

When you create a one-to-one connection between record types, in both record types you can connect each record only with one record from the other record type.

For example, if you connect campaigns with projects and you choose this type of connection, you can connect one campaign with one project. One project can be connected only to one campaign. 

A real-life example of a one-to-one relationship is the one existing between a person and their country's unique identifier (like a Social Security Number, Passport ID, local identification ID): each person has only one unique identifier for a country and each unique identifier can be linked to only one person. 

When you select this connection type, you can later change it to any other connection type. 

-->



