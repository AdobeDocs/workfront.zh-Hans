---
title: Adobe Workfront Planning AI助手概述
description: 您可以使用AI助手根据当前页面上下文和记录结构生成、更新或删除记录。 用户的命令和AI执行这些命令共同工作，以确保AI所做的更改准确反映在您的环境中。
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 53f57953-fb9f-47ef-be18-a7164c844682
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/3I5y7eTZml-nkAiAYnBFuaw72DyXgNG12D-EVYVourA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
    internal-label: Get started
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: b529b3aded4ab92015683a0ddccd152bc2cc798c
workflow-type: tm+mt
source-wordcount: '988'
ht-degree: 1%
---
# Adobe Workfront规划AI助手概述



<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在发布到“预览”版之后，启用了“快速发布”的客户的生产环境中每月还会提供相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>



{{planning-important-intro}}

您可以使用AI助手，根据当前页面上下文对Adobe Workfront Planning中的记录和其他对象进行更改或更新。

用户的命令和AI执行这些命令共同工作，以确保AI所做的更改准确反映在您的环境中。

>[!IMPORTANT]
>
><span class="preview">在某些组织中，AI助手已被CX Coworker所取代。 有关信息，请参阅[Adobe Workfront规划CX Coworker概述](/help/quicksilver/planning/general/planning-cx-coworker-overview.md)。</span>

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
     <p>您的管理员必须执行以下操作才能允许访问AI助手：</p>
   <ul>
   <li><p>当您同时具有Workflow和Planning包时，将工作流和Planning许可证类型添加到您的访问级别</p></li>
   <li><p>取消选择访问级别中的“禁用Workfront AI助手”设置</p></li></ul>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>   <p>管理工作区</a>的权限 </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>  </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>系统设置</p></td> 
   <td>   <p>您的Workfront管理员必须在设置的系统首选项区域中选择启用AI设置，并签署AI才能访问AI助手</p>  
    </td> 
  </tr> 
</tbody> 
</table>

有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


## 关于AI助理的注意事项

* 必须先为贵组织启用AI助手，然后该助手才可供贵公司的用户使用。

  有关信息，请参阅[AI助手概述](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md)。

* Workfront为您的组织启用代理后，主Workfront管理员即可使用该代理。 有关信息，请参阅[配置系统首选项](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md)。

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

>[!NOTE]
>
><span class="preview">如果贵组织已获得对CX Coworker的访问权限，则查找CX Coworker与查找AI助手类似。 有关信息，请参阅[Adobe Workfront规划CX Coworker概述](/help/quicksilver/planning/general/planning-cx-coworker-overview.md)。</span>


您可以在Workfront Planning的以下区域中找到AI助手：

* 屏幕右上角的主导航栏。
* 在记录的详细信息区域中，在预览中打开记录或打开记录的页面之后。

### 访问规划区的人工智能助理

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



