---
title: 提交Adobe Workfront规划请求
description: 当有人从Adobe Workfront Planning中的记录类型页面与您共享指向请求表单的链接后，您可以添加请求以创建与请求表单关联的记录类型的记录。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: 9b5ba629fa2f50f0425f4afbfd4faa891d917845
workflow-type: tm+mt
source-wordcount: '1000'
ht-degree: 0%

---

# 提交Adobe Workfront Planning请求以创建记录

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->
<!--take Preview and Prod references out when releasing to Prod all-->

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

当有人从Adobe Workfront Planning中的记录类型页面与您共享指向请求表单的链接后，您可以添加请求以创建与请求表单关联的记录类型的记录。

Workfront用户和外部用户可以向Planning记录类型提交请求并创建记录。<!--double check on the external users-->

本文介绍了如何提交请求以将新记录添加到记录类型。

有关工作区管理员如何创建请求表单并将其与记录类型关联的信息，请参阅[在Adobe Workfront规划中创建和管理请求表单](/help/quicksilver/planning/requests/create-request-form.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 产品</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront规划<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront计划*</p></td>
   <td>
<p>以下任意Workfront计划：</p>
<ul><li>选择</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning不适用于旧版Workfront计划</p>
   </td>
<tr>
   <td role="rowheader"><p>Adobe Workfront规划包*</p></td>
   <td>
<p>任何 </p>  
<p>有关每个Workfront计划中包括的内容的更多信息，请联系您的Workfront客户经理。 </td>
<tr>
   <td role="rowheader"><p>Adobe Workfront平台</p></td>
   <td>
<p>贵组织的Workfront实例必须载入AdobeUnified Experience，才能访问Workfront Planning的所有功能。</p>
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">AdobeWorkfront的Unified Experience</a>。 </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td>
   <td>
   <p>外部、参与者、轻度或标准许可证</p>
   <p>Workfront计划不适用于旧版Workfront许可证</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>访问级别配置</p></td>
   <td> <p>Adobe Workfront Planning没有访问级别控制</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>对象权限</p></td>
   <td>
   <p>查看工作区或更高权限(如果您是Workfront用户)</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>要访问Workfront中的Planning区域，必须为您分配一个布局模板，该模板包括主菜单中的Planning区域。 </p>
   <p> 但是，向Workfront Planning提交请求不需要访问“规划”区域。 </p>  
</td>
  </tr>
 </tbody>
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

在向Workfront Planning请求表单提交请求之前，必须满足以下条件：

* Workfront Planning中必须存在以下项：

   * 工作区
   * 与请求表单关联的记录类型。 有关信息，请参阅[在Adobe Workfront Planning中创建申请表单](/help/quicksilver/planning/requests/create-request-form.md)。

* 必须以您可以访问链接的方式与链接共享请求表单。 存在以下情况：

   * 如果您拥有Workfront帐户，则该链接仅与内部人员共享，并且您具有工作区的参与权限或更高访问权限。 Workfront外部的人员无法访问内部共享的链接。
   * 如果您没有Workfront帐户，则该链接已与外部人员共享。 Workfront用户还可以访问与外部人员共享的链接。

* 指向表单的链接不得过期。

## 有关向Workfront Planning提交请求的注意事项

* 您只能通过表单的特定链接访问Workfront Planning请求的请求表单。
* 将请求提交到Workfront Planning后无法编辑请求。
* 每个提交的请求都会为与您使用<span class="preview">的表单关联的记录类型创建记录（如果该表单未与批准关联，或者该批准已被所有批准者授予）。</span>
* 通过提交请求表单创建的记录无法与通过任何其他方法添加的记录区分开。 有关信息，请参阅[创建记录](/help/quicksilver/planning/records/create-records.md)。
* <span class="preview">已提交的请求将显示在Workfront </span>请求区域的已提交分区的“计划”选项卡中。

<!--Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some inconsistency between unified-approvals-service and intake-approvals-flow.-->


## 向Workfront Planning提交请求

1. 从Workfront Planning记录类型转到与您共享的链接。

1. 更新表单中可用的字段。 带有星号的字段为必填字段。

   >[!TIP]
   >
   >   如果&#x200B;**主题**&#x200B;字段可用，则在提交请求后，它将不会显示在Workfront Planning中。
   >
   >我们建议您更新请求中尽可能多的字段，以便在将新记录添加到Workfront Planning中的记录类型时使其可识别。

1. 单击&#x200B;**提交**。

   您的表单已提交，并且发生了以下情况：

   * 如果请求表单未与批准关联，或者<span class="preview">如果所有批准者都授予了批准，</span>将向与表单关联的记录类型添加新的记录。

   * 如果申请表单未与批准关联，则<span class="preview">申请将添加到Workfront申请区域已提交分区的Planning选项卡中，并且向记录类型页面中添加新记录。</span>

     ![](assets/planning-tab-in-requests.png)

     >[!IMPORTANT]
     >
     ><span class="preview">所有有权访问至少一个工作区的用户都可以在“请求”区域中查看“计划”选项卡。 您只能查看您或其他人提交到您至少拥有查看权限的工作区的请求。 Workfront管理员可以查看提交到系统中任何工作区的所有请求。</span> <!--ensure this is correct; asking team in slack-->

   * <span class="preview">如果申请表与批准关联，申请会暂时保存到Workfront申请区域已提交部分的Planning选项卡。 没有为与请求表单关联的记录类型创建记录。</span>

     <span class="preview">有关信息，请参阅[向请求表单添加批准](/help/quicksilver/planning/requests/add-approval-to-request-form.md)。</span>
   * <span class="preview">您收到应用内通知和电子邮件通知，告知您请求已成功提交或已发送以供审阅。</span>
   * <span class="preview">如果请求表单与批准关联，则批准者会收到应用程序内通知和电子邮件通知，以审查和批准该请求。</span>

     >[!NOTE]
     >
     ><span class="preview">仅当贵组织的Workfront实例已载入到AdobeUnified Experience时，电子邮件和应用内通知才可见。</span>




