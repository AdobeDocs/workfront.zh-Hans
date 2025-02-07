---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 组管理员必须具有比他们管理的组管理员更高的访问权限
description: 如果组管理员的访问级别低于其管理的权限，他们将无法查看、修改或分配较低的访问级别。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2b501a1e-fb56-44fa-8518-07537dc90a5b
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 0%

---

# 组管理员必须比其管理的组管理员拥有更高的访问权限

如果组管理员的访问级别低于其管理的权限，他们将无法查看、修改或分配较低的访问级别。

## 问题

如果为组管理员分配了具有“团队”查看权限的修改规划者访问级别，但为某些用户分配了具有“团队”编辑权限的“工作人员”访问级别，则组管理员将无法与修改的“工作人员”访问级别进行交互。

![组管理员修改了访问权限](assets/group-admin-modified-access.png)


>[!NOTE]
>
>此逻辑也适用于微调设置下拉菜单。 两个访问级别都可以具有“编辑”访问权限，但是“微调设置”下拉菜单中的设置对于组管理员而言必须更高。
> ![优化设置](assets/fine-tune-your-settings.png)

## 解决方案

组管理员必须在访问级别的所有区域中具有比他们管理的区域更高的权限。
