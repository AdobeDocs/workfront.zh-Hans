---
title: 管理从属连接
description: 作为工作区管理员，您可以在Adobe Workfront Planning中的记录类型之间创建连接字段时定义依赖连接。 添加连接的字段时，您可以启用一个设置，当两个字段同时出现在第三个记录类型中时，该设置指示连接的记录类型的值取决于源记录类型的值（添加连接的记录类型）。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 0a4b902b2ac586b2a893dea29abb90299bee1ec3
workflow-type: tm+mt
source-wordcount: '1332'
ht-degree: 1%

---


# 管理从属连接

<span class="preview">此页面上的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在发布到“预览”版之后，启用了“快速发布”的客户的生产环境中每月还会提供相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

作为工作区管理员，您可以在Adobe Workfront Planning中的记录类型之间创建连接字段时定义依赖连接。

添加连接的字段时，您可以启用一个设置，当两个字段同时出现在第三个记录类型中时，该设置指示连接的记录类型的值取决于源记录类型的值（添加连接的记录类型）。

例如，您可能希望确保区域字段仅显示与选定地理位置关联的值。 这直接在连接字段设置中配置：当将连接从地域记录类型添加到从属记录类型（如区域）时，新设置允许工作区管理员使用在这些记录类型之间已建立的关系将其标记为从属地域记录类型。

配置完毕后，任何引用这两个字段（例如营销策划）的记录类型都会立即看到效果：选择地域值会将“区域”选取器缩小为仅包含那些实际链接到该地域的地区。 这会自动实施记录结构，从而消除不匹配的组合并减少手动清理。

## 访问权限要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 包</p></td> 
   <td> 
<p>要从同一工作区连接记录类型，请执行以下操作： </p>
<ul> 
<li><p>包含任何Planning包的任何Workfront或工作流包</p></li>
<p>或</p>
<li><p>作为独立产品购买时的任何Planning包</p></li>
</ul>

<p>从不同的工作区连接记录类型：</p>

<ul>

<li><p>任何工作流和计划Prime或Ultimate包</p></li>
<p>或</p>
<li><p>作为独立产品购买时的任何Planning Prime或Ultimate软件包</p></li>
</ul>
<p>有关每个Workfront Planning包中所包含内容的更多信息，请联系您的Workfront客户代表。 </p> 
   </td> 
<tr> 
<td> 
   <p> 其他产品</p> </td> 
   <td> 
   <p> 除了Adobe Workfront之外，如果要将记录类型与以下应用程序中的对象连接起来，还必须具备以下功能：</p>
   <ul><li><p>Adobe Experience Manager Assets许可证以及AEM Assets与Workfront之间的集成，用于连接AEM资源与Planning记录类型。</p>
   <p>有关信息，请参阅适用于Experience Manager Assets和Assets Essentials的<a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Adobe Workfront：文章索引</a>。 </p></li>
   <li><p> 用于连接记录类型与GenStudio对象和品牌的Adobe GenStudio for Performance Marketing许可证</p>
   <p>有关信息，请参阅<a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/get-started">Adobe GenStudio for Performance Marketing入门</a>。</p></li></ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p>标准</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>   <p>管理工作区的权限</p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>  </td> 
  </tr>  
</tbody> 
</table>

有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--
Sent a slack message to Norayr, Predator, Snowstorm, Armine for info for this section: 
-->

## 相关连接字段的注意事项


* 只能在已建立连接字段关系的记录类型之间设置从属连接字段。 您无法在不相关的记录类型之间定义依赖关系逻辑。

* 在单独的工作区中，记录类型之间可以有一个从属连接字段。

* 在Planning记录类型与Workfront或AEM对象类型之间不能有从属连接字段。

* 在连接字段设置本身中，依赖关系设置一次配置一个连接，而不是作为全局规则配置。

* 只有在第三个记录类型中同时存在源字段和从属字段时，才会激活两个连接的记录之间的过滤行为。 如果记录类型上只显示两个字段中的一个，则依赖关系无效。

* 相关字段的选择器仅限于在记录级别已链接到选定源值的值；它无法显示或建议未链接的值。

* 如果源字段的值发生更改，则从属字段将被自动清除，而不是保留为无效状态，以防止不匹配的组合持续存在。

  您会收到一则内联或toast消息，说明相关字段被清除的原因。

* 每个依赖字段最多可以有3个直接控制字段。

