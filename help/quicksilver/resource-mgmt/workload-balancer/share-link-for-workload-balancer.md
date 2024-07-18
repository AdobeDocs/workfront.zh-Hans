---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 使用链接共享工作负载均衡器
description: 您可以与其他用户共享工作负载均衡器，其他用户可能没有可用的资源区域。 有关使用工作负载均衡器的信息，请参阅导航工作负载均衡器。
author: Lisa
feature: Resource Management
exl-id: e2d6b1f8-bdc9-4a34-bdc3-b56f7aa2e7a5
source-git-commit: 2c4fe48ef969741ba792e37c28adba86ffdcba9a
workflow-type: tm+mt
source-wordcount: '729'
ht-degree: 0%

---

# 使用链接共享工作负载均衡器

您可以与其他用户共享工作负载均衡器，其他用户可能没有可用的资源区域。 有关使用工作负载均衡器的信息，请参阅[导航工作负载均衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何计划</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>在资源区域使用工作负载均衡器时进行规划</p>
   <p>工作，使用团队或项目的工作负载均衡器时</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看以下内容或更高访问权限：</p> 
    <ul> 
     <li> <p>资源管理</p> </li> 
     <li> <p>项目</p> </li> 
     <li> <p>任务</p> </li> 
     <li> <p>问题</p> </li> 
    </ul> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看或更高权限的项目、任务和问题 </p> <p>有关请求其他访问权限的信息，请参阅<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 从共享链接查看工作负载均衡器中包含的信息

与其他用户共享指向工作负载均衡器的链接时，共享链接中包含以下信息：

* 工作负载均衡器的已分配工作区域。
* 项目、任务、用户信息。 这包括用户分配信息。
* 信息将根据所选过滤器显示。

  >[!IMPORTANT]
  >
  >如果在共享链接后删除过滤器，则从该链接查看工作负载均衡器的用户将收到过滤器已删除的警告。 他们查看已分配工作区域中的所有用户。 这是工作负载均衡器的默认视图。

* 之前选择的周数。

查看工作负载均衡器的用户可通过共享链接自我更新以下选项：

* 以下时间轴选择：

   * 今天
   * “后退”和“前进”图标
   * 日历选择

* “日”、“周”和“月”图标
* “设置”图标
* 显示分派图标

  有关使用这些选项的信息，请参阅[导航工作负载均衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)。

* 显示角色分配图标

  这仅适用于项目的工作负载均衡器。

接收共享链接的用户不能在此链接的工作负载均衡器中执行以下操作：

* 将工作项分配给用户
* 管理用户分配
* 构建新的过滤器或更新最初应用的过滤器

## 从共享链接查看工作负载均衡器中的信息所需的访问权限

您需要以下访问权限才能通过共享链接在工作负载均衡器中查看信息：

* 是有效的Adobe Workfront许可证，您必须登录到Workfront。
* 至少要在访问级别查看对资源管理的访问权限。 有关授予资源管理访问权限的信息，请参阅[授予对资源管理的访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)。
* 查看在工作负载均衡器中显示的项目、任务、问题和用户的权限。

## 通过链接与其他用户共享工作负载均衡器

1. 转到工作负载均衡器

   有关访问工作负载均衡器的信息，请参阅[导航工作负载均衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)。

1. （可选）执行以下一项或多项操作：

   * 更新时间段选择。
   * 单击&#x200B;**天、周**&#x200B;或&#x200B;**月**&#x200B;查看每日、每周或每月的信息。

     ![](assets/month-icon-on-toolbar-selected-wb-350x226.png)

   * 将过滤器应用于“未分配”和“已分配”工作区域。

     有关在工作负载均衡器中过滤信息的信息，请参阅在工作负载均衡器中[过滤信息](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md)。

1. 单击&#x200B;**链接图标** ![](assets/wb-shearable-link-icon-small.png)。

   这会添加指向剪贴板的链接。

1. 执行以下操作之一以与其他人共享链接：

   * 将其粘贴到电子邮件、聊天消息或任何其他应用程序中，并与其他用户共享。
   * 将其作为外部页面添加到自定义分区，将自定义分区添加到用户的配置文件或布局模板，然后与用户、团队、工作角色或组共享布局模板。

     有关创建外部页面的信息，请参阅[在仪表板中嵌入外部网页](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md)。 有关将自定义分区添加到布局模板的信息，请参阅[使用布局模板自定义左侧面板](../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)。

     >[!IMPORTANT]
     >
     >将工作负载均衡器添加到对象的自定义部分时，工作负载均衡器中的信息不按对象进行过滤。 工作负载均衡器显示按最初应用的过滤器过滤的信息。
