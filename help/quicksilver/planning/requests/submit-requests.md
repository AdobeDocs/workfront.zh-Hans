---
title: 提交Adobe Workfront规划请求
description: 当有人从Adobe Workfront Planning中的记录类型页面与您共享指向请求表单的链接后，您可以添加请求以创建与请求表单关联的记录类型的记录。
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '2200'
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

Workfront用户和外部用户可以向Planning记录类型提交请求。 请求为与请求表单关联的记录类型创建记录。<!--double check on the external users-->

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
   * 记录类型
   * 与记录类型关联的请求表单。

     有关信息，请参阅[在Adobe Workfront Planning中创建申请表单](/help/quicksilver/planning/requests/create-request-form.md)。

* 必须以您可以访问的方式共享请求表单。 存在以下情况：

   * 在内部，该表单必须与对工作区具有查看或更高权限的用户共享。

     Workfront用户可以通过链接访问表单，或在Workfront的请求区域找到请求表单。

   * 从外部来看，就是通过与没有Workfront帐户的外部人员共享指向记录表单的链接。

     Workfront用户还可以访问与外部人员共享的链接。

* 如果与链接共享，则指向表单的链接不得过期。

## 有关向Workfront Planning提交请求的注意事项

* 提交请求后，无法在Workfront中编辑该请求。
* 如果表单未与批准关联，或者所有批准者都已授予批准，则每个提交的请求都会为与您使用的表单关联的记录类型创建记录。
* 通过提交请求表单创建的记录与Workfront Planning中通过任何其他方法添加的记录相同。

  有关信息，请参阅[创建记录](/help/quicksilver/planning/records/create-records.md)。
* 通过提交请求表单创建的记录将连接到原始请求。 无法删除此连接。
* 您可以在以下区域查看创建的记录以及用于创建这些记录的请求：
   * Workfront中的“请求”区域

  <div class="preview">

   * Workfront Planning中的记录类型页面
   * Workfront Planning中记录的详细信息区域

  </div>

  >[!TIP]
  >
  ><span class="preview">您可以在Workfront的请求区域的主题字段或Workfront Planning的原始请求连接字段中查看请求名称。</span>



* 已提交的请求将显示在Workfront的请求区域中。
* 提交的规划请求仅在新的请求体验中可见。 您无法在旧版请求体验中看到Planning请求。
有关信息，请参阅[创建并提交请求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)。
* 在提交表单后，某些字段类型在请求表单或请求详细信息页面中的显示方式存在限制。

  有关信息，请参阅[在Adobe Workfront Planning中创建和管理申请表单](/help/quicksilver/planning/requests/create-request-form.md)。

<!--Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some inconsistency between unified-approvals-service and intake-approvals-flow.-->


## 在Workfront的请求区域将请求提交到Workfront规划

{{step1-to-requests}}

1. 启用屏幕右上角的&#x200B;**切换到新体验**&#x200B;设置。
启用此设置可使Workfront计划请求表单在Workfront的&#x200B;**请求**&#x200B;区域中可用。

   >[!TIP]
   >
   >仅当您的Workfront实例登记到Adobe Unified Experience时，此设置才可用。
   >
   >要在此区域提交Workfront Planning请求，您必须满足以下条件：
   >
   >* 您的公司已购买Workfront Planning许可证。
   >
   >* 您有权查看至少一个工作区。

1. 单击&#x200B;**您要提交什么请求**&#x200B;栏打开请求表单列表。
1. 从列表中选择一个请求表单，或开始键入请求表单名称，然后在此表单出现在列表中时将其选定。

   此时将打开一个窗口，其中顶部显示请求表单名称。
