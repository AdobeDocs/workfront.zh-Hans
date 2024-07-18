---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 在工作负载均衡器中管理资源所需的访问权限
description: 没有正确的访问权限或权限，您可能无法在工作负载均衡器查看或管理您的工作分配。
author: Lisa
feature: Resource Management
exl-id: b3da9a62-481e-4503-8f27-136d6513262e
source-git-commit: 2c4fe48ef969741ba792e37c28adba86ffdcba9a
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 0%

---

# 在工作负载均衡器中管理资源所需的访问权限

如果没有正确的访问权限或权限，您可能无法在“工作负载均衡器”中查看或管理您的工作分配。

您必须有权查看要在工作负载均衡器中查看或管理其工作负载的用户。 除此之外，您还必须拥有与工作关联的项目的正确访问级别和正确权限。

## Adobe Workfront计划需要将工作负载均衡器用于不同区域

下表说明了贵公司拥有的Workfront计划与系统中可使用工作负载均衡器的位置之间的关系：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p><b>Workfront 计划</b></p></td> 
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
 </tbody> 
</table>

有关Workfront计划的信息，请参阅[我们的计划](https://www.workfront.com/plans)。

有关可以在Workfront中定位工作负载均衡器的信息，请参阅[定位工作负载均衡器](../../resource-mgmt/workload-balancer/locate-workload-balancer.md)。

## 查看工作负载均衡器所需的访问权限

您必须具有以下权限才能查看工作负载均衡器：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划查看“资源”区域的工作负载均衡器</p>
   <p>用于查看团队或项目的工作负载均衡器的工作</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看资源管理的或更高访问权限</p> <p>有关资源管理访问级别的信息，请参阅文章<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">授予对资源管理的访问权限</a>。</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>对于要查看其工作分配的项目，您具有“查看”权限。 </p> <p>有关项目权限的信息，请参阅文章<a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">在Adobe Workfront中共享项目</a>。</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 管理工作负载均衡器中的分配所需的访问权限

您必须具有以下权限才能管理工作负载均衡器：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>规划以管理资源区域的工作负载均衡器中的分配</p>
   <p>致力于管理团队或项目的工作负载均衡器中的分配</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对资源管理的访问权限</p> 
     <p>有关资源管理访问级别的信息，请参阅文章<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">授予对资源管理的访问权限</a>。</p>
     <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p> 要管理其工作分配的项目的Contribute或更高权限，包括进行工作分配的权限。 </p> <p>有关项目权限的信息，请参阅文章<a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">在Adobe Workfront中共享项目</a>。</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

<!--these notes were inside the table: for the Edit access to Res Management
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">View or higher access to Financial Data, if you want to view information by cost (NOTE: this is not possible yet!)</p>    
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Financial Data access level, see the article<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>. (NOTE: this is not possible yet!)</p>
    -->