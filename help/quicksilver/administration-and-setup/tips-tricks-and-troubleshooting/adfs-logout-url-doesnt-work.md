---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ADFS注销URL不起作用
description: 此页面中描述的过程仅适用于尚未载入Adobe Admin Console的组织。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4d868625-e976-47b4-9e80-f1eca84a2768
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---

# ADFS注销URL不起作用

>[!IMPORTANT]
>
>此页面中描述的过程仅适用于尚未载入到 [!UICONTROL Adobe Admin Console].
>
>如果贵组织已载入 [!UICONTROL Adobe Admin Console]，请参阅 [基于平台的管理差异([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

## 问题

使用ADFS注销URL(https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0)时，您会收到一个消息页面，并显示错误：“访问站点时出现问题。 再次尝试浏览站点。”

如果问题仍然存在，请与此站点的管理员联系，并提供以下参考号以确定问题： **57092dfc-751a-4915-8e6a-b4c5d413f8c6**

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront] 许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>你必须是 [!DNL Workfront] 管理员。 有关更多信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> <p><b>注意</b>:如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 解决方案

1. 在ADFS管理器服务器中，转到 **[!UICONTROL 信任关系]** > **[!UICONTROL 信赖方信托]** > `<your party trust>` 属性。

1. 在 **[!UICONTROL 端点]** ，单击 **[!UICONTROL 添加]**.

1. **[!UICONTROL 端点类型]** = SAML注销，绑定=POST, URL = https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0

   如果您希望将响应URL重定向到其他页面，则可以设置该响应URL。 但我们建议使用ADFS网站，因为它会警告您已注销，但您仍应该关闭浏览器。
