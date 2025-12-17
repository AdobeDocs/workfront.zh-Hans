---
title: 提交Adobe Workfront规划请求
description: 当有人从Adobe Workfront Planning中的记录类型页面与您共享指向请求表单的链接后，您可以添加请求以创建与请求表单关联的记录类型的记录。
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: 5b1993d49ff675b3bab1d470bc756b987fe19d1c
workflow-type: tm+mt
source-wordcount: '1945'
ht-degree: 0%

---

# 提交Adobe Workfront Planning请求以创建记录

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->
<!--take Preview and Prod references out when releasing to Prod all-->

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

工作区管理员在Adobe Workfront Planning中为记录类型构建请求表单后，您可以使用该表单提交将创建与表单关联的记录类型记录的请求。

您可以从以下区域提交Workfront Planning请求：

* 从Workfront的请求区域。
* 从已共享请求表单的直接链接。
* 在记录类型页面中添加或请求新记录时。 有关信息，请参阅[创建记录](/help/quicksilver/planning/records/create-records.md)。

本文介绍了如何提交请求，以从Workfront的“请求”区域或共享链接向记录类型添加新记录。


Workfront用户和外部用户可以向Planning记录类型提交请求并创建记录。<!--double check on the external users-->

有关工作区管理员如何创建请求表单并将其与记录类型关联的信息，请参阅[在Adobe Workfront规划中创建和管理请求表单](/help/quicksilver/planning/requests/create-request-form.md)。

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
   <td><p>任何</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>   <p>查看或更高权限的工作区和记录类型(如果您是Workfront用户)</p>  </td> 
  </tr>  
</tbody> 
</table>

有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

在向Workfront Planning请求表单提交请求之前，必须满足以下条件：

* Workfront Planning中必须存在以下项：

   * 工作区
   * 记录类型。
   * 与记录类型关联的请求表单。

     有关信息，请参阅[在Adobe Workfront Planning中创建申请表单](/help/quicksilver/planning/requests/create-request-form.md)。

* 必须以您可以访问的方式共享请求表单。 存在以下情况：

   * 在内部，该表单必须与对工作区具有查看或更高权限的用户共享。

     Workfront用户可以通过链接访问表单，或在Workfront的请求区域找到请求表单。

   * 如果您没有Workfront帐户，则会与外部人员共享指向该表单的链接。

     Workfront用户还可以访问与外部人员共享的链接。

* 指向表单的链接不得过期。

## 有关向Workfront Planning提交请求的注意事项

* 提交请求后，无法在Workfront中编辑该请求。
* 如果表单未与批准关联，或者所有批准者都已授予批准，则每个提交的请求都会为与您使用的表单关联的记录类型创建记录。
* 在Workfront Planning中，通过提交请求表单创建的记录无法与通过任何其他方法添加的记录区分开来。

  有关信息，请参阅[创建记录](/help/quicksilver/planning/records/create-records.md)。
* 已提交的请求将显示在Workfront请求区域的已提交分区的计划选项卡中。
* 在提交表单后，某些字段类型在请求表单或请求详细信息页面中的显示方式存在限制。

  有关信息，请参阅[在Adobe Workfront Planning中创建和管理申请表单](/help/quicksilver/planning/requests/create-request-form.md)。

<!--Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some inconsistency between unified-approvals-service and intake-approvals-flow.-->


## 在Workfront的请求区域将请求提交到Workfront规划

{{step1-to-requests}}

1. 启用屏幕右上角的&#x200B;**切换到新体验**&#x200B;设置。
启用此设置可使Workfront计划请求表单在Workfront的&#x200B;**请求**&#x200B;区域中可用。

   >[!TIP]
   >
   >仅当满足以下条件时，此设置才可用：
   >
   >* 您的公司已购买Workfront规划包。
   >* 您的Workfront实例已载入到Adobe Unified Experience。
   >* 您有权查看至少一个工作区。
   >

<!--Production-->

