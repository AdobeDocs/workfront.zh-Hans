---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: 访问，模型，漏斗，图表，级别，权限
navigation-topic: access-levels
title: 可用于各种访问级别的每种对象类型的功能
description: 下表列出了各种访问级别中每种对象类型的可用功能。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 91b1b448-5a0b-4e64-a59e-458c8387ecbc
source-git-commit: 8dbb48e6aa2df874caa816468cf2e3ad408ebf7e
workflow-type: tm+mt
source-wordcount: '1447'
ht-degree: 11%

---

# 可用于各种访问级别的每种对象类型的功能

{{highlighted-preview}}

下表列出了各种访问级别中每种对象类型的可用功能。

它还指示Workfront管理员可以使用访问级别禁用或启用哪些操作。

## 项目

只有拥有计划许可证的用户才能被授予对项目的完全访问权限。

| 操作 | 计划人 | 员工 | 查看者 | 请求人 | 外部用户 |
|---|---|---|---|---|---|
| 创建 | ✓&#42; |   |   |   |   |
| 复制 | ✓&#42; |   |   |   |   |
| 删除 | ✓&#42; |   |   |   |   |
| 共享 | ✓&#42; | ✓&#42; |   |   |   |
| 共享系统范围 | ✓&#42; |   |   |   |   |
| 查看 | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| 添加自定义表单 | ✓ |   |   |   |   |
| 更新自定义字段 | ✓ | ✓ |   |   |   |
| 添加审批流程 | ✓ |   |   |   |   |
| 批准项目 | ✓ | ✓ | ✓ |   |   |
| 添加文档 | ✓ | ✓ | ✓ |   |   |
| 添加问题 | ✓ | ✓ |   |   |   |
| 添加任务 | ✓ | ✓ |   |   |   |
| 提供更新/评论 | ✓ | ✓ | ✓ |   |   |
| 更改状态 | ✓ |   |   |   |   |
| 记录小时数 | ✓ | ✓ |   |   |   |
| 编辑分配 | ✓ | ✓ |   |   |   |
| 管理基线 | ✓ |   |   |   |   |
| 管理风险 | ✓ |   |   |   |   |
| 管理财务 | ✓ |   |   |   |   |
| 添加/编辑费用 | ✓ | ✓ |   |   |   |
| 附加模板 | ✓ |   |   |   |   |
| 另存为模板 | ✓ |   |   |   |   |
| 添加/编辑业务案例 | ✓ |   |   |   |   |
| 编辑项目详细信息 | ✓ |   |   |   |   |
| 编辑员工 | ✓ |   |   |   |   |
| 导出至 MS 项目 | ✓ | ✓ | ✓ |   |   |
| 重新计算财务/时间表 | ✓ |   |   |   |   |
| 设置队列属性 | ✓ |   |   |   |   |



&#42; 使用访问级别，Workfront管理员可以禁用或启用此功能。 有关更多信息，请参阅 [可配置对每种对象类型功能的访问](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## 任务

| 操作 | 计划人 | 员工 | 查看者 | 请求人 | 外部用户 |
|---|---|---|---|---|---|
| 创建 | ✓&#42; | ✓&#42; |   |   |   |
| 删除 | ✓&#42; | ✓&#42; |   |   |   |
| 共享 | ✓&#42; | ✓&#42; |   |   |   |
| 共享系统范围 | ✓&#42; |   |   |   |   |
| 查看 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| 添加前置任务 | ✓ | ✓ |   |   |   |
| 添加问题 | ✓ | ✓ |   |   |   |
| 编辑任务（不包括状态） | ✓ | ✓ |   |   |   |
| 更改任务状态 | ✓ | ✓ |   |   |   |
| 添加文档 | ✓ | ✓ | ✓ |   |   |
| 复制任务 | ✓ | ✓ |   |   |   |
| 移动任务 | ✓ | ✓ |   |   |   |
| 记录小时数 | ✓ | ✓ |   |   |   |
| 接受分配 | ✓ | ✓ |   |   |   |
| 进行分配 | ✓ | ✓ | 仅内联编辑 | 仅内联编辑 |   |
| 附加自定义表单 | ✓ | ✓ |   |   |   |
| 编辑自定义字段 | ✓ | ✓ |   |   |   |
| 创建批准流程 | ✓ | ✓ |   |   |   |
| 批准任务 | ✓ | ✓ | ✓ |   |   |
| 编辑财务 | ✓ |   |   |   |   |
| 添加/编辑费用 | ✓ | ✓ |   |   |   |
| 查看财务 | ✓ | ✓ | ✓ |   |   |
| 更新/评论 | ✓ | ✓ | ✓ |   |   |

{style="table-layout:auto"}

