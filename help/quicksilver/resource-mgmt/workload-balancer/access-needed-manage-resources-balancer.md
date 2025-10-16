---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 在工作负载均衡器中管理资源所需的访问权限
description: 没有正确的访问权限或权限，您可能无法在工作负载均衡器查看或管理您的工作分配。
author: Lisa
feature: Resource Management
exl-id: b3da9a62-481e-4503-8f27-136d6513262e
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---

# 在工作负载均衡器中管理资源所需的访问权限

{{preview-fast-release-general}}

没有正确的访问权限或权限，您可能无法在工作负载均衡器查看或管理您的工作分配。

您必须有权查看要在工作负载均衡器中查看或管理其工作负载的用户。 除此之外，您还必须拥有与工作关联的项目的正确访问级别和正确权限。

<!--## Adobe Workfront package needed to use the Workload Balancer for different areas

The following table illustrates the connection between the Workfront plan your company has and where in the system you can use the Workload Balancer:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><p><b>Workfront Plan (Current)</b></p></td> 
   <td> <p><b>Areas where you can access the Workload Balancer</b></p> </td> 
  </tr> 
  <tr> 
   <td>Team or higher </td> 
   <td>Workload Balancer for a team or a project</td> 
  </tr> 
  <tr> 
   <td>Pro or higher</td> 
   <td>Workload Balancer for multiple projects, at the system level</td> 
  </tr> 
  <tr> 
   <td><p><b>Workfront Plan (New)</b></p></td> 
   <td> <p><b>Areas where you can access the Workload Balancer</b></p> </td> 
  </tr>
  <tr> 
   <td>Any </td> 
   <td>Access the Workload Balancer anywhere in Workfront</td> 
  </tr> 
 </tbody> 
</table>

For information about the Workfront plans, see [Our Plans](https://business.adobe.com/cn/products/workfront/pricing.html).

For information about where you can locate the Workload Balancer in Workfront, see [Locate the Workload Balancer](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).-->

## 查看工作负载均衡器所需的访问权限

您必须具有以下权限才能查看工作负载均衡器：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td>Adobe Workfront包</td> 
   <td><p>任何</p></td>
  </tr>
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p>
       <p>计划，在资源区域查看工作负载均衡器；工作，查看团队或项目的工作负载均衡器</p></td>
  </tr>  
  <tr> 
   <td>访问级别配置</td> 
   <td> <p>查看资源管理的或更高访问权限</p> <p>有关资源管理访问级别的信息，请参阅文章<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md">授予对资源管理的访问权限</a>。</p></td> 
  </tr> 
  <tr> 
   <td>对象权限</td> 
   <td> <p>对于要查看其工作分配的项目，您必须具有“查看”权限。 </p> <p>有关项目权限的信息，请参阅文章<a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md">在Adobe Workfront中共享项目</a>。</p></td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

<span class="preview">所有用户都有权在其自己的配置文件上查看工作负载均衡器。 这不受许可证或访问级别的限制。 请注意，用户配置文件上的工作负载均衡器是只读的，无法更改分配和分配。</span>

## 管理工作负载均衡器中的分配所需的访问权限

您必须具有以下权限才能管理工作负载均衡器：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td>Adobe Workfront包</td> 
   <td><p>任何</p></td>
  </tr>
  <tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p>
       <p>计划，在资源区域的工作负载均衡器中管理分配；工作，在团队或项目的工作负载均衡器中管理分配</p></td>
  </tr> 
  <tr> 
   <td>访问级别配置</td>
   <td> <p>编辑对资源管理的访问权限</p>
     <p>有关资源管理访问级别的信息，请参阅文章<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" >授予对资源管理的访问权限</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>对象权限</td> 
   <td> <p> 要管理其工作分配的项目的Contribute或更高权限，包括创建工作分配的权限。 </p> <p>有关项目权限的信息，请参阅文章<a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md">在Adobe Workfront中共享项目</a>。</p></td>
  </tr> 
 </tbody>
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

<!--these notes were inside the table: for the Edit access to Res Management
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">View or higher access to Financial Data, if you want to view information by cost (NOTE: this is not possible yet!)</p>    
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Financial Data access level, see the article<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>. (NOTE: this is not possible yet!)</p>
    -->