1. 在生产环境中，单击&#x200B;**新请求**。

   <!--![New request box with unified Workfront and Planning cards](assets/new-request-box-with-unified-workfront-and-planning-cards.png-->

   打开&#x200B;**新请求**&#x200B;框，其中包含以下信息：

   * 最近访问的6个Workfront请求队列和Planning请求表单将显示在“最近”部分中。
   * 另外50个Workfront请求队列和计划请求表单按字母顺序显示在&#x200B;**所有请求表单**&#x200B;部分中。 您可以搜索默认不显示的请求队列。

1. 从最近访问的请求表单区域中选择一个请求表单或队列，或者在列表中开始键入该表单或队列名称，然后在该表单或队列出现时将其选定。

1. 更新请求表单中可用的字段。 带有红色星号的字段为必填字段。
1. 单击&#x200B;**提交**。

   请求表单关闭，您将返回&#x200B;**请求**&#x200B;区域。

   您的表单已提交，并且发生了以下情况：

   * 如果申请表单与批准无关，申请会添加到Workfront申请区域已提交分区的Planning选项卡中，新记录会添加到与表单关联的记录类型中。

   * 如果申请表单与批准关联，则该申请会添加到Workfront申请区域已提交部分的Planning选项卡中。 只有在所有批准者都批准记录类型后，才会将新记录添加到该记录类型页面。

     有关信息，请参阅[向请求表单添加批准](/help/quicksilver/planning/requests/add-approval-to-request-form.md)。

     ![带有统一工作流计划选项卡切换的“请求”区域](assets/requests-area-with-toggle-for-unified-workflow-planning-tab-open.png)

     >[!IMPORTANT]
     >
     >至少有权访问一个工作区的所有用户都可以查看请求区域中的Planning选项卡。 您只能查看您或其他人提交到您至少拥有查看权限的工作区的请求。 Workfront管理员可以查看提交到系统中任何工作区的所有请求。

   * 该请求仅对所有者、审批者和至少具有工作区查看权限的人员可见。

   * 您会收到应用程序内和电子邮件通知，告知您请求已成功提交或已发送以供审阅。
   * 如果请求表单与批准关联，则批准者会收到应用程序内和电子邮件通知，以供审阅和批准请求。

     >[!NOTE]
     >
     >仅当贵组织的Workfront实例载入到Adobe Unified Experience时，电子邮件和应用程序内通知才可见。
     >
     >电子邮件确认或审批通知中有一个指向请求的链接。

1. （可选）在确认消息中单击&#x200B;**查看您的请求**&#x200B;以打开该请求，或单击&#x200B;**X**&#x200B;图标以关闭确认。

1. （可选）单击&#x200B;**请求**&#x200B;区域中的&#x200B;**计划**&#x200B;选项卡以查看您的请求。
提交至Planning请求表单的所有您有权查看的请求都会显示在列表中。
1. （可选）执行以下任一操作：

   * 单击&#x200B;**筛选器**，开始为要在“规划”选项卡中查看的请求添加条件。

     ![在Planning请求选项卡中编辑筛选器](assets/filters-editing-box-in-requests-planning-tab.png)

     您可以按以下字段进行筛选：

      * **Workspace**：与请求表单关联的工作区。
      * **记录类型**：与请求表单关联的记录类型。
      * **输入日期**：提交请求的日期。
      * **请求表单**：用于提交请求的请求表单的名称。
      * **状态**：请求的状态。
      * **输入者**：添加请求的用户的名称。 如果请求是由Workfront之外的人员添加的，则&#x200B;**输入者**&#x200B;字段显示`N/A`。

        您可以有多个&#x200B;**And**&#x200B;或&#x200B;**Or**&#x200B;加入的筛选器。
在添加筛选条件时，将自动筛选请求列表。

   * 单击&#x200B;**列**&#x200B;并隐藏、显示或重新排列请求列表中的列。

     >[!TIP]
     >
     >您无法再添加任何列。
     >
     >您无法显示&#x200B;**主题**&#x200B;字段。

     ![](assets/columns-editing-box-in-requests-planning-tab.png)


1. 单击列表中的请求名称。

   此时将打开请求详细信息页面。

   ![请求带有注释的页面](assets/new-request-page-with-comment.png)

1. （可选）在“注释”(Comments)区域输入注释。
1. （视情况而定）如果请求表单未与批准关联，或者请求已获批准，请单击请求的名称，然后单击&#x200B;**记录**&#x200B;字段中的记录名称。

   记录页面将在Workfront Planning中打开。

   >[!TIP]
   >
   >* 如果请求表单中未更新记录的主要字段，则请求的“记录”字段中的记录名称将显示为&#x200B;**无标题**。
   >
   >* 如果请求表单与批准关联，则必须先获得批准，然后才能从请求页面访问记录。

1. （可选）单击&#x200B;**记录类型**&#x200B;的名称。

   此时将在Workfront Planning中打开记录类型页面。

## 通过共享链接将请求提交到Workfront Planning的请求表单

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

     请求中的![计划选项卡](assets/planning-tab-in-requests.png)

     >[!IMPORTANT]
     >
     >至少有权访问一个工作区的所有用户都可以查看请求区域中的Planning选项卡。 您只能查看您或其他人提交到您至少拥有查看权限的工作区的请求。 Workfront管理员可以查看提交到系统中任何工作区的所有请求。<!--ensure this is correct; asking team in slack-->

   * 您会收到应用程序内和电子邮件通知，告知您请求已成功提交或已发送以供审阅。
   * 如果请求表单与批准关联，则批准者会收到应用程序内和电子邮件通知，以供审阅和批准请求。

     >[!NOTE]
     >
     >仅当贵组织的Workfront实例载入到Adobe Unified Experience时，电子邮件和应用程序内通知才可见。

   * <span class="preview">在请求获得批准并创建记录后，“批准者”和“已批准”日期字段显示有关记录上批准的信息。</span>

1. （可选）单击&#x200B;**查看您的请求**&#x200B;以在Workfront中打开该请求。

   <!--Or-->

   <!--Click [Submit another request](https://pulsar.devtest.workfront-dev.com/intake/6740a1ff44bf3a5600cf4481/request) to open the request form and add a new request.-->

1. （可选）单击&#x200B;**主菜单** > **请求** > **计划**&#x200B;选项卡以查看您的请求，然后单击请求的名称。

   此时将打开请求详细信息页面。

   ![请求带有注释的页面](assets/new-request-page-with-comment.png)



1. （可选）在“注释”(Comments)区域输入注释。
1. （视情况而定）如果请求表单未与批准关联，或者请求已获批准，请单击请求的名称，然后单击&#x200B;**记录**&#x200B;字段中的记录名称。

   记录页面将在Workfront Planning中打开。

   >[!TIP]
   >
   >* 如果记录名称未添加到请求表单，则请求的“记录”字段中记录的名称将显示为&#x200B;**无标题**。
   >
   >* 如果请求表单与批准关联，则必须先获得批准，然后才能从请求页面访问记录。

1. （可选）单击&#x200B;**记录类型**&#x200B;的名称。

   此时将在Workfront Planning中打开记录类型页面。




