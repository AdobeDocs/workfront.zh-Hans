---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 创建或编辑环境升级包
description: 环境升级功能旨在提供与配置相关的对象从一个环境移动到另一个环境的功能。 了解如何创建环境升级包，然后可将其安装在其他环境中。
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: c0a841d8f6a4431ff95c1b1d5904c8f41a7c82ca
workflow-type: tm+mt
source-wordcount: '535'
ht-degree: 0%

---

# 创建或编辑环境升级包

## 创建资源包

1. 转到要在其中创建包的环境。 这是复制对象的环境 **从**.
1. 单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon.png) 单击Adobe Workfront右上角的或者（如果可用）单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png) 图标，然后单击 **[!UICONTROL 设置]** ![“设置”图标](/help/_includes/assets/gear-icon-setup.png).
1. 选择 **系统** 在左侧导航中，然后选择 **环境升级**.
1. 单击 **创建包**.

   此时将打开“新建促销活动包”页面。

1. 在 **包名称** 字段，输入包的名称。
1. 在 **描述** 字段中，输入此包的描述。
1. 要将对象添加到包，请单击 **添加对象** 在左侧导航中，选择要添加的对象类型。
1. 从列表中选择一个或多个对象，或在搜索栏中键入名称，然后在对象出现在列表中时将其选定。 您可以在列表中选择多个对象。
1. 单击 **添加（X个对象）** 将所选对象添加到包中。

   例如，如果您选择了三个项目以添加到项目中，则该按钮显示 **添加3个项目**.

   已添加的对象将显示在页面右侧的“包内容”区域中。

1. 要添加其它类型的对象，请重复步骤7-9。
1. （可选）要从包中删除对象，请将鼠标悬停在“包内容”区域中的对象上，然后单击该对象旁边的X。
1. 将所有所需对象添加到包后，单击 **保存并关闭** 保存包而不进行组装。

   或

   单击 **保存并汇编** 以保存和汇编包。

   >[!NOTE]
   >
   >* 如果软件包的名称中包含五个或更多字符并且至少添加了一个对象，则“保存并关闭”和“保存并装配”按钮可用。
   >* 您无法装配处于可安装状态（例如测试或活动）的软件包。

## 编辑或汇编现有包

1. 转到要在其中创建包的环境。 这是复制对象的环境 **从**.
1. 单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon.png) 单击Adobe Workfront右上角的或者（如果可用）单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png) 图标，然后单击 **[!UICONTROL 设置]** ![“设置”图标](/help/_includes/assets/gear-icon-setup.png).
1. 选择 **系统** 在左侧导航中，然后选择 **环境升级**.
1. 从显示的列表中选择程序包。
1. （视情况而定）要查看已存档（已禁用）的包，请启用 **显示已弃用的包** 选项。
1. 要查看内容（包括所有对象及其子对象），请单击中对象类型旁边的下拉箭头 **目录** 部分。
1. 要查看此软件包以前的安装和安装尝试，请单击 **部署**.
1. 要编辑包，请单击 **编辑包** 在屏幕的右上角。
1. 要安装包，请单击 **安装** 在屏幕的右上角。

   有关安装软件包的说明，请参阅 [安装环境升级包](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md).


