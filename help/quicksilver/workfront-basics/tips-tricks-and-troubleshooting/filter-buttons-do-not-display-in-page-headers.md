---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 过滤器按钮不显示在页面标题中
description: 请阅读本文，对页面标题中未显示过滤器按钮的问题进行故障诊断。
feature: Get Started with Workfront
author: Lisa and Alina
exl-id: 327564ed-60df-441a-a38b-a17a8c57adb0
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 1%

---

# 过滤器按钮不显示在页面标题中

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] 许可证</strong></td> 
   <td> <p>[!UICONTROL计划] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置</strong></td> 
   <td> <p>[!UICONTROL系统管理员]</p> </td> 
  </tr> 
 </tbody> 
</table>

## 问题

以下过滤器按钮不会显示在其各自的区域中：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!DNL Adobe Workfront] 面积</strong></td> 
   <td><strong>过滤器按钮</strong></td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL项目] </p> </td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL项目我正在执行]</p> </li> 
     <li> <p>[！我拥有的UICONTROL项目]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><span>[!UICONTROL时间表]</span> </td> 
   <td> 
    <ul> 
     <li> <p><span>[!UICONTROL My Timetime Approvals]</span> </p> </li> 
     <li> <p><span>[!UICONTROL我的时间表]</span> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 解决方案

中的过滤器按钮 [!UICONTROL 项目和时间表] 区域不会显示，因为相应的过滤器未包含在应用于用户的布局模板中。 的 [!DNL Workfront] 管理员必须分配包含过滤器的布局模板。

>[!NOTE]
>
>有时，过滤器会从 [!UICONTROL 列表控件] 区域 [!UICONTROL 设置]. 的 [!DNL Workfront] 管理员必须在此区域的列表中包含这些模板，才能在布局模板中使用这些模板。

1. 验证布局模板是否显示以下过滤器：

   * [!UICONTROL 我正在执行的项目] 和 [!UICONTROL 我拥有的项目] 在 [!UICONTROL 项目] 面积
   * [!UICONTROL 我的时间表批准] 和 [!UICONTROL 我的工时表] 在 [!UICONTROL 时间表] 面积

   要执行此操作，请执行以下操作：

   1. 访问布局模板。
   1. 选择 **[!UICONTROL 列表]** 在 **[!UICONTROL 自定义用户看到的内容]**.
   1. 选择 **[!UICONTROL 项目]** 或 **[!UICONTROL 工时单]** 在 **[!UICONTROL 选择要自定义的列表]**.
   1. 在 **[!UICONTROL 过滤器]** 部分，验证 **[!UICONTROL 我正在执行的项目]**, **[!UICONTROL 我拥有的项目]** （对于项目）和 **[!UICONTROL 我的时间表批准]** 和 **[!UICONTROL 我的工时表]** （对于工时单）。
   1. 单击&#x200B;**[!UICONTROL 保存]**。

   有关更多信息，请参阅 [使用布局模板自定义过滤器、视图和分组](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. 将布局模板分配给正确的用户、作业角色、团队或组。 有关信息，请参阅 [将用户分配到布局模板](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).
