---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Adobe Workfront API调用的域格式
description: 找到要在Adobe Workfront API中使用的域
author: Becky
feature: Workfront API
role: Developer
exl-id: 8f5b78c9-b84f-4f56-b7cc-ba686fac2da1
source-git-commit: b9547764abd4f1f61d93da6bc66d9e6776954f4d
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 1%

---

# Adobe Workfront API调用的域格式

当您对Workfront API进行API调用时，您在调用中使用组织的域。 此域URL的格式因您的组织是否已载入Adobe Unified Shell而异。

要了解您的组织是否位于Adobe Unified Shell上，请检查查看Workfront页面时显示的URL。

| Workfront URL开头为： | API调用的URL： |
|---|---|
| `experience.adobe.com` | `<yourdomain>.my.workfront.adobe.com` |

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>标准</p>
   <p>规划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


要查找域，请执行以下操作：

1. 单击Adobe Workfront右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon.png)，或（如果可用）单击左上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png)，然后单击&#x200B;**[!UICONTROL 设置]** ![设置图标](/help/_includes/assets/gear-icon-setup.png)。
1. 选择&#x200B;**系统**，然后选择&#x200B;**客户信息**。

   屏幕右侧列出了您的域。

   ![域](assets/domain.png)

