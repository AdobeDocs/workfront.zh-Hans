---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Adobe Workfront MCP服务器工具
description: 通过Adobe Workfront MCP服务器可用的工具参考列表，按Workfront区域分组。
author: Courtney
feature: Get Started with Workfront
source-git-commit: f4f73cf44107850573e1a6966568645b9537b757
workflow-type: tm+mt
source-wordcount: '1615'
ht-degree: 5%

---


# Adobe Workfront MCP服务器工具

本文列出了[!DNL Adobe Workfront] MCP服务器向连接的AI代理平台公开的工具。 当您要求平台查找、创建、更新或删除Workfront项目时，它代表您调用这些工具。

有关如何通过AI代理平台使用这些工具的信息，请参阅[使用Adobe Workfront MCP服务器](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md)。 有关如何设置连接的信息，请参阅[配置Adobe Workfront MCP服务器](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)。

>[!IMPORTANT]
>
>AI代理平台使用您的Workfront帐户、访问级别和对象权限在Workfront中执行操作。 只有当您在Workfront中拥有相应的访问权限时，该工具才有效。 Adobe不负责更改人工智能代理平台对Workfront数据所做的更改。


## 读取和写入操作

下表中的每个工具在“操作”列中均被分类为“读取”或“写入”操作：

* **读取**：从Workfront中检索信息而不更改您的数据。 例如，查找项目、列出文档或获取记录的详细信息。
* **写入**：创建、更新或删除Workfront数据。 例如，创建项目、更新记录或删除视图。

您的Workfront管理员可通过系统偏好设置中的两个切换控制AI代理平台可以使用哪些类别的工具：

* **只读MCP工具** （默认启用）
* **写入MCP工具** （默认禁用）

如果AI代理平台可以找到Workfront项目，但无法创建、更新或删除它们，请让您的Workfront管理员启用写入操作。 有关详细信息，请参阅&#x200B;*配置Adobe Workfront MCP服务器*&#x200B;中的[管理员先决条件](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#admin-prerequisites)。

## 审批工具

### 文档

| 标题 | 工具名称 | 作用 | 操作 |
|---|---|---|---|
| 按名称查找文档版本 | `approvals_find_document_version_by_name` | 按文件名查找文档的当前版本ID。 支持部分匹配。 | 读取 |
| 按版本ID获取文档 | `approvals_get_document_by_version_id` | 获取已知文档版本ID的文档详细信息（名称、大小、上传日期、上传程序）。 | 读取 |
| 按项目获取文档 | `approvals_get_documents_by_project` | 列出Workfront项目中的文档，以及每个文档的当前版本ID。 | 读取 |
| 解析文档范围 | `approvals_resolve_document_scope` | 将项目或文件夹展开到其中包含的文档版本ID列表中。 支持项目、文件夹和按名称文件夹范围。 | 读取 |
| 列出AEM链接的文件夹 | `approvals_list_aem_linked_folders` | 列出链接到Workfront的Adobe Experience Manager文档文件夹。 | 读取 |
| 将文档发送到AEM文件夹 | `approvals_send_documents_to_aem_folder` | 将一个或多个Workfront文档移动到与AEM链接的文件夹。 | 写入 |

### 审批工作流

| 标题 | 工具名称 | 作用 | 操作 |
|---|---|---|---|
| 获取审批工作流信息 | `approvals_get_approval_info` | 返回文档版本的当前审批工作流（阶段、参与者、状态）。 | 读取 |
| 创建或更新审批工作流 | `approvals_create_or_update_approval_workflow` | 创建或更新文档版本的审批工作流暂存。 支持线性和平行（图形）阶段依赖关系。 | 写入 |
| 从模板创建审批 | `approvals_create_approval_from_template` | 使用现有模板在文档上创建审批工作流。 | 写入 |
| 请求文档审批 | `approvals_request_document_approval` | 打开引导式表单，请求审批文档版本（标题、审批者/审阅者、可选的截止日期和消息）。 | 写入 |
| 删除审批阶段 | `approvals_delete_approval_stage` | 按名称或职位从审批工作流中删除单个阶段。 只能删除未启动的阶段。 | 写入 |

### 提醒

| 标题 | 工具名称 | 作用 | 操作 |
|---|---|---|---|
| 向参与者发送提醒 | `approvals_send_reminder_to_participants` | 向审批阶段的特定参与者发送提醒电子邮件。 仅适用于已启动、未完成、未锁定的阶段。 | 写入 |
| 向未确定的参与者发送提醒 | `approvals_send_reminder_to_undecided` | 向审批阶段所有未确定的参与者（已通知、已打开或已评论）发送提醒电子邮件。 | 写入 |

### 审批模板

