---
title: Adobe Workfront规划Designer快速入门
description: 您可以使用由AI提供支持的Adobe Planning Designer来轻松配置工作区和数据结构。 Planning Designer支持从创建和配置工作区到定义字段和公式、管理记录、查看更改历史记录和构建自定义视图的所有功能。 无论直接使用还是通过AI Assistant，Planning Designer都为构建和维护结构化、关联的信息提供了一个灵活、强大的环境。
recommendations: noDisplay, noCatalog
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
exl-id: ba7a4b04-5faa-41b6-86d0-4d0ce946ad1e
source-git-commit: 21c98e443a6d6ca79045e2f4aba5f792340833cd
workflow-type: tm+mt
source-wordcount: '1470'
ht-degree: 0%

---

# Adobe Workfront规划Designer快速入门

<!--remove the Beta tags in the screen shots on this page when this is released to GA - maybe March 2, 2026-->

>[!IMPORTANT]
>
>Planning Designer目前仅适用于参与“已关闭的Beta”计划的用户。
>
>本文中的信息介绍了Adobe Workfront Planning，它是Adobe Workfront的一项附加功能。
>
>有关访问Workfront Planning的要求列表，请参阅[Adobe Workfront Planning访问概述](/help/quicksilver/planning/access/access-overview.md)。
> 
>有关Workfront Planning的一般信息，请参阅[Adobe Workfront Planning入门](/help/quicksilver/planning/general/planning-overview.md)。

您可以使用由AI提供支持的Adobe Planning Designer来轻松配置工作区和数据结构。 Planning Designer支持从创建和配置工作区到定义字段和公式、管理记录、查看更改历史记录和构建自定义视图的所有功能。

无论直接使用还是通过AI Assistant，Planning Designer都为构建和维护结构化、关联的信息提供了一个灵活、强大的环境。

有关Workfront Planning的信息，请参阅以下文章：

* [有关Adobe Workfront Planning的一般信息](/help/quicksilver/planning/planning-information.md)
* [Adobe Workfront Planning入门](/help/quicksilver/planning/general/planning-overview.md)
* [Adobe Workfront Planning访问概述](/help/quicksilver/planning/access/access-overview.md)


## 访问要求<!--edit theses??-->

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

## 注册已关闭的Beta项目以规划Designer

目前，您可以通过向我们发送电子邮件(sargism@adobe.com)来请求参加计划Designer的已关闭Beta计划。

收到电子邮件后，我们的工程团队将在您的Workfront实例中打开规划Designer 。

>[!IMPORTANT]
>
>您的公司必须首先接受AI助手协议，然后才能在系统中使用规划Designer。

## 提交关于Planning Designer的反馈

您可以在测试版计划期间提交关于Planning Designer的反馈。

1. 登录到Workfront，然后单击左上角的&#x200B;**主菜单**&#x200B;图标![行主菜单](assets/lines-main-menu.png)，然后单击&#x200B;**计划**。

   **计划**&#x200B;区域打开。

1. 单击&#x200B;**使用AI创建**。<!--update this tag name when they change it-->

   将打开&#x200B;**计划Designer**&#x200B;窗口。

1. 单击页面底部的&#x200B;**在此提交反馈**。
1. 在提供的共享空间中添加您的反馈，然后单击&#x200B;**提交**。
您的反馈将提交给工程和产品团队。

## 关于Planning Designer的注意事项

* 要使用Planning Designer，您首先需要为组织启用AI助手。 要使AI助手对贵组织中的每个人都可用，必须满足以下条件：

   * Workfront必须将AI助手设置为可用于您的组织。

     有关详细信息，请参阅[AI助手先决条件](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant)。
   * 在Workfront为贵组织提供AI助手后，Workfront的主要管理员可以访问该助手。

     有关信息，请参阅[配置系统的基本信息](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md)。
   * Workfront管理员必须接受AI Assistant协议，然后为所有其他用户打开AI Assistant。

     有关详细信息，请参阅[启用或禁用AI助手](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md)。
