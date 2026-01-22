---
title: Adobe Workfront规划Designer快速入门
description: 使用Adobe Planning Designer，您可以生成新的工作区，在Workfront Planning中填写记录类型和字段，或将对象添加到工作区，或查看记录的更改历史记录。
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: bf34bfa2059d227eca3faa3d719adcf4d711e457
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 1%

---


# Adobe Workfront规划Designer快速入门

{{planning-important-intro}}

使用Adobe Planning Designer，您可以生成新的工作区，在Workfront Planning中填写记录类型和字段，或将对象添加到工作区，或查看记录的更改历史记录。

>[!IMPORTANT]
>
>Planning Designer目前仅适用于参与封闭测试阶段的用户。

## 访问要求<!--edit theses-->

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
<p>任何Workfront和Planning包</p>
<p>任何工作流和计划包</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p>标准</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>   <p>管理工作区</a>的权限 </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>  </td> 
  </tr>  
</tbody> 
</table>

有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在封闭式Beta项目中注册计划Designer

<!--edit this Or create a new article under Beta programs?? -->

目前，您可以请求参加计划Designer的已关闭Beta计划。

## 关于Planning Designer的注意事项

<!--these are from the AI Assistant - edit these-->

* 要使用Planning Designer，您首先需要为组织启用AI助手。 要使AI助手对贵组织中的每个人都可用，必须启用以下项：

   * 必须先为贵组织启用AI助手，然后该助手才可供贵公司的用户使用。 有关信息，请参阅[AI助手概述](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md)。
   * 在Workfront为贵组织启用AI助手后，主Workfront管理员可以使用该助手。 有关信息，请参阅[配置系统的基本信息](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md)。

   * Workfront管理员必须为所有其他用户启用AI助手。 有关详细信息，请参阅[启用或禁用AI助手](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md)。

   * AI助手在每个页面的上下文中工作。 您为AI助手提交的请求必须引用您打开的页面中可用的功能。

* 要使用Planning Designer，系统管理员必须在设置的“系统首选项”区域中启用它。

* AI助手在“规划”区域中执行的操作将与Workfront规划权限和Workfront访问级别的上下文相关。 有关信息，请参阅以下文章：

   * [在Adobe Workfront Planning中共享权限概述](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [使用Adobe Workfront Planning时的许可证类型概述](/help/quicksilver/planning/access/license-type-overview.md)

* AI助手代表用户所做的更改在记录的历史记录面板中进行跟踪。

* 您可以使用命令撤消操作。 例如，您可以键入“撤消上次更改”以恢复更改。

* 通过AI助手创建、更新或删除对象时，AI助手会显示预期操作并请求确认。 然后，您可以确认或取消操作。

—>

## 目前可用于Planning Designer的功能

<!--edit these- they are from the Ai Assistant: 

Currently, the AI Assistant is available in the Planning area of Workfront for the following pages:

* Workspace page
* Record type page
* Record page

You can use the AI Assistant to perform the following actions, at this time:

* Search for records. You can search by information contained in any record fields. 
* Create records. An ID with a link to the new record displays after the record is created. You can specify the fields you want to update during the creation process, like dates or description. 
* Create records based on a document that you upload. Workfront supports the following document formats for the AI Assistant:

    PPTX, PDF, DOCX, XLSX, PPT, DOC, TXT, and most image formats
* Update fields for the records you see on the screen
* Delete records
* Restore records that you just deleted

-->

可以使用Planning Designer或AI Assistant执行以下任意操作：

* 创建和配置工作区

* 创建记录类型

* 设计字段或公式字段

* 创建、删除、复制和恢复记录

* 编辑、更新和附加记录中的字段

* 将记录链接到其他记录

* 访问记录更改历史记录

* 构建自定义视图

* 通过导入文档创建记录。 从导入的文档创建记录只能在Planning Designer中使用，而不能在AI助手中使用。<!--add information about supported files-->

  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## 在Workfront Planning中找到Planning Designer

您可以从Workfront Planning主页访问Planning Designer。

<!--add screen shot-->

您还可以使用AI助手来利用Planning Designer提供的相同功能。

## 为您的组织启用Planing Designer

作为Workfront管理员，您必须首先为组织启用Planning Designer 。

<!--add steps here-->

## 使用Planning Designer创建或更新对象

除非另有指定，否则可以使用Planning Designer或AI Assistant在Workfront Planning中创建或更新对象。

1. 登录到Workfront，然后单击屏幕右上角的&#x200B;**主菜单**&#x200B;图标![圆点主菜单](assets/dots-main-menu.png)或左上角的&#x200B;**主菜单**&#x200B;图标![行主菜单](assets/lines-main-menu.png)（如果可用）。

1. 单击&#x200B;**计划**。 此时将打开“规划”区域。

1. 单击&#x200B;**使用AI设计**。

1. 在提供的空白处，开始输入AI Assistant的命令，然后在完成后单击Enter。

   <!--add screen shot-->

   例如，您可以键入类似于以下内容的请求：

   * 创建和配置具有五种记录类型的工作区以管理活动

   * 为当前年份的每月创建营销活动

   * 为营销设计工作区的状态添加营销活动字段

   * 删除所有处于过时状态的记录

   * 将所有Planning营销活动更新为“活动”状态

   * 将营销活动连接到营销设计工作区中的角色

   * 显示“情人节”营销活动的更改历史记录

   * 在营销设计工作区中构建营销活动的时间线视图

   * 通过导入文档创建记录。 从导入的文档创建记录只能在Planning Designer中使用，而不能在AI助手中使用。

   <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

   此时将显示一个可视化预览，其中包含助手可生成的内容的示例。

1. 在收到成功的响应后，按照命令行中提供的链接创建、更新或查看请求的对象。