| 标题 | 工具名称 | 作用 | 操作 |
|---|---|---|---|
| 列出审批模板 | `approvals_list_templates` | 列出此Workfront实例中可用的审批模板。 支持按创建者、参与者进行筛选，并按使用情况排序。 | 读取 |
| 按名称搜索模板 | `approvals_search_template_by_name` | 按名称查找审批模板（不区分大小写的部分匹配）。 | 读取 |
| 创建审批模板 | `approvals_create_template` | 创建具有线性或基于图形的阶段依赖关系的新审批模板。 | 写入 |
| 更新审批模板 | `approvals_update_template` | 使用结构化修改更新现有模板（添加或删除参与者、重命名阶段、设置截止日期等）。 | 写入 |

### 查找和用户

| 标题 | 工具名称 | 作用 | 操作 |
|---|---|---|---|
| 获取当前用户 | `approvals_get_current_user` | 返回呼叫用户的Workfront身份，包括名称、用户ID、主团队名称和主团队ID。 | 读取 |
| 按名称查找用户 | `approvals_find_user_by_name` | 按名称（模糊或部分匹配）查找Workfront用户的ID。 返回名称、ID、电子邮件、标题和头像URL。 | 读取 |
| 按名称查找团队 | `approvals_find_team_by_name` | 按名称（模糊或部分匹配）查找Workfront团队的ID。 | 读取 |
| 按名称查找项目 | `approvals_find_project_by_name` | 通过系统中的部分名称匹配查找Workfront项目。 | 读取 |
| 按所有者获取项目 | `approvals_get_projects_by_owner` | 列出呼叫用户是所有者的Workfront项目。 | 读取 |
| 获取Adobe区域 | `approvals_get_adobe_region` | 返回云提供商所在地区的Adobe名称。 | 读取 |

## 规划工具

### 工作区

| 标题 | 工具名称 | 作用 | 操作 |
|---|---|---|---|
| 获取工作区 | `planning_get_workspace` | 按ID或别名检索工作区的完整详细信息。 | 读取 |
| 获取工作区列表 | `planning_get_workspace_list` | 列出所有可用工作区以及基于游标的分页。 | 读取 |
| 创建工作区 | `planning_create_workspace` | 创建新的空工作区以组织记录类型、字段和数据。 | 写入 |
| 从模板创建工作区 | `planning_create_workspace_from_template` | 创建使用现有模板预填充的新工作区。 | 写入 |
| 更新工作区 | `planning_update_workspace` | 部分更新工作区 — 名称、描述、图标、部分或所有者。 | 写入 |
| 删除工作区 | `planning_delete_workspace` | 永久删除工作区及其所有数据。 | 写入 |
| 将工作区转换为模板 | `planning_convert_workspace_to_template` | 将现有工作区另存为可重用的模板（需要管理员）。 | 写入 |
| 获取工作区共享 | `planning_get_workspace_sharing` | 返回工作区的当前共享和权限配置。 | 读取 |
| 修改工作区共享 | `planning_modify_workspace_sharing` | 更新谁有权访问工作区以及什么权限级别。 | 写入 |

### 记录类型

| 标题 | 工具名称 | 作用 | 操作 |
|---|---|---|---|
| 获取记录类型 | `planning_get_record_type` | 获取记录类型的完整详细信息，包括其字段和视图。 | 读取 |
| 创建记录类型 | `planning_create_record_types` | 在工作区部分中创建一个或多个记录类型。 | 写入 |
| 更新记录类型 | `planning_update_record_type` | 部分更新记录类型的名称、描述、图标或颜色。 | 写入 |
| 删除记录类型 | `planning_delete_record_type` | 永久删除记录类型及其所有记录、字段和视图。 | 写入 |
| 列出全局记录类型 | `planning_list_global_record_types` | 列出当前用户可见的所有集中定义的（全局）记录类型。 | 读取 |
| 列出可添加全局记录类型 | `planning_list_addable_global_record_types` | 列出可添加到特定工作区的全局记录类型。 | 读取 |
| 向工作区添加全局记录类型 | `planning_add_global_record_type_to_workspace` | 将全局记录类型链接到指定的工作区。 | 写入 |
| 从工作区中删除全局记录类型 | `planning_remove_global_record_type_from_workspace` | 从工作区中取消全局记录类型的链接；删除该工作区中的所有记录。 | 写入 |
| 获取外部记录工作区 | `planning_get_external_record_workspaces` | 查找哪些工作区和记录类型连接到特定外部记录。 | 读取 |
| 获取记录类型共享 | `planning_get_record_type_sharing` | 返回特定记录类型的共享和权限。 | 读取 |
| 修改记录类型共享 | `planning_modify_record_type_sharing` | 更新谁可以访问记录类型以及什么权限级别。 | 写入 |

