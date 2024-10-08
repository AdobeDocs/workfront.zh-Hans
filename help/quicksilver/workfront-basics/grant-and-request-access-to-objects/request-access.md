---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: 请求访问对象
description: 您对Adobe Workfront中对象的可见性取决于您对该类型对象的访问权限以及您对单个对象的权限。
author: Alina
feature: Get Started with Workfront
exl-id: ad1c525c-42a8-4fb7-a2cd-7792e1c280ab
source-git-commit: 73f339b54985b725f265d582992a43b9f80dbd7c
workflow-type: tm+mt
source-wordcount: '1416'
ht-degree: 0%

---

# 请求访问对象

您对Adobe Workfront中对象的可见性取决于您对该类型对象的访问权限以及您对单个对象的权限。

>[!NOTE]
>
>本文介绍了如何请求对所有对象的权限，以下对象除外：
>
>* Adobe Workfront Scenario Planner中的Scenario Planner计划。 有关详细信息，请参阅[在Scenario Planner](../../scenario-planner/request-access-to-plan.md)中请求对计划的访问权限。 这需要额外的许可证。
>
>* Workfront Planning中的视图和工作区。 有关详细信息，请参阅[在Adobe Workfront Planning中共享权限概述](/help/quicksilver/planning/access/sharing-permissions-overview.md)。


Workfront管理员会配置您对访问级别中某类对象的访问权限。 有关详细信息，请参阅[访问级别和权限如何协同工作](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md)。

如果您需要拥有Workfront中特定对象的权限，则可以请求对这些对象的访问权限。 您可以请求在Workfront中附加访问（或权限），而不是向Workfront管理员或对象所有者发送电子邮件来解释您的需求。

如果有人与您共享指向对象的链接，则您可以请求对对象的初始访问权限，或者您可以请求对您至少查看过的对象的附加访问权限。

例如，您可能具有某个项目的查看权限，但您需要将任务添加到该项目。 在这种情况下，您可以请求项目的Contribute权限。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

要共享对象，必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>新增：标准</p> 
   <p>当前：工作或更高</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>查看您请求权限对象的访问权限或更高</p> </td> 
  </tr> 
 </tbody> 
</table>

*有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 了解标准共享规则

以下标准共享规则在您的Workfront系统中设置为默认选项后，会自动生效。

* 分配给任务或问题的用户具有其Contribute访问权限。
* 项目、Portfolio和项目群经理对其拥有的对象具有管理访问权限。
* 对话中包含的用户对对话发生的对象具有查看访问权限。
* 分配为批准者的用户对等待批准的对象具有查看权限。
* 共享功能板时，该功能板上的所有报告也将以相同的访问权限共享给相同的用户。
* 对象所有者无法将访问权限扩展到超出其对该对象的访问权限（如管理员所定义）。

## 请求访问

您可以请求对当前无权访问的对象的初始访问权限，也可以请求对您只有有限访问权限的对象的附加访问权限。

* [请求初始访问](#request-initial-access)
* [请求附加访问权限](#request-additional-access)

### 请求初始访问  {#request-initial-access}

如果您还不能访问某个对象，而您是通过链接导航到该对象的，则会显示一个屏幕，通知您无权查看该信息。

要请求对对象的初始访问权限，请执行以下操作：

1. 单击&#x200B;**请求访问**。\
   显示&#x200B;**请求访问**&#x200B;对话框。

1. （视情况而定）如果多个用户具有授予您额外访问权限的相应访问权限，则用户名称旁边会显示一个下拉箭头。
1. 从下拉列表中选择要接收访问请求的用户。\
   下拉列表中只显示10个用户。 该列表按字母顺序排序。\
   有关此下拉菜单中列出用户顺序的更多信息，请参阅“请求访问”和“请求更多访问”下拉菜单的[层次结构](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus)。

1. 从下拉列表中，选择您请求的访问类型。
1. （可选）在&#x200B;**P.S.**&#x200B;字段中，为用户指定一个注释，说明您需要额外访问权限的原因。

   ![](assets/request-access-dialog-350x314.png)

如果您没有对象的访问级别权限，并且尝试从链接访问该对象，则会显示一个屏幕，通知您联系Workfront管理员。

例如，如果您没有项目组合访问权限，但是为您提供了项目组合的链接，您会看到以下消息：\
![](assets/permission-request-initial2-350x96.png)

### 请求附加访问权限 {#request-additional-access}

要请求对已有限访问权限的对象的附加访问权限，请执行以下操作：

1. 转到要请求附加访问权限的对象。

1. 单击项目名称右侧的&#x200B;**更多**&#x200B;菜单，然后单击&#x200B;**请求更多访问权限**。

   ![](assets/request-access-in-project-350x201.png)

1. （视情况而定）如果多个用户具有授予您额外访问权限的相应访问权限，则用户名称旁边会显示一个下拉箭头。
1. 从下拉列表中选择要接收访问请求的用户。\
   下拉列表中只显示10个用户。 该列表按字母顺序排序。\
   有关此下拉菜单中列出用户顺序的更多信息，请参阅“请求访问”和“请求更多访问”下拉菜单的[层次结构](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus)。

1. 从下拉列表中，选择您请求的访问级别。
1. （可选）在&#x200B;**P.S.**&#x200B;字段中，指定有关为何需要其他访问权限的注释。
1. 单击&#x200B;**请求访问**。\
   ![](assets/request-access-dialog-350x314.png)

## “请求访问”和“请求更多访问”下拉菜单的层次结构 {#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus}

* [了解“请求访问”和“请求更多访问”下拉菜单中列出的用户层次结构](#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus)
* [了解对象的所有者](#understand-the-owner-of-an-object)

### 了解“请求访问”和“请求更多访问”下拉菜单中列出的用户层次结构 {#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus}

在填充对象的“请求访问”或“请求更多访问”列表时，Workfront会选择最多十个在共享对象方面充当不同角色的用户列表，如下所述。 这些用户可以向请求该对象的用户授予对该对象的访问权限。\
然后，生成的列表将按其名称的字母升序排序。\
Workfront在“请求访问”和“请求更多访问”列表中最多显示10个用户。

“请求访问”或“请求更多访问”下拉菜单中的用户顺序由以下规则指定：

* 列表中的第一个用户是对象“所有者”，如[了解对象的所有者](#understand-the-owner-of-an-object)中所述。
* 随后，该列表将填充单独共享该对象的用户。 它们按字母顺序列出。
* 然后，该列表中进一步填充了通过与团队、组或公司共享而获得所需访问权限的用户。 它们按字母顺序列出。
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
   <td>所有者是Portfolio所有者。 <p>他们可能与项目组合创建者不同。 </p></td> 
  </tr> 
  <tr> 
   <td>文档</td> 
   <td>所有者是文档的所有者（上传文档的用户），如果文档丢失或他们无权访问，则为文档所在对象的所有者。</td> 
  </tr> 
  <tr> 
   <td>报告和仪表板</td> 
   <td>所有者是创建者、报告或仪表板。 </td> 
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


