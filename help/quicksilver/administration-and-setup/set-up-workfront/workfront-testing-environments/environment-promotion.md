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
source-git-commit: 68c3a66a91f4c0936d256398b5d30518226396a6
workflow-type: tm+mt
source-wordcount: '2346'
ht-degree: 3%

---

# 将对象从其中移出 [!DNL Workfront] 环境到另一个环境

<!-- 
TO DO

Overview of value
Check for any code changes
Fix {}
Add to tocs
-->

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

* [工作对象](#work-objects)
* [报表对象](#reporting-objects)
* [自定义数据对象](#custom-data-objects)
* [组织对象](#organization-objects)
* [其他配置对象](#other-configuration-objects)


### 工作对象

| 可提升的对象 | 包含的可升级子对象 |
| --- | --- |
| 项目（项目） | 项目<br>任务<br>指定任务<br>前置任务<br>公司<br>覆盖率<br>组<br>角色<br>团队<br>批准流程<br>批准路径<br>审批步骤<br>步骤审批者<br>计划<br>非工作日<br>队列定义<br>队列主题组<br>队列主题<br>路由规则<br>里程碑路径<br>里程碑<br>小时类型<br>资源池<br>类别<br>类别参数<br>参数<br>参数组<br>参数选项<br>类别显示逻辑 |
| 模板（模板） | 模板<br>模板任务<br>模板任务分派<br>模板任务前置任务<br>公司<br>覆盖率<br>组<br>角色<br>团队<br>批准流程<br>批准路径<br>审批步骤<br>步骤审批者<br>计划<br>非工作日<br>队列定义<br>队列主题组<br>队列主题<br>路由规则<br>里程碑路径<br>里程碑<br>小时类型<br>资源池<br>类别<br>类别参数<br>参数<br>参数组<br>参数选项<br>类别显示逻辑 |

### 报表对象

| 可提升的对象 | 包含的可升级子对象 |
| --- | --- |
| 布局模板(UITMPL) | 布局模板<br>仪表板<br>日历<br>日历部分<br>外部页面<br>报表<br>筛选<br>分组<br>视图<br>参数 |
| 仪表板(PTLTAB) | 仪表板<br>日历<br>日历部分<br>外部页面<br>报表<br>筛选<br>分组<br>视图<br>参数 |
| 日历(CALEND) | 日历<br>日历部分 |
| 外部页面(EXTSEC) | 外部页面 |
| 报告(PTLSEC) | 报表<br>筛选<br>分组<br>视图<br>参数 |
| 过滤器(UIFT) | 筛选<br>参数 |
| 分组(UIGB) | 分组<br>参数 |
| 视图(UIVW) | 视图<br>参数 |

### 自定义数据对象

| 可提升的对象 | 包含的可升级子对象 |
| --- | --- |
| 类别(CTGY) | 类别<br>类别参数<br>参数<br>参数组<br>参数选项<br>类别显示逻辑<br>组 |
| 参数（参数） | 参数<br>参数选项 |
| 参数组(PGRP) | 参数组 |

### 组织对象

| 可提升的对象 | 包含的可升级子对象 |
| --- | --- |
| 组（组） | 组 <br>子组（最多5个级别）<br>类别<br>类别参数<br>参数<br>参数组<br>参数选项<br>类别显示逻辑 |
| 角色(ROLE) | 角色 |
| 团队（团队） | 团队<br>组 |
| 公司(CPY) | 公司<br>覆盖率<br>类别<br>类别参数<br>参数<br>参数组<br>参数 <br>类别显示逻辑<br>组 |
| Portfolio（端口） | Portfolio<br>项目<br>组<br>类别<br>类别参数<br>参数<br>参数组<br>参数选项<br>类别显示逻辑 |
| 计划(PRGM) | 项目<br>Portfolio<br>组<br>类别<br>类别参数<br>参数<br>参数组<br>参数选项<br>类别显示逻辑 |

### 其他配置对象

| 可提升的对象 | 包含的可升级子对象 |
| --- | --- |
| 批准流程(ARVPRC) | 批准流程<br>批准路径<br>审批步骤<br>步骤审批者<br>角色<br>团队<br>组 |
| 时间表(SCHED) | 计划<br>非工作日<br>组 |
| 里程碑路径(MPATH) | 里程碑路径<br>里程碑 |
| 周期性时间表(TSPRO) | 周期性工时表<br>小时类型 |
| 小时类型（小时） | 小时数类型 |
| 费用类型(EXPTYP) | 费用类型 |
| 风险类型(RSKTYP) | 风险类型 |
| 资源池(RSPL) | 资源池 |

## 身份验证

API对每个请求进行身份验证，以确保客户端有权查看或修改请求的对象。

身份验证是通过传入会话ID或API密钥执行的，可使用以下方法提供该密钥：

### 请求标头身份验证

首选的身份验证方法是传递包含会话令牌的名为SessionID的请求标头。 这有一个优势，就是可以安全抵御 [跨站点请求伪造(CSRF)](http://en.wikipedia.org/wiki/Cross-site_request_forgery) 攻击，并且不会出于缓存目的干扰URI。

以下是请求标头的示例：

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

## API端点

* [创建资源包](#create-a-package)
* [获取程序包列表](#get-a-list-of-packages)
* [按ID获取包](#get-a-package-by-id)
* [获取包的配置定义](#get-a-packages-configuration-definition)
* [替换包详细信息和定义](#replace-package-details-and-definition)
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

#### 标题

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

#### 个回应

```json
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "status": "ASSEMBLING",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d"
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

#### 标题

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

#### 个回应

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
            "version": 1,
            "installationCounts": {},
            "createdAt": "2023-06-06T17:29:21.600Z",
            "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
            "publishedAt": null,
            "customerId": "61aa9d090005fa42152c1cb66659f38d"
        },
        {...}
    ]
}
```

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

#### 标题

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

#### 个回应

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "status": "DRAFT",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "displayEntities": {
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

### 获取包的配置定义

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages/{id}/definition</code></td> 
  </tr> 
  </tbody> 
</table>

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}/definition
```

#### 标题

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

#### 个回应

```
200
```

```json
{
    "packageEntities": {
        "GROUP": [
           {
               "id": "52aa9d0e0005fcee8f212835bdaa2691",
               "name": "Default Group",
               "businessLeaderID": "...",
               "categoryID": "...",
               "defaultInterface": 1,
               "description": "...",
               "extRefID": null,
               "isActive": true,
               "isGroupPublic": true,
               "isPublic": true,
               "parentID": null,
               "rootID": null,
               "rootName": null,
               "uiTemplateID": null
           }
        ],
        "ROLE": [
           {...}
        ],
        ...
    }
}
```

### 替换包详细信息和定义

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>PUT /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

此调用将替换促销活动包的所有内容。

该请求要求提供所有可编辑的字段。

可编辑的属性包括：

1. 名称（字符串）
1. description（字符串）
1. 源（包含URL验证的字符串）
1. 状态（带值验证的字符串）
1. 版本（整数）
1. packageEntities（集合）

状态选项包括：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>组装</td> 
   <td><p>在组装对象时，将自动指定此状态。</p><p>客户无法直接设置此状态。</p></td> 
  </tr> 
  <tr> 
   <td>草稿</td> 
   <td><p>在装配过程结束时或创建空升级包时，会分配此状态。</p><p>客户可以将促销包移回此状态。</p><p>处于此状态时，无法在任何环境中安装升级包。</p></td> 
  </tr> 
  <tr> 
   <td>测试</td> 
   <td><p>此状态允许在任何“预览”或“自定义刷新”沙盒中安装升级包。 处于此状态时，无法在生产环境中安装软件包。</p></td> 
  </tr> 
  <tr> 
   <td>活动</td> 
   <td><p>此状态允许在任何环境（包括生产环境）中安装升级包。</p><p>当程序包状态设置为“活动”时， <code>publishedAt</code> 日期会自动设置为请求的当前时间戳。</p></td> 
  </tr> 
  <tr> 
   <td>已禁用</td> 
   <td><p>此状态将用于隐藏以前使用的升级包，这些升级包将来不会安装到任何环境中。</p><p>当软件包处于此状态时，无法将其安装到任何环境中。</p><p>当程序包状态设置为DISABLED时， <code>retiredAt</code> 日期会自动设置为请求的当前时间戳。</p><p>建议使用此状态而不是使用<code>DELETE /package</code> 终结点，因为它可检索，并且使用此包进行的任何部署都将保留安装历史记录。</p></td> 
  </tr> 
  <tr> 
   <td>ASSEMBLY_FAILED</td> 
   <td><p>如果ASSEMBLY阶段失败，则升级包会自动处于此状态。</p><p>要将包返回到ASSEMBLY阶段，必须再次触发提取过程。</p></td> 
  </tr> 
  </tbody> 
</table>

#### URL

```
PUT https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### 标题

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

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
    "description": "This promotion package contains configuration to support the agency onboarding processes... with a description change",
    "source": "https://{domain}.{environment}.workfront.com",
    "status": "TESTING",
    "version": 1,
    "metadata": {
        "displayOrder": ["GROUP","ROLE","TMPL","PROJ","PTLTAB"],
        "historyOrder": ["GROUP","ROLE","TMPL","TTSK","PROJ","PTLTAB"], 
        "installOrder": ["GROUP","ROLE","TMPL","TTSK","TPRED","TASSGN","PROJ","QUED","RRUL","QUET","UIFT","UIGB","UIVW","PTLTAB"], 
        "summaryOrder": ["GROUP","ROLE","TMPL"], 
        "shapeVersion": 2
    },
    "packageEntities": {
        "GROUP": [
           {
               "id": "52aa9d0e0005fcee8f212835bdaa2691",
               "name": "Default Group",
               "businessLeaderID": "...",
               "categoryID": "...",
               "defaultInterface": 1,
               "description": "...",
               "extRefID": null,
               "isActive": true,
               "isGroupPublic": true,
               "isPublic": true,
               "parentID": null,
               "rootID": null,
               "rootName": null,
               "uiTemplateID": null
           }
        ],
        "ROLE": [
           {...}
        ],
        ...
    }
}
```

#### 个回应

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "status": "TESTING",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "displayEntities": {
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
1. 源（包含URL验证的字符串）
1. 状态（带值验证的字符串）
1. 版本（整数）
1. packageEntities（集合）

   或

   objectCollections（数组）

提供 `packageEntities` 将使用提供的配置定义更新促销活动包。

提供 `objectCollections` 将从以下位置开始重新提取 `source` 与升级包关联的环境。 此 `source` 在以下情况下必须提供字段 `objectCollections` 提供了。

#### URL

```
PATCH https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```


#### 标题

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

#### 个回应

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "status": "ACTIVE",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": "2023-06-06T19:39:01.600Z",
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "displayEntities": {
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

#### 标题

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

#### 个回应

```
200
```

```
Deleted
```

### 执行预运行

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
   <td><p>在目标环境中找到相应的记录时，该操作将设置为USEEXISTING ，并且 <code>targetId</code> 在中捕获 <code>translationmap</code>.</p><p>当此操作在 <code>translationmap</code> 提供给 <code>/install</code> 终结点，安装服务将不会创建记录。 但是，它会使用 <code>targetId</code> 包括在可能引用此记录的其他对象的映射条目中。</p><p>例如，在包将部署到的目标环境中可以找到“默认组”。 由于不可能有两个“默认组”记录，因此安装服务将在任何其他包含对“默认组”的引用的对象创建操作中使用现有组的GUID，如项目、表单或与此组相关的任何其他实体。</p><p><b>注释:</b> <ul><li><p>分配USEEXISTING操作后，将不会修改目标环境中的现有记录。 </p><p>例如，如果在从中构建包的沙盒中“默认组”的描述已更改，并且目标环境中的描述值不同，则在使用此项安装后，值将保持不变 <code>translationmap</code>.</li></ul></td> 
  </tr> 
  <tr> 
   <td>忽略</td> 
   <td><p>此操作不会自动设置。</p><p>它提供在执行之前手动覆盖分配的CREATE或USEEXISTING操作的能力 <code>/install</code> 呼叫。</p><p><b>注释: </b><ul><li><p>如果最初设置为CREATE的记录设置为IGNORE，则任何子记录也应设置为IGNORE。</p><p>例如，如果模板记录已使用CREATE操作进行映射，并且安装用户希望将其从部署中排除，则他们可以将模板的操作设置为IGNORE。</p><p>在这种情况下，如果安装用户未将模板任务、模板任务分配、模板任务前置任务、队列定义、队列主题、路由规则等也设置为IGNORE，则部署将导致安装尝试失败。</p></li><li><p>如果最初设置为USEEXISTING的记录设置为IGNORE，则安装过程中可能会产生一些不良影响。</p><p>例如，如果使用USEEXISTING操作映射了组记录，并且安装用户将操作更改为IGNORE，则对于需要组的对象（例如，如果没有分配组，项目不能存在），系统默认组将被分配给该项目。</p></li><li><p>如果最初设置为USEEXISTING的记录设置为CREATE，则安装过程中可能会产生一些不良影响，因为许多Workfront实体具有唯一名称约束。</p><p>例如，如果用USEEXISTING操作映射了“Default Group”记录，并且安装用户将操作更改为CREATE，因为已经有一个“Default Group”，安装尝试将无法完成所有步骤。 组名称必须是唯一的。</p><p>某些实体没有唯一名称约束。 对于这些对象，进行此更改将导致两个具有相同名称的记录。 例如，模板、项目、视图、筛选器、分组、报告和仪表板不需要唯一名称限制。 最佳做法是为这些记录指定唯一的名称，但不会强制执行。</p></li></ul></p></td> 
  </tr> 
  </tbody> 
</table>

当前不支持更新 `action` 在此服务的alpha功能中。 允许进行更新的选项 `action` 是我们正在研究的东西。

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/:id/prepare-installation
```

#### 标题

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

#### 个回应

```
200
```

```json
{}
```

### 执行安装

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /install</code></td> 
  </tr> 
  </tbody> 
</table>

此调用将尝试将升级包安装到POSTURL中标识的目标环境中。

#### 选项

如果 `translationmap` POST正文中未提供，进程将自动启动 `/prepare-installation` 呼叫。 此 `translationmap` 返回的内容将按原样使用，没有机会进行审查或调整。

如果 `translationmap` POST正文中提供了，安装过程将使用提供的映射。 这样，安装用户就可以在执行安装尝试之前查看并进行必要的调整。

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations/{id}/install
```

#### 标题

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

#### 个回应

```
200
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

#### 标题

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

#### 个回应

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
        "status": "COMPLETED",
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

#### 标题

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

#### 个回应

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
    "status": "COMPLETED",
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