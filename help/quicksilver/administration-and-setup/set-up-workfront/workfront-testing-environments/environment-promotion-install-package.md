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
source-git-commit: f65fbe7ceab19cee75aa0346c389907707c47c8b
workflow-type: tm+mt
source-wordcount: '401'
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
1. 对于每个有冲突的对象，选择如何解决冲突。

   要解决冲突，请单击对象类型旁边的下拉箭头，然后选择要执行的操作。

   有关更多信息，请参阅 [冲突](#collisions) 本文内容
1. 要将包部署到新环境，请单击 **部署** 在屏幕的右上角。

## 冲突

当作为安装包的一部分的对象已存在于目标环境中时，会发生冲突。 发生这种情况时，可以选择如何解决冲突。 冲突将在对象级别上解决。

您可以通过单击每个对象类型旁边的下拉菜单来查看冲突。 冲突显示在“冲突”列中。

要解决冲突，请在“部署操作”列中选择操作，或者使用已显示的默认操作。

* **使用新名称创建**：在目标环境中创建新对象。 如果对象存在于目标环境中，则可以使用新名称创建新对象。 如果目标环境中不存在该对象，则可以使用新名称或对象在包中的名称来创建对象。
* **使用现有**：未安装包中的对象，并且目标环境中已存在的对象保持不变。
* **覆盖**：包中的对象替换目标环境中的现有对象。
<!--
* Do not use: The object in the package is not installed in the target environment. If you select Do not use, an error message will appear detailing how this choice will affect other objects or fields.
-->

默认值为 `Create new` 如果目标环境中不存在该对象，并且 `Use existing` 如果目标环境中确实存在该对象。 您可以通过单击还原到默认映射 **重置为默认映射**.



<!--
## Collisions

A collision occurs when <!--???--.

In Workfront, a potential collision is marked with a blue dot. You can select 

You can select whether to show all package contents, or collisions only.

## Comparison tool

-->
