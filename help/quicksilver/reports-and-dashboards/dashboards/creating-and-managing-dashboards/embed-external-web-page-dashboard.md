---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: 在功能板中嵌入外部网页
description: 您可以在功能板中嵌入外部网页，以便从Adobe Workfront内的其他系统或其他Workfront页面访问相关信息。
author: Nolan
feature: Reports and Dashboards
exl-id: 04b623b5-38b0-4c32-b54e-204f1d422e45
source-git-commit: 5a4c98f9ce6bb7eb936a0b24b634d2545a0f13ee
workflow-type: tm+mt
source-wordcount: '984'
ht-degree: 0%

---

# 在功能板中嵌入外部网页

您可以在功能板中嵌入外部网页，以便从Adobe Workfront内的其他系统或其他Workfront页面访问相关信息。

例如，如果贵组织具有基于Web的文档存储库、Wiki或其他内容管理系统，其中包含通过URL定期访问的项目信息，则可以通过在功能板上创建外部页面，将该信息显示到Workfront中。

>[!IMPORTANT]
>
>出于安全考虑，某些网站不允许您将网页嵌入为iFrame。 如果要在功能板中嵌入的网页不允许此操作，则该页面不会显示在功能板中。 但是，您仍可以通过单击功能板的名称来访问外部页面。\
>![](assets/qs-empty-external-page-report-350x165.png)\
>要允许嵌入您拥有的网站，请与Web管理员合作，以调整 **X-Frame-Options** 设置。 有关更多信息，请参阅 [X-Frame-Options](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Frame-Options).


>[!IMPORTANT]
>
>功能板页面不再作为功能板中嵌入的外部页面受支持。 虽然不会自动修改现有功能板以删除这些外部页面，但对功能板的任何修改（包括此类引用）在删除或更改引用之前将无法保存。
>
>具体而言，不再支持以下Workfront.com子域：
>
>* /功&#x200B;能板
>* /dashboard/:ID &#x200B;
>* /portfolio/:ID/content-dashboard__:dashboardID &#x200B;
>* /program/:ID/content-dashboard__:dashboardID &#x200B;
>* /project/:ID/content-dashboard__:dashboardID &#x200B;
>* /task/:ID/content-dashboard__:dashboardID &#x200B;
>* /template/:ID/content-dashboard__:dashboardID &#x200B;
>* /templatetask/:ID/content-dashboard__:dashboardID &#x200B;
>* /resourcemanagement/:ID/content-dashboard__:dashboardID &#x200B;
>* /team/:ID/content-dashboard__:dashboardID &#x200B;
>* /iteration/:ID/content-dashboard__:dashboardID &#x200B;
>* /requests/:ID/content-dashboard__:dashboardID &#x200B;
>* /group/:ID/content-dashboard__:dashboardID &#x200B;
>* /billingrecord/:ID/content-dashboard__:dashboardID
>
>作为替代解决方案，请考虑在功能板中包含列表报表，如 [将报表添加到功能板](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md)

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront计划*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront许可证*</strong></td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>编辑对报表、功能板和日历的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>管理功能板的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

您必须先创建功能板，然后才能在其中嵌入外部页面。

有关创建功能板的信息，请参阅 [创建功能板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## 在功能板中嵌入外部页面

>[!IMPORTANT]
>
>如果不再需要外部页面，您可以从功能板中删除该页面。 但是，在Workfront中创建外部页面后，您将无法删除该页面。 您只能使用API删除外部页面。 有关更多信息，请参阅 [从功能板中删除外部页面](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md).

1. 找到要在Workfront中显示的页面URL，并复制地址栏中的URL。

   >[!NOTE]
   >
   >如果您将URL共享到Workfront对象，请记住，某些URL会随着时间过期。 例如，文档URL在打开后过期。 这将配置为一项安全措施，并且根据设计，这些URL将被视为非静态URL，因此不应共享。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png)，然后单击 **功能板**.

1. 要编辑现有功能板，请选择要在其中嵌入网站页面的功能板，然后单击 **功能板操作**，然后选择 **编辑** 中。\
   或\
   要创建新功能板，请单击 **新功能板**.\
   有关创建功能板的更多信息，请参阅 [创建功能板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

1. 单击 **添加外部页面**.

   ![](assets/qs-add-external-page-350x239.png)

1. 指定 **名称** （对于外部页面）。
1. 指定 **描述**.
1. 将您之前复制的URL粘贴到 **URL** 字段。\
   您可以指定以下类型的URL:

   * 指向网页的https（加密）URL。\
      只有URL会加载https（已加密）页面。\
      ![](assets/add-external-page-dialog-qs-350x247.png)

   * 包含特定网站会话信息的模板URL。\
      例如： *https://localhost/?session=!$$SESSION}*
您必须登录到指定的网站才能显示外部页面。\
      有关如何从Workfront获取SessionID的信息，请参阅 [API基础知识](../../../wf-api/general/api-basics.md).\
      出于安全原因，Workfront管理员可以配置系统首选项的方式不允许在外部页面中使用会话信息。 在这种情况下，功能板上不会加载外部页面。\
      有关系统安全首选项的详细信息，请参阅 [配置系统安全首选项](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).\
      ![external_page_with_session_id_example_png](assets/external-page-with-session-id-example-350x134.png)

1. 单击&#x200B;**保存**。\
   页面会自动添加到功能板。 如果将来创建功能板，则可以添加外部页面。 外部页面将在可用报表中找到。

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: Alina: *** This is linked to: Creating Dashboards, and Editing Dashboards.)
   </MadCap:conditionalText>
   -->

## 更新功能板中的外部页面

要更新功能板中使用的外部页面的信息，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png)，然后单击 **功能板**.
1. 选择要更新的功能板，然后单击 **编辑** ![](assets/edit-icon.png).

   ![选择编辑图标。](assets/nwe-editdashboard2021-350x188.png)

1. 在屏幕右侧，找到要更新的外部页面，然后单击 **编辑** 图标。\
   ![](assets/nwe-inline-edit-external-page-350x226.png)

1. 在 **编辑外部页面** 对话框，更新要更改的字段，然后单击 **保存**.
1. （可选）单击 **删除** 图标 ![](assets/delete.png) 从功能板中删除外部页面。 有关更多信息，请参阅 [从功能板中删除外部页面](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md).
1. 在左下角，单击 **保存并关闭**.

## 在报表中查看外部页面

您可以在外部页面报表中查看Workfront中的所有外部页面。

1. 转到 **主菜单** 图标 ![](assets/main-menu-icon.png) > **报表**.
1. 单击 **新建报表** >选择 **外部页面**.

   ![](assets/external-page-new-report-in-dropdown-nwe.png)

1. （可选）更新报表的“查看”、“过滤器”或“分组”选项卡。

   有关更多信息，请参阅 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 单击 **保存并关闭**.

   您可以在新报表中查看与系统中外部页面关联的名称和URL。

   ![](assets/external-page-report-name-url-columns-nwe-350x213.png)
