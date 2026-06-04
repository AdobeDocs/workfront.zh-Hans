---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ADFS注销URL不起作用
description: 本页中介绍的过程仅适用于尚未载入Adobe Admin Console的组织。
author: Becky, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4d868625-e976-47b4-9e80-f1eca84a2768
TQID: https://experienceleague.adobe.com/RRaLL70JcSBcvoS6EUFuWj5Ejwljekt4QuQ3kXDx-44
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 250
ht-degree: 6%

---

# ADFS注销URL不起作用

<!-- Audited: 1/2024 -->

<!--Remove me October 2026-->

>[!IMPORTANT]
>
>此页面上描述的过程仅适用于尚未载入[!UICONTROL Adobe Admin Console]的组织。
>
>由于所有组织现在都已登记到Adobe Admin Console，因此本文将在不久的将来删除。
>
>如果您的组织已加入[!UICONTROL Adobe Admin Console]，请参阅[基于平台的管理差异([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)。

## 问题

使用ADFS注销URL (https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0)时，您会收到一个消息页面，该页面显示以下错误：“访问站点时出现问题。 再次尝试浏览该网站。”

如果问题仍然存在，请与此站点的管理员联系，并提供以下参考号以识别问题： **57092dfc-751a-4915-8e6a-b4c5d413f8c6**

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront]包</td> 
   <td>“任一”</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront]许可证</td> 
   <td>
   <p>标准</p>
   <p>规划</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>[！UICONTROL系统管理员]</td>  
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 解决方案

1. 在ADFS管理器服务器中，转到&#x200B;**[!UICONTROL 信任关系]** > **[!UICONTROL 信赖方信任]** > `<your party trust>`属性。

1. 在&#x200B;**[!UICONTROL 端点]**&#x200B;选项卡下，单击&#x200B;**[!UICONTROL 添加]**。

1. **[!UICONTROL 终结点类型]** = SAML注销，绑定= POST，URL = https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0

   如果希望将响应URL重定向到其他页面，则可以设置此响应URL。 但我们建议使用ADFS站点，因为它会警告您已注销，但您仍应关闭浏览器。
