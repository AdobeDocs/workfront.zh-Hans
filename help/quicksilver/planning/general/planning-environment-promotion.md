---
title: 将环境提升用于Adobe Workfront Planning
description: 您可以使用“环境提升”功能将Workfront Planning工作区、记录类型、字段和视图从一个Workfront环境复制到另一个环境。 在源环境中将配置组装到一个包中并将其安装到目标环境中，而不是手动重建所有内容。
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 82ebe4df89bd9db39629b36c31c0ae2a4e133838
workflow-type: tm+mt
source-wordcount: '1377'
ht-degree: 2%
---

# 将环境提升用于Adobe Workfront Planning

<!--add to TOC-->
<!--add to miniTOC-->

<!--
Not sure if this bit will ever be needed because this only exists when both Preview and Prod have the features in parity. Features released here always come to both environments at the same time: 

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

>[!IMPORTANT]
>
>本文中的信息介绍了Adobe Workfront Planning。 贵公司必须购买附加的Planning包才能访问Workfront Planning。
>
>如果您的组织购买了Workfront Planning作为独立产品，则此处描述的功能将不可用。
>
>有关Workfront Planning的一般信息，请参阅[Adobe Workfront Planning入门](/help/quicksilver/planning/general/planning-overview.md)。
> 
>

<!--
Future - when they make it available in Planning: replace the above with this OR ... insert the snippet:

>[!IMPORTANT]
>
>The information in this article refers to Adobe Workfront Planning which your organization can purchase either as an Adobe Workfront package or a standalone product. 
>
>Not all capabilities included in the Planning package are available to Workfront Planning when it is purchased as a standalone product. 
>
>For general information about Workfront Planning, see [Get started with Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).
> 
>For information about Workfront Planning as a standalone product, see [Get started with Adobe Workfront Planning as a standalone product](/help/quicksilver/planning/planning-sta/planning-sta-overview.md). 
>
-->

您可以使用Workfront的环境升级功能，将Workfront工作区及其附加对象从一个Adobe Workfront环境复制到另一个环境。

在源环境中将配置组装到一个包中并将其安装到目标环境中，而不是手动重建所有内容。

将环境升级与Planning一起使用类似于将其用于Workfront。 有关详细信息，请参阅文章[Adobe Workfront测试环境](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-testing-environments.md)中的“环境升级”部分。

## 有关将Environment Promotion与Planning一起使用的注意事项

* 您必须是Workfront管理员才能使用环境升级。
* 将工作区复制到另一个环境时，也将通过环境升级导入与该工作区关联的以下对象：

  * 工作区
  * Workspace部分
  * 记录类型
  * 字段
  * 视图
  * 层级
  * 共享所有对象的设置
  * 请求表单
  * 业务规则
  * 连接的对象
  * 工作区所依赖的对象或其他对象共享的对象，如组、团队、工作角色、公司和用户。

    存在以下情况：

    * 如果目标环境中已存在同名对象，Workfront会标记冲突并决定其处理方式。
    * 如果共享对象的团队或组在目标环境中不存在，则升级会创建该团队。
  <!--* Automations -- this is not promoted, for now, per Lilit -->
* 对于每个对象，可以执行以下操作：

  * 将其创建为新对象
  * 使用现有对象，但使用新名称创建对象
  * 覆盖现有对象。 覆盖将替换目标中的配置。
* 不能导出以下对象：

  * 属于要复制的工作区的自动化
  * 记录
  * 不属于导出工作区的字段

* 无法提升跨工作区连接的记录类型，除非它们已存在于目标环境中。

  我们建议先提升包含跨工作区可连接记录类型的工作区，然后才提升引用这些记录类型的工作区。

* 安装可能需要几分钟的时间。 如果需要，您可以从结果页面回滚安装。
* 我们建议尽可能先测试该流程，然后再继续。 在将沙盒提升至生产环境之前，您可以将其安装到沙盒或预览环境。


## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront包</p></td> 
   <td> 
<p>Prime或Ultimate Workflow包，以及Prime或Ultimate Planning包</p>
<!--This might come later: <p>Prime or Ultimate Planning package when purchased as a standalone product</p>-->
   </td> 
   </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p>工作流标准</p>    
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>计划许可证</p></td> 
   <td><p>规划标准</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td> <p>您必须是系统管理员</p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>   <p>管理工作区的权限</p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>  
   </td> 
  </tr>  
</tbody> 
</table>

有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 使用环境升级导入Planning配置

以下是将Planning配置提升到其他环境的主要步骤：

