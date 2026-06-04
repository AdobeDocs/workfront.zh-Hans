---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 错误：自动设置的用户无法登录
description: 如果自动配置用户尝试首次登录并收到系统未为他们分配访问级别的错误，这可能是因为您的系统缺少与请求许可证关联的访问级别。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4c88933e-d3da-447e-ab6c-be9261a94a19
TQID: https://experienceleague.adobe.com/jUBGb9lqH9QL34Rw-oEhjty3l3wAf8avcLgtVe1-VSg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 200
ht-degree: 8%

---

# 错误：自动设置的用户无法登录

当自动设置用户尝试首次登录时，他们收到以下错误：

`Expect one user but found 0. ${subdomain} ${lane} ${email}`

## 问题

系统未为新用户分配访问级别。

默认情况下，自动资源调配使用请求许可证类型。 当不存在具有请求许可证的访问级别时，系统无法为用户分配访问级别。

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

使用请求许可证创建基本访问级别：

1. 转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 访问级别]**。

1. 单击&#x200B;**[!UICONTROL 新建访问级别]**。
1. 输入&#x200B;**[!UICONTROL 名称]**。
1. 在&#x200B;**[!UICONTROL 许可证类型]**&#x200B;下拉菜单中，选择请求。
1. 单击&#x200B;**[!UICONTROL 保存更改]**。

使用请求许可证创建访问级别后，请让用户使用其SSO凭据登录。