&#42; 使用访问级别，Workfront管理员可以禁用或启用此功能。 有关更多信息，请参阅 [可配置对每种对象类型功能的访问](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## 问题

| 操作 | 计划人 | 员工 | 查看者 | 请求人 | 外部用户 |
|---|---|---|---|---|---|
| 创建 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| 编辑 | ✓ | ✓ | ✓ | ✓ |   |
| 删除 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| 共享 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| 共享系统范围 | ✓&#42; |   |   |   |   |
| 查看 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| 附加自定义表单 | ✓ | ✓ | ✓ | ✓ |   |
| 编辑自定义字段 | ✓ | ✓ | ✓ | ✓ |   |
| 批准问题 | ✓ | ✓ | ✓ | ✓ |   |
| 添加审批流程 | ✓ | ✓ | ✓ | ✓ |   |
| 添加文档 | ✓ | ✓ | ✓ | ✓ |   |
| 复制问题 | ✓ | ✓ | ✓ | ✓ |   |
| 移动问题 | ✓ | ✓ | ✓ | ✓ |   |
| 记录小时数 | ✓ | ✓ |   |   |   |
| 将问题转化为项目 | ✓ | ✓ |   |   |   |
| 将问题转换为任务 | ✓ |   |   |   |   |
| 接受分配 | ✓ | ✓ |   |   |   |
| 进行分配 | ✓ | ✓ |   |   |   |
| 添加更新和注释 | ✓ | ✓ | ✓ | ✓ |   |



&#42; 使用访问级别，Workfront管理员可以禁用或启用此功能。 有关更多信息，请参阅 [可配置对每种对象类型功能的访问](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## 项目组合

只有拥有计划许可证的用户才能拥有项目组合的完全访问权限。

| 操作 | 计划人 | 员工 | 查看者 | 请求人 | 外部用户 |
|---|---|---|---|---|---|
| 创建 | ✓&#42; |   |   |   |   |
| 删除 | ✓&#42; |   |   |   |   |
| 共享 | ✓&#42; |   |   |   |   |
| 共享系统范围 | ✓&#42; |   |   |   |   |
| 查看 | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| 编辑详细信息 | ✓ |   |   |   |   |
| 附加自定义表单 | ✓ |   |   |   |   |
| 编辑自定义字段 | ✓ |   |   |   |   |
| 添加和删除项目 | ✓ |   |   |   |   |
| 批准项目 | ✓ |   |   |   |   |
| Portfolio优化 | ✓ |   |   |   |   |
| 添加文档 | ✓ | ✓ | ✓ |   |   |
| 添加更新和注释 | ✓ | ✓ | ✓ |   |   |



&#42; 使用访问级别，Workfront管理员可以禁用或启用此功能。 有关更多信息，请参阅 [可配置对每种对象类型功能的访问](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## 项目群

只有拥有计划许可证的用户才能完全访问程序。

| 操作 | 计划人 | 员工 | 查看者 | 请求人 | 外部用户 |
|---|---|---|---|---|---|
| 创建 | ✓&#42; |   |   |   |   |
| 删除 | ✓&#42; |   |   |   |   |
| 共享 | ✓&#42; |   |   |   |   |
| 共享系统范围 | ✓&#42; |   |   |   |   |
| 查看 | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| 编辑详细信息 | ✓ |   |   |   |   |
| 附加自定义表单 | ✓ |   |   |   |   |
| 编辑自定义字段 | ✓ |   |   |   |   |
| 添加和删除项目 | ✓ |   |   |   |   |
| 批准项目 | ✓ |   |   |   |   |
| 项目组合的最优化 | ✓ |   |   |   |   |
| 添加文档 | ✓ | ✓ | ✓ |   |   |
| 添加添加更新和注释 | ✓ | ✓ | ✓ |   |   |



&#42; 使用访问级别，Workfront管理员可以禁用或启用此功能。 有关更多信息，请参阅 [可配置对每种对象类型功能的访问](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## 报告、功能板和日历

拥有计划许可证的用户可以完全访问报告。 所有其他访问级别都具有查看报表的权限。

| 操作 | 计划人 | 员工 | 查看者 | 请求 | 外部用户 |
|---|---|---|---|---|---|
| 创建 | ✓&#42; |   |   |   |   |
| 删除 | ✓&#42; |   |   |   |   |
| 查看内置报告 | ✓&#42; |   |   |   |   |
| 共享 | ✓&#42; | ✓ | ✓ |   |   |
| 公开共享日历和报告 | ✓&#42; |   |   |   |   |
| 共享系统范围 | ✓&#42; |   |   |   |   |
| 查看 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |
| 编辑 | ✓ |   |   |   |   |
| 复制 | ✓ |   |   |   |   |

