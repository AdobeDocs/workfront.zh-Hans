---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: 配置对Blueprint的访问权限
description: 作为系统管理员，您可以通过设置请求队列来存储请求，从而为用户启用请求安装Blueprint的访问权限。 在那里，您只有一个位置可以跟踪和更新请求。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d85f363f-2ab4-45cb-b851-a7f33e1ca905
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# 配置对Blueprint的访问权限

所有[!DNL Adobe Workfront]用户都可以浏览Blueprint的目录。

作为系统管理员，您可以：

* 将[!UICONTROL Blueprint]添加到布局模板的主菜单，并将布局模板分配给用户或组。 有关详细信息，请参阅[使用布局模板自定义[!UICONTROL 主菜单]](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)和[将用户分配给布局模板](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)。

  >[!NOTE]
  >
  >* 未分配布局模板的用户将在[!UICONTROL 主菜单]中看到[!UICONTROL Blueprint]图标。
  >* 创建新布局模板时，[!UICONTROL 主菜单]的[!UICONTROL 活动项]列表中默认包含[!UICONTROL Blueprint]图标。


* 通过设置用于存储请求的请求队列，为用户启用访问，以请求安装Blueprint。 在那里，您只有一个位置可以跟踪和更新请求。 有关更多信息，请按照以下步骤操作。
* 安装Blueprint。 有关信息，请参阅[安装Blueprint](../../administration-and-setup/blueprints/blueprints-install.md)。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划</strong></td> 
   <td> <p> 任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe[!DNL Workfront]许可证</strong></td> 
   <td>[！UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置</strong></td> 
   <td> <p>[！UICONTROL系统管理员]</p> </td> 
  </tr> 
 </tbody> 
</table>

## 先决条件 {#prerequisites}

* 您必须使用现有请求队列来存储Blueprint请求。 项目必须另存为请求队列，并且必须处于[!UICONTROL 当前]状态。
* 请求队列必须是公共的。 在请求队列详细信息中，&#39;&#39;[!UICONTROL 谁可以将请求添加到此队列？“]”必须设置为&#x200B;**[!UICONTROL 任何人]**。

>[!TIP]
>
>如果要为Blueprint请求创建新的请求队列，则应该在配置Blueprint访问之前构建它。 有关创建请求队列的信息，请参阅[创建请求队列](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。

## 选择请求队列以存储Blueprint请求

在用户请求您为其安装Blueprint之前，您必须为这些请求选择请求队列。 在定义请求队列之前，用户只能浏览Blueprint目录。

1. 单击[!DNL Adobe Workfront]右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL Blueprints]**。
1. 单击目录屏幕右上角的&#x200B;**[!UICONTROL 配置Blueprint请求]**。

   <!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>In the <strong>Configure blueprints</strong> dialog, ensure that the <strong>Configure request queues</strong> tab is selected.</p> </li>
   -->

1. 在&#x200B;**[!UICONTROL 配置Blueprint]**&#x200B;对话框中，开始键入活动请求队列的名称，并在该名称出现在搜索结果中时将其选定。

   >[!IMPORTANT]
   >
   >此列表中只显示公共请求队列。 要使您的请求队列公开，请参阅上面的[先决条件](#prerequisites)部分。

   已设置请求队列首选项，用户现在可以请求Blueprint安装。

   ![配置请求队列](assets/Blueprints_access_setup_request_queue.png)

1. （可选）若要更改实际请求队列，请单击&#x200B;**[!UICONTROL 编辑此请求队列]**。

   请求队列项目将在新的浏览器选项卡中打开，您可以根据需要对其进行更新。

1. （可选）如果请求队列包含主题组或队列主题，则可以从列表中选择它们。
1. 要返回Blueprint目录，请单击&#x200B;**[!UICONTROL 关闭]**。

>[!NOTE]
>
>安装请求的Blueprint时，您应该将请求队列中的问题状态更改为&#x200B;**[!UICONTROL 已关闭]**&#x200B;或&#x200B;**[!UICONTROL 已解决]**，以便通知请求者。 有关安装Blueprint的信息，请参阅[安装Blueprint](../../administration-and-setup/blueprints/blueprints-install.md)。
