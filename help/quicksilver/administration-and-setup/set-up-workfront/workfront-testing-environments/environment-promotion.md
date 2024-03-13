---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 将对象从一个环境移动到另一个环境
description: 环境升级功能旨在提供与配置相关的对象从一个环境移动到另一个环境的功能。 它不支持移动事务性对象的功能（只有有限的例外）。
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: dd3c29df-4583-463a-b27a-bbfc4dda8184
source-git-commit: b44c83314a06592e21ab3c4316e2574b75e85715
workflow-type: tm+mt
source-wordcount: '1894'
ht-degree: 2%

---

# 在对象之间移动 [!DNL Workfront] 使用环境 [!DNL Workfront] 环境提升API

环境升级功能旨在提供与配置相关的对象从一个环境移动到另一个环境的功能。 您可以使用Workfront API移动这些对象，如本文所述。

有关使用Workfront应用程序在环境之间移动对象的说明，请参阅：

* [创建或编辑环境升级包](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
* [安装环境升级包](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] 计划</td> 
   <td> <p>Enterprise、Prime或Ultimate</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!DNL Workfront] 许可证</p> </td> 
   <td> <p>[！UICONTROL计划] </p> <p>您必须是 [!DNL Workfront] 管理员。 有关的信息 [!DNL Workfront] 管理员，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理权限</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">对象权限</p> </td> 
   <td> <p>全部</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">支持包</td> 
   <td> <p>[！UICONTROL Plus]、[！UICONTROL Preferred]或[！UICONTROL Enterprise]</p> <p>标准支持包无权访问自定义刷新沙盒，但有权访问预览沙盒。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 先决条件

创建升级包端点假定您已配置源环境。 此API调用需要手动创建 [!DNL Workfront] 对象代码和对象GUID。 此地图的特定结构如下所述。

## 环境升级支持的对象

环境升级功能旨在提供与配置相关的对象从一个环境移动到另一个环境的功能。 它不支持移动事务性对象的功能（只有有限的例外）。

