---
content-type: tips-tricks-troubleshooting
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-groups
title: 用户名已在使用中
description: 当您收到用户名已被获取的错误时，请阅读这些提示。
author: Lisa
feature: People Teams and Groups
exl-id: dc9accf0-7ef4-4555-9b1c-d69b2110f3da
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# 用户名已在使用中

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
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证</strong></td> 
   <td> <p>[!UICONTROL计划]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置</strong></td> 
   <td> <p>[!UICONTROL系统管理员]</p> </td> 
  </tr> 
 </tbody> 
</table>

## 问题

创建新用户时， [!UICONTROL 哇] 显示错误，表明用户名已被使用。 此电子邮件在系统中没有其他事件。 为什么会显示此内容？

## 解决方案

由于当前用户名或电子邮件地址不唯一，因此可能会发生这种情况 [!DNL Adobe Workfront] 实例。 用户可以在不同的实例中使用相同的用户名或电子邮件地址。 例如，用户A可以将以下电子邮件地址与 [!DNL Workfront] 帐户：usera@company1.com和usera@company2.com。

>[!NOTE]
>
>主 [!DNL Workfront] 如果管理员位于同一群集上的单独Workfront实例中，则无法具有相同的用户名或电子邮件地址。
>
>如果实例位于不同的群集上，则主管理员可以具有相同的用户名或电子邮件地址。 您可以查看实例所在的群集，该群集位于 [!UICONTROL 设置] > [!UICONTROL 系统] > [!UICONTROL 客户信息].

### 检查您的用户名在实例中是否唯一

确保用户名和电子邮件地址在当前 [!DNL Workfront] 实例：

1. 作为 [!DNL Workfront] 管理员，单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 用户]**.
1. 在人员列表中，查看 **[!UICONTROL 电子邮件]** 列，以确保不存在重复的电子邮件。
1. 向视图中添加用户名列。

   1. 在 **[!UICONTROL 查看]** 下拉菜单中，单击 **[!UICONTROL 自定义视图]**.
   1. 单击 **[!UICONTROL 添加列]**.
   1. 在搜索字段中，键入 *[!UICONTROL 用户名]*.
   1. 选择 **[!UICONTROL 用户]** > **[!UICONTROL 用户名]**.
   1. 保存视图。\
      这会导致视图显示可在其中查找副本的用户名。

1. 在人员列表中，查看 **[!UICONTROL 用户名]** 列，以确保不存在重复的用户名。
