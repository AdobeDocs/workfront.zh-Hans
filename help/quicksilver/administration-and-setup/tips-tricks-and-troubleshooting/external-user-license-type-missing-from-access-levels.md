---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 访问级别中缺少外部用户许可证类型
description: 我在“设置”中的访问级别下无法再看到外部用户许可证类型。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: fcc876d9-0512-424a-a731-6bbacd55af3f
TQID: https://experienceleague.adobe.com/g65Yq7r0Hvr6ZyC2niVw4Dnbil37epPeoyfQVOWOiy8
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 119
ht-degree: 14%

---

# 访问级别中缺少外部用户许可证类型

## 问题

我在“设置”中的访问级别下无法再看到外部用户许可证类型。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 包</td> 
   <td><p>“任一”</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 许可证</td> 
   <td><p>标准</p>
       <p>规划</p></td>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>[！UICONTROL系统管理员]</td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 解决方案

1. 转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 系统]** > **[!UICONTROL 首选项]**。

1. 在&#x200B;**[!UICONTROL 安全性]**&#x200B;部分中，确保启用了选项&#x200B;**[!UICONTROL 通过使用没有Workfront帐户的人员的电子邮件地址与其协作]**。

   如果未启用此选项，则外部用户不会出现在访问级别设置中。