{style="table-layout:auto"}

&#42; 使用访问级别，Workfront管理员可以禁用或启用此功能。 有关更多信息，请参阅 [可配置对每种对象类型功能的访问](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

>[!NOTE]
>
>请求者只能查看与其共享的报告

## 筛选器、视图和分组

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
   <td>共享系统范围</td> 
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

&#42; 使用访问级别，Workfront管理员可以禁用或启用此功能。 有关更多信息，请参阅 [可配置对每种对象类型功能的访问](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## 文档

| 操作 | 计划人 | 员工 | 查看者 | 请求人 | 外部用户 |
|---|---|---|---|---|---|
| 创建 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| 删除（文档和文件夹） | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| 共享 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| 公开（外部）共享 | ✓&#42; |   |   |   |   |
| 共享系统范围 | ✓&#42; | ✓&#42; |   |   |   |
| 查看 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |
| 编辑详细信息 | ✓ | ✓ | ✓ | ✓ |   |
| 下载 | ✓ | ✓ | ✓ | ✓ | ✓ |
| 结账 | ✓ | ✓ | ✓ | ✓ |   |
| 添加批准者 | ✓ | ✓ | ✓ | ✓ |   |
| 批准文档 | ✓ | ✓ | ✓ | ✓ | ✓ |
| 附加自定义表单 | ✓ | ✓ | ✓ | ✓ |   |
| 编辑自定义字段 | ✓ | ✓ | ✓ | ✓ |   |
| 移动到（对象） | ✓ | ✓ | ✓ | ✓ |   |
| 发送至（集成） | ✓ | ✓ | ✓ | ✓ |   |
| 添加更新和注释 | ✓ | ✓ | ✓ | ✓ |   |
| 上传新版本 | ✓ | ✓ | ✓ | ✓ |   |
| 删除版本 | ✓ | ✓ | ✓ | ✓ |   |
| 预览 | ✓ | ✓ | ✓ | ✓ | ✓ |
| Proof | ✓ | ✓ | ✓ | ✓ |   |
| 生成校对 | ✓ | ✓ |   |   |   |
| 移除校对 | ✓ | ✓ | ✓ | ✓ |   |
| 添加/删除&#42;&#42; | ✓ | ✓ | ✓ | ✓ |   |
| 重命名&#42;&#42; | ✓ | ✓ | ✓ | ✓ |   |
| 链接（与集成） | ✓ | ✓ | ✓ | ✓ |   |
| 取消链接（与集成） | ✓ | ✓ | ✓ | ✓ |   |

{style="table-layout:auto"}

&#42; 使用访问级别，Workfront管理员可以禁用或启用此功能。 有关更多信息，请参阅 [可配置对每种对象类型功能的访问](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;仅适用于文档文件夹，不适用于文档

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
   <td>编辑、删除、停用、以身份登录或重置任何用户的密码</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>编辑、删除、取消激活、以用户身份登录或重置他们管理的组中的任何用户的密码</td> 
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

&#42; 使用访问级别，Workfront管理员可以禁用或启用此功能。 有关更多信息，请参阅 [可配置对每种对象类型功能的访问](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

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
   <td>编辑他们所在的团队</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>编辑团队所管理的组中的团队</td> 
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

&#42; 使用访问级别，Workfront管理员可以禁用或启用此功能。 有关更多信息，请参阅 [可配置对每种对象类型功能的访问](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## 模板

| 操作 | 计划人 | 员工 | 查看者 | 请求人 | 外部用户 |
|---|---|---|---|---|---|
| 创建 | ✓&#42; |   |   |   |   |
| 删除 | ✓&#42; |   |   |   |   |
| 共享 | ✓&#42; |   |   |   |   |
| 共享系统范围 | ✓&#42; |   |   |   |   |
| 查看 | ✓&#42; |   |   |   |   |
| 复制 | ✓ |   |   |   |   |
| 编辑模板详细信息 | ✓ |   |   |   |   |

{style="table-layout:auto"}

&#42; 使用访问级别，Workfront管理员可以禁用或启用此功能。 有关更多信息，请参阅 [可配置对每种对象类型功能的访问](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## 财务数据

只有拥有计划许可证的用户才能完全访问财务数据。

此处不包括“请求”和“外部用户”许可证类型，因为它们无权访问这些对象和区域。

