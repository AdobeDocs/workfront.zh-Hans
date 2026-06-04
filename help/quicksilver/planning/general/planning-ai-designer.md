---
title: Adobe Workfront规划Designer快速入门
description: 您可以使用由AI提供支持的Adobe Planning Designer来轻松配置工作区和数据结构。 Planning Designer支持从创建和配置工作区到定义字段和公式、管理记录、查看更改历史记录和构建自定义视图的所有功能。 无论直接使用还是通过AI Assistant，Planning Designer都为构建和维护结构化、关联的信息提供了一个灵活、强大的环境。
recommendations: noDisplay, noCatalog
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
exl-id: ba7a4b04-5faa-41b6-86d0-4d0ce946ad1e
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/YZRzcl8ymUo85jplCgKOx-qI83Gqa4CUI6saxfijtec
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 1469
ht-degree: 0%

---

# Adobe Workfront规划Designer快速入门

<!--remove the Beta tags in the screen shots on this page when this is released to GA - maybe March 2, 2026-->

>[!IMPORTANT]
>
>Planning Designer当前适用于处于Beta状态的所有客户。
>
>本文中的信息介绍了Adobe Workfront Planning，它是Adobe Workfront的一项附加功能。
>
>有关访问Workfront Planning的要求列表，请参阅[Adobe Workfront Planning访问概述](/help/quicksilver/planning/access/access-overview.md)。
> 
>有关Workfront Planning的一般信息，请参阅[Adobe Workfront Planning入门](/help/quicksilver/planning/general/planning-overview.md)。

您可以使用由AI提供支持的Adobe Planning Designer来轻松配置工作区和数据结构。 Planning Designer支持从创建和配置工作区到定义字段和公式、管理记录、查看更改历史记录和构建自定义视图的所有功能。

无论直接使用还是通过AI Assistant，Planning Designer都为构建和维护结构化、关联的信息提供了一个灵活、强大的环境。

有关Workfront Planning的信息，请参阅以下文章：

* [Adobe Workfront Planning的一般信息和文章索引](/help/quicksilver/planning/planning-information.md)
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
   <p><span class="preview">系统管理员为您的组织启用Planning Designer</span></p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>   <p>管理工作区</a>的权限 </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>  
   </td> 
  </tr>  
</tbody> 
</table>

有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 为您的组织启用Planning Designer

作为系统管理员，您可以为组织启用Planning Beta 。 打开此设置后，Workfront实例中的每个人可以在其“规划”区域中查看Planning Designer的功能。

1. 以Workfront管理员身份登录Workfront。
1. 单击&#x200B;**主菜单** ![主菜单图标](assets/main-menu-shell.png)，然后单击&#x200B;**设置**。
1. 转到&#x200B;**系统** > **首选项** > **AI首选项**。
1. 打开&#x200B;**启用AI**，并确保已与Adobe签署了Gen AI协议。
1. 打开&#x200B;**计划Designer**&#x200B;设置。

   系统首选项中的![规划Designer设置](assets/planning-designer-toggle-in-system-preferences.png)

1. 单击&#x200B;**保存**。

   Planning Designer创建或编辑工作区的功能现在可供贵组织中有权访问Planning的所有用户使用。

<!--

## Turn off the Planing Designer for your organization

After your Workfront administrator accepts the AI Assistant agreement, the Planning Designer is turned on for everyone in your organization, by default. 

To turn it off: 

1. Log in to Workfront as a System Administrator. 
1. Click **Main Menu** ![Main menu icon](assets/main-menu-shell.png) in the upper-left corner of the screen, then click **Setup**.
1. Click **System** >  in the left panel, then go to the **AI preferences** area.
1. Turn off the **Planning Onboarding** setting.
1. Click **Save**.

    This removes the Planning Designer for all users in the system.

-->

<!--

## Enroll in the Closed Beta program for the Planning Designer

Currently, you can request to participate in the Closed Beta program for the Planning Designer by sending us an email to sargism@adobe.com.

After we receive the email, our Engineering team will turn on the Planning Designer in your Workfront instance. 

>[!IMPORTANT]
>
>Your company must first accept the AI Assistant agreement before the Planning Designer is available in your system. 

-->

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

* 要使用Planning Designer，您首先需要为组织启用AI。 要使AI功能对贵组织中的每个人都可用，必须满足以下条件：

   * Workfront必须使AI功能对您的组织可用。

     有关详细信息，请参阅[AI助手先决条件](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant)。
   * 在Workfront为贵组织提供AI功能后，Workfront的主要管理员可以访问该功能。

     有关信息，请参阅[配置系统的基本信息](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md)。
   * Workfront管理员必须接受Gen AI协议，然后为您的组织启用AI和规划Designer。

     有关详细信息，请参阅[启用或禁用AI助手](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md)。
* 系统管理员为您的组织打开AI和Planning Designer后，默认情况下，Planning Designer可供所有用户使用。
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

<!--On March 2: * Edit workspaces-->

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
  >虽然我们支持.XLSX文件类型，但它们不能用于通过Planning Designer进行大规模记录导入。
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

1. 单击&#x200B;**使用AI创建**，或单击&#x200B;**创建工作区**，然后使用顶部的提示窗口指示您要创建的工作区类型。<!--update this when they change it to Generate with AI-->

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
1. （可选）要编辑工作区，请执行以下操作之一：

   * 打开工作区并手动对其进行更改。 有关信息，请参阅[编辑工作区](/help/quicksilver/planning/architecture/edit-workspaces.md)。
   * 单击&#x200B;**使用AI编辑**。 这将打开Planning Designer。 重复上述步骤以使用AI，并对工作区进行进一步更改。


