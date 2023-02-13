---
title: 审核日志
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 作为Adobe Workfront管理员，您可以使用审核日志跟踪过去90天内在系统中触发的用户更改。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6adb4146-42fd-4eda-b46f-c61d7ff71df6
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '1462'
ht-degree: 4%

---

# 审核日志

作为Adobe Workfront管理员，您可以使用下面描述的审核日志跟踪过去90天内在系统中触发的用户更改。

有关查看和筛选要在这些审核日志中查看的内容的说明，请参阅 [查看和导出审核日志](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## 您可以在审核日志中找到的信息

每个审核日志条目中记录以下字段：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">日期和时间</td> 
   <td>操作发生时。</td> 
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
   <td> 用户执行的操作，如“更改”、“创建”和“删除”。 </td> 
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
   <td role="rowheader">IP地址</td> 
   <td> <p>执行操作时执行操作的用户的IP地址。</p> <p>IP地址不适用于某些系统操作。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 审核日志类型以及触发这些日志类型的操作

* [访问级别](#access-level)
* [公司](#company)
* [完成情况](#condition)
* [自定义字段](#custom-field)
* [自定义表单](#custom-forms)
* [自定义分区](#custom-section)
* [汇率](#exchange-rate)
* [组](#group)
* [职位角色](#job-roles)
* [登录尝试](#login-attempt)
* [优先级](#priority)
* [项目首选项](#project-preferences)
* [严重程度](#severity)
* [状态](#status)
* [任务和问题首选项](#tasks-issues-preferences)
* [用户](#user)

### 访问级别 {#access-level}

当用户执行下列操作之一时，系统会生成访问级别日志条目：

* 创建访问级别
* 删除访问级别
* 更改访问级别：

   * 修改许可证类型
   * 对项目、任务、问题、Portfolio、程序、报表、文档、用户或模板的权限更改

      >[!NOTE]
      >
      >系统不会记录对Financial Data或以下访问类型的任何权限更改：查看和编辑。
      >
      >例如，如果用户将计划员访问类型从“查看”更改为“编辑”，则系统将不显示“微调设置”下拉菜单中包含的信息。

### 公司 {#company}

当用户执行以下操作之一时，系统会生成公司审核日志条目：

* 创建公司
* 更改公司：

   * 重命名
   * 添加或删除成员
   * 在其“组”字段中添加、编辑或删除值
   * 添加或编辑职务角色的公司开单费率
   * 删除职务角色的公司帐单费率
   * 将其设置为组织的主公司
   * 附加或删除自定义表单

* 删除公司

有关状态的更多信息，请参阅 [状态概述](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### 完成情况 {#condition}

当用户执行下列操作之一时，系统会生成“条件”审核日志条目：

* 创建条件
* 更改条件：

   * 更改名称
   * 更改颜色
   * 将其设置为默认值
   * 更改或删除条件描述
   * 隐藏或显示条件

* 删除条件

有关配置作业角色的更多信息，请参阅 [创建或编辑自定义条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

### 自定义字段 {#custom-field}

当用户执行下列操作之一时，系统会生成“自定义字段”审核日志条目：

* 创建自定义字段
* 更改自定义字段：

   * 更改名称、标签、说明或格式
   * 更改显示类型

      仅当字段为以下类型之一时，才可使用此选项：单行，段落，下拉框，复选框，单选按钮

   * 更改字段大小

      仅当字段为以下类型之一时，才可使用此选项：单行，段落，带格式的文本

   * 添加、删除或隐藏字段选择
   * 编辑字段选择标签或值
   * 配置要默认选择或未选择的字段选项
   * 配置下拉字段以允许多个选择或单个选择
   * 配置显示或不显示日期字段
   * 编辑超链接或更改描述性文本字段中的值

* 删除自定义字段
* 共享自定义字段

### 自定义表单 {#custom-forms}

当用户执行以下操作之一时，系统会生成自定义Forms审核日志条目：

* 创建自定义表单
* 更改自定义表单：

   * 更改名称或描述
   * 启用或禁用“为活动”
   * 添加或删除字段或部分
   * 对于自定义部分，请在“其他设置”下更改设置
   * 将字段更改为必填或非必填
   * 更改自定义字段中的计算
   * 在“说明”悬停文本中隐藏或显示与计算字段关联的公式
   * 启用或禁用更新以前的计算
   * 添加或更改跳过逻辑或显示逻辑

      <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>Adds or changes a filter for a typeahead field</p></li>   
     -->

* 删除自定义表单
* 共享自定义表单

### 自定义分区 {#custom-section}

当用户在自定义表单中执行下列操作之一时，系统会生成“自定义区域”审核日志条目：

* 创建自定义部分
* 更改自定义部分的名称或描述
* 删除自定义部分

有关自定义表单中自定义部分的信息，请参阅 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

### 汇率 {#exchange-rate}

当用户执行下列操作之一时，系统会生成一个汇率审核日志条目：

* 创建汇率
* 更改汇率：

   * 添加货币
   * 更改货币的汇率
   * 将货币设置为整个系统中所有项目和报表的基本（默认）货币

* 删除汇率

有关配置汇率的详细信息，请参阅 [设置汇率](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

### 组 {#group}

当用户执行下列操作之一时，系统会生成组审核日志条目：

* 创建群组
* 删除群组
* 更改群组：

   * 添加或删除用户
   * 添加或删除子组

### 职位角色 {#job-roles}

当用户执行下列操作之一时，系统会生成“作业角色”审核日志条目：

* 创建作业角色
* 更改作业角色：

   * 更改名称
   * 添加、更改或删除描述
   * 添加、更改或删除每小时成本（成本/小时）
   * 添加、更改或删除开单费率（帐单/小时）

* 删除作业角色

有关配置作业角色的更多信息，请参阅 [创建和管理作业角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

### 登录尝试 {#login-attempt}

当用户执行下列操作之一时，系统会生成“登录尝试”审核日志条目：

* 在Workfront（在浏览器和移动设备应用程序中）中登录、注销或失败的登录尝试
* 在任何Workfront集成(例如，Workfront for Slack和Workfront for Salesforce)中登录、注销或失败
* 登录或注销Workfront API

当Workfront管理员使用“以登录方式登录”功能时，登录尝试日志不会记录。

>[!NOTE]
>
>如果贵组织已载入Adobe Admin Console，则此选项不可用。 如需详细信息，请咨询您的网络或IT管理员。

### 优先级 {#priority}

当用户执行下列操作之一时，系统会生成“优先级”审核日志条目：

* 创建优先级
* 更改优先级：

   * 更改名称
   * 更改颜色
   * 将其设置为默认值
   * 添加、更改或删除优先级描述
   * 隐藏或显示优先级

* 删除优先级

有关配置优先级的更多信息，请参阅 [创建和自定义优先级](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md).

### 项目首选项 {#project-preferences}

当用户执行下列操作之一时，系统会生成“项目首选项”审核日志条目：

* 创建自定义季度
* 更改项目首选项：

   * 锁定或解锁
   * 更改其设置之一
   * 启用、禁用或编辑
   * 编辑时间轴计算

* 删除自定义季度

有关项目首选项的更多信息，请参阅 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

### 严重程度 {#severity}

当用户执行下列操作之一时，系统会生成严重性审核日志条目：

* 创建问题严重性
* 更改问题严重性：

   * 更改名称
   * 更改颜色
   * 将其设置为默认值
   * 更改或删除严重性的描述
   * 隐藏或显示严重性

* 删除问题严重性

有关配置作业角色的更多信息，请参阅 [创建或自定义问题严重性](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md).

### 状态 {#status}

当用户执行下列操作之一时，系统会生成状态审核日志条目：

* 在系统或组级别创建状态
* 更改系统或组级别的状态：

   * 重命名
   * 将其设为默认状态
   * 锁定或解锁
   * 隐藏或取消隐藏
   * 更改颜色或描述

* 删除系统或组级别上的状态

有关状态的更多信息，请参阅 [状态概述](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### 任务和问题首选项 {#tasks-issues-preferences}

当用户通过以下方式之一更改“任务和问题”首选项时，系统会生成“任务和问题”首选项审核日志条目：

* 锁定或解锁首选项
* 更改首选项的设置
* 更改任务、问题或请求的访问设置

有关任务和问题首选项的详细信息，请参阅 [配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### 用户 {#user}

当用户执行下列操作之一时，系统会生成用户审核日志条目：

* 创建用户

   <!--
  DRAFTED IN FLARE:
  Gevorg checking with Jonah on whether this note should be here:
  
  -->

   >[!NOTE]
   >
   >如果贵组织已载入Adobe Admin Console，则此选项不可用。 如需详细信息，请咨询您的网络或IT管理员。

* 删除用户
* 更改用户的访问级别、公司、团队或群组
* 激活用户
* 停用用户