* 依赖项级别限制为6个连接。 这意味着最多可以连接7个记录类型。

* 为使依赖关系链正常工作，所有依赖字段必须同时存在于同一记录类型中。

## 创建从属连接

1. 作为工作区管理员，转到Workfront Planning中的记录类型，然后在表视图中将其打开。
1. 单击表格视图右上角的&#x200B;**+**&#x200B;图标以添加新字段。
1. 单击&#x200B;**新建连接**，然后开始为第二个记录类型添加新连接。

   >[!TIP]
   >
   >您只能在两个Planning记录类型之间创建从属连接。 无法在Workfront或AEM中的记录类型和对象之间创建依赖关系。
1. 在&#x200B;**连接设置**&#x200B;部分中，打开&#x200B;**使此连接依赖于**。

   >[!TIP]
   >
   >启用&#x200B;**使此连接依赖**&#x200B;设置将自动启用&#x200B;**在链接的记录类型上创建相应的字段**。 每个记录类型最多有500个字段。

   ![新连接选项卡中启用了依赖连接](assets/dependent-connection-enabled-setting.png)

1. 继续设置连接，如文章[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)中所述。
1. 单击&#x200B;**保存**。

   出现以下情况：

   * 这两个记录类型之间的连接已创建，当它们在同一记录类型上一起显示时，它们的值将相互依赖。
   * 为第二记录类型创建显示第一记录类型的对应字段。
   * 当两个记录类型都连接到第三记录类型时，显示为第二连接的记录字段的选择的值是连接到第一记录的值。 作为第一个记录类型的选项显示的值是连接到第二个记录类型的值。

     有关信息，请参阅本文中的[相关连接记录类型的示例](#example-of-dependent-connected-record-types)部分。
   * 已连接记录字段的列标题中有一个指示说明该字段处于依赖连接关系。

     列标题](assets/dependent-icon-tooltip-in-column-header.png)中的![依赖图标工具提示

1. （可选且推荐）转到第三记录类型，并将第一和第二记录类型添加为连接的记录字段。

   ![第三个记录类型上的依赖已连接字段指示器](assets/dependent-connected-field-indicator-on-a-third-record-type.png)

## 相关连接记录类型的示例

本节提供了一个简单示例，说明如何设置从属记录类型以及它们如何用于第三个记录类型。

1. 在您可以管理的工作区中，创建以下记录类型：

   * 促销活动
   * 国家/地区
   * 大陆

1. 在&#x200B;**国家/地区**&#x200B;记录类型中，添加以下记录：

   * 法国
   * 美国
   * 日本
1. 在&#x200B;**大陆**&#x200B;记录类型中，添加以下记录：

   * 欧洲
   * 美国
   * 亚洲

1. 从&#x200B;**国家/地区**&#x200B;记录类型中，为&#x200B;**大陆**&#x200B;创建连接的依赖字段。

   这会添加以下连接的记录字段：

   * **大陆**&#x200B;记录类型的&#x200B;**国家/地区**&#x200B;连接记录字段。
   * **国家/地区**&#x200B;记录类型的&#x200B;**大陆**&#x200B;连接记录字段。

1. 执行下列操作之一：

   * 从&#x200B;**国家/地区**&#x200B;记录类型表视图中，为大陆连接的记录字段添加以下值：

     * 法国的欧洲
     * 美国代表美国
     * 日本的亚洲
   * 从&#x200B;**大陆**&#x200B;记录类型表视图中，为&#x200B;**国家/地区**&#x200B;连接的记录字段添加以下值：

     * 法国代表欧洲
     * 美国
     * 日本代表亚洲
1. 将&#x200B;**国家/地区**&#x200B;和&#x200B;**大陆**&#x200B;连接的字段添加到&#x200B;**Campaign**&#x200B;记录类型表视图。
1. 在&#x200B;**促销活动**&#x200B;记录类型上为&#x200B;**国家/地区**&#x200B;字段选择&#x200B;**日本**。 请注意，对于营销活动上的&#x200B;**大陆**&#x200B;连接字段，唯一可用的值是&#x200B;**亚洲**。

   或

   为Campaign记录类型上的&#x200B;**大陆**&#x200B;字段选择&#x200B;**欧洲**。

   请注意，对于营销活动中的&#x200B;**国家/地区**&#x200B;已连接字段，可用的唯一值是&#x200B;**法国**。



