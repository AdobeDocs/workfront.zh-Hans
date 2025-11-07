---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: 请求访问对象
description: 您对Adobe Workfront中对象的可见性取决于您对该类型对象的访问权限以及您对单个对象的权限。
author: Courtney
feature: Get Started with Workfront
exl-id: ad1c525c-42a8-4fb7-a2cd-7792e1c280ab
source-git-commit: 883ec4eaa2258de2e464acf14b6b4083db05b99a
workflow-type: tm+mt
source-wordcount: '1327'
ht-degree: 1%

---

# 请求访问对象

<!-- Audited: 4/2025 -->

您对Adobe Workfront中对象的可见性取决于您对该类型对象的访问权限以及您对单个对象的权限。

>[!NOTE]
>
>本文介绍了如何请求对所有对象的权限，以下对象除外：
>
>* Adobe Workfront Scenario Planner中的Scenario Planner计划。 有关详细信息，请参阅[在Scenario Planner](../../scenario-planner/request-access-to-plan.md)中请求对计划的访问权限。 这需要额外的许可证。
>
>* Workfront Planning中的视图和工作区。 有关详细信息，请参阅[在Adobe Workfront Planning中共享权限概述](/help/quicksilver/planning/access/sharing-permissions-overview.md)。 这需要额外的许可证。


Workfront管理员会配置您对访问级别中某类对象的访问权限。 有关详细信息，请参阅[访问级别和权限如何协同工作](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md)。

如果您需要拥有Workfront中特定对象的权限，则可以请求对这些对象的访问权限。 您可以请求Workfront中的其他访问（或权限），而不是向Workfront管理员或对象所有者发送电子邮件来解释您的需求。

如果有人与您共享指向对象的链接，您可以请求对对象的初始访问权限，或者您可以请求对您已具有查看权限的对象进行附加访问权限。 例如，您可能具有某个项目的查看权限，但您需要将任务添加到该项目。 在这种情况下，您可以请求项目的Contribute权限。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>标准</p> 
   <p>工作或更高</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>查看您请求权限对象的访问权限或更高</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 了解标准共享规则

以下标准共享规则是Workfront系统中的默认选项，会自动生效：

* 分配给任务或问题的用户具有任务或问题的Contribute访问权限。
* 项目、Portfolio和项目群经理对自己拥有的对象具有管理访问权限。
* 对话中包含的用户对对话发生的对象具有查看访问权限。
* 分配为批准者的用户对等待批准的对象具有查看权限。
* 共享功能板时，该功能板上的所有报告也将以相同的访问权限共享给相同的用户。
* 对象所有者无法将访问权限扩展到超出其对该对象的访问权限（如管理员所定义）。

## 请求访问

您可以请求对当前无权访问的对象的初始访问权限，也可以请求对您只有有限访问权限的对象的附加访问权限。

