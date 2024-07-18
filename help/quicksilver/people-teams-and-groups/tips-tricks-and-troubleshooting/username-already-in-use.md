---
content-type: tips-tricks-troubleshooting
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-groups
title: 用户名已被使用
description: 当出现用户名已被占用的错误时，请阅读这些提示。
author: Lisa
feature: People Teams and Groups
exl-id: dc9accf0-7ef4-4555-9b1c-d69b2110f3da
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# 用户名已被使用

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
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证</strong></td> 
   <td> <p>[！UICONTROL计划]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置</strong></td> 
   <td> <p>[！UICONTROL系统管理员]</p> </td> 
  </tr> 
 </tbody> 
</table>

## 问题

创建新用户时，显示[!UICONTROL 糟糕]错误，说明用户名已被占用。 在系统中没有出现过此电子邮件。 为什么显示此信息？

## 解决方案

这可能是因为用户名或电子邮件地址在当前[!DNL Adobe Workfront]实例中不是唯一的。 用户在单独的实例中可以拥有相同的用户名或电子邮件地址。 例如，用户A可能具有以下与[!DNL Workfront]帐户关联的电子邮件地址：usera@company1.com和usera@company2.com。

>[!NOTE]
>
>如果主[!DNL Workfront]管理员位于同一群集上的不同Workfront实例中，则他们不能拥有相同的用户名或电子邮件地址。
>
>如果实例位于不同的群集上，则主管理员可以具有相同的用户名或电子邮件地址。 您可以在[!UICONTROL 设置] > [!UICONTROL 系统] > [!UICONTROL 客户信息]下查看实例所在的群集。

### 检查您的用户名在实例中是否唯一

确保用户名和电子邮件地址在当前[!DNL Workfront]实例中是唯一的：

1. 作为[!DNL Workfront]管理员，单击[!DNL Adobe Workfront]右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 用户]**。
1. 在人员列表中，查看&#x200B;**[!UICONTROL 电子邮件]**&#x200B;列，确保没有重复的电子邮件。
1. 在视图中添加用户名列。

   1. 在&#x200B;**[!UICONTROL 视图]**&#x200B;下拉菜单中，单击&#x200B;**[!UICONTROL 自定义视图]**。
   1. 单击&#x200B;**[!UICONTROL 添加列]**。
   1. 在搜索字段中，键入&#x200B;*[!UICONTROL 用户名]*。
   1. 选择&#x200B;**[!UICONTROL 用户]** > **[!UICONTROL 用户名]**。
   1. 保存视图。\
      这将生成一个显示用户名的视图，您可以在其中查找重复项。

1. 在人员列表中，查看&#x200B;**[!UICONTROL 用户名]**&#x200B;列以确保没有重复的用户名。
