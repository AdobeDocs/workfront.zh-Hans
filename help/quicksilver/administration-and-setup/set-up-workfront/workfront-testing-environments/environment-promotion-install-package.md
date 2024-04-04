---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 安装环境升级包
description: 环境升级功能旨在提供与配置相关的对象从一个环境移动到另一个环境的功能。 了解如何将环境升级包安装到目标环境中。
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: fe213fe7-5bb8-479c-926b-761cbdd7ba4e
source-git-commit: 5d84d50b8984bbff7bbc02ffc0ce86ec1f486742
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# 安装环境升级包

>[!NOTE]
>
>要安装软件包，您必须登录到要安装软件包的环境。 这是复制对象的环境 **到**.

1. 转到要在其中安装包的环境。
1. 单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon.png) 单击Adobe Workfront右上角的或者（如果可用）单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png) 图标，然后单击 **[!UICONTROL 设置]** ![“设置”图标](/help/_includes/assets/gear-icon-setup.png).
1. 选择 **系统** 在左侧导航中，然后选择 **环境升级**.
1. 从显示的列表中选择程序包。
1. 要安装包，请单击 **安装** 在屏幕的右上角。
1. 将包中的每个对象映射到目标环境中的相应对象。

   有关更多信息，请参阅 [映射](#mapping) 本文内容


## 映射

每种对象类型都列在左侧导航和卡片中。 信息卡会显示该类型的对象以及这些对象是否存在于目标环境中。 您可以确定如何将这些对象移动到目标环境。

* 新建：在目标环境中创建新对象。 如果对象存在于目标环境中，则可以使用新名称创建新对象。 如果目标环境中不存在该对象，则可以使用新名称或对象在包中的名称来创建对象。
* 使用existing：未安装包中的对象，并且目标环境中已存在的对象保持不变。
* 覆盖现有对象： （当前不可用）包中的对象将替换目标环境中的现有对象。
* 不使用：包中的对象未安装在目标环境中。 如果选择“不使用”，则会出现一条错误消息，详细说明该选择将如何影响其他对象或字段。

默认值为 `Create new` 如果目标环境中不存在该对象，并且 `Use existing` 如果目标环境中确实存在该对象。 您可以通过单击还原到默认映射 **重置为默认映射**.



<!--
## Collisions

A collision occurs when <!--???--.

In Workfront, a potential collision is marked with a blue dot. You can select 

You can select whether to show all package contents, or collisions only.

## Comparison tool

-->
