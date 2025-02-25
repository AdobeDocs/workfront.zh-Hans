---
title: 提交Adobe Workfront规划请求
description: 当有人从Adobe Workfront Planning中的记录类型页面与您共享指向请求表单的链接后，您可以添加请求以创建与请求表单关联的记录类型的记录。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: f3f33d870859408db5ec3dc306cf1d4209c126a3
workflow-type: tm+mt
source-wordcount: '1017'
ht-degree: 0%

---

# 提交Adobe Workfront Planning请求以创建记录

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->
<!--take Preview and Prod references out when releasing to Prod all-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

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
<p>贵组织的Workfront实例必须载入Adobe Unified Experience，才能访问Workfront Planning的所有功能。</p>
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">适用于Workfront的Adobe Unified Experience</a>。 </p>
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
* 如果表单与批准无关，或者所有批准者都授予了批准，则每个提交的请求都会为您使用的表单创建的记录类型创建记录。
* 通过提交请求表单创建的记录无法与通过任何其他方法添加的记录区分开。 有关信息，请参阅[创建记录](/help/quicksilver/planning/records/create-records.md)。
* 已提交的请求将显示在Workfront请求区域的已提交分区的计划选项卡中。

<!--Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some inconsistency between unified-approvals-service and intake-approvals-flow.-->


## 向Workfront Planning提交请求

<!--
<div class="preview">

Submitting requests to Workfront Planning differs depending on what environment you use. 

### Submit a request to Workfront Planning in the Preview Environment

>[!NOTE]
>
>After the monthly releases to Production, the features described in this section are also available in the Production environment for customers who enabled fast releases.

{{step1-to-requests}}

1. Enable the **Switch to a new experience** setting, in the upper-right corner of he screen. 
   Enabling this setting makes the Workfront Planning request forms available in the **Requests** area of Workfront.

   >[!TIP]
   >
   >   This setting is available only when your company has purchased a Workfront Planning package. 

1. Click **New request**. (********* update scree shot at release ********)

   ![New request box with unified Workfront and Planning cards](assets/new-request-box-with-unified-workfront-and-planning-cards.png)

   The New request area opens with the following information: 

   * The 6 most recently accessed Workfront request queues and Planning request forms display in the Recent section. 
   * 50 additional Workfront request queues and Planning request forms display in alphabetical order in the **All request forms** section. You can search for a request queue that does not display by default. 

1. Do one of the following:

   * Click the card for one of the Planning request forms in the Recent or All request forms sections
   * Start typing the name of a Planning request form in the search box, then click the card when it displays in the list. 

   The request form opens.

1. Update the fields available in the request form. Fields with a red asterisk are required. 
1. Click **Submit**.
    
   The request form closes and you return to the **Requests** area. 

   Your form is submitted and the following things occur:

   * If the request form was not associated with an approval, the request is added to the Planning tab of the Submitted section of the Workfront Requests area and a new record is added to the record type associated with the form.
   
   * If the request form was associated with an approval, the request is added to the Planning tab of the Submitted section of the Workfront Requests area. A new record is added to the record type page only after all the approvers have approved it.
   
      For information, see [Add an approval to a request form](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

      ![](assets/requests-area-with-toggle-for-unified-workflow-planning-tab-open.png)

      >[!IMPORTANT]
      >
      >All users who have access to at least one workspace can view the Planning tab in the Requests area. You can view only the requests submitted by you or anyone else to the workspaces that you have at least permissions to View. Workfront administrators can view all requests submitted to any workspace in the system. (******** ensure this is correct; asking team in slack **************)

   * You receive an in-app and an email notification that the request has either been submitted successfully or has been sent for review.
   * If the request form was associated with an approval, the approvers receive an in-app and an email notification to review and approve the request.

      >[!NOTE]
      >
      >The email and in-app notifications are visible only when your organization's instance of Workfront is onboarded to the Adobe Unified Experience.

1. (Optional) Click the **Planning** tab in the Requests area to view your request. 
1. (Conditional) If the request form is not associated with an approval, or if the request has been approved, click the name of the request, then click the name of the record in the **Record** field. 

   The record's page opens. 

   >[!TIP]
   >
   >* If the record name was not added to the request form, the name of the record in the Record field of the request displays as **Untitled**. 
   >
   >* If the request form is associated with an approval, the approval must be granted before you can access the record from the request page. 

</div>

### Submit a request to Workfront Planning in the Production environment

-->

1. 从Workfront Planning记录类型转到与您共享的链接。

1. 更新表单中可用的字段。 带有星号的字段为必填字段。

   >[!TIP]
   >
   >   如果&#x200B;**主题**&#x200B;字段可用，则在提交请求后，它将不会显示在Workfront Planning中。
   >
   >我们建议您更新请求中尽可能多的字段，以便在将新记录添加到Workfront Planning中的记录类型时使其可识别。

1. 单击&#x200B;**提交**。

   您的表单已提交，并且发生了以下情况：

   * 如果申请表单与批准无关，申请会添加到Workfront申请区域已提交分区的Planning选项卡中，新记录会添加到与表单关联的记录类型中。

   * 如果申请表单与批准关联，则该申请会添加到Workfront申请区域已提交部分的Planning选项卡中。 只有在所有批准者都批准记录类型后，才会将新记录添加到该记录类型页面。

     有关信息，请参阅[向请求表单添加批准](/help/quicksilver/planning/requests/add-approval-to-request-form.md)。

     ![](assets/planning-tab-in-requests.png)

     >[!IMPORTANT]
     >
     >至少有权访问一个工作区的所有用户都可以查看请求区域中的Planning选项卡。 您只能查看您或其他人提交到您至少拥有查看权限的工作区的请求。 Workfront管理员可以查看提交到系统中任何工作区的所有请求。<!--ensure this is correct; asking team in slack-->

   * 您会收到应用程序内和电子邮件通知，告知您请求已成功提交或已发送以供审阅。
   * 如果请求表单与批准关联，则批准者会收到应用程序内和电子邮件通知，以供审阅和批准请求。

     >[!NOTE]
     >
     >仅当贵组织的Workfront实例载入到Adobe Unified Experience时，电子邮件和应用程序内通知才可见。

1. （可选）单击“请求”区域中的&#x200B;**计划**&#x200B;选项卡以查看您的请求。
1. （视情况而定）如果请求表单未与批准关联，或者请求已获批准，请单击请求的名称，然后单击&#x200B;**记录**&#x200B;字段中的记录名称。

   此时将打开记录的页面。

   >[!TIP]
   >
   >* 如果记录名称未添加到请求表单，则请求的“记录”字段中记录的名称将显示为&#x200B;**无标题**。
   >
   >* 如果请求表单与批准关联，则必须先获得批准，然后才能从请求页面访问记录。