* [请求初始访问](#request-initial-access)
* [请求附加访问权限](#request-additional-access)

### 请求初始访问  {#request-initial-access}

如果您还不能访问某个对象，而要从链接导航到该对象，则会显示一个屏幕，通知您无权查看该信息。

要请求对对象的初始访问权限，请执行以下操作：

1. 单击&#x200B;**请求访问**。 显示&#x200B;**请求访问**&#x200B;对话框。

1. （视情况而定）如果多个用户具有授予您额外访问权限的相应访问权限，则用户名称旁边会显示一个下拉箭头。 从下拉列表中选择将收到访问请求的用户。

   下拉列表中只显示10个用户，该列表按字母顺序排序。 有关此下拉菜单中列出用户顺序的更多信息，请参阅“请求访问”和“请求更多访问”下拉菜单的[层次结构](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus)。

1. 从下拉列表中，选择您请求的访问类型。
1. （可选）在&#x200B;**P.S.**&#x200B;字段中，输入有关为何需要其他访问权限的注释。

   ![请求访问对话框](assets/request-access-to-project.png)

1. 单击&#x200B;**请求访问**。

<!--
If you do not have access level rights to an object and you try to access that object from a link, a screen is displayed informing you to contact the Workfront administrator.

For example, if you do not have portfolio access, but you were given a link to a portfolio, you would see the following message:  
![](assets/permission-request-initial2-350x96.png)
-->

### 请求附加访问权限 {#request-additional-access}

要请求对已有限访问权限的对象的附加访问权限，请执行以下操作：

1. 转到要请求附加访问权限的对象。

1. 单击项目名称右侧的&#x200B;**更多**&#x200B;菜单，然后单击&#x200B;**请求更多访问权限**。

   ![请求更多访问权限](assets/more-menu-request-more-access.png)

1. （视情况而定）如果多个用户具有授予您额外访问权限的相应访问权限，则用户名称旁边会显示一个下拉箭头。 从下拉列表中选择将收到访问请求的用户。

   下拉列表中只显示10个用户，该列表按字母顺序排序。 有关此下拉菜单中列出用户顺序的更多信息，请参阅“请求访问”和“请求更多访问”下拉菜单的[层次结构](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus)。

1. 从下拉列表中，选择您请求的访问级别。
1. （可选）在&#x200B;**P.S.**&#x200B;字段中，输入有关为何需要其他访问权限的注释。

   ![请求访问对话框](assets/request-access-to-project.png)

1. 单击&#x200B;**请求访问**。

## 请求访问和请求更多访问下拉菜单的层次结构 {#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus}

* [了解“请求访问”和“请求更多访问”下拉菜单中列出的用户层次结构](#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus)
* [了解对象的所有者](#understand-the-owner-of-an-object)

### 了解“请求访问”和“请求更多访问”下拉菜单中列出的用户层次结构 {#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus}

在填充对象的“请求访问”或“请求更多访问”列表时，Workfront会选择最多10个用户的列表，这些用户履行各种职责，可以为请求访问的用户授予对象访问权限。 随后，生成的列表将按其名称的字母升序排序。

请求访问或请求更多访问下拉列表中的用户顺序由以下规则决定：

* 列表中的第一个用户是对象“所有者”，如[了解对象的所有者](#understand-the-owner-of-an-object)中所述。
* 随后，该列表将填充单独共享该对象的用户。 它们按字母顺序列出。
* 随后，该列表中还会进一步填充用户，这些用户可通过与其团队、组或公司共享来获取所需的访问权限。 它们按字母顺序列出。
* 如果列表为空，则会添加Workfront管理员，以便始终有可向其请求访问权限的人员。 它们按字母顺序列出。
* 列表中的每个用户都必须具有所请求的对象访问权限和共享对象的权限。

### 了解对象的所有者 {#understand-the-owner-of-an-object}

对象的所有者的定义如下：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>对象</strong> </th> 
   <th><strong>对象所有者的定义</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>项目</td> 
   <td>所有者是项目所有者，或者如果缺少项目所有者或项目所有者没有所需访问权限，则是父项目组合的所有者。 <p>他们可能与项目创建者不同。 </p></td> 
  </tr> 
  <tr> 
   <td>任务</td> 
   <td>所有者是主要受分配人，或者如果主要受分配人缺失或他们无权访问，则为任务所在项目的所有者（如上所述）。 <p>他们可能与任务创建者不同。 </p></td> 
  </tr> 
  <tr> 
   <td>问题</td> 
   <td> <p>所有者是问题的主要联系人，如果问题缺失或所有者没有必要访问权限，则为问题所在项目的所有者（如上所述）。 </p> <p>他们可能与问题创建者不同。 </p> </td> 
  </tr> 
  <tr> 
   <td>项目组合</td> 
   <td>该所有者是Portfolio所有者。 <p>他们可能与项目组合创建者不同。 </p></td> 
  </tr> 
  <tr> 
   <td>文档</td> 
   <td>所有者是文档的所有者（上传文档的用户），如果文档丢失或他们无权访问，则为文档所在对象的所有者。</td> 
  </tr> 
  <tr> 
   <td>报告和仪表板</td> 
   <td>所有者是报告或仪表板的创建者。 </td> 
  </tr> 
  <tr> 
   <td>日程表</td> 
   <td>所有者是日历的创建者。 默认情况下，所有用户均有分配给他们的日历。 他们被视为该日历的所有者。 </td> 
  </tr> 
  <tr> 
   <td>过滤器、视图和分组</td> 
   <td>过滤器、视图或分组的所有者是创建者。 </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><span>计划</span> </td> 
   <td> <p><span>所有者是计划的创建者。</span> </p> <p>这需要额外的许可证。 </p> <p><span>有关Workfront Scenario Planner的信息，请参阅</span> <a href="../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Scenario Planner概述</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>目标</td> 
   <td> <p>所有者是指定为所有者的用户。 他们可能与目标创建者不同。 </p> <p>这需要额外的许可证。 </p> <p>有关Workfront目标的信息，请参阅<a href="../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Adobe Workfront目标概述</a>。 </p> </td> 
  </tr> 
 </tbody> 
</table>


