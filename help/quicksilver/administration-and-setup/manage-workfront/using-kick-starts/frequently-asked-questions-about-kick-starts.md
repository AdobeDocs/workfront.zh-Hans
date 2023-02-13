---
user-type: administrator
content-type: faq
product-area: system-administration
keywords: kickstart，kickstart，kickstarts，kickstarts
navigation-topic: use-kick-starts
title: 有关Kick-Start的常见问题解答
description: 查找有关使用Kick-Starts导入和导出Workfront数据的常见问题解答。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f286e03e-93a8-43f5-8c2d-2c36203776a8
source-git-commit: 1ebdb3797e30a7e06f4dfd4a7e0e5f540351c126
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# 有关Kick-Start的常见问题解答

以下是有关启动的常见问题：

## 为什么我在尝试导入Kick-Start文件时收到此错误：“您的文件正确，但未导入任何内容？”

### 回答

Kick-Start文件中可能缺少以下三项之一：

1. 的 **isNew** 列必须设置为 **TRUE** ，用于所有要导入的项目。 **isNew** 必须 **TRUE** 因为您只能通过Kick-Start导入新数据。 您无法通过Kick-Start修改现有数据。 您可以在电子表格中的其他行中使用 **isNew = FALSE** 但是，这些行将不会导入。

1. &#x200B;文件需要在数据标题开始之前有一个空行。
1. &#x200B;Excel工作表需要具有正确的名称。

使用Kick-Start时，我们建议先下载Kick-Start模板，手动填充正确的数据，然后将其导入回Adobe Workfront。

有关使用Kick-Start在Workfront中正确导入数据的更多信息，请参阅 [使用“启动”模板将数据导入Adobe Workfront](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## 为什么我在尝试使用Kick-Start文件将小时导入Workfront时会收到此错误：&quot;未找到主键值为&quot;null&quot;的用户？&quot;

### 回答

错误是指与小时关联的用户的GUID。

要解决此问题，请执行以下操作：

1. 导出空白的“启动”模板 **小时** 仅对象。\
   有关导出空白启动文件的更多信息，请参阅  [使用“启动”模板将数据导入Adobe Workfront](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

1. 手动复制原始Kick-Start中的数据，并将其粘贴到空文件中。\
   为每个列执行此操作。
1. 再次尝试导入新文件。\
   Kick-Start应成功导入。

## 为什么Kick-Start导入中的用户配置文件中没有填充国家/地区字段？

### 问题

使用字段导入用户Kick-Start时 **setCountry**，则该数据不会从用户配置文件传入国家/地区。

### 回答

如果用户启用了统一用户管理(UUM)或AdobeIdentity Management系统(IMS)，则 **国家/地区** 字段仅接受国家/地区代码值（例如，US、GB、IN）。 验证 **setCountry** 导入之前，启动模板中的字段正在使用国家/地区代码值。

有关使用Kick-Start在Workfront中正确导入数据的更多信息，请参阅 [使用“启动”模板将数据导入Adobe Workfront](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).
