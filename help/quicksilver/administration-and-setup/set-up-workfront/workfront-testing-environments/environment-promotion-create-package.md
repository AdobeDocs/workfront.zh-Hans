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
exl-id: 0ac8c7df-2d38-4291-861e-52fb5e748537
source-git-commit: 2e4bcd6400971104e9138fab0faf20d33af32e51
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 0%

---

# 创建或编辑环境升级包

您必须在要从&#x200B;**复制对象**&#x200B;的环境中创建一个包。 例如，如果您在自定义刷新沙盒环境中配置项目并将其提升到生产环境，则必须在自定义刷新沙盒环境中创建包。

>[!IMPORTANT]
>
>如果在为环境升级配置对象时刷新了自定义刷新沙盒，则该配置将在刷新中丢失。 我们建议您不要刷新“自定义刷新沙盒”，除非所有未完成的环境升级对象和包都已成功升级。

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

## 创建资源包

1. 转到要在其中创建包的环境。 这是您要从&#x200B;**复制对象**&#x200B;的环境。
1. 单击Adobe Workfront右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon.png)，或（如果可用）单击左上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png)，然后单击&#x200B;**[!UICONTROL 设置]** ![设置图标](/help/_includes/assets/gear-icon-setup.png)。
1. 在左侧导航中选择&#x200B;**系统**，然后选择&#x200B;**环境升级**。
1. 单击&#x200B;**创建包**。

   此时将打开“新建促销活动包”页面。

1. 在&#x200B;**包名称**&#x200B;字段中，输入包的名称。
1. 在&#x200B;**描述**&#x200B;字段中，输入此包的描述。
1. 要将对象添加到包，请在左侧导航中，选择要添加的对象类型。
1. 从显示的列表中选择一个或多个对象，或在搜索栏中键入名称，然后在对象出现在列表中时将其选定。 您可以在列表中选择多个对象。

   该列表包括最多500个所选对象类型的对象。 要查找不在列表中的对象，请使用搜索栏。
1. 单击&#x200B;**添加（X对象）**&#x200B;以将所选对象添加到包。

   >[!INFO]
   >
   >**示例**
   >
   >如果已选择三个项目添加到项目中，则按钮显示&#x200B;**添加3个项目**。

   已添加的对象将显示在页面右侧的“包内容”区域中。

1. 要添加其它类型的对象，请重复步骤7-9。
1. （可选）要从包中删除对象，请将鼠标悬停在“包内容”区域中的对象上，然后单击该对象旁边的X。
1. 将所有所需对象添加到包后，单击&#x200B;**保存并关闭**&#x200B;以保存包而不进行组装。

   或

   单击&#x200B;**保存并装配**&#x200B;以保存并装配包。

   >[!NOTE]
   >
   >* 如果软件包的名称中包含五个或更多字符并且至少添加了一个对象，则“保存并关闭”和“保存并装配”按钮可用。
   >* 您无法装配处于可安装状态（例如测试或活动）的软件包。

## 编辑或汇编现有包

包必须处于`DRAFT`状态才能编辑。

1. 转到要在其中编辑包的环境。 这是最初创建包的环境。
1. 单击Adobe Workfront右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon.png)，或（如果可用）单击左上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png)，然后单击&#x200B;**[!UICONTROL 设置]** ![设置图标](/help/_includes/assets/gear-icon-setup.png)。
1. 在左侧导航中选择&#x200B;**系统**，然后选择&#x200B;**环境升级**。
1. 从显示的列表中选择程序包。
1. （视情况而定）要查看禁用的包，请启用&#x200B;**显示已弃用的包**&#x200B;选项。
1. （可选）要查看内容（包括所有对象及其子对象），请单击&#x200B;**内容**&#x200B;部分中对象类型旁边的下拉箭头。
1. （可选）要查看此包的先前安装和安装尝试，请单击&#x200B;**部署**。
1. （可选）要编辑包，请单击屏幕右上角的&#x200B;**编辑包**。
包必须处于`DRAFT`状态才能编辑。 要将包移动到`DRAFT`状态，请在&#x200B;**状态**&#x200B;字段中，选择`Draft`。 然后，您可以继续编辑包。
1. 若要安装包，请单击屏幕右上角的&#x200B;**安装**。

   有关安装包的说明，请参阅[安装环境升级包](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)。
