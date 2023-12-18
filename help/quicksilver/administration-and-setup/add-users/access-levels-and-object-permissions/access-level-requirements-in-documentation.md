---
title: 访问级别要求
content-type: reference
product-area: system-administration
keywords: 访问，级别，系统，管理员，规划者，工作人员，查看者，请求者，外部，用户
navigation-topic: access-levels
description: Workfront文档操作方法文章包含一个表，其中说明了执行该过程所需的访问和权限。 本文更详细地说明了访问要求表，并包含更多信息的链接。
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
source-git-commit: d786a5bd86bcc1a4fbacf022cc9fbee9cb321da5
workflow-type: tm+mt
source-wordcount: '745'
ht-degree: 0%

---

# Workfront文档中的访问级别要求

Workfront文档操作方法文章包含一个表，其中说明了此过程所需的访问和权限要求。 通过此访问要求表，您可以了解您是否可以在Workfront中执行特定操作，或者为什么您可能无法执行。 本文介绍“访问要求”表的每个元素，并提供故障排除提示以及指向更深入信息的链接。

如果给定文章的“访问要求”表中没有行，则该操作没有此类型的要求。

>[!NOTE]
>
>如果您对此表中的任何字段如何应用于您有任何疑问，请与Workfront管理员联系。

## 访问要求表

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> Adobe Workfront计划是指贵组织已购买的一组功能。 大多数Workfront功能在所有计划中均可用，只有少数例外，这些功能主要与战略规划和企业控制相关。 
   <ul><li>要了解您的组织使用哪种Adobe Workfront计划（包括您的组织使用的是新打包模型还是当前打包模型），请联系您的Workfront管理员。</li>
   <li>有关Workfront管理员如何查找您组织的Workfront计划的说明，请参阅 <a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-plan" class="MCXref xref">查看贵组织的集群和Workfront计划</a>.</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> Adobe Workfront许可证是指分配给您的许可证所包含的一组Workfront功能。 例如，一个用户可能拥有一份许可证，其中包括将工作项目标记为完成和记录时间，而另一个用户拥有一份许可证，仅允许他们批准资产或提交请求。 <p> 
   <ul>
   <li>要了解您分配的许可证，请与Workfront管理员联系。</li>
   <li>Adobe Workfront正在过渡到一个新的定价和打包模式。 有关许可证的信息，请参阅：
   <ul>
   <li>新增： <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">新许可证概述</a></li>
   <li>当前： <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">许可证概述</a></li></ul></li>
   <li>如果您拥有正确的访问级别，但仍没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.
   </ul>
      </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别</td> 
   <td> 访问级别是您可以在Workfront中执行操作的一组权限，由Workfront管理员设置。 <p>Workfront具有与Workfront许可证对应的内置访问级别，但Workfront管理员可以创建更多访问级别，以更准确地反映组织所需的权限集。</p>
   <ul>
    <li>Adobe Workfront正在过渡到一个新的定价和打包模式。 有关每个模型的访问级别的信息，请参阅：
   <ul>
   <li>新增： <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md" class="MCXref xref">新访问级别概述</a></li>
   <li>当前： <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref">访问级别概述</a></li></ul></li>
    <li>要了解访问级别的详细信息，请与Workfront管理员联系</li>
    <li>如果您是Workfront管理员，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">配置对Adobe Workfront的访问权限</a> 了解有关授予访问级别中特定对象的访问权限的详细信息。</li>  
   <li>如果您拥有正确的访问级别，但仍没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</li>
    </td>
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td><p>对象权限是指在创建单个Workfront对象或与您共享这些对象时，您对它们拥有的访问权限。 例如，您必须对特定项目具有查看权限才能查看该项目，即使您的访问级别允许您查看项目。 “访问要求”表的此部分描述了在文章中执行操作所需的任何特定对象权限。</p>
   <p>有关请求对对象的附加访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>Workfront提供了一些可在Workfront之外购买的产品。
   <p>描述在这些附加产品内执行的过程的文章在此处列出了所需的产品。</p>
   <ul>
   <li>Adobe Experience Manager Assets或Assets Essentials </li>
   <li>Workfront Fusion</li>
   <li>Workfront Goals</li>
   <li>Workfront Scenario Planner</li>
   </ul>
   <p>要了解您的组织是否已购买这些附加产品之一，请联系您的Workfront管理员。</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion许可证</td> 
   <td>Adobe Workfront Fusion与Workfront具有不同的许可模型。 
   <ul><li>当前：当前许可证模型基于执行的操作数，对组织可以执行的操作没有限制。 </li>
   <li>旧版：旧版许可证基于方案是否能够连接到第三方应用程序，或者方案是否仅用于Workfront自动化。 </li>
   </ul>
   有关Fusion许可的信息，请参阅 <a href="/help/quicksilver/workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">Workfront Fusion许可证</a>.
   </td> 
  </tr> 
 </tbody> 
</table>