1. 更新请求表单中可用的字段。 带有红色星号的字段为必填字段。
1. 单击&#x200B;**提交**。

   请求表单关闭，您将返回&#x200B;**请求**&#x200B;区域。

   您的表单已提交，并且发生了以下情况：

   * 如果申请表单与批准无关，申请会添加到Workfront申请区域的“申请”列表中，并在主页的“我的申请”小组件中，新记录会添加到与表单关联的记录类型中。

     以下字段在请求区域显示请求和记录信息，并在主页显示我的请求小组件：

      * **主题**：在“请求”区域中添加的原始请求的名称。 您无法从请求列表中隐藏或删除&#x200B;**主题**&#x200B;字段。
      * **创建的对象**：从请求创建的记录在Planning中的名称。
      * **对象类型**：在Planning中，根据请求创建记录的工作区和记录类型的名称。
      * **状态**：请求对象的状态。
      * **请求表单**：与Planning中的记录类型关联的请求表单的名称。

   * 如果申请表单与批准关联，则该申请会添加到“Workfront申请”区域的“申请”列表中，并且我的申请小组件的状态为“未决审阅”。 只有在批准者批准记录类型页面后，才会将新记录添加到该页面。

     有关信息，请参阅[向请求表单添加批准](/help/quicksilver/planning/requests/add-approval-to-request-form.md)。

   * <span class="preview">您可以将“原始请求连接”字段添加到Planning中的记录类型，以显示创建记录的原始请求的名称。 有关信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。</span>
   * 该请求仅对所有者、审批者和至少具有工作区查看权限的人员可见。 Workfront管理员可以查看提交到系统中任何工作区的所有请求。

   * 您会收到应用程序内和电子邮件通知，告知您请求已成功提交或已发送以供审阅。
   * 如果请求表单与批准关联，则批准者会收到应用程序内和电子邮件通知，以供审阅和批准请求。

     >[!NOTE]
     >
     >仅当贵组织的Workfront实例载入到Adobe Unified Experience时，电子邮件和应用程序内通知才可见。
     >
     >电子邮件确认或审批通知中有一个指向请求的链接。

1. （可选）在确认消息中单击&#x200B;**查看您的请求**&#x200B;以打开该请求，或单击&#x200B;**X**&#x200B;图标以关闭确认。
1. （可选）从请求列表中，执行以下任一操作：

   * 单击&#x200B;**筛选器**，开始添加条件以便在“请求”列表中查看哪些请求。

     ![在请求区域编辑筛选器](assets/filters-editing-box-in-requests-planning-tab.png)

     您可以按以下字段进行筛选：

      * **Workspace**：与请求表单关联的工作区。
      * **记录类型**：与请求表单关联的记录类型。
      * **输入日期**：提交请求的日期。
      * **请求表单**：用于提交请求的请求表单的名称。
      * **状态**：请求的状态。
      * **输入者**：添加请求的用户的名称。 如果请求是由Workfront之外的人员添加的，则&#x200B;**输入者**&#x200B;字段显示`N/A`。
      * **已创建对象状态**：已创建记录的状态。

     您可以有多个&#x200B;**And**&#x200B;或&#x200B;**Or**&#x200B;加入的筛选器。
在添加筛选条件时，将自动筛选请求列表。

   * 单击&#x200B;**列**&#x200B;打开&#x200B;**字段可见性和顺序**&#x200B;框，然后隐藏、显示或重新排列请求列表中的列。

     >[!TIP]
     >
     >您无法再添加任何列。

     请求区域中的![列编辑框](assets/columns-editing-box-in-requests-planning-tab.png)
   * 单击请求列表右上角的&#x200B;**+**&#x200B;图标以打开&#x200B;**列管理器**&#x200B;并在请求列表中添加或删除列。

1. 单击列表中的请求名称。

   此时将打开请求详细信息页面。

   ![请求带有注释的页面](assets/new-request-page-with-comment.png)

1. （可选）在&#x200B;**注释**&#x200B;区域输入注释。
1. （视情况而定）如果请求表单未与批准关联，或者请求已获批准，请单击请求的名称，然后单击&#x200B;**创建的对象**&#x200B;字段中的记录名称。

   记录页面将在Workfront Planning中打开。

   >[!TIP]
   >
   >* 如果请求表单中未更新记录的主要字段，则请求的“记录”字段中的记录名称将显示为&#x200B;**无标题**。
   >
   >* 如果请求表单与批准关联，则必须先获得批准，然后才能从请求页面访问记录。

