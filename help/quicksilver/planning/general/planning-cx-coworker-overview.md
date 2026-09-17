---
title: Adobe Workfront规划CX Coworker概述
description: 您可以使用Workfront Planning中的CX Coworker对Planning中的记录和其他对象执行类似的操作，通常在界面中执行这些操作。 用户的命令和AI执行这些命令共同工作，以确保AI所做的更改准确反映在您的环境中。
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: d5f36e0c8dbd9749503de25b75e70bf18b1d187b
workflow-type: tm+mt
source-wordcount: '1007'
ht-degree: 1%
---

# Adobe Workfront规划CX Coworker概述


<span class="preview">此页面上的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在发布到“预览”版之后，启用了“快速发布”的客户的生产环境中每月还会提供相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>


{{planning-important-intro}}

CX Coworker是一个对话式界面，您可以在其中以简单的语言描述目标，然后它可以在您的Adobe和连接的系统中规划、执行和验证工作，然后再重新引入以供您审批。

CX Coworker保留了AI Assistant目前所做的一切，同时在新的全屏体验和Workfront右边栏中添加了更强大的端到端功能。

它在您组织的现有产品级访问控制内运行，因此用户只能执行在Workfront中已允许他们执行的操作，默认情况下具有只读访问权限，并且写访问权限由Workfront管理员控制。

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

* Workfront为您的组织启用代理后，主Workfront管理员即可使用该代理。 有关信息，请参阅[配置系统的基本信息](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md)。

* Workfront管理员必须为所有其他用户启用AI助手。 有关详细信息，请参阅[启用或禁用AI助手](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md)。

* AI助手在每个页面的上下文中工作。 您为AI助手提交的请求必须引用您打开的页面中可用的功能。

* AI助手在“规划”区域中执行的操作将与Workfront规划权限和Workfront访问级别的上下文相关。 有关信息，请参阅以下文章：

  * [在Adobe Workfront Planning中共享权限概述](/help/quicksilver/planning/access/sharing-permissions-overview.md)
  * [使用Adobe Workfront Planning时的许可证类型概述](/help/quicksilver/planning/access/license-type-overview.md)

* AI助手代表用户所做的更改在记录的历史记录面板中进行跟踪。

* AI助理采取的行动是永久性的，而且可能不可逆转。 例如，删除字段操作不能撤销。 在接受之前，请查看AI助手建议的所有操作。

* 通过AI助手创建、更新或删除对象时，AI助手会显示预期操作并请求确认。 然后，您可以确认或取消操作。

## 当前可用于AI助手的功能

目前，AI助手可在Workfront的“规划”区域访问以下页面：

* Workspace页面
* 记录类型页面
* 记录页面

此时可以使用AI助手执行以下操作：

* 搜索记录。 您可以按任何记录字段中包含的信息进行搜索。
* 创建记录。 创建记录后，将显示一个包含指向新记录的链接的ID。 您可以指定要在创建过程中更新的字段，如日期或说明。
* 根据上传的文档创建记录。 Workfront支持AI助理的以下文档格式：

  PPTX、PDF、DOCX、XLSX、PPT、DOC、TXT和大多数图像格式
* 更新您在屏幕上看到的记录的字段
* 删除记录
* 恢复您刚刚删除的记录


## 在Workfront规划中找到AI助手

您可以在Workfront Planning的以下区域中找到AI助手：

* 屏幕右上角的主导航栏。
* 在记录的详细信息区域中，在预览中打开记录或打开记录的页面之后。

## 访问规划区的人工智能助理

1. 登录到Workfront，然后单击左上角的&#x200B;**主菜单**&#x200B;图标![行主菜单](assets/lines-main-menu.png)，然后单击&#x200B;**计划**。

   此时将打开“规划”区域。

1. 单击&#x200B;**工作区信息卡**。

1. （可选）单击&#x200B;**记录类型卡片**。

1. （可选）单击&#x200B;**记录**&#x200B;以打开记录的&#x200B;**详细信息**&#x200B;页面。

1. 单击全局导航栏屏幕右上角或记录预览或页面右上角的&#x200B;**AI助手图标**。

   ![AI助手图标](assets/ai-assistant-icon-highlighted.png)

1. 在提供的空白处，开始输入AI Assistant的命令，然后在完成后单击Enter。

   带有空命令框的![AI助手面板](assets/ai-assistant-panel-with-empty-command-box.png)

   例如，您可以键入以下内容之一：

   * 创建开始日期为7月4日、结束日期为7月30日的营销活动
   * 更新夏季促销活动记录的描述字段，日期待定
   * 删除最后一个记录
   * 恢复记录

   当AI助手处理命令时，将显示一个视觉指示器，设置响应时间的期望值。

   收到成功响应后，请按照提供的链接或注意左侧的更改内容。