* 系统管理员为您的组织启用AI助手后，如果已经为您的组织提供了Planning Designer，则默认情况下它可供所有用户使用。
* 在Planning区域使用Planning Designer时，AI助手也可以执行由Planning Assistant执行的操作。
* AI助手在“规划”区域中执行的操作或由Planning Designer执行的操作与您的Workfront Planning权限和Workfront访问级别相关。

  有关信息，请参阅以下文章：

   * [在Adobe Workfront Planning中共享权限概述](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [使用Adobe Workfront Planning时的许可证类型概述](/help/quicksilver/planning/access/license-type-overview.md)

* AI助手或规划Designer代表用户所做的更改在记录历史记录面板中进行跟踪。

* 规划Designer采取的行动是永久性的，并且可能不可逆转。 例如，删除字段操作不能撤销。 在接受之前，请审阅Designer建议的所有操作。

  >[!IMPORTANT]
  >
  >当通过Planning Designer创建、更新或删除对象时，提示将仅要求确认不可逆的操作。 例如，删除记录类型或工作区是不可逆的。 删除记录是不可能的。 只有在尝试删除记录类型或工作区时，Planning Designer才会要求确认。

* 使用Planning Designer创建工作区和记录类型时，也会自动创建视图和字段。

## 目前可用于Planning Designer的功能

可以使用Planning Designer或AI Assistant执行以下任意操作：

* 创建和配置工作区

* 创建记录类型，包括定义全局记录类型并将其添加到工作区

* 设计字段或公式字段

* 创建、删除、复制和恢复记录

* 编辑、更新和附加记录中的字段

* 将记录链接到其他记录

* 访问记录更改历史记录

* 构建自定义视图

* 通过导入文档创建记录

  例如，您可以上传公司中组织结构图的图片，Planning Designer可基于该图片创建工作区。

  从导入的文档创建对象仅在Planning Designer中可用，在AI助手中不可用。

  >[!IMPORTANT]
  >
  >尽管我们支持.XLSX和.CSV文件类型，但它们不能用于通过Planning Designer进行大规模记录导入。
  >如果此时需要导入大量记录，我们建议您使用Planning中提供的手动功能进行导入。
  >
  >有关详细信息，请参阅[通过从CSV或Excel文件导入信息来创建记录](/help/quicksilver/planning/records/import-file-to-create-records.md)。
  >有关文件类型限制，请参阅[使用由AI提供支持的表单填写功能通过提示或文档填写请求](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md)中的“基于上载的文档获取建议”部分。


  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## 使用Planning Designer创建或更新对象

除非另有指定，否则可以使用Planning Designer或AI Assistant在Workfront Planning中创建或更新对象。

1. 登录到Workfront，然后单击左上角的&#x200B;**主菜单**&#x200B;图标![行主菜单](assets/lines-main-menu.png)，然后单击&#x200B;**计划**。

   **计划**&#x200B;区域打开。<!--update screen shot when they change the name of the button-->

   ![“工作区”页面上的“使用AI设计”按钮](assets/design-with-ai-button-on-workspaces-page.png)

1. 单击&#x200B;**使用AI创建**。<!--update this when they change it-->

   将打开&#x200B;**计划Designer**&#x200B;窗口。<!--remove the Beta tag here when this removes from Beta-->

   ![计划Designer窗口](assets/planning-designer-window.png)

1. 在提供的空白处，开始为AI助手键入提示，然后在完成时单击Enter。

   <!--add screen shot-->

   例如，您可以键入类似于以下内容的提示：

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

   >[!TIP]
   >
   >某些对象会立即创建，无需确认。

1. （可选）键入其他提示以进一步编辑对象。
1. （可选）单击&#x200B;**显示或隐藏预览屏幕**&#x200B;图标![隐藏或显示预览屏幕图标](assets/hide-show-preview-screen-in-planning-designer.png)以打开或关闭右侧的预览屏幕。
1. 单击&#x200B;**在新选项卡中打开工作区** ![在新选项卡中打开工作区](assets/open-workspace-on-new-tab-icon.png)以在新选项卡中打开要更新的工作区。
1. 单击&#x200B;**关闭**&#x200B;图标&#x200B;**X**&#x200B;以关闭Planning Designer并打开“工作区”区域。
1. 打开使用Planning Designer编辑的工作区，然后对其对象进行进一步更改。

## 为您的组织关闭Planing Designer

在Workfront管理员接受AI助手协议后，默认情况下将为组织中的每个人打开规划Designer 。

要将其关闭，请执行以下操作：

1. 以系统管理员身份登录到Workfront。
1. 单击屏幕左上角的&#x200B;**主菜单** ![主菜单图标](assets/main-menu-shell.png)，然后单击&#x200B;**设置**。
1. 单击左侧面板中的&#x200B;**系统** >，然后转到&#x200B;**AI首选项**&#x200B;区域。
1. 关闭&#x200B;**Planning Onboarding**&#x200B;设置。<!--add new screen shot with info icon and new name of the toggle; ensure you don't show the AI Reviewer if it is not in Prod yet-->

   系统首选项中的![规划Designer设置](assets/planning-designer-toggle-in-system-preferences.png)
1. 单击&#x200B;**保存**。

   这将删除系统中所有用户的Planning Designer。
