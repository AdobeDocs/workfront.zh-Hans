---
title: 删除自定义完成情况
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: 您可以删除自定义完成情况。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 5fbd4989-460b-4380-a136-8a9f6b79787d
TQID: https://experienceleague.adobe.com/jHR0a3-MzkRRrlZ-h-X9f0n5HQbO9nDhWSxqy8KnWa8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 222
ht-degree: 9%

---

# 删除自定义完成情况

如果不再需要某个自定义条件，您可以删除该条件。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 包</td> 
   <td><p>“任一”</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p>
       <p>规划</p></td>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>系统管理员</td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 删除自定义完成情况

{{step-1-to-setup}}

1. 单击&#x200B;**项目首选项** > **条件**。

1. 选择要删除的条件所在的对象类型（**项目**、**任务**&#x200B;或&#x200B;**问题**）的选项卡。

1. 单击要删除的条件名称旁边的&#x200B;**删除**。
1. 在出现的&#x200B;**删除完成情况**&#x200B;框中，从下拉列表中选择一个新完成情况，该新完成情况适用于使用该完成情况的所有项目、任务或问题。

   仅当自定义条件与您要删除的内置条件相等时，它们才在下拉列表中可用。 例如，如果要删除与“处于风险中”相等的条件，则只能选择与“处于风险中”相等的自定义条件。

1. 单击&#x200B;**删除条件**。

>[!NOTE]
>
>您无法删除内置完成情况，这些完成情况符合目标、存在风险和存在问题。 但是，您可以更改它们的名称和颜色。
>
>有关编辑自定义条件的信息，请参阅[创建或编辑自定义条件](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)。
