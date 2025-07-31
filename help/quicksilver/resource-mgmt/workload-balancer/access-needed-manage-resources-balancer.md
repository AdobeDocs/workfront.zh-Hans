---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 在工作负载均衡器中管理资源所需的访问权限
description: 没有正确的访问权限或权限，您可能无法在工作负载均衡器查看或管理您的工作分配。
author: Lisa
feature: Resource Management
exl-id: b3da9a62-481e-4503-8f27-136d6513262e
source-git-commit: 78d73d0d7bd0ffc00ae1afed0adb324501e0c310
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

# 在工作负载均衡器中管理资源所需的访问权限

{{preview-fast-release-general}}

没有正确的访问权限或权限，您可能无法在工作负载均衡器查看或管理您的工作分配。

您必须有权查看要在工作负载均衡器中查看或管理其工作负载的用户。 除此之外，您还必须拥有与工作关联的项目的正确访问级别和正确权限。

## Adobe Workfront计划需要将工作负载均衡器用于不同区域

下表说明了贵公司拥有的Workfront计划与系统中可使用工作负载均衡器的位置之间的关系：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p><b>Workfront计划（当前版本）</b></p></td> 
   <td> <p><b>您可以访问工作负载均衡器的区域</b></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">团队或更高 </td> 
   <td>团队或项目的工作负载均衡器</td> 
  </tr> 
  <tr> 
   <td role="rowheader">专业或专业以上</td> 
   <td>在系统级别为多个项目提供工作负载均衡器</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p><b>Workfront计划（新）</b></p></td> 
   <td> <p><b>您可以访问工作负载均衡器的区域</b></p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">任何 </td> 
   <td>在Workfront中的任意位置访问工作负载均衡器</td> 
  </tr> 
 </tbody> 
</table>

有关Workfront计划的信息，请参阅[我们的计划](https://business.adobe.com/products/workfront/pricing.html)。

有关可以在Workfront中定位工作负载均衡器的信息，请参阅[定位工作负载均衡器](../../resource-mgmt/workload-balancer/locate-workload-balancer.md)。

## 查看工作负载均衡器所需的访问权限

您必须具有以下权限才能查看工作负载均衡器：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>新增：标准</p>
       <p>或</p>
       <p>当前：计划，在资源区域查看工作负载均衡器；</br>
       工作：查看团队或项目的工作负载均衡器</p></td>
  </tr>  
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>查看资源管理的或更高访问权限</p> <p>有关资源管理访问级别的信息，请参阅文章<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">授予对资源管理的访问权限</a>。</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>对于要查看其工作分配的项目，您必须具有“查看”权限。 </p> <p>有关项目权限的信息，请参阅文章<a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">在Adobe Workfront中共享项目</a>。</p></td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

<span class="preview">所有用户都有权在其自己的配置文件上查看工作负载均衡器。 这不受许可证或访问级别的限制。 请注意，用户配置文件上的工作负载均衡器是只读的，无法更改分配和分配。</span>

## 管理工作负载均衡器中的分配所需的访问权限

您必须具有以下权限才能管理工作负载均衡器：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>新增：标准</p>
       <p>或</p>
       <p>当前：计划，用于管理资源区域的工作负载均衡器中的分配；</br>
       工作，用于管理团队或项目的工作负载均衡器中的分配</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对资源管理的访问权限</p> 
     <p>有关资源管理访问级别的信息，请参阅文章<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">授予对资源管理的访问权限</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p> 要管理其工作分配的项目的Contribute或更高权限，包括创建工作分配的权限。 </p> <p>有关项目权限的信息，请参阅文章<a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">在Adobe Workfront中共享项目</a>。</p></td>
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

<!--these notes were inside the table: for the Edit access to Res Management
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">View or higher access to Financial Data, if you want to view information by cost (NOTE: this is not possible yet!)</p>    
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Financial Data access level, see the article<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>. (NOTE: this is not possible yet!)</p>
    -->
