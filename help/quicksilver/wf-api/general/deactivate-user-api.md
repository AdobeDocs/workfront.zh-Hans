---
content-type: api
product-area: user-management
navigation-topic: general-api
title: 通过API停用用户
description: 通过API停用用户
author: Becky
feature: Workfront API
role: Developer
exl-id: 45b06cce-4622-4739-b9f3-2edb9101c099
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---


# 通过API停用用户

当用户离开您的组织时，您可以停用该用户，使其的Adobe Workfront许可证可供其他用户使用，并防止意外地为他们分配工作。 通过停用用户，您可以保留用户的工作历史记录，包括其工作分配以及与注释、小时和文档的关联。

要了解有关停用用户的更多信息，请参阅&quot; [停用或重新激活用户](../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

有关使用核心API的信息，请参阅 [API基础知识](../../wf-api/general/api-basics.md).

要通过API停用用户，请执行以下操作：

1. 使用以下API请求生成API密钥：

```
<domain>.my.workfront.com/attask/api/v15.0/user?action=generateApiKey&username=`username`&password=`password`&method=PUT`
```

1. 找到要取消激活的用户的GUID。

   1. 使用以下API请求检索系统中所有用户的GUID，请注意 **isActive** 字段显示 **true** 适用于当前处于活动状态且 **false** 对于已取消激活的用户：

```
<domain>`.my.workfront.com/attask/api/v15.0/USER/search?fields=isActive
```

1. 找到要取消激活的用户的GUID，请使用以下内容 **PUT** 请求更改用户的 **isActive** 字段值至 **false**：

```
<domain>`.my.workfront.com/attask/api/v15.0/USER/`<user's GUID>`?updates={"isActive":"false"}&method=put&apiKey=`<apiKey>`&fields=isActive
```

1. 响应会显示 **isActive** 字段值已从 **true** 到 **false**&#x200B;指示用户已停用：

<!-- [Copy](javascript:void(0);) -->
<pre><code>{<br>&nbsp;&nbsp;&nbsp;&nbsp;data:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ID:&nbsp;"592125e60089b88fae8b51c08383e144",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;name:&nbsp;"Tyler Reid",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;objCode:&nbsp;"USER",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;isActive:&nbsp;false&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br>}<br></code></pre>
