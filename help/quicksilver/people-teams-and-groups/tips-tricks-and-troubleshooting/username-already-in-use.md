---
content-type: tips-tricks-troubleshooting
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-groups
title: 用户名已被使用
description: 当出现用户名已被占用的错误时，请阅读这些提示。
author: Lisa
feature: People Teams and Groups
exl-id: dc9accf0-7ef4-4555-9b1c-d69b2110f3da
source-git-commit: 722295463c1338a70ff42c26acf69b09cf33f725
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 1%

---

# 用户名已被使用

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td>
   <p>标准</p>
   <p>规划</p></td>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td><p>系统管理员</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

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

{{step-1-to-users}}

1. 在人员列表中，查看&#x200B;**[!UICONTROL 电子邮件]**&#x200B;列，确保没有重复的电子邮件。
1. 在视图中添加用户名列。

   1. 在&#x200B;**[!UICONTROL 视图]**&#x200B;下拉菜单中，单击&#x200B;**[!UICONTROL 自定义视图]**。
   1. 单击&#x200B;**[!UICONTROL 添加列]**。
   1. 在搜索字段中，键入&#x200B;*[!UICONTROL 用户名]*。
   1. 选择&#x200B;**[!UICONTROL 用户]** > **[!UICONTROL 用户名]**。
   1. 保存视图。\
      这将生成一个显示用户名的视图，您可以在其中查找重复项。

1. 在人员列表中，查看&#x200B;**[!UICONTROL 用户名]**&#x200B;列以确保没有重复的用户名。
