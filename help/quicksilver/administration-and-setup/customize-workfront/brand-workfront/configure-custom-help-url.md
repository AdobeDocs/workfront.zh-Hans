---
title: 配置自定义帮助URL
user-type: administrator
product-area: system-administration
navigation-topic: brand-workfront
description: 如果您创建自定义内部帮助站点，其中包含有关贵组织如何使用Workfront的信息，则可以配置主菜单帮助图标以转到该站点。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d2b63508-1943-4f9e-888e-8f1bfb54c33e
source-git-commit: 17aaf70977aa6ce0276676c6a30fd6c951be956c
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 4%

---

# 配置自定义帮助 URL

如果您创建自定义内部帮助站点，其中包含有关贵组织如何使用Workfront的信息，则可以配置主菜单帮助图标以转到该站点。

![自定义帮助按钮](assets/custom-help-button.png)

这不会影响整个Workfront中的上下文相关帮助链接，这些链接会将用户转到Workfront帮助站点。

有关用户如何访问您在Workfront中配置的自定义帮助URL和常规Workfront帮助网站的信息，请参阅[访问Adobe Workfront帮助](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/access-workfront-help.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td><p>任何</p></td> 
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

## 配置自定义帮助URL

{{step-1-to-setup}}

1. 单击&#x200B;**系统** > **首选项**。
1. 在&#x200B;**常规首选项**&#x200B;部分的&#x200B;**自定义帮助URL**&#x200B;字段中，键入自定义帮助站点所在的URL。

   如果您的自定义帮助位置需要登录凭据，则用户在从Workfront访问站点时需要这些凭据。 如果您未使用单点登录(SSO)，则可能需要将自定义帮助网站的凭据与Workfront凭据分开管理。

1. 单击&#x200B;**保存**。

   保存自定义帮助URL后，可以通过删除自定义URL并单击“保存”**返回到默认的Workfront帮助站点。**
