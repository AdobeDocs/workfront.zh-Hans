---
title: Adobe Workfront规划Designer快速入门
description: 使用Adobe Planning Designer，您可以生成新的工作区，在Workfront Planning中填写记录类型和字段，将对象添加到工作区，或查看记录的更改历史记录。
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 866b237db5d109b0a435145119a6412e41d960ab
workflow-type: tm+mt
source-wordcount: '1020'
ht-degree: 1%

---


<!--add these at release to the metadata:

author: Alina, Becky
feature: Workfront Planning
role: User, Admin -->

# Adobe Workfront规划Designer快速入门

{{planning-important-intro}}

您可以使用由AI提供支持的Adobe Planning Designer来生成新工作区，向工作区中添加对象（记录类型、记录、视图或字段），或查看记录的更改历史记录。

>[!IMPORTANT]
>
>Planning Designer目前仅适用于参与“已关闭的Beta”计划的用户。

有关Workfront Planning的信息，请参阅以下文章：

* [有关Adobe Workfront Planning的一般信息](/help/quicksilver/planning/planning-information.md)
* [Adobe Workfront Planning入门](/help/quicksilver/planning/general/planning-overview.md)
* [Adobe Workfront Planning访问概述](/help/quicksilver/planning/access/access-overview.md)


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

* 要使用Planning Designer，您的组织必须满足使用Workfront AI Assistant的要求。

  有关详细信息，请参阅[AI助手先决条件](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant)。

* 要使用Planning Designer，系统管理员必须在设置的“系统首选项”区域中启用它。

* 可以使用提示构建Planning对象，方法是从Planning区域使用Workfront AI助手，或使用Planning Designer。

* AI助手在“规划”区域中执行的操作或由Planning Designer执行的操作与您的Workfront Planning权限和Workfront访问级别相关。

  有关信息，请参阅以下文章：

   * [在Adobe Workfront Planning中共享权限概述](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [使用Adobe Workfront Planning时的许可证类型概述](/help/quicksilver/planning/access/license-type-overview.md)

* Planning Designer代表用户所做的更改在记录的“历史记录”面板中进行跟踪。

* 您可以使用命令撤消操作。 例如，您可以键入“撤消上次更改”以恢复更改。

* 通过Planning Designer创建、更新或删除对象时，将显示预期操作并请求确认。 然后，您可以确认或取消操作。

* 使用Planning Designer创建工作区和记录类型时，也会自动创建视图和字段。

## 目前可用于Planning Designer的功能

可以使用Planning Designer或AI Assistant执行以下任意操作：

* 创建和配置工作区

* 创建记录类型

* 设计字段或公式字段

* 创建、删除、复制和恢复记录

* 编辑、更新和附加记录中的字段

* 将记录链接到其他记录

* 访问记录更改历史记录

* 构建自定义视图

* 通过导入文档创建记录。

  从导入的文档创建记录只能在Planning Designer中使用，而不能在AI助手中使用。

  有关接受的文件类型和大小的信息，请参阅文章[使用由AI提供支持的表单填写功能使用提示或文档填写请求中的“文档护栏”部分](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md)。

  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## 为您的组织启用Planing Designer

作为Workfront管理员，您必须首先为组织启用Planning Designer 。

<!--add steps here-->

1. 以系统管理员身份登录Workfront。
1. 单击屏幕左上角的&#x200B;**主菜单** ![主菜单图标](assets/main-menu-shell.png)，然后单击&#x200B;**设置**。
1. 单击左侧面板中的&#x200B;**系统** >，然后转到&#x200B;**AI首选项**&#x200B;区域。
1. 打开以下设置：
   * **启用AI**
   * **选择加入AI Betas**
   * **规划Designer**

   系统首选项中的![规划Designer设置](assets/planning-designer-toggle-in-system-preferences.png)
1. 单击&#x200B;**保存**。

   系统中所有拥有Standard许可证的用户现在都可以在Planning区域的Workspaces主页上看到&#x200B;**使用AI设计**&#x200B;按钮。<!--check screen shot-->

   在“工作区”页面上![使用AI设计按钮](assets/design-with-ai-button-on-workspaces-page.png)

   所有用户现在都可以启动并使用Planning Designer创建和更新Workfront Planning对象。

## 使用Planning Designer创建或更新对象

除非另有指定，否则可以使用Planning Designer或AI Assistant在Workfront Planning中创建或更新对象。

1. 登录到Workfront，然后单击左上角的&#x200B;**主菜单**&#x200B;图标![行主菜单](assets/lines-main-menu.png)。

1. 单击&#x200B;**计划**。 此时将打开“规划”区域。

1. 单击&#x200B;**使用AI设计**。

   将打开&#x200B;**计划Designer**&#x200B;窗口。

   ![计划Designer窗口](assets/planning-designer-window.png)

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

1. 收到成功响应后，按照提示区域中提供的链接创建、更新或查看请求的对象。

   当您同意创建对象时，您的更改将显示在提示区域的右侧。

   您可以在提示右侧的预览区域中查看工作区、记录类型、字段、视图和记录。
1. （可选）键入其他提示以进一步编辑对象。
1. （可选）单击&#x200B;**切换AI工作区预览屏幕**&#x200B;图标![隐藏或显示预览屏幕图标](assets/hide-show-preview-screen-in-planning-designer.png)以打开或关闭右侧的预览屏幕。
1. 单击&#x200B;**在新选项卡中打开工作区** ![在新选项卡中打开工作区](assets/open-workspace-on-new-tab-icon.png)以在新选项卡中打开要更新的工作区。
1. 单击&#x200B;**关闭**&#x200B;图标&#x200B;**X**&#x200B;以关闭Planning Designer并打开“工作区”区域。
1. 打开使用Planning Designer编辑的工作区，然后对其对象进行进一步更改。




