---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Adobe Workfront API调用的域格式
description: 找到要在Adobe Workfront API中使用的域
author: Becky
feature: Workfront API
role: Developer
exl-id: 8f5b78c9-b84f-4f56-b7cc-ba686fac2da1
source-git-commit: c2ce6776ceebe3c1d3915e3791fc84eb0245ba4d
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 0%

---

# Adobe Workfront API调用的域格式

当您对Workfront API进行API调用时，您在调用中使用组织的域。 此域URL的格式因您的组织是否已载入到AdobeUnified Shell而异。

要了解您的组织是否位于Unified ShellAdobe上，请检查查看Workfront页面时显示的URL。

| Workfront URL开头为： | API调用的URL： |
|---|---|
| `<yourdomain>.my.workfront.com` | `<yourdomain>.my.workfront.com` |
| `experience.adobe.com` | `<yourdomain>.my.workfront.adobe.com` |

要查找域，请执行以下操作：

1. 单击Adobe Workfront右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon.png)，或（如果可用）单击左上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png)，然后单击&#x200B;**[!UICONTROL 设置]** ![设置图标](/help/_includes/assets/gear-icon-setup.png)。
1. 选择&#x200B;**系统**，然后选择&#x200B;**客户信息**。

   屏幕右侧列出了您的域。

   ![域](assets/domain.png)

