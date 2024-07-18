---
content-type: reference
product-area: documents
navigation-topic: workfront-dam-within-workfront
title: Adobe Workfront许可角色类型与Adobe Workfront DAM角色类型
description: Adobe Workfront管理员使用访问级别来确定用户在应用程序中可以执行的操作。
author: Courtney
feature: Digital Content and Documents
exl-id: dcca0158-dc31-4aba-bd87-90ccc64e77cb
source-git-commit: 5469598d57fec1a744ddb44cf2accb94e1f70941
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 2%

---

# Adobe Workfront许可角色类型与Adobe Workfront DAM角色类型

Adobe Workfront管理员使用访问级别来确定用户在应用程序中可以执行的操作。

* 在Workfront中，许可决定用户的访问级别。
* 在Workfront DAM中，角色类型定义了用户对DAM中资源的访问权限。

由于许可证类型和角色类型不可互换，因此在一个应用程序中拥有访问级别并不意味着在另一个应用程序中拥有访问。 例如，在Workfront中拥有工作许可证的用户不会在Workfront DAM中自动分配投稿人角色。

## Workfront 许可证类型

作为Workfront管理员，您可以通过分配许可证类型来定义用户具有的访问级别。 每个许可证都附带一组默认访问功能，在将许可证分配给用户之前，您可以修改这些功能。 

可使用许可确定用户在Workfront中可以查看和执行的操作。 Workfront提供五种许可类型：

* 计划
* 工作
* 评论
* 请求
* 外部的

有关Workfront中各种许可证类型的说明，请参阅[旧版许可证概述](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md)。

## Workfront DAM角色类型

作为Workfront DAM Workfront管理员，您可以为用户分配角色类型，以定义他们对资源的访问权限。 此外，角色类型还指定DAM中用户可以工作的区域。

建立用户访问权限时，角色类型可与组配合使用。 组控制用户对文件夹和资产本身的访问权限。 角色类型确定用户可以对资源执行的操作。 所有DAM用户必须至少与一个组关联。 要了解有关角色类型和访问配置的更多信息，请参阅Workfront DAM中的帮助。

Workfront DAM中有四种不同的角色类型可用：

### Brand Portal

此角色类型的用户只能访问DAM中的Brand Connect门户。 在该门户中，用户可以查看和下载他们有权访问的资产。

Brand Portal用户可以通过创建和共享灯箱与他人协作。

### 普通用户

具有此角色类型的用户可以从Workfront DAM和Brand Connect门户查看和下载资产。

普通用户还可以通过创建和共享灯箱与他人协作。

### 投稿人

具有此角色类型的用户有权访问Workfront DAM和Brand Connect门户。

参与者可以查看、下载、上传、编辑、移动和删除他们有权访问的资源和文件夹。 此外，参与者可以通过创建和共享灯箱与他人协作。 

### 管理员

Workfront管理员有权访问Brand Connect门户和Workfront DAM中的所有内容，包括已过期或处于非活动状态的资源。

要具有管理员访问权限，具有管理员角色类型的用户必须位于管理员组中。
