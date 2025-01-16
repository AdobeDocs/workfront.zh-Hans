---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 在Workfront中将对象从一个环境移动到另一个环境
description: 环境升级功能旨在提供与配置相关的对象从一个环境移动到另一个环境的功能。 它不支持移动事务性对象的功能（只有有限的例外）。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 8b4c04f5-f519-44e9-8429-0ce80c2d7c5b
source-git-commit: 9a588df1ef48b40056c5228c8ff03b5819eb4410
workflow-type: tm+mt
source-wordcount: '1041'
ht-degree: 2%

---

# 在Workfront环境之间移动对象概述（环境升级）

利用环境升级功能，可将对象从一个Workfront环境移动到另一个环境。 例如，您可以在沙盒环境中创建并配置模板，因为您知道任何测试都不会影响组织的实际数据。 配置和测试模板后，您可以将其移至生产环境，随时使用。

此过程称为“环境升级”。

您可以在Workfront中执行此过程，方法是创建要移动的对象包，然后在新环境中安装该包。

* 有关在Workfront中执行此流程的具体说明，请参阅：

   * [创建或编辑环境升级包](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
   * [安装环境升级包](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)

* 有关通过Workfront API执行此过程的说明，请参阅[使用 [!DNL Workfront] API](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion.md)在 [!DNL Workfront] 环境之间移动对象。

[观看此功能的视频演示](https://video.tv.adobe.com/v/3429735/){target=_blank}

## 环境升级支持的对象

环境升级功能旨在提供与配置相关的对象从一个环境移动到另一个环境的功能。 这些是可配置的对象，如项目、团队或自定义表单。

由于环境升级涉及对象配置，因此不包括事务性对象（频繁更改或高度依赖于用例的对象）。 事务性对象的示例包括文档、问题、请求、更新和验证决策。

* [工作对象](#work-objects)
* [报表对象](#reporting-objects)
* [自定义数据对象](#custom-data-objects)
* [组织对象](#organization-objects)
* [其他配置对象](#other-configuration-objects)


### 工作对象

| 可提升的对象 | 包含的可升级链接对象 |
| --- | --- |
| 项目（项目） | 项目<br>任务<br>分配<br>前置任务<br>公司<br>覆盖率<br>组<br>角色<br>团队<br>审批流程<br>审批路径<br>审批步骤<br>步骤审批者<br>计划<br>非工作日<br>队列定义<br>队列主题组<br>队列主题<br>路由规则<br>里程碑路径<br>里程碑<br>小时类型<br>资源池<br>类别<br>类别参数<br>参数<br>参数组<br>参数选项<br>类别显示逻辑 |
| 模板（模板） | 模板<br>模板任务<br>模板任务分配<br>模板任务前置任务<br>公司<br>覆盖率<br>组<br>角色<br>团队<br>审批流程<br>审批路径<br>审批步骤<br>步骤审批者<br>计划<br>非工作日<br>队列定义<br>队列主题组<br>队列主题<br>路由规则<br>里程碑路径<br>里程碑<br>小时类型<br>资源池<br>类别<br>类别参数<br>参数<br>参数组<br>参数选项<br>类别显示逻辑 |

### 报表对象

| 可提升的对象 | 包含的可升级链接对象 |
| --- | --- |
| 布局模板(UITMPL) | 布局模板<br>仪表板<br>日历<br>日历节<br>外部页面<br>报告<br>筛选器<br>分组<br>视图<br>参数<br>组 |
| 仪表板(PTLTAB) | 仪表板<br>日历<br>日历节<br>外部页面<br>报告<br>筛选器<br>分组<br>视图<br>参数 |
| 日历(CALEND) | 日历<br>日历节 |
| 外部页面(EXTSEC) | 外部页面 |
| 报告(PTLSEC) | 报告<br>筛选器<br>分组<br>视图<br>参数 |
| 过滤器(UIFT) | 筛选器<br>参数 |
| 分组(UIGB) | 分组<br>参数 |
| 视图(UIVW) | 查看<br>参数 |

### 自定义数据对象

| 可提升的对象 | 包含的可升级链接对象 |
| --- | --- |
| 类别(CTGY) | 类别<br>类别参数<br>参数<br>参数组<br>参数选项<br>类别显示逻辑<br>组 |
| 参数（参数） | 参数<br>参数选项 |
| 参数组(PGRP) | 参数组 |

### 组织对象

| 可提升的对象 | 包含的可升级链接对象 |
| --- | --- |
| 组（组） | 组<br>子组（最多5个级别）*<br>类别<br>类别参数<br>参数<br>参数组<br>参数选项<br>类别显示逻辑 |
| 角色(ROLE) | 角色 |
| 团队（团队） | 团队<br>组 |
| 公司(CPY) | 公司<br>覆盖率<br>类别<br>类别参数<br>参数<br>参数组<br>参数<br>类别显示逻辑<br>组 |
| Portfolio（端口） | Portfolio<br>程序<br>组<br>类别<br>类别参数<br>参数<br>参数组<br>参数选项<br>类别显示逻辑 |
| 计划(PRGM) | 程序<br>Portfolio<br>组<br>类别<br>类别参数<br>参数<br>参数组<br>参数选项<br>类别显示逻辑 |

### 其他配置对象

| 可提升的对象 | 包含的可升级链接对象 |
| --- | --- |
| 批准流程(ARVPRC) | 审批流程<br>审批路径<br>审批步骤<br>步骤审批者<br>角色<br>团队<br>组 |
| 时间表(SCHED) | 计划<br>非工作日<br>组 |
| 里程碑路径(MPATH) | 里程碑路径<br>里程碑 |
| 周期性时间表(TSPRO) | 周期性时间表<br>小时类型 |
| 小时类型（小时） | 小时数类型 |
| 费用类型(EXPTYP) | 费用类型 |
| 风险类型(RSKTYP) | 风险类型 |
| 资源池(RSPL) | 资源池 |
| 访问级别(ACSLVL) | 访问级别 |
| 费率卡(RTCRD) | 费率卡 |
| 位置/分类器(CLSF) | 位置/分类器 |

\*当前不可用

<!--

>[!NOTE]
>
>Actions (ignore, select existing, and create new) are available on the following objects:
>
>* Role
>* Team
>* Company
>* Group

-->

## 环境提升状态

环境升级包在创建并准备在环境之间移动时经历多个状态。 您可以在Workfront中的包列表中看到这些状态，如果您使用Workfront API，也可以在API响应中看到这些状态。

这些状态包括：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>未装配</td> 
   <td><p>此状态将自动指定，表示已保存但尚未装配的软件包。 </p><p>用户无法直接设置此状态。</p></td> 
  </tr> 
  <tr> 
   <td>组装</td> 
   <td><p>在组装对象时，将自动指定此状态。 </p><p>组合是指自动识别要包含在包中的对象和子对象，并将这些对象及其数据添加到包中的过程。</p><p>用户无法直接设置此状态。</p></td> 
  </tr> 
  <tr> 
   <td>草稿</td> 
   <td><p>此状态在装配过程结束时或创建空升级包时指定。</p><p>用户可以将促销活动包移回此状态。</p><p>处于此状态时，无法在任何环境中安装升级包。</p></td> 
  </tr> 
  <tr> 
   <td>测试</td> 
   <td><p>此状态允许在任何“预览”或“自定义刷新”沙盒中安装升级包。 处于此状态时，无法在生产环境中安装软件包。</p></td> 
  </tr> 
  <tr> 
   <td>活动</td> 
   <td><p>此状态允许在任何环境（包括生产环境）中安装升级包。</p><p>当程序包状态设置为ACTIVE时，<code>publishedAt</code>日期将自动设置为请求的当前时间戳。</p></td> 
  </tr> 
  <tr> 
   <td>已禁用</td> 
   <td><p>此状态用于隐藏以前使用的升级包，这些升级包将来不会安装到任何环境中。</p><p>当软件包处于此状态时，无法将其安装到任何环境中。</p><p>当程序包状态设置为DISABLED时，<code>retiredAt</code>日期将自动设置为请求的当前时间戳。</p><p>建议在使用<code>DELETE /package</code>终结点时使用该状态，因为它是可检索的，并且使用此包进行的任何部署都将保留安装历史记录。</p></td> 
  </tr> 
  <tr> 
   <td>ASSEMBLY_FAILED</td> 
   <td><p>如果ASSEMBLY阶段失败，则升级包会自动处于此状态。</p><p>要将软件包返回到ASSEMBLY阶段，必须再次触发装配过程。</p><p>有关汇编包的详细信息，请参阅创建或编辑环境升级包一文中的<a href="https://experienceleague.adobe.com/en/docs/workfront/using/administration-and-setup/set-up-wf/testing-environments/environment-promotion-create-package#edit-or-assemble-an-existing-package">编辑或汇编现有包</a>部分。</td> 
  </tr> 
  </tbody> 
</table>

## 资源

* 有关环境升级的常见问题解答，请参阅[环境升级常见问题解答](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-faq.md)
* 有关疑难解答建议，请参阅[环境提升疑难解答](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-troubleshooting.md)


