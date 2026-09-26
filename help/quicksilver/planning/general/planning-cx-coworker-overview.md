---
title: Adobe Workfront规划CX Coworker概述
description: 您可以使用Workfront Planning中的CX Coworker对Planning中的记录和其他对象执行类似的操作，通常在界面中执行这些操作。 用户的命令和AI执行这些命令共同工作，以确保AI所做的更改准确反映在您的环境中。
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: eb361af2-3e4f-4a79-b5f3-7a344ac5794c
    internal-label: Workfront Planning
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 3934b1b333f86c8c700617871bfaac23d2b19213
workflow-type: tm+mt
source-wordcount: '1128'
ht-degree: 1%
---

# Adobe Workfront规划CX Coworker概述

<!--replaced information from the AI Assistant for Planning article with CX Coworker-->

<span class="preview">此页面上的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在发布到“预览”版之后，启用了“快速发布”的客户的生产环境中每月还会提供相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>


{{planning-important-intro}}

CX Coworker是一个对话式界面，您可在其中以简单的语言描述目标，然后它可以在您的Workfront Planning和其他连接的Adobe系统中规划、执行和验证工作，然后再重新引入以供您审批。

CX Coworker保留了AI Assistant目前所做的一切，同时在新的全屏体验和Workfront右边栏中添加了更强大的端到端功能。

它在您组织的现有产品级访问控制内运行，因此用户只能执行在Workfront中已允许他们执行的操作，默认情况下具有只读访问权限，并且写访问权限由Workfront管理员控制。

>[!IMPORTANT]
>
>CX Coworker当前不适用于医疗、金融或某些其他行业中具有敏感数据的组织。 AI助手可供这些组织使用。
>
>有关详细信息，请参阅[AI助手概述](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md)。


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
<p>带规划包的任何Workfront或工作流</p>
或
<p>作为独立产品购买时的任何Planning包</p>
   </td> </tr>
 <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p>标准</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe计划许可证</p></td> 
   <td><p>标准</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td>  
   <p>您的管理员必须执行以下操作，以允许在Planning中访问CX Coworker：</p>
   <ul>
   <li><p>当您同时具有Workflow和Planning包时，将工作流和Planning许可证类型添加到您的访问级别</p></li>
   <li><p>取消选择访问级别中的“禁用Workfront中的CX Coworker面板”设置。 默认情况下，该复选框处于选中状态。</p></li></ul>
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>   <p>管理工作区</a>的权限 </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>  </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>系统设置</p></td> 
   <td>   <p>您的Workfront管理员必须在“设置”的“系统首选项”区域中选择只读和只读MCP工具。 默认情况下，选择只读MCP工具。</p> 
    </td> 
  </tr> 
</tbody> 
</table>

有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## CX Coworker的注意事项

* 在为贵公司用户启用CX Coworker之前，必须为其启用该工具。

  有关信息，请参阅[CX Coworker概述](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md)。

* 在Workfront为您的Workfront实例启用代理后，它可供主要Workfront管理员使用，他们可以为您的组织启用它。 有关信息，请参阅[配置系统首选项](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md)。

* Workfront管理员还必须在您的访问级别为您启用CX Coworker。 有关信息，请参阅[创建和修改访问级别](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

* CX Coworker可处理Workfront或Workfront Planning中的信息和对象，并且您具有相应的访问权限。 在Planning右边栏中，“同事”面板在您已打开的工作区、记录类型或记录页面的上下文中运行。

* CX Coworker在Planning区域中执行的操作与Workfront Planning权限和Workfront访问级别的上下文相关。 有关信息，请参阅以下文章：

  * [在Adobe Workfront Planning中共享权限概述](/help/quicksilver/planning/access/sharing-permissions-overview.md)
  * [使用Adobe Workfront Planning时的许可证类型概述](/help/quicksilver/planning/access/license-type-overview.md)

* CX Coworker代表用户所做的更改在记录的“历史记录”面板中进行跟踪。

* CX Coworker采取的行动是永久性的，而且可能不可逆转。 例如，删除字段操作不能撤销。 在接受之前，请审阅CX Coworker建议的所有操作。

* 通过CX Coworker创建、更新或删除对象时，CX Coworker会显示预期操作并请求确认。 然后，您可以确认或取消操作。

## CX Coworker当前可用的功能

目前，CX Coworker在Workfront的Planning区域可用，它使用一组技能来访问和处理Planning对象的信息。 有关详细信息，请参阅[CX Coworker技能](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-skills.md)。

您可以使用CX Coworker执行以下操作：

* 搜索记录。 您可以按任何记录字段中包含的信息进行搜索。
* 创建记录。 创建记录后，将显示一个包含指向新记录的链接的ID。 您可以指定要在创建过程中更新的字段，如日期或说明。
* 根据上传的文档创建记录。 Workfront支持CX Coworker的以下文档格式：

  PPTX、PDF、DOCX、XLSX、PPT、DOC、TXT和大多数图像格式
* 更新您在屏幕上看到的记录的字段
* 删除、复制或恢复记录
* 将记录链接到其他记录
* 查看记录的更改历史记录


## 在Workfront Planning中找到CX Coworker

您可以在Workfront Planning的以下区域中找到CX Coworker：

* 屏幕右上角的主导航栏。
* 在新的选项卡中打开记录时，将其置于记录的详细信息区域中。

## 访问“规划”区域中的CX Coworker

1. 登录到Workfront，然后单击左上角的&#x200B;**主菜单**&#x200B;图标![行主菜单](assets/lines-main-menu.png)，然后单击&#x200B;**计划**。

   此时将打开“规划”区域。

   在页面的右上角找到&#x200B;**Co-worker**&#x200B;图标![Co-worker图标](assets/coworker-icon.png)，或继续执行以下步骤。

1. 单击&#x200B;**工作区信息卡**。

1. 单击&#x200B;**记录类型卡片**。

1. 单击&#x200B;**记录**&#x200B;以打开记录的&#x200B;**详细信息**&#x200B;页面，然后单击&#x200B;**在新标签中打开**&#x200B;图标![在新标签中打开](assets/open-workspace-on-new-tab-icon.png)。

1. 单击屏幕右上角的&#x200B;**CX Coworker图标** ![同事图标](assets/coworker-icon.png)。

1. 在提供的空白处，开始输入CX Coworker的命令，然后在操作完成后单击Enter 。

   ![带有空命令框的CX Coworker面板](assets/cx-coworker-right-rail.png)

   例如，您可以键入以下内容之一：

   * 创建新的营销活动记录，称为2026年夏季促销
   * 将夏季促销活动记录中的预算字段更新为$75,000
   * 删除名为“旧促销”的活动记录
   * 恢复我意外删除的营销活动

   >[!TIP]
   >
   >在要求Workfront对对象执行编辑操作之前，请确保您的CX Coworker管理员在系统首选项中启用了仅写MCP工具。

   CX Coworker处理命令时会显示一个视觉指示器，并设置响应时间的预期值。

   收到成功响应后，请按照提供的链接或注意左侧的更改内容。


1. （可选）单击&#x200B;**展开全屏**&#x200B;图标![展开全屏图标](assets/expand-full-screen-icon.png)以在完整的浏览器选项卡中打开同事聊天框。


