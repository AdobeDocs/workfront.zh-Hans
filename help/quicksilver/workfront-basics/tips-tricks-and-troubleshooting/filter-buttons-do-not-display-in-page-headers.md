---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 过滤器按钮未显示在页眉中
description: 阅读本文以解决页眉中不显示过滤器按钮的问题。
feature: Get Started with Workfront
author: Nolan and Alina
exl-id: 327564ed-60df-441a-a38b-a17a8c57adb0
source-git-commit: 114d306d99ae9ba0a18abd63a6137ad0568ab202
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 1%

---

# 过滤器按钮未显示在页眉中

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe[!DNL Workfront]许可证</strong></td> 
   <td> <p>[!UICONTROL 计划] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置</strong></td> 
   <td> <p>[!UICONTROL 系统管理员]</p> </td> 
  </tr> 
 </tbody> 
</table>

## 问题

以下筛选按钮不在其各自的区域显示：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!DNL Adobe Workfront] 区域</strong></td> 
   <td><strong>筛选器按钮</strong></td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 项目] </p> </td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL 我参与的项目]</p> </li> 
     <li> <p>[!UICONTROL 我拥有的项目]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><span>[!UICONTROL 时间表]</span> </td> 
   <td> 
    <ul> 
     <li> <p><span>[!UICONTROL 我的工时表批准]</span> </p> </li> 
     <li> <p><span>[!UICONTROL 我的时间表]</span> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 解决方案

[!UICONTROL 项目和时间表]区域中的筛选器按钮不显示，因为相应的筛选器未包含在应用于用户的布局模板中。 [!DNL Workfront]管理员必须分配包含筛选器的布局模板。

>[!NOTE]
>
>有时从[!UICONTROL 设置]中的[!UICONTROL 列表控件]区域移除筛选器。 [!DNL Workfront]管理员必须在此区域的列表中包含这些项，才能在布局模板中使用。

1. 验证布局模板是否显示以下过滤器：

   * 在[!UICONTROL 项目]区域[!UICONTROL 我所在的项目]和[!UICONTROL 我拥有的项目]
   * [!UICONTROL 我的工时表批准]和[!UICONTROL 我的工时表]（在[!UICONTROL 工时表]区域中）

   为此，请执行以下操作：

   1. 访问布局模板。
   1. 在&#x200B;**[!UICONTROL 自定义用户看到的内容]**&#x200B;下选择&#x200B;**[!UICONTROL 列表]**。
   1. 在&#x200B;**[!UICONTROL 下选择**&#x200B;[!UICONTROL &#x200B;项目&#x200B;]&#x200B;**或**&#x200B;[!UICONTROL &#x200B;时间表&#x200B;]&#x200B;**选择要自定义的列表]**。
   1. 在&#x200B;**[!UICONTROL 筛选器]**&#x200B;部分中，验证是否选择了我所在的&#x200B;**[!UICONTROL 项目]**、**[!UICONTROL 我拥有的项目]**（项目）和&#x200B;**[!UICONTROL 我的工时表批准]**&#x200B;和&#x200B;**[!UICONTROL 我的工时表]**（时间表）。
   1. 单击&#x200B;**[!UICONTROL 保存]**。

   有关详细信息，请参阅[使用布局模板自定义筛选器、视图和分组](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)。

1. 将布局模板分配给正确的用户、工作角色、团队或组。 有关信息，请参阅[将用户分配给布局模板](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)。
