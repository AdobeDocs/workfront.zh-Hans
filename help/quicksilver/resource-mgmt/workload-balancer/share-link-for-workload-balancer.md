---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 使用链接共享工作负载平衡器
description: 您可以与可能没有可用资源区域的其他用户共享负载平衡器。 有关使用工作负载平衡器的信息，请参阅导航工作负载平衡器。
author: Alina
feature: Resource Management
exl-id: e2d6b1f8-bdc9-4a34-bdc3-b56f7aa2e7a5
source-git-commit: a74cc358c547e11a55cce728ad5330712ed0bd49
workflow-type: tm+mt
source-wordcount: '711'
ht-degree: 0%

---

# 使用链接共享工作负载平衡器

您可以与可能没有可用资源区域的其他用户共享负载平衡器。 有关使用工作负载平衡器的信息，请参阅 [导航工作负载平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意计划</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看或更高权限访问以下内容：</p> 
    <ul> 
     <li> <p>资源管理</p> </li> 
     <li> <p>项目</p> </li> 
     <li> <p>任务</p> </li> 
     <li> <p>问题</p> </li> 
    </ul> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看项目、任务和问题的权限或更高权限 </p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 从共享链接查看负载平衡器时，其中包含的信息

当您与其他用户共享指向工作负载平衡器的链接时，共享链接中包含以下信息：

* 工作负载平衡器的已分配工作区。
* 项目、任务、用户信息。 这包括用户分配信息。
* 该信息将根据所选过滤器显示。

   >[!IMPORTANT]
   >
   >如果在共享链接后删除过滤器，则从链接中查看工作负载平衡器的用户会收到一条警告，指出这些过滤器已被删除。 他们在“已分配的工作”区域中查看所有用户。 这是工作负载平衡器的默认视图。

* 先前选择的周数。

从共享链接查看工作负载平衡器以更新自身的用户可以使用以下选项：

* 以下时间轴选择：

   * 今天
   * 后向和前向图标
   * 日历选择

* “日”、“周”和“月”图标
* 设置图标
* 显示分配图标

   有关使用这些选项的信息，请参阅 [导航工作负载平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

* 显示角色分配图标

   此功能仅适用于项目的工作负载平衡器。

接收共享链接的用户无法在工作负载平衡器中通过此链接执行以下操作：

* 将工作项分配给用户
* 管理用户分配
* 生成新的或更新最初应用的过滤器

## 从共享链接查看工作负载平衡器中的信息所需的访问权限

您需要以下访问权限才能从共享链接查看工作负载平衡器中的信息：

* 有效的Adobe Workfront许可证，您必须登录到Workfront。
* 至少在访问级别中查看对资源管理的访问权限。 有关授予资源管理访问权限的信息，请参阅 [授予对资源管理的访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).
* 查看工作负载平衡器中显示的项目、任务、问题和用户的权限。

## 通过链接与其他用户共享工作负载平衡器

1. 转到工作负载平衡器

   有关访问工作负载平衡器的信息，请参阅 [导航工作负载平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. （可选）执行以下一项或多项操作：

   * 更新时间段选择。
   * 单击 **日、周**&#x200B;或 **月** 查看每日、每周或每月信息。

      ![](assets/month-icon-on-toolbar-selected-wb-350x226.png)

   * 将过滤器应用到“未分配”和“已分配”工作区。

      有关在工作负载平衡器中过滤信息的信息，请参阅 [在工作负载平衡器中筛选信息](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

1. 单击 **链接图标** ![](assets/wb-shearable-link-icon-small.png).

   这会将链接添加到剪贴板。

1. 执行以下操作之一以与他人共享链接：

   * 将其粘贴到电子邮件、聊天消息或任何其他应用程序中，并与其他用户共享。
   * 将其作为外部页面添加到自定义部分，将自定义部分添加到用户的配置文件或布局模板，然后与用户、团队、工作角色或组共享布局模板。

      有关创建外部页面的信息，请参阅 [在功能板中嵌入外部网页](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md). 有关向布局模板添加自定义部分的信息，请参阅 [使用布局模板自定义左侧面板](../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).

      >[!IMPORTANT]
      >
      >将工作负载平衡器添加到对象的自定义部分时，该对象不会过滤工作负载平衡器中的信息。 工作负载平衡器显示按最初应用的过滤器过滤的信息。