* [在源环境中创建包](#create-a-package-in-the-source-environment)
* [使包准备就绪，可以安装](#make-the-package-ready-to-install)
* [在目标环境中安装包](#install-the-package-in-the-target-environment)
* [验证结果](#verify-the-results)

按照以下部分中的说明在两个Workfront环境之间复制Planning配置。

### 在源环境中创建包

1. 转到已放置所需配置的源环境。
1. 在源环境中，单击&#x200B;**主菜单** ![主菜单](assets/main-menu-shell.png)，然后转到&#x200B;**设置** > **系统** > **环境升级**。
**配置包**&#x200B;列表显示现有包的状态、源环境以及部署位置。
1. 单击&#x200B;**创建包**。

   >[!TIP]
   >
   >软件包在组装和安装之前需要至少一个对象。
1. 在&#x200B;**包详细信息**&#x200B;选项卡上，输入包的&#x200B;**名称**&#x200B;和&#x200B;**描述**。 源环境已填充了当前（源）环境。
1. 在左侧的对象类型列表中，选择&#x200B;**规划工作区**。
1. 搜索要提升的工作区，选中其复选框，然后单击&#x200B;**添加规划工作区**。 工作区显示在&#x200B;**包内容**&#x200B;下。

   已为“环境升级”选择![Workspace](assets/workspace-selected-for-environment-promotion.png)
1. 单击&#x200B;**保存并汇编**。

   Workfront将组合包，并在包的&#x200B;**更新**&#x200B;选项卡上添加一个条目。 您可以查看包在“内容”选项卡上包含的内容。
1. （有条件，可选）如果要稍后完成，请单击“保存”并关闭&#x200B;**&#x200B;**。
1. （可选）单击&#x200B;**内容**&#x200B;以查看包的内容，或单击&#x200B;**部署**&#x200B;以查看是否已多次部署此包。

   继续使包准备好安装。

### 使包准备就绪，可以安装

在目标环境中安装包之前，我们建议您先在测试环境中测试包。

1. 按照上一部分所述完成生成包后，单击&#x200B;**包详细信息**，然后单击&#x200B;**编辑**，将&#x200B;**状态**&#x200B;设置为&#x200B;**测试**，然后单击&#x200B;**保存并关闭**。

   >[!TIP]
   >
   >生成包后，其状态设置为&#x200B;**草稿**。 **活动**&#x200B;状态只有在您首先测试包之后才可用。
1. （推荐）单击“**安装**”，然后选择一个可用的测试环境来部署它并测试配置。

   >[!TIP]
   >
   >当状态设置为&#x200B;**Testing**&#x200B;时，生产环境不可作为选项之一使用。

1. 在测试环境中安装之后，再次单击&#x200B;**编辑**，并将&#x200B;**状态**&#x200B;设置为&#x200B;**活动**，然后单击&#x200B;**保存并关闭**。

   >[!TIP]
   >
   >在测试环境中安装该软件包与在生产环境中安装它类似，如以下部分所述。

   请继续阅读以下部分，以在目标环境中安装包。


### 在目标环境中安装包

1. 在验证包页面后，单击&#x200B;**安装**。
1. 在&#x200B;**目标环境**&#x200B;列表中，选择要部署到的环境（例如，您的生产环境），然后单击&#x200B;**继续**。 默认目标是当前环境。
1. 在&#x200B;**包信息**&#x200B;页面上，确认源环境和要部署到的环境。
1. 在&#x200B;**对象映射**&#x200B;部分中，展开每个对象分组（如&#x200B;**Planning工作区**）以查看对象。

   >[!TIP]
   >
   >如果有任何工作区对象与其共享，则组、团队、角色、公司和用户可能会显示在此处。

1. 对于每个对象，查看&#x200B;**冲突**&#x200B;和&#x200B;**状态**&#x200B;列，然后从列表中选择&#x200B;**部署操作**。 从以下选项中进行选择：


   * **新建**：将对象添加到目标。 当未检测到冲突时，请使用此选项。
   * **使用existing**：将对象映射到目标中已存在的对象，例如具有相同名称的工作区。
   * **使用新名称创建**：将对象添加到您指定的名称下。
   * **覆盖**：将目标中的现有对象替换为包中的对象。

   >[!TIP]
   >
   >如果系统未找到具有相同ID的工作区，则会尝试根据工作区名称查找匹配项。

1. （可选）要一次更改多个对象，请选中这些对象的复选框，在组顶部的部署操作列表中选择一个操作，然后单击应用于选定项。 使用列表上方的过滤器（如“仅显示错误”）来关注特定对象。
1. 解决所有错误指示器。 如果您为对象选择&#x200B;**使用existing**，则还必须选择它映射到的对象。  否则，状态将显示错误，**部署**&#x200B;将保持不可用。
1. 单击&#x200B;**部署**，然后单击&#x200B;**部署**&#x200B;以确认。


   Workfront显示了一个安装页面，其消息为&#x200B;**正在安装此包**。 这可能需要几分钟的时间。

   安装完成后，该页面将显示一条成功消息、安装包的环境以及已安装对象的列表，其中每个对象的状态都为，如&#x200B;**Used existing**&#x200B;或&#x200B;**Installed (Create new)**。
1. （可选）如果需要还原安装并从目标环境中删除配置，请单击&#x200B;**回滚安装**。

   继续验证安装结果。

### 验证结果

1. 转到目标环境> **主菜单** > **计划**&#x200B;并查找导入的工作区。
1. 打开记录类型和视图，确认字段和布局与源匹配。 由于不包含记录，因此表为空。


