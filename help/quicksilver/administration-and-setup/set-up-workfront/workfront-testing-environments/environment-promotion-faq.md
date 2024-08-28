---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 环境提升常见问题解答
description: 探索有关Workfront环境升级的常见问题。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: e9794262-80cc-4641-a5c6-7130cf008ba2
source-git-commit: 2bbfd449d913a5134c9c36b1ee10567973c56eaa
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 3%

---

# 环境提升常见问题解答

以下是有关环境升级的常见问题解答：

## 是否支持跨域提升？

### 答案

当前不支持跨域环境升级。 您必须在同一域中的环境之间升级。

## Adobe业务平台/IMS是否是提升环境的先决条件？

### 答案

不可以。环境升级适用于启用了IMS和非IMS的Workfront实例。

## 我们如何确定Workfront实例是在Prime还是Ultimate许可证上？

### 答案

* Workfront管理员可以找到您组织的许可证。

   1. 单击Adobe Workfront右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon.png)，或（如果可用）单击左上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png)，然后单击&#x200B;**[!UICONTROL 设置]** ![设置图标](/help/_includes/assets/gear-icon-setup.png)。
   1. 单击左侧面板中的&#x200B;**系统**
   1. 要查看您的Workfront计划，请选择&#x200B;**许可证**。
您的计划将显示在页面的右上角附近。
      ![](assets/locate-plan.png)

  或
* 请联系您的Workfront客户代表。

## Environment Promotion是双向的吗？

### 答案

可以。例如，您可以从Sandox提升到Production，或从Production提升到Sandbox。

## 是否支持共享？

### 答案

否，当前不支持共享。

## 回滚功能何时可用？

### 答案

回滚是重中之重，目前正在开发中。 我们预计将在2024年第3季度或第四季度发布回滚功能。

## 是否可以选择跳过单个组件的升级？ 存在选项“`Use Existing`”、“`Overwrite`”和“`Save with a new Name`”的情况下，是否可以添加`Skip`以跳过单个参数的升级？

### 答案


* “使用现有”与“跳过”或忽略部署相同，因为它映射到目标环境中的现有对象，并且不进行任何更改。
* 要跳过对象，我们建议删除
不想从升级包或直接从源环境安装的任何对象。 移除对象后，重新装配包。
