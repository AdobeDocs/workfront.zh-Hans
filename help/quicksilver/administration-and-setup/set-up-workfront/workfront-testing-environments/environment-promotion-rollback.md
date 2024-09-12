---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 回滚环境升级包
description: 环境升级功能旨在提供与配置相关的对象从一个环境移动到另一个环境的功能。 了解如何从目标环境回滚已安装的升级包。
author: Becky
feature: System Setup and Administration
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 70f7e2a8-bb27-4546-afb7-53e0eec30bf1
source-git-commit: 7e15301dae4b761d19c85a3581bfdb4540ed40fd
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 1%

---

# 回滚环境升级包



安装包后，可以将其回滚。 这将删除包在目标环境中所做的更改，并将受影响的对象恢复到其以前的配置。

您可以在安装促销活动包后的24小时内将其回滚。 24小时后，回滚功能将不再可用于该安装。

## 访问要求

您必须具备以下条件：

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront]计划</strong>
   </td>
   <td> <p>新增：Prime或Ultimate</p><p>或</p><p>当前：不可用</p>
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront]个许可证</strong>
   </td>
   <td> <p>[！UICONTROL标准版]</p><p>或</p><p>当前：不可用</p>
   </td>
  </tr>
   <tr>
   <td>访问级别配置
   </td>
   <td>您必须是[!DNL Workfront]管理员。
   </td>
  </tr>
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## 先决条件

* 必须先安装环境升级包，然后才能回滚。

  有关说明，请参阅[安装环境升级包](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)。


## 确定是否可回滚特定包部署

要了解特定包部署是否可以回滚，请考虑以下事项：

* 自安装包以来必须经过不到24小时。
* 只能回滚最新的包部署。
* 可以回滚失败的部署。
* 无法回滚。


## 回滚已安装的环境升级包

1. 转到安装包的环境。
1. 单击Adobe Workfront右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon.png)，或（如果可用）单击左上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png)，然后单击&#x200B;**[!UICONTROL 设置]** ![设置图标](/help/_includes/assets/gear-icon-setup.png)。
1. 在左侧导航中选择&#x200B;**Environment Promotion**。
1. 选择要回滚的包，然后单击&#x200B;**部署**。
1. 将鼠标悬停在要回滚的部署（安装）上，然后在该部署行右侧出现时单击回滚。

   或

   单击要回退的部署，然后单击屏幕右上角的&#x200B;**回退包**。

   >[!IMPORTANT]
   >
   >部署发生的时间必须少于24小时，然后才能回滚。 无法回滚已超过24小时的安装。

1. （可选）在“回滚预览”区域中，查看回滚部署时将发生的更改。
1. 单击屏幕右上角的&#x200B;**回滚**。
