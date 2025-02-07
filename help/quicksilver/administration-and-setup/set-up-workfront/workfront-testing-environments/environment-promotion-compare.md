---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 比较环境之间的对象
description: 您可以跨环境比较对象，以确保环境升级包中包含所需的对象。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 085b0f04-5a9c-49b9-86d7-2363731ee067
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# 比较环境之间的对象

您可以在环境之间比较对象，以确保环境升级包中包含所需的对象。

您可以选择要比较的环境和对象类型。 Workfront会比较两个环境中选定类型的所有对象，并显示有关对象差异的数据。

## 访问要求

您必须具备以下条件：

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront]计划</strong>
   </td>
   <td> Prime或Ultimate（仅限新计划）
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront]个许可证</strong>
   </td>
   <td> [！UICONTROL标准版]
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

您的组织必须位于Adobe业务平台上，才能比较环境之间的对象。

## 生成对象比较

1. 转到要在其中比较对象的环境。
1. 单击Adobe Workfront右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon.png)，或（如果可用）单击左上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png)，然后单击&#x200B;**[!UICONTROL 设置]** ![设置图标](/help/_includes/assets/gear-icon-setup.png)。
1. 在左侧导航中选择&#x200B;**系统**，然后选择&#x200B;**环境升级**。
1. 单击屏幕右上角附近的&#x200B;**比较环境**。
1. 在&#x200B;**Source环境**&#x200B;字段中，选择要在其中创建包的环境。 这是您要从&#x200B;**复制对象**&#x200B;的环境。
1. 在&#x200B;**目标环境**&#x200B;字段中，选择要安装包的环境。 这是您正在将对象&#x200B;**复制到**&#x200B;的环境。
1. 在&#x200B;**要比较的对象**&#x200B;区域中，选择要在不同环境之间进行比较的对象类型。
1. 单击屏幕右上角附近的&#x200B;**生成比较**。

   根据比较对象的数量和大小，生成比较可能需要一些时间。

## 查看对象比较

比较生成完成后，将显示比较。

该列表包括源环境中存在的选定类型的对象，这些对象在目标环境中是否缺失，以及两者之间是否存在字段差异。

>[!BEGINSHADEBOX]

![比较示例](assets/environment-promotion-comparison.png)

在此示例中：

* 第一行显示存在于目标环境中但与源环境不同的对象。
* 第二行显示存在于目标环境中的对象，该对象与源环境中的对象相同。
* 第三行显示目标环境中不存在的对象。

>[!ENDSHADEBOX]

要查看特定对象差异，请执行以下操作：

1. 单击该对象行中的放大镜图标![比较图标](assets/compare-icon.png)。

   此时将打开一个窗口，其中包含该对象的所有字段。 差异以红色标记。

## 通过对象比较创建包

可直接通过对象比较创建包。

有关说明，请参阅“创建或编辑环境升级包”一文中的[通过对象比较创建包](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md#create-a-package-from-an-object-comparison)。
