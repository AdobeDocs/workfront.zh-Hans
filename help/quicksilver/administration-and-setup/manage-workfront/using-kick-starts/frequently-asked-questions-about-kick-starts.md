---
user-type: administrator
content-type: faq
product-area: system-administration
keywords: kickstart，kick-start，kickstarts，kick-starts
navigation-topic: use-kick-starts
title: 有关Kick-Starts的常见问题解答
description: 查找有关使用Kick-Starts导入和导出Workfront数据的常见问题解答。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f286e03e-93a8-43f5-8c2d-2c36203776a8
source-git-commit: 1ebdb3797e30a7e06f4dfd4a7e0e5f540351c126
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# 有关Kick-Starts的常见问题解答

以下是有关Kick-Starts的常见问题解答：

## 为什么在尝试导入快速启动文件时会收到此错误：“您的文件正确，但未导入任何内容？”

### 答案

Kick-Start文件中可能缺少以下三个内容之一：

1. 对于所有要导入的项目，**isNew**&#x200B;列必须设置为&#x200B;**TRUE**。 **isNew**&#x200B;必须是&#x200B;**TRUE**，因为您只能通过Kick-Start导入新数据。 您无法通过Kick-Start修改现有数据。 电子表格中可以有其他行，其中&#x200B;**isNew = FALSE**，但这些行将不会导入。

1. 文&#x200B;件需要在数据的标头之前有一个空行。
1. Excel&#x200B;工作表需要具有正确的名称。

使用Kick-Starts时，我们建议首先下载Kick-Start模板，手动为其填充正确数据，然后将其导入回Adobe Workfront。

有关使用Kick-Start在Workfront中正确导入数据的更多信息，请参阅[使用Kick-Start模板将数据导入Adobe Workfront](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)。

## 为什么我在尝试使用快速启动文件将小时数导入Workfront时收到此错误：“未找到具有主键值“空”的用户？”

### 答案

错误是指与小时关联的用户的GUID。

要解决此问题：

1. 仅导出&#x200B;**小时**&#x200B;对象的空白快速启动模板。\
   有关导出空白快速启动文件的更多信息，请参阅[使用快速启动模板将数据导入Adobe Workfront](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)中的“导出快速启动模板”。

1. 手动从原始快速启动中复制数据并将其粘贴到空文件中。\
   对每一列执行此操作。
1. 再次尝试导入新文件。\
   Kick-Start应该可以成功导入。

## 为什么Kick-Start导入的用户配置文件上未填充country字段？

### 问题

使用字段&#x200B;**setCountry**&#x200B;导入用户Kick-Start时，该数据不会进入用户配置文件中的国家/地区。

### 答案

如果用户启用了统一用户管理(UUM)或AdobeIdentity Management System (IMS)，**国家/地区**&#x200B;字段仅接受国家/地区代码值（例如，US、GB、IN）。 在导入之前，请验证快速启动模板中的&#x200B;**setCountry**&#x200B;字段是否正在使用国家/地区代码值。

有关使用Kick-Start在Workfront中正确导入数据的更多信息，请参阅[使用Kick-Start模板将数据导入Adobe Workfront](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)。
