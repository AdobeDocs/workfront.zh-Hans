---
title: 审核日志
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 作为Adobe Workfront管理员，您可以使用审核日志跟踪过去90天内系统中触发的用户更改。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6adb4146-42fd-4eda-b46f-c61d7ff71df6
source-git-commit: 822c4e13ab62d129d0a7c603105251e52578576d
workflow-type: tm+mt
source-wordcount: '1465'
ht-degree: 3%

---

# 审核日志

<!--Audited: 01/2024-->

作为Adobe Workfront管理员，您可以使用下述审核日志跟踪过去90天内系统中触发的用户更改。

有关查看和筛选您想要在这些审核日志中查看内容的说明，请参阅[查看和导出审核日志](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md)。

## 可在审核日志中找到的信息

每个审核日志条目中记录了以下字段：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">日期和时间</td> 
   <td>操作发生的时间。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">日志类型</td> 
   <td>审核日志的类型，如访问级别或自定义表单。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">用户名</td> 
   <td> <p>执行操作的用户的名称。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">操作</td> 
   <td> 用户执行的操作，如更改、创建和删除。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象</td> 
   <td> 因操作而受影响的对象的名称。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">详细信息</td> 
   <td>有关操作的其他详细信息。 将鼠标悬停在文本上可阅读完整消息。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">IP 地址</td> 
   <td> <p>执行操作时执行操作的用户的IP地址。</p> <p>IP地址对于某些系统操作不可用。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 审核日志类型和触发这些类型的操作

