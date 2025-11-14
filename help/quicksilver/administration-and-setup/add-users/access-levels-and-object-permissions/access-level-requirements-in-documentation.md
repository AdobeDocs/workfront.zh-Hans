---
title: Workfront中的访问要求文档
content-type: reference
product-area: system-administration
keywords: 访问，级别，系统，管理员，规划者，工作人员，查看者，请求者，外部，用户
navigation-topic: access-levels
description: Workfront文档操作方法文章包含一个表，其中说明了执行该过程所需的访问和权限。 本文更详细地说明了访问要求表，并包含更多信息的链接。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 39ea0d53-ec31-4644-b772-cfe260b8e013
source-git-commit: c1c30696dc9ef324103467f3bdcb83609cf5d1d8
workflow-type: tm+mt
source-wordcount: '1010'
ht-degree: 0%

---

# Workfront文档中的访问要求

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
   <td role="rowheader">Adobe Workfront包</td> 
   <td> Adobe Workfront包是指您的组织已购买的一组功能。 大多数Workfront功能在所有资源包中都可用，只有少数例外，这些功能主要与战略规划和企业控制相关。 <p>2022年以前存在的包不在列表中。</p>
   <p>Workfront包分为三个区域。 某些区域提供了不同的包，如Select、Prime和Ultimate。<p>
   <ul>
   <li><b>Workfront工作流</b>：包含与操作相关的功能，如任务管理、审批和工时表。 此包进一步分为工作流选择、工作流Prime和工作流Ultimate包。</li>
   <li><b>Workfront计划</b>：包含与战略计划相关的功能。 此包进一步分为Planning Select、Planning Prime和Planning Ultimate包。</li>
   <li><b>Workfront自动化和集成</b>：包括与自动化流程以及与其他应用程序集成相关的功能。</li>
   </ul>
  <p>贵组织可能在这些区域中的一个或多个区域购买了Workfront包。</p>
  <p>以前，Workfront提供Workfront Select、Workfront Prime和Workfront Ultimate包，而不区分工作流、规划以及自动化和集成。 您的组织可能位于这些旧包之一。 
   <ul><li>要了解贵组织使用哪个Adobe Workfront包（包括贵组织使用的是当前打包模型还是旧打包模型），请与Workfront管理员联系。</li>
   <li>有关Workfront管理员如何找到您组织的Workfront包的说明，请参阅<a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-package" class="MCXref xref">查看您组织的群集和Workfront包</a>。</li><li>有关Workfront包的更多信息，请参阅<a href="https://business.adobe.com/products/workfront/pricing.html">Adobe Workfront定价和打包</a>。</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> Adobe Workfront许可证是指分配给您的许可证所包含的一组Workfront功能。 例如，一个用户可能拥有一份许可证，其中包括将工作项目标记为完成和记录时间，而另一个用户拥有一份许可证，仅允许他们批准资产或提交请求。 <p> 
   <ul>
   <li>要了解您分配的许可证，请与Workfront管理员联系。</li>
   <li>有关许可证的信息，请参阅：
   <ul>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">新许可证概述</a></li>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">许可证概述</a></li></ul></li>
   <li>如果您拥有正确的访问级别，但仍没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-package" class="MCXref xref">创建或修改自定义访问级别</a>。
   </ul>
      </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td><p>由于Workfront与其他Adobe产品密切合作，因此Workfront中的某些过程会直接与这些产品交互。 要遵循这些步骤，贵组织必须已购买该产品。 例如，要使用允许Workfront与Adobe Experience Manager Assets交互的功能，您的组织必须已购买Adobe Experience Manager Assets。</p>
   <p>描述使用其他产品执行的过程的文章列出了此表产品线中的所需产品。</p>
   <p>要了解您的组织是否已购买这些附加产品之一，请联系您的Workfront管理员。</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别</td> 
   <td> 访问级别是您可以在Workfront中执行操作的一组权限，由Workfront管理员设置。 <p>Workfront具有与Workfront许可证对应的内置访问级别，但Workfront管理员可以创建更多访问级别，以更准确地反映组织所需的权限集。</p>
   <ul>
    <li>有关访问级别的信息，请参阅：
   <ul>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md" class="MCXref xref">新访问级别概述</a></li>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref">访问级别概述</a></li></ul></li>
    <li>要了解访问级别的详细信息，请与Workfront管理员联系</li>
    <li>如果您是Workfront管理员，请参阅<a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">配置对Adobe Workfront的访问权限</a>，了解有关授予访问级别中特定对象的访问权限的详细信息。</li>  
   <li>如果您拥有正确的访问级别，但仍没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</li>
    </td>
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td><p>对象权限是指在创建单个Workfront对象或与您共享这些对象时，您对它们拥有的访问权限。 例如，您必须对特定项目具有查看权限才能查看该项目，即使您的访问级别允许您查看项目。 “访问要求”表的此部分描述了在文章中执行操作所需的任何特定对象权限。</p>
   <p>有关请求对对象的附加访问权限的信息，请参阅<a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问权限</a>。</p><p>有关共享对象的信息，请参阅<a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md" class="MCXref xref">共享对象</a>。</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">版面模板</td> 
   <td><p>布局模板控制您在主菜单中看到的内容，并由Workfront管理员配置。 本行说明了Workfront的所有特定区域，您必须将这些区域包含在主菜单中才能执行此操作。</p><p>通常，如果文章指示您单击主菜单中的某个区域，而该区域在主菜单中不可见，请联系您的Workfront管理员以确定是否可以将该区域提供给您使用。</p><p>
   有关Workfront管理员如何配置主菜单的信息，请参阅<a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref">使用布局模板自定义主菜单</a>。</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion许可证</td> 
   <td>Adobe Workfront Fusion与Workfront具有不同的许可模型。 
   <ul><li>当前许可证模型基于执行的操作数，对组织可以执行的操作没有限制。 </li>
   <li>旧版许可证基于方案是否能够连接到第三方应用程序，或者方案是否仅用于Workfront自动化。 </li>
   </ul>
   有关Fusion许可的信息，请参阅<a href="https://experienceleague.adobe.com/en/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration" class="MCXref xref">Workfront Fusion许可证</a>。
   </td> 
  </tr> 
 </tbody> 
</table>
