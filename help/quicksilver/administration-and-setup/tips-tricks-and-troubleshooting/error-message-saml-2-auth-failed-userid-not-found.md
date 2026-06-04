---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 错误消息： SAML 2.0身份验证失败：未找到用户标识符
description: 使用SAML 2.0时，出现“SAML 2.0身份验证失败 — 用户标识符未找到”错误，表示未从ADFS声明规则传递UID或名称ID。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
TQID: https://experienceleague.adobe.com/YxLEE1OvD-Wo3FSd5ewXMfijsTaCjjCjzAx-EWWlBPE
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 225
ht-degree: 8%

---

# 错误消息： SAML 2.0身份验证失败：未找到用户标识符

## 问题

我在使用SAML 2.0时收到此错误：“SAML 2.0身份验证失败：未找到用户标识符。”

## 原因

当未从&#x200B;**ADFS声明规则**&#x200B;传递&#x200B;**UID**&#x200B;或&#x200B;**名称ID**&#x200B;时，会发生这种情况。

在ADFS中，**信赖方信任**&#x200B;需要有一个传递&#x200B;**UID**&#x200B;或&#x200B;**名称ID**&#x200B;值的&#x200B;**声明规则**。 当您运行&#x200B;**[!DNL Workfront]测试连接**&#x200B;时，如果成功，它将显示此连接。

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

1. 编辑&#x200B;**[!UICONTROL ADFS信息]**&#x200B;时，在&#x200B;**[!UICONTROL 信赖方信任]** >选择对象>**[!UICONTROL 编辑声明规则]**&#x200B;中。

1. **[!UICONTROL LDAP属性]** （左列）应具有&#x200B;**[!UICONTROL 电子邮件地址]** （或任何唯一标识符）。

1. **[!UICONTROL 传出声明类型]** （右列）应为&#x200B;**[!UICONTROL 名称ID]**。

   >[!NOTE]
   >
   >它不必具有LDAP属性电子邮件地址。 可以使用任何标识用户的唯一标识符，但必须将其作为&#x200B;**NAME ID**&#x200B;传递到[!DNL Adobe Workfront]。
