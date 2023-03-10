---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: 访问，模型，漏斗，图，级别，权限
navigation-topic: access-levels
title: 可用于每种对象类型的功能
description: 下表列出了各种访问级别中每种对象类型可用的功能。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 91b1b448-5a0b-4e64-a59e-458c8387ecbc
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '1457'
ht-degree: 12%

---

# 可用于每种对象类型的功能

下表列出了各种访问级别中每种对象类型可用的功能。

它还指示Workfront管理员可以使用访问级别禁用或启用哪些操作。

## 项目

只有具有计划许可证的用户才能获得项目的完全访问权限。

| 操作 | 计划人 | 员工 | 查看者 | 请求人 | 外部用户 |
|---|---|---|---|---|---|
| 创建 | ✓&#42; |   |   |   |   |
| 复制 | ✓&#42; |   |   |   |   |
| 删除 | ✓&#42; |   |   |   |   |
| 共享 | ✓&#42; | ✓&#42; |   |   |   |
| 在系统范围内共享 | ✓&#42; |   |   |   |   |
| 查看 | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| 添加自定义表单 | ✓ |   |   |   |   |
| 更新自定义字段 | ✓ | ✓ |   |   |   |
| 添加批准流程 | ✓ |   |   |   |   |
| 批准项目 | ✓ | ✓ | ✓ |   |   |
| 添加文档 | ✓ | ✓ | ✓ |   |   |
| 添加问题 | ✓ | ✓ |   |   |   |
| 添加任务 | ✓ | ✓ |   |   |   |
| 提供更新/评论 | ✓ | ✓ | ✓ |   |   |
| 更改状态 | ✓ |   |   |   |   |
| 日志小时数 | ✓ | ✓ |   |   |   |
| 编辑分配 | ✓ | ✓ |   |   |   |
| 管理基线 | ✓ |   |   |   |   |
| 管理风险 | ✓ |   |   |   |   |
| 管理财务 | ✓ |   |   |   |   |
| 添加/编辑费用 | ✓ | ✓ |   |   |   |
| 附加模板 | ✓ |   |   |   |   |
| 另存为模板 | ✓ |   |   |   |   |
| 添加/编辑业务案例 | ✓ |   |   |   |   |
| 编辑项目详细信息 | ✓ |   |   |   |   |
| 编辑人员配置 | ✓ |   |   |   |   |
| 导出至 MS 项目 | ✓ | ✓ | ✓ |   |   |
| 重新计算财务/时间表 | ✓ |   |   |   |   |
| 设置队列属性 | ✓ |   |   |   |   |



&#42; 使用访问级别，Workfront管理员可以禁用或启用此功能。 有关更多信息，请参阅 [可配置地访问每种对象类型的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## 任务

| 操作 | 计划人 | 员工 | 查看者 | 请求人 | 外部用户 |
|---|---|---|---|---|---|
| 创建 | ✓&#42; | ✓&#42; |   |   |   |
| 删除 | ✓&#42; | ✓&#42; |   |   |   |
| 共享 | ✓&#42; | ✓&#42; |   |   |   |
| 在系统范围内共享 | ✓&#42; |   |   |   |   |
| 查看 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| 添加前置任务 | ✓ | ✓ |   |   |   |
| 添加问题 | ✓ | ✓ |   |   |   |
| 编辑任务（不包括状态） | ✓ | ✓ |   |   |   |
| 更改任务状态 | ✓ | ✓ |   |   |   |
| 添加文档 | ✓ | ✓ | ✓ |   |   |
| 复制任务 | ✓ | ✓ |   |   |   |
| 移动任务 | ✓ | ✓ |   |   |   |
| 日志小时数 | ✓ | ✓ |   |   |   |
| 接受分配 | ✓ | ✓ |   |   |   |
| 进行分配 | ✓ | ✓ | 仅在行内编辑 | 仅在行内编辑 |   |
| 附加自定义表单 | ✓ | ✓ |   |   |   |
| 编辑自定义字段 | ✓ | ✓ |   |   |   |
| 创建审批流程 | ✓ | ✓ |   |   |   |
| 批准任务 | ✓ | ✓ | ✓ |   |   |
| 编辑财务 | ✓ |   |   |   |   |
| 添加/编辑费用 | ✓ | ✓ |   |   |   |
| 查看财务 | ✓ | ✓ | ✓ |   |   |
| 更新/评论 | ✓ | ✓ | ✓ |   |   |

