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
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '241'
ht-degree: 0%

---

# ADFS注销URL不起作用

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>本页中介绍的过程仅适用于尚未加入[!UICONTROL Adobe Admin Console]的组织。
>
>如果您的组织已加入[!UICONTROL Adobe Admin Console]，请参阅[基于平台的管理差异([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)。

## 问题

使用ADFS注销URL (https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0)时，您会收到一个消息页面，该页面显示以下错误：“访问站点时出现问题。 再次尝试浏览该网站。”

如果问题仍然存在，请与此站点的管理员联系，并提供以下参考号以识别问题： **57092dfc-751a-4915-8e6a-b4c5d413f8c6**

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe[!DNL Workfront]许可证</td> 
   <td> 
   <p>新增：标准</p>
   或
   <p>当前：计划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>[！UICONTROL系统管理员]</td>  
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 解决方案

1. 在ADFS管理器服务器中，转到&#x200B;**[!UICONTROL 信任关系]** > **[!UICONTROL 信赖方信任]** > `<your party trust>`属性。

1. 在&#x200B;**[!UICONTROL 端点]**&#x200B;选项卡下，单击&#x200B;**[!UICONTROL 添加]**。

1. **[!UICONTROL 终结点类型]** = SAML注销，绑定=POST，URL = https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0

   如果希望将响应URL重定向到其他页面，则可以设置此响应URL。 但我们建议使用ADFS站点，因为它会警告您已注销，但您仍应关闭浏览器。