有关可升级对象及其包含的可升级子对象的列表，请参见 [环境升级支持的对象](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#supported-objects-for-environment-promotion) 在文章中 [在Workfront环境之间移动对象概述](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md).

## 身份验证

API对每个请求进行身份验证，以确保客户端有权查看或修改请求的对象。

身份验证是通过传入会话ID或API密钥执行的，可使用以下方法提供该密钥：

### 请求标头身份验证

首选的身份验证方法是传递包含会话令牌的名为SessionID的请求标头。 这有一个优势，就是可以安全抵御 [跨站点请求伪造(CSRF)](https://en.wikipedia.org/wiki/Cross-site_request_forgery) 攻击，并且不会出于缓存目的干扰URI。

以下是请求标头的示例：

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

## API端点

* [创建资源包](#create-a-package)
* [获取程序包列表](#get-a-list-of-packages)
* [按ID获取包](#get-a-package-by-id)
* [更新包的特定属性](#update-specific-properties-of-a-package)
* [删除资源包](#delete-a-package)
* [执行预运行](#execute-a-pre-run)
* [执行安装](#execute-an-installation)
* [获取特定软件包的安装列表](#get-a-list-of-installations-for-a-specific-package)
* [获取安装的安装详细信息](#get-the-installation-details-for-an-installation)

### 创建资源包

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /packages</code></td> 
  </tr> 
  </tbody> 
</table>

此调用执行多步骤流程。

第一步会创建一个处于“ASSEMBLING”状态的空促销包。

第二步使用 `objectCollections` 在POST正文中提供的数组，用于汇编来自Workfront的请求记录。 完成此步骤可能需要几分钟，具体取决于请求的记录数以及Workfront配置。 在此流程结束时，空的促销活动包将更新为 `packageEntities` 并且状态自动设置为“草稿”。


>[!NOTE]
>
>请注意的结构 `objectCollections`  数组。
>
>数组中的每一项包含 `objCode` 与Workfront API Explorer中记录的目标代码对应的键。
>
>每个项目还包含 `entities` 收藏集。 这需要 `ID` 字段。 它也可以接受一个可选的 `name` 属性以便于了解 `ID` 表示。
>
>对于在中请求的允许对象代码列表 `objectCollections` 列表，请参见 [环境升级支持的对象](#supported-objects-for-environment-promotion) 部分。

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages
```

#### 标头

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

或

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### 正文

```json
{
    "name": "Agency Onboarding - 2023-06-06",
    "description": "This promotion package contains configuration to support the agency onboarding processes...",
    "source": "https://{domain}.{environment}.workfront.com",
    "objectCollections": [
        {
            "objCode": "PROJ",
            "entities": [
                {
                    "ID": "6419b8b9001151ee258921a4f7597ba1",
                    "name": "Agency Request"
                }
            ]
        },
        {
            "objCode": "TMPL",
            "entities": [
                {
                    "ID": "6419b8b9001151ee258921a4f7597bb2",
                    "name": "New Agency Onboarding"
                },
                {
                    "ID": "6419b8b9001151ee258921a4f7597bc3",
                    "name": "New Agency Offboarding"
                }
            ]
        },
        {
            "objCode": "PTLTAB",
            "entities": [
                {
                    "ID": "645e6435000b4aaebe4776f4a42ed5ad",
                    "name": "Agency Performance and Readiness"
                }
            ]
        }
    ]
}
```

#### 响应

```json
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "ASSEMBLING",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d"
    }
}
```

### 获取程序包列表

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages</code></td> 
  </tr> 
  </tbody> 
</table>

此调用会返回属于客户的未过滤促销包列表。

响应将包括从客户的任何沙盒、预览或Workfront的生产实例创建的所有包。

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages
```

#### 标头

```json
{
    "apikey": "**********"
}
```

或

```json
{
    "sessionID": "*****************"
}
```

#### 正文

_空_

#### 响应

```
200
```

```json
{
    "data": [
        {
            "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
            "name": "Agency Onboarding - 2023-06-06",
            "description": "This promotion package contains configuration to support the agency onboarding processes...",
            "status": "ASSEMBLING",
            "createdAt": "2023-06-06T17:29:21.600Z",
            "deletedAt": null
},
        {...}
    ]
}
```

&lt;! — 检查上面的“状态” — 它是否已添加？—>

### 按ID获取包

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

此调用返回所请求促销活动包的详细信息。

无论升级包的原始来源如何，均可通过任何环境发出请求。

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### 标头

```json
{
    "apikey": "**********"
}
```

或

```json
{
    "sessionID": "*****************"
}
```

#### 正文

_空_

#### 响应

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "DRAFT",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "packageEntities": {
            "GROUP": [
               {
                   "id": "52aa9d0e0005fcee8f212835bdaa2691",
                   "name": "Default Group",
                   "description": "null"
                   - or -
                   "description": "..."
               }
            ],
            "ROLE": [
               {...}
            ],
            ...
        }
   }
}
```

### 更新包的特定属性

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>PATCH /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

此调用会更新促销活动正文中提供的促销PATCH包的任何内容。

可编辑的属性包括：

1. 名称（字符串）
1. description（字符串）
1. 状态（带值验证的字符串）

有关可用状态的详细说明，请参阅 [环境提升状态](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#environment-promotion-statuses) 在文章中 [在Workfront环境之间移动对象概述](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md).


#### URL

```
PATCH https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```


#### 标头

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

或

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### 正文

```json
{
    "status": "ACTIVE"
}
```

#### 响应

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "ACTIVE",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "publishedAt": "2023-06-06T19:39:01.600Z",
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "packageEntities": {
            "GROUP": [
               {
                   "id": "52aa9d0e0005fcee8f212835bdaa2691",
                   "name": "Default Group",
                   "description": "..."
               }
            ],
            "ROLE": [
               {...}
            ],
            ...
        }
   }
}
```

### 删除资源包

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>DELETE /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

此调用将删除促销包记录。 此操作不可逆。

>[!NOTE]
>
>与删除促销包相反，建议将包的状态更改为“已禁用”。 这将允许检索包，并保留其部署位置的安装历史记录。

#### URL

```
DELETE https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### 标头

```json
{
    "apikey": "**********"
}
```

或

```json
{
    "sessionID": "*****************"
}
```

#### 正文

_空_

#### 响应

```
200
```

```
Deleted
```

### 执行预运行

>[!IMPORTANT]
>
>在执行安装之前，必须执行此预运行。 在执行安装时，将使用从此调用生成的ID。

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST  {customer-domain}/environment-promotion/api/v1/packages/{id}/prepare-installation</code></td> 
  </tr> 
  </tbody> 
</table>

此调用会对包定义与URL中标识的目标环境进行比较。

结果是一个JSON主体，用于标识是否在目标环境中找到升级对象。

对于每个升级对象，请使用下列选项之一 `actions`  将设置：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>创建</td> 
   <td><p>当在目标环境中找不到相应的记录时，该操作将设置为CREATE。</p><p>当此操作在 <code>translationmap</code> 提供给 <code>/install</code> 终结点，安装服务将创建记录。</p></td> 
  </tr> 
  <tr> 
   <td>USEEXISTING</td> 
   <td><p>在目标环境中找到相应的记录时，该操作将设置为USEEXISTING ，并且 <code>targetId</code> 在中捕获 <code>translationmap</code>.</p><p>当此操作在 <code>translationmap</code> 提供给 <code>/install</code> 终结点，安装服务将不会创建记录。 但是，它会使用 <code>targetId</code> 包括在可能引用此记录的其他对象的映射条目中。</p><p>例如，在包将部署到的目标环境中可以找到“默认组”。 由于不可能有两个“默认组”记录，因此安装服务将在任何其他包含对“默认组”的引用的对象创建操作中使用现有组的GUID，如项目、表单或与此组相关的任何其他实体。</p><p><b>注意：</b> <ul><li><p>分配USEEXISTING操作后，将不会修改目标环境中的现有记录。 </p><p>例如，如果在从中构建包的沙盒中“默认组”的描述已更改，并且目标环境中的描述值不同，则在使用此项安装后，值将保持不变 <code>translationmap</code>.</li></ul></td> 
  </tr> 
  <tr> 
   <td>覆盖</td> 
   <td><p>此操作不会自动设置。</p><p>此操作提供更新目标环境中存在的对象的功能。 它提供在执行之前手动覆盖分配的CREATE或USEEXISTING操作的能力 <code>/install</code> 呼叫。<ul><li>用户可以更新测试环境中的对象，然后使用OVERWRITING操作更新目标环境中的该对象。</p></li><li><p>如果用户最初安装了一个升级包，以后又有一个新的（或更新的）升级包包含对初始包中对象的更改，则用户可以使用“覆盖”来替换（覆盖）以前安装的对象。 </p></li><ul></td> 
  </tr> 
  <tr> 
   <td>忽略</td> 
   <td><p>此操作不会自动设置。</p><p>它提供在执行之前手动覆盖分配的CREATE或USEEXISTING操作的能力 <code>/install</code> 呼叫。</p><p><b>注释： </b><ul><li><p>如果最初设置为CREATE的记录设置为IGNORE，则任何子记录也应设置为IGNORE。</p><p>例如，如果模板记录已使用CREATE操作进行映射，并且安装用户希望将其从部署中排除，则他们可以将模板的操作设置为IGNORE。</p><p>在这种情况下，如果安装用户未将模板任务、模板任务分配、模板任务前置任务、队列定义、队列主题、路由规则等也设置为IGNORE，则部署将导致安装尝试失败。</p></li><li><p>如果最初设置为USEEXISTING的记录设置为IGNORE，则安装过程中可能会产生一些不良影响。</p><p>例如，如果使用USEEXISTING操作映射了组记录，并且安装用户将操作更改为IGNORE，则对于需要组的对象（例如，如果没有分配组，项目不能存在），系统默认组将被分配给该项目。</p></li><li><p>如果最初设置为USEEXISTING的记录设置为CREATE，则安装过程中可能会产生一些不良影响，因为许多Workfront实体具有唯一名称约束。</p><p>例如，如果用USEEXISTING操作映射了“Default Group”记录，并且安装用户将操作更改为CREATE，因为已经有一个“Default Group”，安装尝试将无法完成所有步骤。 组名称必须是唯一的。</p><p>某些实体没有唯一名称约束。 对于这些对象，进行此更改将导致两个具有相同名称的记录。 例如，模板、项目、视图、筛选器、分组、报告和仪表板不需要唯一名称限制。 最佳做法是为这些记录指定唯一的名称，但不会强制执行。</p></li></ul></p></td> 
  </tr> 
  </tbody> 
</table>

当前不支持更新 `action` 在此服务的alpha功能中。 允许进行更新的选项 `action` 是我们正在研究的东西。

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/:id/prepare-installation
```

#### 标头

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

或

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### 正文

```json
{}
```

#### 响应

```
200
```

```json
{
    "environmentPromotionPackageId": "45f2ae94-76c0-4b13-8f3b-f688de83043d",
    "environmentPromotionPackageVersion": 1,
    "id": "c0bc79bd-c9c1-4b5b-b118-b1241392de0e",
    "userId": "5ba38da500b752fd66439d4f6a9999a1",
    "customerId": "5ba38d9d00b74f0c7a38b1b487fc9710",
    "status": "PREPARING",
    "environment": "mmi.my.workfront.com",
    "registeredAt": "2023-10-19T20:00:16.697Z",
    "updatedAt": "2023-10-19T20:00:16.701Z",
    "translationMap": {
        "CTGY": {
            "62d9c9a0000013aeeefe7242a0a5fdb2": {
                "name": "Example Document Form",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c9a0000013aeeefe7242a0a5fdb2"
            }
        },
        "PGRP": {
            "62d1eee4001c6618e6b9f9a588ba1598": {
                "name": "Asset Detail",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee4001c6618e6b9f9a588ba1598"
            }
        },
        "GROUP": {
            "5ba38da500b752b0f46d13186030b7ad": {
                "name": "Default Group",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "5ba38da500b752b0f46d13186030b7ad"
            }
        },
        "PARAM": {
            "62d1eee400f8578895166ee91a83f97a": {
                "name": "Asset Type",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee400f8578895166ee91a83f97a"
            },
            "62d1eee50001407c713514a8970b58e4": {
                "name": "Keywords",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee50001407c713514a8970b58e4"
            },
            "62d1eee5000333ac3981ea4f3df6d88e": {
                "name": "Permitted Uses",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee5000333ac3981ea4f3df6d88e"
            },
            "62d1eee5000b188e9ec8039a097fc7ab": {
                "name": "File Format",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee5000b188e9ec8039a097fc7ab"
            },
            "62d1eee500100c159fd5f838ce560507": {
                "name": "CTA",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee500100c159fd5f838ce560507"
            },
            "62d9c988001c1f23954dbb9d646335b5": {
                "name": "Other CTA",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c988001c1f23954dbb9d646335b5"
            },
            "62d9c9880070f546cf4c798ea6c3eaa4": {
                "name": "Other Audience",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c9880070f546cf4c798ea6c3eaa4"
            },
            "62d9c990006258baf1b40f2569c3eab7": {
                "name": "Target Audience",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c990006258baf1b40f2569c3eab7"
            }
        }
    }
}
```

>[!NOTE]
>
>执行安装所需的ID是 `id` 字段。 在此示例中， `id` 字段的顶部第三，其值以 `c0bc79bd`.

### 执行安装

>[!IMPORTANT]
>
>在执行安装之前，必须先执行预运行。 在执行安装时，将使用从预运行生成的ID。
>
>如果在执行预运行后对目标环境（包将部署到的环境）进行了任何更改，我们建议再次执行预运行。 如果不再次执行预运行，则可能无法准确完成执行，或者安装可能会失败。
>
>有关执行预运行的说明，请参阅 [执行预运行](#execute-a-pre-run).

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /install</code></td> 
  </tr> 
  </tbody> 
</table>

此调用将尝试将升级包安装到POSTURL中标识的目标环境中。

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations/{id}/install
```

#### 标头

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

或

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### 正文

```json
{
}
```

#### 响应

```
202
```


```json
{}
```

### 获取特定软件包的安装列表

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /v1/installations?environmentPromotionPackageId={environmentPromotionPackageId}
</code></td> 
  </tr> 
  </tbody> 
</table>

结果包括已部署该包的所有环境中的安装事件。 它们不限于发出请求的环境的安装。 这允许您识别哪些环境已收到此包。

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations?environmentPromotionPackageId={environmentPromotionPackageId}
```

#### 标头

```json
{
    "apikey": "**********"
}
```

或

```json
{
    "sessionID": "*****************"
}
```

#### 正文

_空_

#### 响应

```
200
```

```json
[
    {
        "id": "2892b936-e09e-455a-935f-e1462ab9753c",
        "environmentPromotionPackageId": "4fae2b9d-d315-45f4-909f-a0c0d79fc65d",
        "environmentPromotionPackageVersion": 1,
        "userId": "8fbbc5bcf4f94a5b862483ee05573e73",
        "customerId": "54286d78b064451096752b99bf968481",
        "status": "INSTALLED",
        "environment": "https://{domain}.{environment}.workfront.com",
        "registeredAt": "2021-03-16T02:21:31.908Z",
        "updatedAt": null,
        "translationMap": {
            "ROLE": {
                "5f6d114f006883209828ddd9088e63b3": {
                    "name": "DAM Curator",
                    "action": "USEEXISTING",
                    "isValid": true,
                    "targetId": "600f4bed00028a718599f29575840053"
                },
                "ad535a9ebe647361e053a7656a0a1575": {
                    "name": "Copywriter",
                    "action": "USEEXISTING",
                    "isValid": true,
                    "targetId": "600f162700001ca051081c06667b14a4"
                },
                ...
            },
            "TMPL": {
                "5f9b317c00b3db5af69abcd1ed5f82aa": {
                    "name": "Digital Asset Production (Integrated)",
                    "action": "CREATE",
                    "isValid": true,
                    "targetId": "6054cda40000d5af63dc811d9c2b3a07"
                },
                ...
            },
            ...
        }
    },
    {...}
]
```

### 获取安装的安装详细信息

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /installations/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

此调用将返回最终 `translationMap` 安装服务为特定安装生成的。

每个记录将说明规定的内容 `action` 以及操作是否成功。

对于具有CREATE的记录 `action` 该 `targetId` 字段将在目标系统中使用新创建记录的值设置。 此外， `installationStatus` 字段将设置为INSTALLED。

对于具有USEEXISTING的记录 `action` 该 `targetId` 字段，并且 `installationStatus` 字段将设置为REGISTERED。 这表示映射过程已完成，并且安装服务确认已评估记录，并且没有要执行的任何操作。

如果记录具有CREATE `action` 但未能成功创建记录，然后 `installationStatus` 将设置为“失败”，并且还会提供失败的原因。

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations/{id}
```

#### 标头

```json
{
    "apikey": "**********"
}
```

或

```json
{
    "sessionID": "*****************"
}
```

#### 正文

_空_

#### 响应

```
200
```

```json
{
    "id": "2892b936-e09e-455a-935f-e1462ab9753c",
    "environmentPromotionPackageId": "4fae2b9d-d315-45f4-909f-a0c0d79fc65d",
    "environmentPromotionPackageVersion": 1,
    "userId": "8fbbc5bcf4f94a5b862483ee05573e73",
    "customerId": "54286d78b064451096752b99bf968481",
    "status": "INSTALLED",
    "environment": "https://{domain}.{environment}.workfront.com",
    "registeredAt": "2021-03-16T02:21:31.908Z",
    "updatedAt": null,
    "translationMap": {
        "ROLE": {
            "5f6d114f006883209828ddd9088e63b3": {
                "name": "DAM Curator",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "600f4bed00028a718599f29575840053"
            },
            ...
        },
        "TMPL": {
            "5f9b317c00b3db5af69abcd1ed5f82aa": {
                "name": "Digital Asset Production (Integrated)",
                "action": "CREATE",
                "isValid": true,
                "targetId": "6054cda40000d5af63dc811d9c2b3a07"
            },
            ...
        },
        ...
    }
}
```



<!--table templates

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /packages</code></td> 
  </tr> 
  </tbody> 
</table>

<table style="table-layout:fixed"> 
 <col> 
 <tbody> 
  <tr> 
   <td><b></b></td> 
  </tr> 
  <tr> 
   <td><pre></pre></td> 
  </tr> 
  </tbody> 
</table>
-->
