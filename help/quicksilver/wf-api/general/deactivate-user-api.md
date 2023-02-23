---
content-type: api
product-area: user-management
navigation-topic: general-api
title: 通过API停用用户
description: 通过API停用用户
author: John
feature: Workfront API
exl-id: 45b06cce-4622-4739-b9f3-2edb9101c099
source-git-commit: c1cec2c08c66c704385cde1abd0c019fd59702da
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---


# 通过API停用用户

当用户离开您的组织时，您可以停用用户，将其Adobe Workfront许可证提供给其他用户，并防止他们意外地被分配到工作。 通过取消激活用户，可保留其工作历史记录，包括其工作分配以及与注释、小时和文档的关联。

要了解有关取消激活用户的更多信息，请参阅 [停用或重新激活用户](../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

有关使用核心API的信息，请参阅 [API基础知识](../../wf-api/general/api-basics.md).

要通过API停用用户，请执行以下操作：

1. 使用以下API请求生成API密钥：

```
<domain>.my.workfront.com/attask/api/v15.0/user?action=generateApiKey&username=`username`&password=`password`&method=PUT`
```

1. 找到要停用的用户的GUID。

   1. 请使用以下API请求来检索系统中所有用户的GUID，请注意 **isActive** 字段显示 **true** 适用于当前处于活动状态和 **false** 对于已停用的用户：

```
<domain>`.my.workfront.com/attask/api/v15.0/USER/search?fields=isActive
```

1. 找到要停用的用户的GUID，使用以下 **PUT** 更改用户 **isActive** 字段值 **false**:

```
<domain>`.my.workfront.com/attask/api/v15.0/USER/`<user's GUID>`?updates={"isActive":"false"}&method=put&apiKey=`<apiKey>`&fields=isActive
```

1. 响应将显示 **isActive** 字段值已从 **true** to **false**&#x200B;表示用户已停用：

<!-- [Copy](javascript:void(0);) -->
<pre></pre>
