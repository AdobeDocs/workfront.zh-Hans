---
product-area: resource-management
navigation-topic: resource-planning
title: 使用链接共享资源规划者用户视图
description: Adobe Workfront可以为资源规划者的用户视图生成唯一的URL，您可将该URL作为外部页面嵌入到仪表板中，或者在新的浏览器选项卡中单独打开它。 在将资源规划者信息与可能无权直接访问资源区域的用户共享时，这非常有用。
author: Lisa
feature: Resource Management
exl-id: feb2ec26-f1a6-4581-9e1d-be948a2170c3
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 1%

---

# 使用链接共享资源规划者用户视图

Adobe Workfront可以为资源规划者的用户视图生成唯一的URL，您可将该URL作为外部页面嵌入到仪表板中，或者在新的浏览器选项卡中单独打开它。 在将资源规划者信息与可能无权直接访问资源区域的用户共享时，这非常有用。

![带有链接的用户视图](assets/rp-user-view-with-link-highlight-350x49.png)

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td><p>任何</p></td>
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p>
       <p>规划</p></td> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td> <p>查看资源管理、项目和用户的或更高访问权限</p> <p>查看对财务数据的访问权限以查看成本信息</p></td> 
  </tr> 
  <tr> 
   <td>对象权限</td> 
   <td> <p>查看您想在资源规划者中显示的项目或授予更高的权限</p></td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

为资源规划者的用户视图生成唯一URL时，请考虑以下事项：

* 您只能获取用户视图的唯一URL。 项目视图或角色视图中不存在用于生成URL的选项。
* 您可以与其他用户（包括“工作”和“审阅”许可用户）共享URL。\
  他们必须有权查看其他用户，以便通过您与他们共享的URL在资源规划者中查看信息。
* 当您与其他用户共享URL时，会保存以下信息：

   * 时间段的类型（周、月、季度）。
   * 您应用的过滤器。
   * 显示的类型（小时或FTE）。

要在资源规划者的用户视图中获取唯一URL并与其他用户共享，请执行以下操作：

{{step1-to-resourcing}}

1. 选择&#x200B;**按用户查看**。
1. （可选）选择要在资源规划程序中查看信息所依据的时间范围。 从以下项中选择：

   * 周
   * Month
   * 季度

1. （可选）选择要按&#x200B;**FTE**&#x200B;还是&#x200B;**Hours**&#x200B;查看信息。\
   ![选择FTE或小时](assets/rp-hours-or-fte-in-user-view.png)

1. （可选）将过滤器应用于资源规划者。\
   有关应用筛选器的信息，请参阅[资源规划者中的筛选器信息](../../resource-mgmt/resource-planning/filter-resource-planner.md) 。

1. 单击&#x200B;**超链接**&#x200B;图标。\
   ![超链接图标和URL](assets/rp-generate-url-from-link-icon.png)

1. 单击&#x200B;**复制URL**。\
   这会将“用户视图”中资源规划者的唯一URL复制到剪贴板。

1. （可选）执行以下操作之一：

   * 将URL粘贴到另一个应用程序以发送给另一个用户。\
     用户必须登录到Workfront才能在“用户”视图中查看资源规划者。
   * 打开新的浏览器选项卡或窗口，并粘贴您复制的链接，然后在键盘上单击Enter以在新选项卡或窗口中打开Resource Planner。
   * 执行以下操作：

     <!--   
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     (NOTE:&nbsp;turn this into a numbered list)   
     </MadCap:conditionalText>   
     -->

      1. 转到&#x200B;**报告**>**仪表板**>**新仪表板**>**添加外部页面。**

      1. 将您复制到剪贴板的链接粘贴到&#x200B;**URL**&#x200B;字段中。
      1. 单击&#x200B;**保存**，然后单击&#x200B;**保存+关闭**。\
         这会将URL嵌入到仪表板中，并且资源规划者的用户视图显示在单独的仪表板中。

1. （可选）如果将URL嵌入到仪表板中，请考虑将其添加到布局模板或与其他可能无权访问资源管理区域的用户共享。\
   有关将功能板添加到布局模板的信息，请参阅[创建和管理布局模板](../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) 。\
   有关共享功能板的信息，请参阅[共享功能板](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) 。\
   查看共享URL时，用户可以查看最初应用于资源规划者的设置的信息。 用户必须登录到Workfront才能查看共享URL。\
   ![显示有资源规划者的示例仪表板](assets/user-view-dashoard-from-unique-url-350x85.png)