| 操作 | 计划人 | 员工 | 查看者 |
|---|---|---|---|
| 编辑角色记帐和成本费率 | ✓&#42; |   |   |
| 编辑用户计费和成本率 | ✓&#42; |   |   |
| 查看角色记帐和成本费率 | ✓&#42; |   |   |
| 查看用户计费和成本费率 | ✓&#42; |   |   |
| 管理开票记录 | ✓ |   |   |
| 管理费用 | ✓ | ✓ |   |
| 查看财务数据 | ✓&#42; | ✓&#42; | ✓&#42; |
| <span class="preview">管理费率卡</span> | ✓ |   |   |
| 在资源计划工具中按成本查看信息 | ✓ |   |   |
| 资源规划工具中的预算资源&#42;&#42; | ✓ |   |   |
| 在资源计划工具中查看资源分配&#42; | ✓ | ✓ | ✓ |
| 在项目中创建风险 | ✓ |   |   |
| 查看项目风险 | ✓ | ✓ | ✓ |

{style="table-layout:auto"}

&#42; 使用访问级别，Workfront管理员可以禁用或启用此功能。 有关更多信息，请参阅 [可配置对每种对象类型功能的访问](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;需要额外访问资源管理。

## 资源管理

只有拥有计划许可证的用户才能完全访问 [选择对象或区域]. 其他许可证类型对Workfront中的资源管理的访问权限有限或没有访问权限。

| 操作 | 计划人 | 员工 | 查看者 | 请求人 | 外部用户 |
|---|---|---|---|---|---|
| 在“规划者”中编辑优先级和预算小时数 | ✓&#42; |   |   |   |   |
| 创建、编辑、删除资源池&#42;&#42; | ✓&#42; |   |   |   |   |
| `Update Planned Hours in the Workload Balancer`&#42;&#42;&#42; | `✓*` |   |   |   |   |
| 在资源规划程序中查看项目优先级 | ✓&#42; |   |   |   |   |
| 在资源计划工具中查看资源分配 | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| 查看资源池 | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| 资源规划工具中的预算资源&#42;&#42; | ✓ |   |   |   |   |
| 将资源池附加到项目、模板和用户 | ✓ |   |   |   |   |

{style="table-layout:auto"}

&#42; 使用访问级别，Workfront管理员可以禁用或启用此功能。 有关更多信息，请参阅 [可配置对每种对象类型功能的访问](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;需要拥有对财务数据的附加访问权限，以及项目财务的权限。 如果您向无权访问财务数据的规划者用户授予资源管理访问权限，则该用户仍然可以在资源规划者中查看小时分配，但无法切换到“成本”视图或查看业务案例。 有关更多信息，请参阅 [授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) 和 [共享对象的财务权限](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).

&#42;&#42;&#42;需要Contribute到对象的权限，并在“高级设置”下启用Make Assignments。 有关信息，请参阅部分 [了解继承的权限和对象的层次结构](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#sharing-an-object) 在文章中 [对象权限共享概述](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## 场景规划器区域

| 操作 | 计划人 | 员工 | 查看者 | 请求人 | 外部用户 |
|---|---|---|---|---|---|
| 创建/编辑现有计划和计划 | ✓ | ✓ | ✓ |   |   |
| 添加或编辑有关计划和计划的工作角色信息&#42; | ✓ | ✓ | ✓ |   |   |
| 添加或编辑有关计划和计划的成本信息&#42; | ✓ | ✓ | ✓ |   |   |
| 删除计划和计划 | ✓ | ✓ | ✓ |   |   |
| 在主菜单中查看方案 ![](assets/esp-icon-in-main-menu.png) | ✓ | ✓ | ✓ | |   |
| 查看用户创建的计划和计划&#42; | ✓ | ✓ | ✓ |   |   |

{style="table-layout:auto"}

>[!NOTE]
>
>用户只有在与其共享指向计划的链接时，才能查看其他用户创建的计划。

&#42; 为了使用户在计划或计划中查看财务数据，他们需要访问财务数据。 有关更多信息，请参阅 [授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## Workfront目标区域

| 操作 | 查看 | 编辑 |
|---|---|---|
| 创建 |   | ✓ |
| 编辑/删除所有目标 |   | ✓ |
| 在主菜单中查看目标 | ✓ | ✓ |
| 从共享链接查看“目标”区域 | ✓ | ✓ |
| 查看系统中的所有目标 | ✓ | ✓ |
| 激活/停用/关闭所有目标 |   | ✓ |
| 创建/编辑/删除活动 |   | ✓ |
| 创建/编辑/删除结果 |   | ✓ |
| 添加对齐的目标 |   | ✓ |
| 更新结果或活动的进度 |   | ✓ |
| 拥有目标、结果或活动 | ✓ | ✓ |
| 对目标的评论 | ✓ | ✓ |
| 复制目标 |   | ✓ |
| 在左侧面板中查看“目标列表”部分 | ✓ | ✓ |
| 在左侧面板中查看“图形”部分 | ✓ | ✓ |
| 在左侧面板中查看“目标对齐方式”部分 | ✓ | ✓ |