{style=&quot;table-layout:auto&quot;}

&#42; 使用访问级别，Workfront管理员可以禁用或启用此功能。 有关更多信息，请参阅 [可配置地访问每种对象类型的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## 问题

| 操作 | 计划人 | 员工 | 查看者 | 请求人 | 外部用户 |
|---|---|---|---|---|---|
| 创建 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| 编辑 | ✓ | ✓ | ✓ | ✓ |   |
| 删除 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| 共享 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| 在系统范围内共享 | ✓&#42; |   |   |   |   |
| 查看 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| 附加自定义表单 | ✓ | ✓ | ✓ | ✓ |   |
| 编辑自定义字段 | ✓ | ✓ | ✓ | ✓ |   |
| 批准问题 | ✓ | ✓ | ✓ | ✓ |   |
| 添加批准流程 | ✓ | ✓ | ✓ | ✓ |   |
| 添加文档 | ✓ | ✓ | ✓ | ✓ |   |
| 复制问题 | ✓ | ✓ | ✓ | ✓ |   |
| 移动问题 | ✓ | ✓ | ✓ | ✓ |   |
| 日志小时数 | ✓ | ✓ |   |   |   |
| 将问题转换为项目 | ✓ | ✓ |   |   |   |
| 将问题转换为任务 | ✓ |   |   |   |   |
| 接受分配 | ✓ | ✓ |   |   |   |
| 分配 | ✓ | ✓ |   |   |   |
| 添加更新和注释 | ✓ | ✓ | ✓ | ✓ |   |



&#42; 使用访问级别，Workfront管理员可以禁用或启用此功能。 有关更多信息，请参阅 [可配置地访问每种对象类型的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## 项目组合

只有具有计划许可证的用户才能完全访问项目组合。

| 操作 | 计划人 | 员工 | 查看者 | 请求人 | 外部用户 |
|---|---|---|---|---|---|
| 创建 | ✓&#42; |   |   |   |   |
| 删除 | ✓&#42; |   |   |   |   |
| 共享 | ✓&#42; |   |   |   |   |
| 在系统范围内共享 | ✓&#42; |   |   |   |   |
| 查看 | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| 编辑详细信息 | ✓ |   |   |   |   |
| 附加自定义表单 | ✓ |   |   |   |   |
| 编辑自定义字段 | ✓ |   |   |   |   |
| 添加和删除项目 | ✓ |   |   |   |   |
| 批准项目 | ✓ |   |   |   |   |
| Portfolio优化 | ✓ |   |   |   |   |
| 添加文档 | ✓ | ✓ | ✓ |   |   |
| 添加更新和注释 | ✓ | ✓ | ✓ |   |   |



&#42; 使用访问级别，Workfront管理员可以禁用或启用此功能。 有关更多信息，请参阅 [可配置地访问每种对象类型的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## 项目群

只有具有计划许可证的用户才能完全访问程序。

| 操作 | 计划人 | 员工 | 查看者 | 请求人 | 外部用户 |
|---|---|---|---|---|---|
| 创建 | ✓&#42; |   |   |   |   |
| 删除 | ✓&#42; |   |   |   |   |
| 共享 | ✓&#42; |   |   |   |   |
| 在系统范围内共享 | ✓&#42; |   |   |   |   |
| 查看 | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| 编辑详细信息 | ✓ |   |   |   |   |
| 附加自定义表单 | ✓ |   |   |   |   |
| 编辑自定义字段 | ✓ |   |   |   |   |
| 添加和删除项目 | ✓ |   |   |   |   |
| 批准项目 | ✓ |   |   |   |   |
| 项目组合的最优化 | ✓ |   |   |   |   |
| 添加文档 | ✓ | ✓ | ✓ |   |   |
| 添加更新和注释 | ✓ | ✓ | ✓ |   |   |



