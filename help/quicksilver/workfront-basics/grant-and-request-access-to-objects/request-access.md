---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: 请求对对象的访问
description: 您对Adobe Workfront中对象的可见性取决于您对此类型对象的访问权限以及您对单个对象的权限。
author: Alina
feature: Get Started with Workfront
exl-id: ad1c525c-42a8-4fb7-a2cd-7792e1c280ab
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '1424'
ht-degree: 0%

---

# 请求对对象的访问

您对Adobe Workfront中对象的可见性取决于您对此类型对象的访问权限以及您对单个对象的权限。

>[!NOTE]
>
>本文介绍了如何在Adobe Workfront方案规划器中请求除计划之外的所有对象的权限。 有关请求访问计划的信息，请参阅 [请求对方案计划员中计划的访问权限](../../scenario-planner/request-access-to-plan.md). 这需要额外的许可证。

Workfront管理员在访问级别中配置您对对象类型的访问权限。 有关更多信息，请参阅 [访问级别和权限如何协同工作](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

如果您需要对Workfront中的特定对象拥有权限，则可以请求对这些对象的访问权限。 您无需向Workfront管理员或对象所有者发送电子邮件以解释您的需求，而是可以在Workfront中请求其他访问（或权限）。

如果某人与您共享指向对象的链接，则可以请求对对象的初始访问权限，或者您也可以请求对您至少查看的对象的附加访问权限。

例如，您可能拥有某个项目的“查看”权限，但您需要向该项目添加任务。 在这种情况下，您可以请求对项目拥有Contribute权限。

## 访问要求

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access or higher to the objects you request permissions to</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

要共享对象，必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看对您请求权限的对象的访问权限或更高权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 了解标准共享规则

以下标准共享规则将自动生效，因为在Workfront系统中，这些规则被设置为默认选项。 

* 分配给任务或问题的用户对该任务或问题具有Contribute访问权限。 
* 项目、Portfolio和项目群经理对他们拥有的对象具有“管理”访问权限。
* 对话中包含的用户对进行对话的对象具有查看访问权限。
* 分配为批准者的用户对等待批准的对象具有查看访问权限。
* 在共享功能板时，功能板上的所有报表也会以相同访问权限共享给相同用户。 
* 对象所有者无法扩展对对象的访问权限，超出其对管理员定义的该对象的访问权限。

## 请求访问

您可以请求对您当前无权访问的对象的初始访问权限，也可以请求对您仅具有有限访问权限的对象的附加访问权限。

* [请求初始访问](#request-initial-access)
* [请求其他访问](#request-additional-access)

### 请求初始访问  {#request-initial-access}

如果您还没有对象的访问权限，并且您从链接导航到该对象，则会显示一个屏幕，通知您您无权查看信息。  

要请求对象的初始访问，请执行以下操作：

1. 单击 **请求访问**.\
   的 **请求访问** 对话框。

1. （视情况而定）如果多个用户拥有相应的访问权限以授予您附加访问权限，则用户名称旁边会显示一个下拉箭头。 
1. 从下拉列表中选择要接收访问请求的用户。\
   下拉列表中仅显示10个用户。 列表按字母顺序排序。\
   有关此下拉菜单中所列用户顺序的更多信息，请参阅  [“请求访问”和“请求更多访问”下拉菜单的层次结构](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus).

1. 从下拉列表中，选择您请求的访问类型。
1. （可选）在 **P.S.** 字段中，为用户指定有关为何需要其他访问权限的说明。

   ![](assets/request-access-dialog-350x314.png)

如果您没有对象的访问权限级别，并尝试从链接访问该对象，则会显示一个屏幕，通知您联系Workfront管理员。 

例如，如果您没有组合访问权限，但获得了指向组合的链接，则会看到以下消息：\
![](assets/permission-request-initial2-350x96.png)

### 请求其他访问 {#request-additional-access}

要请求对您已经具有有限访问权限的对象的附加访问权限，请执行以下操作：

1. 转到要请求其他访问权限的对象。

1. 单击 **更多** 菜单，然后单击 **请求更多访问权限**.\
   ![](assets/request-access-in-project-350x201.png)

1. （视情况而定）如果多个用户拥有相应的访问权限以授予您附加访问权限，则用户名称旁边会显示一个下拉箭头。
1. 从下拉列表中选择要接收访问请求的用户。\
   下拉列表中仅显示10个用户。 列表按字母顺序排序。\
   有关此下拉菜单中所列用户顺序的更多信息，请参阅  [“请求访问”和“请求更多访问”下拉菜单的层次结构](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus).

1. 从下拉列表中，选择您请求的访问级别。
1. （可选）在 **P.S.** 字段，请指定有关为什么需要其他访问权限的说明。
1. 单击 **请求访问**.\
   ![](assets/request-access-dialog-350x314.png)

## “请求访问”和“请求更多访问”下拉菜单的层次结构 {#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus}

* [了解“请求访问”和“请求更多访问”下拉菜单中列出的用户层次结构](#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus)
* [了解对象的所有者](#understand-the-owner-of-an-object)

### 了解“请求访问”和“请求更多访问”下拉菜单中列出的用户层次结构 {#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus}

在对象上填充“请求访问”或“请求更多访问”列表时，Workfront会选择一个最多十个用户的列表，这些用户在共享对象时可以履行各种角色，如下所述。 这些用户可以向请求对象的用户授予对对象的访问权限。\
然后，生成的列表按其名称以升序字母顺序排序。\
Workfront在“请求访问”和“请求更多访问”列表中最多显示10个用户。 

“请求访问”或“请求更多访问”下拉菜单中的用户顺序由以下规则决定： 

* 列表中的第一个用户是对象“所有者”，如 [了解对象的所有者](#understand-the-owner-of-an-object). 
* 然后，该列表会填充各个共享对象的用户。 按字母顺序列出。
* 然后，该列表中会进一步填充通过与团队、组或公司共享获得所需访问权限的用户。 按字母顺序列出。
* 如果列表为空，则会添加Workfront管理员，以便始终有人请求获取访问权限。 按字母顺序列出。 
* 列表中的每个用户都必须具有请求的对对象的访问权限，并有权共享该对象。 

### 了解对象的所有者 {#understand-the-owner-of-an-object}

对象的所有者定义如下：

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
   <td>所有者是项目所有者，或者，如果项目所有者缺失或者他们没有必要的访问权限，则是父项目组合的所有者。 <p>他们可能与项目创建者不同。 </p></td> 
  </tr> 
  <tr> 
   <td>任务</td> 
   <td>责任人是主要任务负责人，或者，如果主要任务负责人缺失或他们没有必要的访问权限，则任务所在项目的责任人（如上所定义）。 <p>他们可能与任务创建者不同。 </p></td> 
  </tr> 
  <tr> 
   <td>问题</td> 
   <td> <p>所有者是问题的主要联系人，或者，如果缺失该联系人或者他们没有必要的访问权限，则是问题所在项目的所有者，如上所定义。 </p> <p>他们可能与期刊创建者不同。 </p> </td> 
  </tr> 
  <tr> 
   <td>项目组合</td> 
   <td>所有者是Portfolio所有者。 <p>他们可能与组合创建者不同。 </p></td> 
  </tr> 
  <tr> 
   <td>文档</td> 
   <td>所有者是文档的所有者（上载文档的用户），或者，如果文档缺失或他们没有必要的访问权限，则是文档所在对象的所有者。</td> 
  </tr> 
  <tr> 
   <td>报表和功能板</td> 
   <td>所有者是创建者、报表或功能板。 </td> 
  </tr> 
  <tr> 
   <td>日历</td> 
   <td>所有者是日历的创建者。 所有用户都默认为其分配了日历。 他们被视为该日历的所有者。 </td> 
  </tr> 
  <tr> 
   <td>过滤器、视图和分组</td> 
   <td>过滤器、视图或分组的所有者是创建者。 </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><span>计划</span> </td> 
   <td> <p><span>所有者是计划的创建者。</span> </p> <p>这需要额外的许可证。 </p> <p><span>有关Workfront方案规划器的信息，请参阅</span> <a href="../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">方案计划员概述</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>目标</td> 
   <td> <p>所有者是指定为所有者的用户。 他们可能与目标创建者不同。 </p> <p>这需要额外的许可证。 </p> <p>有关Workfront目标的信息，请参阅 <a href="../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Adobe Workfront目标概述</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

 
