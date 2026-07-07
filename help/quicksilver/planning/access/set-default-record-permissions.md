---
title: 设置记录的默认权限
description: 修改记录类型或工作区设置时，可以设置记录的默认权限。 您可以为将为记录类型添加的所有记录授予“打开”或“受限”权限。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: a76a39fde984bece43cda9812c436d81f41eb989
workflow-type: tm+mt
source-wordcount: '724'
ht-degree: 3%

---


# 设置记录的默认权限

<span class="preview">此页面上的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在发布到“预览”版之后，启用了“快速发布”的客户的生产环境中每月还会提供相同的功能。</span>\
<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}


修改记录类型或工作区设置时，可以设置记录的默认权限。

您可以为将为记录类型添加的所有记录授予“打开”或“受限”权限。


## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。 

<!--
at GA, check that the Workfront plans article linked below has Planning info
-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 包</p></td> 
   <td> 
<p>带规划包的任何Workfront或工作流</p>

</tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p>“任一”</p> 
   <p><b>注释</b></p>
   <p>只有拥有Standard许可证的人员才能获得记录的管理权限。 所有其他许可证只能具有“查看”权限，并且它们的“管理”选项为灰色。</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>  <p>管理对工作区和记录类型的权限</p>  
   <p><b>重要</b></p>
   <p>只有对工作区具有管理权限的用户才能共享记录</p></td> 
  </tr>
</tbody> 
</table>

有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 设置默认记录权限的注意事项

配置默认记录权限时，请考虑以下事项：

* 每个记录类型一次只能有一个默认权限规则处于活动状态。
* 更改规则只影响更改后创建的记录。 现有记录保留其当前权限。
* 无论规则如何，系统管理员和工作区管理员始终保留对每个记录的“管理”访问权限。
* 创建记录后，可以在其共享对话框中单独更改其权限，而不会影响默认规则。
* 对于全局记录类型，每个工作区（主工作区和辅助工作区）都可以配置自己的默认规则，新记录会采用创建它们的工作区的规则。

## 为工作区配置默认记录权限

1. 前往工作区> **更多**&#x200B;菜单![更多菜单](assets/more-menu.png) > **设置** > **记录类型**。

   ![Workspace记录类型设置区域](assets/workspace-record-types-settings-area.png)

1. （可选）单击&#x200B;**记录类型**&#x200B;的单元格以编辑记录类型名称。

1. 在&#x200B;**新记录权限默认值**&#x200B;列中，单击要更新其权限的记录类型的单元格。

1. 从以下选项中进行选择：

   * **打开**：所有工作区参与者都可以管理新创建的记录。 这是所有现有记录类型和新记录类型的当前默认行为。
   * **受限制**：只有记录创建者和您明确添加的任何人都可以编辑新创建的记录。 其他所有人仅具有查看权限。

1. （视情况而定）如果您要将默认权限从&#x200B;**受限制**&#x200B;更改为&#x200B;**打开**，请单击&#x200B;**切换到打开**&#x200B;框中的&#x200B;**切换**&#x200B;以确认您的选择。
1. （视情况而定）如果您选择&#x200B;**受限制的**，请在&#x200B;**谁可以编辑记录**&#x200B;列中添加其他编辑器。 您可以添加用户、组、团队、角色或公司。

   >[!NOTE]
   >
   >* 记录创建者始终包括在内，不能删除。
   >* 您只能选择对记录类型具有Contribute或Manage权限的实体。

   更改会自动保存。 保存后，规则将立即生效，并自动应用于为该记录类型创建的所有记录。

## 为记录类型配置默认记录权限

1. 转到记录类型> **更多**&#x200B;菜单![更多菜单](assets/more-menu.png) > **设置** > **记录设置**。

   ![记录类型设置区域中的“记录设置”选项卡](assets/record-settings-tab-in-record-type-settings-area.png)

1. 在&#x200B;**记录权限类型**&#x200B;字段中，单击以下选项之一：

   * **打开**：所有工作区参与者都可以管理新创建的记录。 这是所有现有记录类型和新记录类型的当前默认行为。
   * **受限制**：只有记录创建者和您明确添加的任何人都可以编辑新创建的记录。 其他所有人仅具有查看权限。
1. （视情况而定）如果您要将默认权限从&#x200B;**受限制**&#x200B;更改为&#x200B;**打开**，请单击&#x200B;**切换到打开**&#x200B;框中的&#x200B;**切换**&#x200B;以确认您的选择。
1. （视情况而定）如果您选择&#x200B;**受限制的**，请在&#x200B;**谁可以编辑记录**&#x200B;字段中添加其他编辑器。 您可以添加用户、组、团队、角色或公司。

   >[!NOTE]
   >
   >* 记录创建者始终包括在内，不能删除。
   >* 您只能选择对记录类型具有Contribute或Manage权限的实体。

   更改会自动保存。 保存后，规则将立即生效，并自动应用于为该记录类型创建的所有记录。