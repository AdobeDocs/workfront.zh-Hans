---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: 在Adobe Workfront中列出具有验证许可证的用户
description: 您可以查看哪些用户当前在Adobe Workfront中通过下列任一方式启用了“用户可以生成验证”选项。
author: Courtney
feature: Digital Content and Documents
exl-id: 4d45ecd9-4348-43a4-9fa7-090b996b4695
TQID: https://experienceleague.adobe.com/9P5Bp9TrJ1ECSwpK7C4AW4rQlTQOBH4U7-CPYl92RKU
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 312
ht-degree: 6%

---

# 在Adobe Workfront中列出具有验证许可证的用户

您可以查看哪些用户当前在Adobe Workfront中通过下列任一方式启用了“用户可以生成验证”选项。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>“任一”</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> 
   <p>标准</p> 
   <p>规划</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>编辑以下项的访问权限：</p> 
    <ul> 
     <li> <p>创建报告、功能板和日历</p> </li> 
     <li> <p>创建筛选器、视图和分组</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 创建用户报告

您可以创建用户报告，以查看哪些用户可以生成验证：

1. 导航到&#x200B;**报告**&#x200B;区域。
1. 单击&#x200B;**新建报表**&#x200B;下拉菜单，然后单击&#x200B;**用户报表**。

1. 在&#x200B;**筛选器**&#x200B;选项卡上，单击&#x200B;**添加筛选器规则**。

1. 在可用字段中，展开&#x200B;**用户**，然后单击&#x200B;**拥有证明许可证**。

1. 选择&#x200B;**等于** > **True**。

   ![report_proflicenses.png](assets/report-prooflicenses-350x135.png)

1. 单击&#x200B;**保存+关闭**。

   报表会显示Workfront中分配了验证许可证的所有用户。

## 更新人员视图

您可以在“人员”视图中添加新列，以查看哪些用户可以生成验证：

1. 转到&#x200B;**人员**&#x200B;区域。
1. 单击&#x200B;**人员**&#x200B;选项卡。
1. 在&#x200B;**视图**&#x200B;下拉菜单中，执行以下任一操作：

   * 若要将此信息添加到现有视图，请选择要自定义的视图，然后单击&#x200B;**自定义视图**。
   * 若要将此信息添加到新视图，请单击&#x200B;**新建视图**。

1. 单击&#x200B;**添加列**。
1. 在可用字段中，展开&#x200B;**用户**，然后单击&#x200B;**拥有证明许可证**。

1. 单击&#x200B;**完成**，然后单击&#x200B;**保存视图**&#x200B;或&#x200B;**另存为新视图**。

   该视图显示&#x200B;**True**&#x200B;或&#x200B;**False**，具体取决于用户是否分配了验证许可证。
