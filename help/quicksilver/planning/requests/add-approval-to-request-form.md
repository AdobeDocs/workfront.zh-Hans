---
title: 在Adobe Workfront Planning中为申请表单添加批准
description: 您可以在Adobe Workfront Planning请求表单中添加批准流程，以在创建记录之前为每个提交的请求启动批准。
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
source-git-commit: 2ffd06f2f50d14b6d33bc79c92616ebed1d58fed
workflow-type: tm+mt
source-wordcount: '1195'
ht-degree: 1%

---

# 在Adobe Workfront Planning中为申请表单添加批准

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

您可以在Adobe Workfront Planning请求表单中添加批准流程，以在创建记录之前为每个提交的请求启动批准。

本文介绍了工作区经理如何向与记录类型关联的请求表单添加批准。

有关在Workfront Planning中创建申请表单的信息，请参阅[在Adobe Workfront Planning中创建和管理申请表单](/help/quicksilver/planning/requests/create-request-form.md)。

有关向记录类型提交请求以创建记录的信息，请参阅[提交Adobe Workfront Planning请求以创建记录](/help/quicksilver/planning/requests/submit-requests.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront包</p></td> 
   <td> 
<p>任何Workfront包和任何Planning包</p>
或
<p>任何工作流包和任何计划包</p>

<p>有关每个Workfront Planning包中所包含内容的更多信息，请联系您的Workfront客户代表。</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p>标准</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>   <p>管理对工作区的权限并记录类型</a> </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>  </td> 
  </tr>  
</tbody> 
</table>

有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 有关将审批添加到请求表单的注意事项

* 您可以向请求表单添加一个或多个批准者。 您只能添加用户作为批准者。
* 对于通过提交请求表单而创建的记录，您可以在“批准者”和“批准日期”字段中显示批准信息。 有关信息，请参阅[创建字段](/help/quicksilver/planning/fields/create-fields.md)。
* 向请求表单添加多个批准者时，所有批准者都必须接受请求，然后才能在Workfront Planning中创建记录。
* 如果所有批准者都批准了该请求，则将为与请求表单关联的记录类型创建记录。
* 如果至少有一个批准者拒绝了请求，并且所有其他批准者都批准了该请求，则会在Workfront中为请求区域创建一个请求，但不会为与请求表单关联的记录类型创建记录。
* 向请求表单添加审批是可选的。 如果申请表单与批准无关，Workfront Planning会在提交申请后立即创建记录。

## 在生产环境中向请求表单添加批准

1. 开始为记录类型创建请求表单，如[在Adobe Workfront Planning中创建和管理请求表单](/help/quicksilver/planning/requests/create-request-form.md)中所述。
1. 单击&#x200B;**配置**。

   显示&#x200B;**配置**&#x200B;区域。

   ![配置选项卡](assets/configuration-tab.png)
1. 在&#x200B;**审批者**&#x200B;字段中，开始键入要设置为审批者的用户或团队的名称，然后当该名称或团队显示在列表中时将其选定。
1. （可选且有条件）如果您设置了多个审批者，并且只需要一个审批者即可做出决策，请启用&#x200B;**仅需要一个决策**&#x200B;选项。

   <!--most of the Note below is duplicated in the Create a request form article-->

   >[!NOTE]
   >
   >
   >* 您可以将一个或多个批准者添加到请求表单。
   >
   >* 如果添加多个审批人，但未启用“仅需要一个决策”选项，则所有审批人必须在Workfront Planning创建记录之前审批该请求。
   >
   >* 如果至少有一位审批者拒绝了请求，则该请求会被拒绝，并且不会创建记录。 该请求仍保留在Workfront的请求区域中。
   >
   >* 如果您添加多个审批者，但未启用“只需一个决策”选项，则所有审批者必须在请求被批准或拒绝之前做出决策。
   >
   >* 如果将团队设置为批准者，则只需从团队中做出一个决策。


1. （可选）如果您以前从未共享过该请求表单，请单击&#x200B;**发布**。

   或

   单击&#x200B;**共享**&#x200B;以共享表单，然后单击&#x200B;**复制链接**。
1. （可选）用户使用您共享的链接并提交请求后，Workfront Planning会向审批者发送审批应用程序内通知和电子邮件。

   >[!NOTE]
   >
   >   贵组织的Workfront实例必须载入到Adobe Unified Experience，用户才能接收电子邮件和应用程序内通知。


   有关批准请求的信息，请参阅[批准请求](/help/quicksilver/planning/requests/approve-request.md)。

<div class="preview">

## 将审批规则添加到请求表单

>[!NOTE]
>
>此功能仅在“预览”环境中可用。

审批规则根据已提交请求中的字段值定义审批流程。

例如，如果请求表单具有“Campaign type”字段，则可以创建一个规则，在字段的值为“Digital”时将请求发送给一个人，在字段的值为“Print”时将请求发送给另一个人。

添加审批规则时，请考虑以下事项：

* 您可以将一个或多个批准者添加到批准规则。
* 如果至少有一位审批者拒绝了请求，则该请求会被拒绝，并且不会创建记录。 该请求仍保留在Workfront的请求区域中。
* 如果您添加多个审批者，但未启用“只需一个决策”选项，则所有审批者必须在请求被批准或拒绝之前做出决策。
* 如果将团队设置为批准者，则只需从团队中做出一个决策。

有关添加审批的详细信息，请参阅[将审批添加到请求表单](/help/quicksilver/planning/requests/add-approval-to-request-form.md)。

要为请求表单设置批准规则，请执行以下操作：

1. 开始为记录类型创建请求表单，如[在Adobe Workfront Planning中创建和管理请求表单](/help/quicksilver/planning/requests/create-request-form.md)中所述。
1. 单击&#x200B;**设置**。

   此时将显示“设置”选项卡。

1. 要开始配置审批规则，请单击左侧导航中的审批![审批图标](assets/approvals-icon-on-form.png)。

1. （可选）如果要设置默认审批流程，请将至少一个用户或团队添加到默认审批规则区域的&#x200B;**审批者**&#x200B;字段中，然后单击&#x200B;**只需一个决策**&#x200B;复选框（如果要在任何默认审批者批准记录后创建记录）。

   ![默认审批规则区域](assets/default-approvers.png)

   <!--below bullet list is duplicated in the Add approval to a request form article-->

1. （可选）对于每个附加批准规则，执行以下操作：

   1. 单击&#x200B;**添加批准规则**
   1. 单击占位符标题“无标题的批准规则”并输入批准规则的名称。
   1. 单击&#x200B;**选择字段**&#x200B;并选择激活规则的字段。
   1. 选择规则的运算符。 运算符因字段类型而异。
   1. 如果选定的运算符需要一个值，请单击加号图标并添加一个或多个值。
   1. （可选）使用AND或OR添加更多条件，方法是单击添加条件并配置其他条件，如步骤C-E中所述。
   1. 在审批规则的“操作”区域的&#x200B;**审批者**&#x200B;字段中，添加至少一位满足条件时要在审批者处设置的用户或团队。
   1. &#x200B;
      1. （视情况而定）如果希望在任何一位批准者批准记录后创建记录，请选中&#x200B;**仅需要一个决策**&#x200B;复选框。

1. 单击&#x200B;**保存**&#x200B;以保存审批规则。
1. （可选）如果您以前从未共享过该请求表单，请单击&#x200B;**发布**。

</div>
