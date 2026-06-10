---
product-area: programs
navigation-topic: create and manage programs
title: 将现有项目添加到Portfolio
description: 您可以将现有项目添加到项目组合。 由于程序不能存在于两个不同的项目组合中，因此添加现有程序会将其从一个项目组合永久移动到另一个项目组合。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 73dbe277-12d2-4041-8a02-91ccf5f8b465
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/LkyWuPHqv0muTinWZT1PMKPGUNErWulIIxHmXVtPIVg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: c6b02fbaf2ee03728543c9d34068e4dd353ac441
workflow-type: tm+mt
source-wordcount: 382
ht-degree: 3%

---

# 将现有项目群添加到项目组合

<!--Audited: 05/2026-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release. </span>   

<span class="preview">For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). </span>
-->

您可以将现有项目添加到项目组合。 由于程序不能存在于两个不同的项目组合中，因此添加现有程序会将其从一个项目组合永久移动到另一个项目组合。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 包</td> 
   <td> <p>“任一”</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td> <p>[!UICONTROL 标准版]</p><p>[!UICONTROL 计划]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>[!UICONTROL Edit]对[!UICONTROL 项目组合]和[!UICONTROL 项目]的访问权限 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>项目组合和项目群的[!UICONTROL Manage]权限</p> </td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>New: [!UICONTROL Standard] </p><p>Or </p><p>Current: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL Edit] access to Portfolios and Programs </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions to the portfolio and the program</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## 将现有项目群添加到项目组合

>[!NOTE]
>
>当您的组织同时使用旧版Workfront和Adobe云存储来存储文档时，将会出现以下情况：
>
>
>* 当您将Adobe云存储程序添加到旧版Workfront存储产品组合，并且该产品组合没有附加任何文档时，该项目组合将转换为Adobe云存储。
>* 当您将Adobe云存储程序添加到旧版Workfront存储产品组合，并且该产品组合具有附加文档时，该产品组合文档存储仍保留在Workfront存储上。 但是，从产品组合中删除了旧版Workfront存储图标![旧版Workfront存储图标](assets/legacy-storage-project-icon.png)。
>* 您不能将旧版Workfront存储程序添加到Adobe云存储产品组合。
>
>有关详细信息，请参阅[项目和相关对象的文档管理概述](/help/quicksilver/manage-work/projects/manage-projects/manage-documents-on-projects.md)。
>
>并非所有Workfront实例都具有这两种类型的文档存储。

<!--
For preview/ Prod. release, rewrite the bullets above:
* You cannot add an Adobe cloud storage program to a Legacy storage portfolio, or a Legacy program to an Adobe cloud storage portfolio.
-->

要将现有项目添加到另一个项目组合，请执行以下操作：

1. 转到项目组合，然后单击左侧面板中的&#x200B;**[!UICONTROL 程序]**。
1. 单击&#x200B;**[!UICONTROL 新建项目]**。
1. 单击&#x200B;**[!UICONTROL 现有计划]**。

   将打开&#x200B;**添加程序**&#x200B;框。<!--check screen shot - I logged changes for this casing-->

   ![添加程序框](assets/add-programs-box.png)

   >[!IMPORTANT]
   >
   >添加现有项目群会将与该项目群关联的所有项目纳入项目组合。 请注意不要无意间以这种方式移动项目。

1. 在&#x200B;**[!UICONTROL 将程序添加到此项目组合]**&#x200B;字段中，键入程序的名称，然后当程序显示在列表中时将其选定。<!--see the name of this field, I suggested changes here-->

   您可以添加多个项目。

1. （可选）如果您决定不将其添加到项目组合，请单击项目名称旁边的&#x200B;**删除**&#x200B;图标![删除图标](assets/delete-icon.png)。

1. 单击&#x200B;**[!UICONTROL 添加程序]**。

   项目群显示在所选项目组合的&#x200B;**[!UICONTROL 项目群]**&#x200B;选项卡中。

