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
exl-id: fe213fe7-5bb8-479c-926b-761cbdd7ba4e
source-git-commit: 7ca27795ec115a112acb55113bfade4a5fee15ad
workflow-type: tm+mt
source-wordcount: '946'
ht-degree: 0%

---

# 安装环境升级包

创建包后，可在其他环境中安装包。

您必须在要将对象&#x200B;**复制到**&#x200B;的环境中安装包。 例如，如果您在自定义刷新沙盒环境中配置项目并将其提升到生产环境，则必须在生产环境中安装包。

>[!IMPORTANT]
>
>* 如果在为环境升级配置对象时刷新了自定义刷新沙盒，则该配置将在刷新中丢失。 我们建议您不要刷新“自定义刷新沙盒”，除非所有未完成的环境升级对象和包都已成功升级。
>* 作为包安装的一部分在目标环境中创建的对象&#x200B;**不**&#x200B;具有与原始环境中的对象相同的ID。 这是因为在创建对象时，系统分配了ID。

## 访问要求

您必须具备以下条件：

<table>
  <tr>
   <td>Adobe Workfront包
   </td>
   <td> <p>Prime或Ultimate</p>
   </td>
  </tr>
  <tr>
   <td><strong>Workfront许可证</strong>
   </td>
   <td> <p>标准</p>&gt;
   </td>
  </tr>
   <tr>
   <td>访问级别配置
   </td>
   <td><p>您必须是Workfront管理员。</p>
   </td>
  </tr>
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## 先决条件

必须先创建环境升级包，然后才能安装它。

有关说明，请参阅[创建或编辑环境升级包](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)。

## 安装的软件包状态

软件包必须处于ACTIVE状态才能安装在生产环境中。

我们建议将包迁移到TESTING状态，并在另一个沙盒中安装以测试包。  如果此测试成功，并且没有错误，请将包移动到“活动”状态以在生产环境中安装包。

要编辑资源包的状态，请执行以下操作：

1. 按照“创建和编辑环境提升包”一文中[编辑或汇编现有包](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md#create-or-edit-an-environment-promotion-package)中的说明选择包。
1. 单击&#x200B;**编辑包**。
1. 单击&#x200B;**状态**。
1. 从下拉菜单中选择所需的状态。

有关状态的更多信息，请参阅在Workfront环境之间移动对象概述一文中的[环境升级状态](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#environment-promotion-statuses)。

## 安装包

>[!NOTE]
>
>* 要安装软件包，您必须登录到要安装软件包的环境。 这是您正在将对象&#x200B;**复制到**&#x200B;的环境。

1. 转到要在其中安装包的环境。
1. 单击Adobe Workfront右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon.png)，或（如果可用）单击左上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png)，然后单击&#x200B;**[!UICONTROL 设置]** ![设置图标](/help/_includes/assets/gear-icon-setup.png)。
1. 在左侧导航中选择&#x200B;**系统**，然后选择&#x200B;**环境升级**。
1. 从显示的列表中选择程序包。
1. 对于每个有冲突的对象，选择如何解决冲突。

   要解决冲突，请单击对象类型旁边的下拉箭头，然后选择要执行的操作。

   有关详细信息，请参阅本文中的[冲突](#collisions)
1. 要将包部署到新环境中，请单击屏幕右上角的&#x200B;**部署**。

## 冲突

冲突是在安装的目标环境中找到的对象，该对象与从源环境安装的某个对象相匹配。 通过比较源对象的名称和ID与目标环境中的对象来检测冲突。 还将源对象与先前安装的对象的记录进行比较，以检测冲突。

发生冲突时，可以选择如何解决冲突。 冲突将在对象级别上解决。

您可以通过单击每个对象类型旁边的下拉菜单来查看冲突。 冲突显示在“冲突”列中。

>[!NOTE]
>
>检测到的冲突可能不是您要在安装中覆盖或使用的对象。 我们建议验证检测到的冲突，以确保安装目标正确。

要解决冲突，请在“部署操作”列中选择操作，或者使用已显示的默认操作。

* **使用新名称创建**：在目标环境中创建新对象。 如果对象存在于目标环境中，则可以使用新名称创建新对象。 如果目标环境中不存在该对象，则可以使用新名称或对象在包中的名称来创建对象。
* **使用现有**：未安装包中的对象，并且目标环境中已存在的对象保持不变。
* **覆盖**：包中的对象将替换目标环境中的现有对象。

  即使未检测到冲突，您也可以选择要覆盖的对象。

  有关覆盖如何影响父对象和子对象的详细信息，请参阅本文中的[覆盖父对象和子对象](#overwriting-parent-and-child-objects)。
<!--
* Do not use: The object in the package is not installed in the target environment. If you select Do not use, an error message will appear detailing how this choice will affect other objects or fields.
-->

如果目标环境中不存在该对象，则默认值为`Create new`；如果目标环境中存在该对象，则默认值为`Use existing`。 您可以通过单击&#x200B;**重置为默认映射**&#x200B;还原为默认映射。

## 覆盖父对象和子对象

升级包中的某些对象可能具有子对象。 例如，项目（父）具有任务（子）。 覆盖父对象时，子对象的处理方式如下：

* 同时存在于包和目标中的子对象将在目标中更新以匹配包。
* 将创建存在于包中但不存在于目标中的子对象。
* 存在于目标中但不存在于包中的子对象将保持不变。

此功能会影响以下父对象和子对象：

| 父对象 | 子对象 |
|---|---|
| 项目 | 任务<br>QueueDef（队列定义）<br>RoutingRule |
| 模板 | TemplateTask<br>QueueDef（队列定义）<br>RoutingRule |
| 参数（自定义表单字段） | ParameterOption（自定义表单字段选项） |
| 日历信息 | 日历节 |
| QueueDef（队列定义） | QueueTopicGroup<br>队列主题 |