1. （可选）单击&#x200B;**记录类型**&#x200B;的名称。

   此时将在Workfront Planning中打开记录类型页面。

## 通过共享链接将请求提交到Workfront Planning的请求表单

此部分中的信息仅适用于从共享链接提交请求的Workfront用户。 外部人员无法访问Workfront内部区域，如请求或主页。

1. 从Workfront Planning记录类型转到与您共享的链接。

1. 更新表单中可用的字段。 带有星号的字段为必填字段。

   >[!TIP]
   >
   >   如果&#x200B;**主题**&#x200B;字段可用，则在提交请求后，它将不会显示在Workfront Planning中。
   >
   >我们建议您更新请求中尽可能多的字段，以便在将新记录添加到Workfront Planning中的记录类型时使其可识别。

1. 单击&#x200B;**提交**。

   您的表单已提交，并且发生了以下情况：

   * 如果申请表单与批准无关，申请会添加到Workfront申请区域的“申请”列表中，并在主页的“我的申请”小组件中，新记录会添加到与表单关联的记录类型中。

   * 如果申请表单与批准关联，则该申请会添加到“Workfront申请”区域和“我的申请”小组件的“申请”列表中。 只有在所有批准者都批准记录类型后，才会将新记录添加到该记录类型页面。

     有关信息，请参阅[向请求表单添加批准](/help/quicksilver/planning/requests/add-approval-to-request-form.md)。

     >[!IMPORTANT]
     >
     >您只能查看您或其他人提交到您至少拥有查看权限的工作区的请求。 Workfront管理员可以查看提交到系统中任何工作区的所有请求。<!--ensure this is correct; asking team in slack-->

   * 您会收到应用程序内和电子邮件通知，告知您请求已成功提交或已发送以供审阅。
   * 如果请求表单与批准关联，则批准者会收到应用程序内和电子邮件通知，以供审阅和批准请求。

     >[!NOTE]
     >
     >仅当贵组织的Workfront实例载入到Adobe Unified Experience时，电子邮件和应用程序内通知才可见。

   <!-- <span class="preview"> After the request was approved and the record was created, the Approved by and Approved date fields display information about the approval on the record.</span>-->

1. （可选）单击&#x200B;**查看您的请求**&#x200B;以在Workfront中打开该请求。

   <!--Or-->

   <!--Click [Submit another request](https://pulsar.devtest.workfront-dev.com/intake/6740a1ff44bf3a5600cf4481/request) to open the request form and add a new request.-->

1. （可选）单击&#x200B;**主菜单** > **请求**&#x200B;以查看您的请求，然后单击请求的名称。

   此时将打开请求详细信息页面。

   ![请求带有注释的页面](assets/new-request-page-with-comment.png)

1. （可选）在“注释”(Comments)区域输入注释。
1. （视情况而定）如果请求表单未与批准关联，或者请求已获批准，请单击请求的名称，然后单击&#x200B;**创建的对象**&#x200B;字段中的记录名称。

   记录页面将在Workfront Planning中打开。

   >[!TIP]
   >
   >* 如果记录名称未添加到请求表单，则请求的“记录”字段中记录的名称将显示为&#x200B;**无标题**。
   >
   >* 如果请求表单与批准关联，则必须先获得批准，然后才能从请求页面访问记录。

1. （可选）单击&#x200B;**对象类型**&#x200B;的名称。

   此时将在Workfront Planning中打开记录类型页面。

## 通过复制现有请求创建请求

您可以在Workfront的请求列表中复制请求，然后编辑详细信息并将其作为新请求提交。

这仅在新的请求体验中可用。

有关说明，请参阅[复制并提交请求](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md)。

## 从现有草稿创建草稿和请求

您可以创建请求的草稿，然后返回草稿并稍后作为请求提交。

这仅在新的请求体验中可用。

有关说明，请参阅[从草稿创建请求](/help/quicksilver/manage-work/requests/create-requests/create-requests-from-drafts.md)。