### 记录

| 标题 | 工具名称 | 作用 | 操作 |
|---|---|---|---|
| 获取记录 | `planning_get_record` | 按ID检索单个记录的完整详细信息。 | 读取 |
| 搜索记录 | `planning_search_records` | 搜索和筛选记录类型中的记录。 | 读取 |
| 批量记录操作 | `planning_bulk_record_actions` | 在单个请求中创建、更新、删除或恢复多个记录。 | 写入 |
| 创建连接记录 | `planning_create_connection_record` | 在连接的外部系统（例如，Workfront项目）中创建新记录。 | 写入 |
| 更新记录顺序 | `planning_update_records_order` | 更改记录类型中记录的显示顺序。 | 写入 |
| 获取记录更改日志 | `planning_get_record_change_log` | 返回记录的字段级编辑历史记录。 | 读取 |
| 获取记录共享 | `planning_get_record_sharing` | 返回特定记录的共享配置。 | 读取 |
| 修改记录共享 | `planning_modify_records_sharing` | 更新谁可以访问一条或多条记录以及什么权限级别。 | 写入 |

### 字段

| 标题 | 工具名称 | 作用 | 操作 |
|---|---|---|---|
| 获取字段 | `planning_get_field` | 按ID检索字段的完整详细信息和值架构。 | 读取 |
| 创建字段 | `planning_create_fields` | 向记录类型添加一个或多个字段（列）。 | 写入 |
| 更新字段 | `planning_update_field` | 部分更新字段的名称、描述、选项或配置。 | 写入 |
| 删除字段 | `planning_delete_field` | 从记录类型中永久删除字段及其所有数据。 | 写入 |

### 视图

| 标题 | 工具名称 | 作用 | 操作 |
|---|---|---|---|
| 获取视图 | `planning_get_view` | 按ID返回视图的完整详细信息。 | 读取 |
| 创建视图 | `planning_create_view` | 为记录类型创建新表、时间轴或日历视图。 | 写入 |
| 更新视图 | `planning_update_view` | 部分更新现有视图的配置、筛选器或排序。 | 写入 |
| 删除视图 | `planning_delete_view` | 永久删除视图（记录不受影响）。 | 写入 |
| 获取视图共享 | `planning_get_view_sharing` | 返回特定视图的共享配置。 | 读取 |
| 修改视图共享 | `planning_modify_view_sharing` | 更新谁可以访问视图以及什么权限级别。 | 写入 |

### 模板

| 标题 | 工具名称 | 作用 | 操作 |
|---|---|---|---|
| 获取模板列表 | `planning_get_template_list` | 列出所有可用的工作区模板以及摘要信息。 | 读取 |
| 获取模板 | `planning_get_template` | 按ID检索特定模板的完整详细信息。 | 读取 |

### 搜索和实用工具

| 标题 | 工具名称 | 作用 | 操作 |
|---|---|---|---|
| 搜索资源 | `planning_search_resources` | 按名称跨工作区、记录类型和视图进行搜索。 | 读取 |
| 搜索共享数据 | `planning_search_sharing_data` | 按名称查找用于共享和权限的用户、组、团队、角色和公司。 | 读取 |
| 搜索用户 | `planning_search_users` | 搜索支持分页的用户。 | 读取 |

## 工作流工具

工作流工具是AI代理平台用于处理任何Workfront对象（项目、任务、问题、小时、任务、程序、项目组合等）的通用操作。

| 标题 | 工具名称 | 作用 | 操作 |
|---|---|---|---|
| 搜索对象 | `workflow_search_any_object` | 使用灵活的过滤器参数、排序和分页搜索Workfront对象。 | 读取 |
| 创建对象 | `workflow_create_any_object` | 创建新的Workfront对象，如项目、任务、问题、小时、分配、项目群或项目组合。 | 写入 |
| 更新对象 | `workflow_update_any_object` | 更新现有Workfront对象中的字段。 | 写入 |
| 删除对象 | `workflow_delete_any_object` | 按ID删除Workfront对象。 需要明确的用户确认才能执行操作。 | 写入 |
| 解析字段名称 | `workflow_resolve_field_names_any_object` | 将用户提供的字段名称或标签转换为底层Workfront API字段名称，以便AI代理平台可以构建准确的请求。 | 读取 |

## 如何更新工具

当Adobe发布新版本的Workfront MCP服务器时，AI代理平台会自动使用更新的工具集。 您无需重新连接或更改任何内容。



## 即将推出的其他工具

我们正努力在未来将以下工具添加到Workfront MCP服务器：

* 评论
* 展示板