---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: 在功能板中嵌入外部网页
description: 您可以将外部网页嵌入到功能板中，以提供对Adobe Workfront内其他系统或其他Workfront页面相关信息的访问。
author: Nolan
feature: Reports and Dashboards
exl-id: 04b623b5-38b0-4c32-b54e-204f1d422e45
source-git-commit: 3b3ba7cc6a975af71205f7f524e1a9a91a9d3810
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 0%

---

# 在功能板中嵌入外部网页

<!--Audited: 01/2024-->

您可以将外部网页嵌入到功能板中，以提供对其他系统或Adobe Workfront中相关信息的访问。

例如，如果贵组织有一个基于Web的文档存储库、Wiki或其他内容管理系统，其中包含通过URL定期访问的项目信息，则可以通过在功能板上创建外部页面将该信息显示到Workfront中。

>[!IMPORTANT]
>
>* 出于安全原因，某些网站不允许您将网页作为iframe嵌入。 如果要嵌入到仪表板中的网页不允许这样做，则该页面不会显示在仪表板中。 但是，您仍然可以通过单击功能板的名称来访问外部页面。\
>![](assets/qs-empty-external-page-report-350x165.png)\
>要允许嵌入您拥有的网站，请与Web管理员合作以调整 **X-Frame-Options** 设置。 有关更多信息，请参阅 [X-Frame-Options](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Frame-Options).
>
>
>* 仪表板中不再支持将仪表板页面嵌入外部页面。 虽然不会自动修改现有功能板以删除这些外部页面，但在删除或更改引用之前，无法保存对包含此类引用的功能板所做的任何修改。
> 具体而言，不再支持以下Workfront.com子域：
>
>     * /&#x200B;功能板
>     * /dashboard/：ID&#x200B;
>     * /portfolio/：ID/content-dashboard__：dashboardID&#x200B;
>     * /program/：ID/content-dashboard__：dashboardID&#x200B;
>     * /project/：ID/content-dashboard__：dashboardID&#x200B;
>     * /task/：ID/content-dashboard__：dashboardID&#x200B;
>     * /template/：ID/content-dashboard__：dashboardID&#x200B;
>     * /templatetask/：ID/content-dashboard__：dashboardID&#x200B;
>     * /resourcemanagement/：ID/
>     * content-dashboard__：dashboardID&#x200B;
>     * /team/：ID/content-dashboard__：dashboardID&#x200B;
>     * /iteration/：ID/content-dashboard__：dashboardID&#x200B;
>     * /requests/：ID/content-dashboard__：dashboardID&#x200B;
>     * /group/：ID/content-dashboard__：dashboardID&#x200B;
>     * /billingrecord/：ID/content-dashboard__：dashboardID
>
>作为替代解决方案，请考虑在功能板中包含列表报表，如中所述 [将报表添加到功能板](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md)

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront计划</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront许可证*</strong></td> 
   <td> <p>当前：计划 </p>
   或
   <p>新增：标准 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置</strong></td> 
   <td> <p>编辑对报告、功能板和日历的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。 有关更多信息，请参阅 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 先决条件

必须先创建功能板，然后才能在其中嵌入外部页面。

有关创建功能板的信息，请参阅 [创建功能板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## 在功能板中嵌入外部页面

>[!IMPORTANT]
>
>如果不再需要某个外部页面，您可以从功能板中删除该页面。 但是，在Workfront中创建外部页面后，您无法删除该页面。 您只能使用API删除外部页面。 有关更多信息，请参阅 [从功能板中删除外部页面](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md).

1. 找到要在Workfront中显示的页面的URL，并复制位于地址栏中的URL。

   >[!NOTE]
   >
   >如果您要与Workfront对象共享URL，请记住，某些URL会随着时间的推移而过期。 例如，文档URL在打开后过期。 这是作为一项安全措施配置的，并且从设计角度来看，它们被视为非静态URL，不应共享。

{{step1-to-dashboards}}

1. 要编辑现有功能板，请选择要嵌入网站页面的功能板，然后单击 **仪表板操作**，然后单击 **编辑**
或\
   要创建新仪表板，请单击 **新建仪表板**.\
   有关创建功能板的详细信息，请参阅 [创建功能板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

1. 单击 **添加外部页面** 在 **选择布局/添加报告/添加日历** 区域。

   ![](assets/qs-add-external-page-350x239.png)

   此 **添加外部页面** 框显示。

1. 指定有关外部页面的以下信息：

   * **名称**：添加功能板的名称。
   * **描述**：添加有关功能板的更多信息，以标识它包含的信息。 保存后，该描述将显示在仪表板上，供有权查看该描述的每个人查看。
   * **URL**：将您之前复制的URL粘贴到此字段中。

     您可以指定以下类型的URL：

      * 指向网页的https（加密）URL。\
        只有使用URL加载的https（加密）页面。\
        ![](assets/add-external-page-dialog-qs-350x247.png)

      * 包含特定网站会话信息的模板URL。\
        例如： *https://localhost/?session={！$$SESSION}*
您必须登录到指定的网站才能显示外部页面。\
        有关如何从Workfront获取SessionID的信息，请参阅 [API基础知识](../../../wf-api/general/api-basics.md).\
        出于安全原因，Workfront管理员可能会通过不允许在外部页面中使用会话信息的方式配置您的系统首选项。 在这种情况下，外部页面不会在功能板上加载。\
        有关系统安全首选项的详细信息，请参阅 [配置系统安全首选项](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).\
        ![external_page_with_session_id_example.png](assets/external-page-with-session-id-example-350x134.png)

   * **高度**：键入大于0的数字以定义外部页面在功能板上占用的空间。 默认高度为500。

1. 单击&#x200B;**保存**。

   该页面会自动添加到功能板。

   如果您创建其他功能板，则可以找到此外部页面并将其添加到其他功能板。 创建或编辑功能板时，您可以在可用报告和日历列表中找到所有现有的外部页面。

   <!--
    *** This is linked to: Creating Dashboards, and Editing Dashboards.
   -->

## 更新仪表板中的外部页面

要更新功能板中使用的外部页面的信息，请执行以下操作：

{{step1-to-dashboards}}

1. 单击要更新的仪表板名称以将其打开，然后单击 **仪表板操作**，则 **编辑**.

   此 **仪表板详细信息** 框打开。

1. 在 **选择布局/添加报告/添加日历** 区域 **仪表板详细信息** 框中，找到要更新的外部页面，将鼠标悬停在该页面上，然后单击 **编辑** 图标。\
   ![](assets/nwe-inline-edit-external-page-350x226.png)

1. 在 **编辑外部页面** 框中，更新要更改的字段，然后单击 **保存**.
1. （可选）单击 **删除** 图标 ![](assets/delete.png) 以从功能板中删除外部页面。 有关更多信息，请参阅 [从功能板中删除外部页面](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md).
1. 单击 **保存+关闭**.

## 在报表中查看外部页面

您可以在外部页面报表中查看Workfront中的所有外部页面。

{{step1-to-reports}}

1. 单击 **新建报告** >选择 **外部页面**.

   ![](assets/external-page-new-report-in-dropdown-nwe.png)

1. （可选）更新报表的视图、过滤器或分组选项卡。

   有关更多信息，请参阅 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 单击 **保存+关闭**.

   您可以在新的报告中查看与系统中外部页面关联的名称和URL。

   ![](assets/external-page-report-name-url-columns-nwe-350x213.png)