&#42; 使用访问级别，Workfront管理员可以禁用或启用此功能。 有关更多信息，请参阅 [可配置地访问每种对象类型的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## 报表、功能板和日历

拥有计划许可证的用户可以拥有对报告的完全访问权限。 所有其他访问级别都具有查看报表的权限。

| 操作 | 计划人 | 员工 | 查看者 | 请求 | 外部用户 |
|---|---|---|---|---|---|
| 创建 | ✓&#42; |   |   |   |   |
| 删除 | ✓&#42; |   |   |   |   |
| 查看内置报告 | ✓&#42; |   |   |   |   |
| 共享 | ✓&#42; | ✓ | ✓ |   |   |
| 公开共享日历和报表 | ✓&#42; |   |   |   |   |
| 在系统范围内共享 | ✓&#42; |   |   |   |   |
| 查看 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |
| 编辑 | ✓ |   |   |   |   |
| 复制 | ✓ |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

&#42; 使用访问级别，Workfront管理员可以禁用或启用此功能。 有关更多信息，请参阅 [可配置地访问每种对象类型的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

>[!NOTE]
>
>请求者只能查看与他们共享的报表

## 过滤器、视图和分组

<table> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p>操作</p> </th> 
   <th> <p>计划人</p> </th> 
   <th> <p>员工</p> </th> 
   <th> <p>查看者</p> </th> 
   <th> <p>请求人</p> </th> 
   <th>外部用户<br></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>创建</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>删除</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>共享</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>在系统范围内共享</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>查看</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>编辑</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; 使用访问级别，Workfront管理员可以禁用或启用此功能。 有关更多信息，请参阅 [可配置地访问每种对象类型的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## 文档

| 操作 | 计划人 | 员工 | 查看者 | 请求人 | 外部用户 |
|---|---|---|---|---|---|
| 创建 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| 删除（文档和文件夹） | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| 共享 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| 公开（外部）共享 | ✓&#42; |   |   |   |   |
| 在系统范围内共享 | ✓&#42; | ✓&#42; |   |   |   |
| 查看 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |
| 编辑详细信息 | ✓ | ✓ | ✓ | ✓ |   |
| 下载 | ✓ | ✓ | ✓ | ✓ | ✓ |
| 结帐 | ✓ | ✓ | ✓ | ✓ |   |
| 添加批准者 | ✓ | ✓ | ✓ | ✓ |   |
| 批准文档 | ✓ | ✓ | ✓ | ✓ | ✓ |
| 附加自定义表单 | ✓ | ✓ | ✓ | ✓ |   |
| 编辑自定义字段 | ✓ | ✓ | ✓ | ✓ |   |
| 移动到（对象） | ✓ | ✓ | ✓ | ✓ |   |
| 发送到（集成） | ✓ | ✓ | ✓ | ✓ |   |
| 添加更新和注释 | ✓ | ✓ | ✓ | ✓ |   |
| 上传新版本 | ✓ | ✓ | ✓ | ✓ |   |
| 删除版本 | ✓ | ✓ | ✓ | ✓ |   |
| 预览 | ✓ | ✓ | ✓ | ✓ | ✓ |
| Proof | ✓ | ✓ | ✓ | ✓ |   |
| 生成校样 | ✓ | ✓ |   |   |   |
| 删除校样 | ✓ | ✓ | ✓ | ✓ |   |
| 添加/删除&#42;&#42; | ✓ | ✓ | ✓ | ✓ |   |
| 重命名&#42;&#42; | ✓ | ✓ | ✓ | ✓ |   |
| 链接（与集成） | ✓ | ✓ | ✓ | ✓ |   |
| 取消链接（与集成） | ✓ | ✓ | ✓ | ✓ |   |

{style=&quot;table-layout:auto&quot;}

&#42; 使用访问级别，Workfront管理员可以禁用或启用此功能。 有关更多信息，请参阅 [可配置地访问每种对象类型的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;仅适用于文档文件夹，而不适用于文档

## 用户

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p>操作</p> </th> 
   <th> <p>计划人</p> </th> 
   <th>员工</th> 
   <th> <p>查看者</p> </th> 
   <th> <p>请求人</p> </th> 
   <th> <p>外部用户**</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>创建</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>删除</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>编辑、删除、停用、登录身份或为任何用户重置密码</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>编辑、删除、取消激活、登录为或重置其管理的组中任何用户的密码</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>查看用户</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>查看联系信息</td> 
   <td>✓</td> 
   <td> ✓</td> 
   <td>✓ </td> 
   <td> ✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; 使用访问级别，Workfront管理员可以禁用或启用此功能。 有关更多信息，请参阅 [可配置地访问每种对象类型的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;外部用户只能搜索其他用户

## 团队

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>操作</p> </th> 
   <th> <p>计划人</p> </th> 
   <th>员工</th> 
   <th> <p>查看者</p> </th> 
   <th> <p>请求人</p> </th> 
   <th> <p>外部用户*</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>创建</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>删除</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>编辑其所在的团队</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>在他们管理的组中编辑团队</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>查看所有团队</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>查看与其组关联的团队</td> 
   <td>✓</td> 
   <td> ✓</td> 
   <td>✓ </td> 
   <td> ✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; 使用访问级别，Workfront管理员可以禁用或启用此功能。 有关更多信息，请参阅 [可配置地访问每种对象类型的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## 模板

| 操作 | 计划人 | 员工 | 查看者 | 请求人 | 外部用户 |
|---|---|---|---|---|---|
| 创建 | ✓&#42; |   |   |   |   |
| 删除 | ✓&#42; |   |   |   |   |
| 共享 | ✓&#42; |   |   |   |   |
| 在系统范围内共享 | ✓&#42; |   |   |   |   |
| 查看 | ✓&#42; |   |   |   |   |
| 复制 | ✓ |   |   |   |   |
| 编辑模板详细信息 | ✓ |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

&#42; 使用访问级别，Workfront管理员可以禁用或启用此功能。 有关更多信息，请参阅 [可配置地访问每种对象类型的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## 财务数据

只有具有计划许可证的用户才能完全访问财务数据。

此处不包括请求和外部用户许可证类型，因为它们无权访问 [选择对象或区域].

| 操作 | 计划人 | 员工 | 查看者 |
|---|---|---|---|
| 编辑角色开单和成本费率 | ✓&#42; |   |   |
| 编辑用户帐单和费用费率 | ✓&#42; |   |   |
| 查看角色开单和成本费率 | ✓&#42; |   |   |
| 查看用户账单和费用费率 | ✓&#42; |   |   |
| 管理帐单记录 | ✓ |   |   |
| 管理费用 | ✓ | ✓ |   |
| 查看财务数据 | ✓&#42; | ✓&#42; | ✓&#42; |
| 在资源计划工具中按成本查看信息 | ✓ |   |   |
| 资源规划工具中的预算资源&#42;&#42; | ✓ |   |   |
| 在资源计划工具中查看资源分配&#42; | ✓ | ✓ | ✓ |
| 在项目上制造风险 | ✓ |   |   |
| 查看项目风险 | ✓ | ✓ | ✓ |

{style=&quot;table-layout:auto&quot;}

&#42; 使用访问级别，Workfront管理员可以禁用或启用此功能。 有关更多信息，请参阅 [可配置地访问每种对象类型的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;需要对资源管理具有其他访问权限。

## 资源管理

只有具有计划许可证的用户才能拥有 [选择对象或区域]. 其他许可证类型可能对Workfront中的资源管理具有有限或无权访问。

| 操作 | 计划人 | 员工 | 查看者 | 请求人 | 外部用户 |
|---|---|---|---|---|---|
| 在“规划者”中编辑优先级和预算小时数 | ✓&#42; |   |   |   |   |
| 创建、编辑、删除资源池&#42;&#42; | ✓&#42; |   |   |   |   |
| `Update Planned Hours in the Workload Balancer`&#42;&#42;&#42; | `✓*` |   |   |   |   |
| 在资源计划器中查看项目优先级 | ✓&#42; |   |   |   |   |
| 在资源计划工具中查看资源分配 | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| 查看资源池 | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| 资源规划工具中的预算资源&#42;&#42; | ✓ |   |   |   |   |
| 将资源池附加到项目、模板和用户 | ✓ |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

&#42; 使用访问级别，Workfront管理员可以禁用或启用此功能。 有关更多信息，请参阅 [可配置地访问每种对象类型的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;需要额外访问财务数据并拥有项目财务权限。 如果您向无权访问财务数据的计划员用户授予资源管理访问权限，则用户仍可以在资源计划器中查看每小时分配，但无法切换到“成本”视图或查看业务案例。 有关更多信息，请参阅 [授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) 和 [共享对象的财务权限](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).

&#42;&#42;&#42;需要具有对对象进行贡献的权限，并在“高级设置”下启用“进行分配”。 有关信息，请参阅 [了解继承的权限和对象的层次结构](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#sharing-an-object) 在文章中 [对象共享权限概述](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## 方案计划员区域

| 操作 | 计划人 | 员工 | 查看者 | 请求人 | 外部用户 |
|---|---|---|---|---|---|
| 创建/编辑现有计划和方案 | ✓ | ✓ | ✓ |   |   |
| 添加或编辑有关计划和计划的工作角色信息&#42; | ✓ | ✓ | ✓ |   |   |
| 添加或编辑有关计划和计划的成本信息&#42; | ✓ | ✓ | ✓ |   |   |
| 删除计划和计划 | ✓ | ✓ | ✓ |   |   |
| 在主菜单中查看方案 ![](assets/esp-icon-in-main-menu.png) | ✓ | ✓ | ✓ |  |   |
| 查看用户创建的计划和方案&#42; | ✓ | ✓ | ✓ |   |   |

{style=&quot;table-layout:auto&quot;}

>[!NOTE]
>
>用户只能查看其他用户创建的计划，前提是与他们共享指向该计划的链接。

&#42; 为了让用户在计划或方案中查看财务数据，他们需要访问财务数据。 有关更多信息，请参阅 [授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## Workfront目标区域

| 操作 | 查看 | 编辑 |
|---|---|---|
| 创建 |   | ✓ |
| 编辑/删除所有目标 |   | ✓ |
| 在主菜单中查看目标 | ✓ | ✓ |
| 通过共享链接查看“目标”区域 | ✓ | ✓ |
| 查看系统中的所有目标 | ✓ | ✓ |
| 激活/取消激活/关闭所有目标 |   | ✓ |
| 创建/编辑/删除活动 |   | ✓ |
| 创建/编辑/删除结果 |   | ✓ |
| 添加一致的目标 |   | ✓ |
| 更新结果或活动的进度 |   | ✓ |
| 拥有目标、结果或活动 | ✓ | ✓ |
| 对目标的评论 | ✓ | ✓ |
| 复制目标 |   | ✓ |
| 在左侧面板中查看目标列表部分 | ✓ | ✓ |
| 在左侧面板中查看图形部分 | ✓ | ✓ |
| 在左侧面板中查看“目标对齐”部分 | ✓ | ✓ |

