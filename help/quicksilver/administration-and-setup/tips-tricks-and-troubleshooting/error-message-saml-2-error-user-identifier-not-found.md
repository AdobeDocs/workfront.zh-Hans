---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 错误消息： SAML 2.0错误：未找到用户标识符
description: 无法成功建立与ADFS的连接。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c4c70532-de4f-4264-b661-2d30cefd403c
TQID: https://experienceleague.adobe.com/H7-Y9pZ-w4K3iEkJTVeHrx1cJJYXHiIMIvO3VoGYq9g
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 180
ht-degree: 9%

---

# 错误消息： SAML 2.0错误：未找到用户标识符

## 问题

无法成功建立与ADFS的连接。

![identifier_not_found.png](assets/identifier-not-found.png)

>[!NOTE]
>
>如果成功建立了测试连接，但仍遇到问题，则属性映射可能不正确，或者联合ID出现问题。 如有疑问，请联系客户支持。

## 原因：

ADFS服务器上的声明不正确。

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
   <td>[!UICONTROL 系统管理员]</td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 解决方案

在ADFS服务器上，确保存在对名称ID的声明：

1. 在Windows中，单击&#x200B;**[!UICONTROL 开始]** > **[!UICONTROL 管理]** > **[!UICONTROL ADFS 2.0管理]**。\
   将显示“ADFS 2.0管理”对话框。

1. 在左侧窗格中选择&#x200B;**[!UICONTROL 信任关系]** > **[!UICONTROL 信赖方信任]**。

1. 右键单击与Adobe Workfront相关的信赖方信任，然后选择&#x200B;**[!UICONTROL 编辑声明规则]**。
1. 验证声明是否具有&#x200B;**[!UICONTROL 名称ID]**&#x200B;的&#x200B;**[!UICONTROL 传出声明类型]**。

![1.png](assets/1-350x287.png)