* [访问级别](#access-level)
* [公司](#company)
* [条件](#condition)
* [自定义字段](#custom-field)
* [自定义表单](#custom-forms)
* [自定义分区](#custom-section)
* [汇率](#exchange-rate)
* [组](#group)
* [职位角色](#job-roles)
* [登录尝试](#login-attempt)
* [优先级](#priority)
* [项目偏好设置](#project-preference)
* [严重性](#severity)
* [状态](#status)
* [任务和问题首选项](#tasks-issues-preferences)
* [用户](#user)

### 访问级别 {#access-level}

当用户执行以下操作之一时，系统会生成访问级别日志条目：

* 创建访问级别
* 删除访问级别
* 更改访问级别：

   * 修改许可证类型
   * 更改对项目、任务、问题、Portfolio、程序、报告、文档、用户或模板的权限

     >[!NOTE]
     >
     >系统不会记录对“财务数据”或以下访问类型中的任何权限更改：“查看”和“编辑”。
     >
     >例如，如果用户将Planner访问类型从查看更改为编辑，系统不会显示微调设置下拉菜单中包含的信息。

### 公司 {#company}

当用户执行以下操作之一时，系统会生成一个“公司”审核日志条目：

* 创建公司
* 更改公司：

   * 重命名
   * 添加或删除成员
   * 添加、编辑或删除其组字段中的值
   * 添加或编辑工作角色的公司记帐费率
   * 删除工作角色的公司记帐费率
   * 将其设置为组织的主要公司
   * 附加或移除自定义表单

* 删除公司

有关状态的详细信息，请参阅[状态概述](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md)。

### 完成情况 {#condition}

当用户执行以下操作之一时，系统会生成“条件”审核日志条目：

* 创建条件
* 更改条件：

   * 更改名称
   * 更改颜色
   * 将其设置为默认值
   * 更改或删除条件的描述
   * 隐藏或显示条件

* 删除条件

有关配置工作角色的更多信息，请参阅[创建或编辑自定义条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)。

### 自定义字段 {#custom-field}

当用户执行以下操作之一时，系统会生成“自定义字段”审核日志条目：

* 创建自定义字段
* 更改自定义字段：

   * 更改名称、标签、说明或格式
   * 更改显示类型

     仅当字段是以下类型之一时，此选项才可用：单行、段落、下拉列表、复选框、单选按钮

   * 更改字段大小

     仅当字段是以下类型之一时才可用：单行、段落、带格式的文本

   * 添加、删除或隐藏字段选项
   * 编辑字段选择标签或值
   * 将字段选择配置为默认选中或不选中
   * 将下拉字段配置为允许多选或单选
   * 配置日期字段以显示或不显示时间
   * 编辑超链接或更改描述性文本字段中的值

* 删除自定义字段
* 共享自定义字段

### 自定义表单 {#custom-forms}

当用户执行以下操作之一时，系统会生成自定义Forms审核日志条目：

* 创建自定义表单
* 更改自定义表单：

   * 更改名称或描述
   * 启用或禁用“活动”
   * 添加或删除字段或部分
   * 对于自定义部分，将更改其他设置下的设置
   * 将字段更改为必填或非必填字段
   * 更改自定义字段中的计算
   * 在说明悬停文本中隐藏或显示与计算字段关联的公式
   * 启用或禁用更新以前的计算
   * 添加或更改跳过逻辑或显示逻辑

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>Adds or changes a filter for a typeahead field</p></li>   
     -->

* 删除自定义表单
* 共享自定义表单

### 自定义分区 {#custom-section}

当用户在自定义表单中执行以下操作之一时，系统会生成“自定义分区”审核日志条目：

* 创建自定义分区
* 更改自定义分区的名称或描述
* 删除自定义分区

有关自定义表单中的自定义节的信息，请参阅[使用表单设计器设计表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

### 汇率 {#exchange-rate}

当用户执行以下操作之一时，系统会生成一个汇率审核日志条目：

* 创建汇率
* 更改汇率：

   * 添加货币
   * 更改币种的汇率
   * 将货币设置为系统中所有项目和报表的基本（默认）货币

* 删除汇率

有关配置汇率的详细信息，请参阅[设置汇率](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)。

### 组 {#group}

当用户执行以下操作之一时，系统会生成一个组审核日志条目：

* 创建组
* 删除组
* 更改组：

   * 添加或删除用户
   * 添加或删除子组

### 职位角色 {#job-roles}

当用户执行以下操作之一时，系统会生成“工作角色”审核日志条目：

* 创建工作角色
* 更改工作角色：

   * 更改名称
   * 添加、更改或删除说明
   * 添加、更改或删除每小时成本（成本/小时）
   * 添加、更改或删除记帐费率（计费/小时）

* 删除工作角色

有关配置工作角色的更多信息，请参阅[创建和管理工作角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)。

### 登录尝试 {#login-attempt}

当用户执行以下操作之一时，系统会生成“登录尝试”审核日志条目：

* 登录、注销或失败Workfront（在浏览器和移动设备应用程序中）的登录尝试
* 在任何Workfront集成(例如，适用于Slack的Workfront和适用于Salesforce的Workfront)中登录、注销或登录尝试失败
* 登录或注销Workfront API

Workfront管理员使用“登录身份”功能时，不会记录登录尝试日志。

>[!NOTE]
>
>如果您的组织已载入Adobe Admin Console，则此项不可用。 如果需要更多信息，请咨询您的网络或IT管理员。

### 优先级 {#priority}

当用户执行以下操作之一时，系统会生成“优先级”审核日志条目：

* 创建优先级
* 更改优先级：

   * 更改名称
   * 更改颜色
   * 将其设置为默认值
   * 添加、更改或删除优先级的说明
   * 隐藏或显示优先级

* 删除优先级

有关配置优先级的详细信息，请参阅[创建和自定义优先级](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md)。

### 项目偏好设置 {#project-preference}

当用户执行以下操作之一时，系统会生成“项目首选项”审核日志条目：

* 创建自定义季度
* 更改项目偏好设置：

   * 锁定或解除锁定
   * 更改其中一个设置
   * 启用、禁用或编辑它
   * 编辑时间线计算

* 删除自定义季度

有关项目首选项的详细信息，请参阅[配置系统范围项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

### 严重性 {#severity}

当用户执行以下操作之一时，系统会生成严重性审核日志条目：

* 创建问题严重性
* 更改问题严重性：

   * 更改名称
   * 更改颜色
   * 将其设置为默认值
   * 更改或移除严重程度的描述
   * 隐藏或显示严重程度

* 删除问题严重程度

有关配置工作角色的更多信息，请参阅[创建或自定义问题严重程度](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md)。

### 状态 {#status}

当用户执行以下操作之一时，系统会生成“状态”审核日志条目：

* 在系统或组级别创建状态
* 更改系统或组级别上的状态：

   * 重命名
   * 使其成为默认状态
   * 锁定或解除锁定
   * 隐藏或取消隐藏它
   * 更改颜色或描述

* 删除系统或组级别上的状态

有关状态的详细信息，请参阅[状态概述](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md)。

### 任务和问题首选项 {#tasks-issues-preferences}

当用户通过以下方式之一更改“任务和问题”首选项时，系统会生成“任务和问题首选项”审核日志条目：

* 锁定或解锁首选项
* 更改首选项的设置
* 更改任务、问题或请求的访问设置

有关任务和问题首选项的详细信息，请参阅[配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

### 用户 {#user}

当用户执行以下操作之一时，系统会生成“用户”审核日志条目：

* 创建用户

  <!--
  DRAFTED IN FLARE:
  Gevorg checking with Jonah on whether this note should be here:
  
  -->

  >[!NOTE]
  >
  >如果您的组织已载入Adobe Admin Console，则此项不可用。 如果需要更多信息，请咨询您的网络或IT管理员。

* 删除用户
* 更改用户的访问级别、公司、团队或组
* 激活用户
* 停用用户
