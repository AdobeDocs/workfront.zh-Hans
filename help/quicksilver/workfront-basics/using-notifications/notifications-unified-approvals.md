---
content-type: reference
navigation-topic: notifications
title: 通知：统一审批
description: 以下通知提醒您统一审批体验的审批活动。 有关配置您收到的通知的信息，请参阅修改您自己的电子邮件通知。
author: Courtney
feature: Get Started with Workfront
exl-id: 6e60a9ec-4fe0-4f3d-a4dd-8dc09d11b834
last-update: 2026-10-20T00:00:00.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: c042179c-157b-516d-b27c-e3bf303e8567
    internal-label: Get Started with Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 7957c410d4a0e39b23b4f5a3d29a794e5deec72a
workflow-type: tm+mt
source-wordcount: '1052'
ht-degree: 0%
---
# 通知：统一审批

{{highlighted-preview}}

使用以下通知随时了解有关统一审查和批准活动的信息。 有关配置您收到的电子邮件通知的信息，请参阅[修改您自己的电子邮件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。

>[!NOTE]
>
>这些通知仅作为即时通知提供，不在每日摘要中提供。


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th>包含的字段</th> 
   <th>默认状态</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>审批已完成 — 已批准</strong> </p> <p>文档审批结束，最终决策为已批准。</p> <p>即时通知电子邮件的主题是： <em>最终决定： （文档）已批准</em></p> </td> 
   <td> <p>最终决定<br>文档<br>审批请求日期<br>到期日期<br>“前往审阅”按钮<br>详细信息块：文档名称、文档详细信息、所有收件人</p> <p><em>包含在部分审批中：</em><br>自定义消息<br>阶段<br>项目</p> </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>审批已完成 — 已审批，但有更改</strong> </p> <p>文档审批结束，最终决定为已批准，但有更改。</p> <p>即时通知电子邮件的主题是： <em>最终决定： （文档）已批准更改</em></p> </td> 
   <td> <p>最终决定<br>文档<br>审批请求日期<br>到期日期<br>“前往审阅”按钮<br>详细信息块：文档名称、文档详细信息、所有收件人</p> <p><em>包含在部分审批中：</em><br>自定义消息<br>阶段<br>项目</p> </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>审批已完成 — 需要工作</strong> </p> <p>文档审批以需求工作的最终决策结束。</p> <p>即时通知电子邮件的主题是： <em>最终决定： （文档）需要工作</em></p> </td> 
   <td> <p>最终决定<br>文档<br>审批请求日期<br>到期日期<br>“前往审阅”按钮<br>详细信息块：文档名称、文档详细信息、所有收件人</p> <p><em>包含在部分审批中：</em><br>自定义消息<br>阶段<br>项目</p> </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>临近截止日期</strong> </p> <p>您所属的文档审批即将到达截止日期。</p> <p>即时通知电子邮件的主题是： <em>审批截止日期已接近（文档）</em></p> </td> 
   <td> <p>请求者<br>您的角色<br>团队<br>审批请求日期<br>到期日期<br>“前往审阅”按钮<br>详细信息块：文档名称、文档详细信息、所有收件人</p> <p><em>包含在部分审批时：</em><br>文档预览<br>自定义消息<br>暂存<br>项目</p> </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>截止日期已错过</strong> </p> <p>您所属的文档审批已超过其截止日期，但无最终决定。</p> <p>即时通知电子邮件的主题为： <em>审批截止日期已错过（文档）</em></p> </td> 
   <td> <p>固定标题<br>审批请求日期<br>到期日期<br>“前往审阅”按钮<br>详细信息块：文档名称、文档详细信息、所有收件人</p> <p><em>包含在部分批准中：</em><br>阶段</p> </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>审核已完成</strong> </p> <p>审阅人对文档批准完成审阅。</p> <p>即时通知电子邮件的主题是： <em>（文档）已审阅</em></p> </td> 
   <td> <p>审阅者<br>文档<br>“前往审阅”按钮<br>详细信息块：文档名称、文档详细信息、所有收件人</p> <p><em>包含在部分审批时：</em><br>文档预览<br>阶段<br>项目</p> </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>视频审批限制即将达到(80%)</strong> </p> <p>视频审批达到其计划视频审批限额的80%。</p> <p>即时通知电子邮件的主题是： <em>您已接近Workfront中的年度视频审批请求限制</em></p> </td> 
   <td> 标题和正文文本<br>请求的视频审批（当前使用情况）<br>总上限（限制）<br>其他收件人<br>“在Workfront中查看”按钮<br>“升级到FIO enterprise”按钮 </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p>已达到<strong>视频审批限制</strong> </p> <p>视频审批达到其计划的视频审批限制。</p> <p>即时通知电子邮件的主题是： <em>您已达到Workfront中的年度视频审批请求限制</em></p> </td> 
   <td> 标题和正文文本<br>请求的视频审批（当前使用情况）<br>总上限（限制）<br>其他收件人<br>“在Workfront中查看”按钮<br>“升级到FIO enterprise”按钮 </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>决策已做出 — 已批准</strong> </p> <p>审批者对文档审批作出批准决策。</p> <p>即时通知电子邮件的主题是： <em>（文档）由（名称）</em>批准</p> </td> 
   <td> <p>决策者<br>决策<br>文档和版本<br>“前往审阅”按钮<br>详细信息块：文档名称、文档详细信息、所有收件人</p> <p><em>包含在部分审批时：</em><br>文档预览<br>自定义消息<br>暂存<br>项目</p> </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>决策已做出 — 已批准，但有更改</strong> </p> <p>审批者对文档审批作出了“已批准”的决策，并对文档审批进行了更改。</p> <p>即时通知电子邮件的主题是： <em>（文档）已批准，更改者为（名称）</em></p> </td> 
   <td> <p>决策者<br>决策<br>文档和版本<br>“前往审阅”按钮<br>详细信息块：文档名称、文档详细信息、所有收件人</p> <p><em>包含在部分审批时：</em><br>文档预览<br>自定义消息<br>暂存<br>项目</p> </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>决策已做出 — 需要工作</strong> </p> <p>批准者决定需要处理文档批准。</p> <p>即时通知电子邮件的主题是： <em>（文档）需要由（名称）</em>工作</p> </td> 
   <td> <p>决策者<br>决策<br>文档和版本<br>“前往审阅”按钮<br>详细信息块：文档名称、文档详细信息、所有收件人</p> <p><em>包含在部分审批时：</em><br>文档预览<br>自定义消息<br>暂存<br>项目</p> </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>添加到分组审批或从分组审批中删除的文档</strong> </p> <p>在您所属的已分组文档审批中添加或删除文档。</p> <p>即时通知电子邮件的主题是： <em>在作为您成员的审批中添加或删除了文档</em></p> </td> 
   <td> <p><strong>已添加：</strong><br>请求者<br>组名<br>缩略图预览<br>日期<br>“前往审阅”按钮<br>详细信息块：组名、资源数、所有收件人</p> <p><em>包含在部分审批时：</em><br>自定义消息<br>项目</p> <p><strong>已删除：</strong><br>请求者<br>组名<br>缩略图预览（无按钮或详细信息块）</p> </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>所有审阅已完成</strong> </p> <p>每个审阅人对文档批准完成审阅。</p> <p>即时通知电子邮件的主题是： <em>所有审阅均已完成（文档）</em></p> </td> 
   <td> <p>文档<br>审批请求日期<br>到期日期<br>“前往审阅”按钮<br>详细信息块：文档名称、文档详细信息、所有收件人</p> <p><em>包含在部分审批中：</em><br>自定义消息<br>阶段<br>项目</p> </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>提醒 — 24小时</strong> </p> <p>您还有24小时来审阅和批准文档。</p> <p>即时通知电子邮件的主题是： <em>提醒： （文档）</em>上需要您的批准</p> </td> 
   <td> <p>请求者<br>您的角色<br>团队<br>审批请求日期<br>到期日期<br>“前往审阅”按钮<br>详细信息块：文档名称、文档详细信息、所有收件人</p> <p><em>包含在部分审批时：</em><br>文档预览<br>自定义消息<br>暂存<br>项目</p> </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>提醒 — 72小时</strong> </p> <p>您还剩72小时来审阅和批准文档。</p> <p>即时通知电子邮件的主题是： <em>提醒： （文档）</em>上需要您的批准</p> </td> 
   <td> <p>请求者<br>您的角色<br>团队<br>审批请求日期<br>到期日期<br>“前往审阅”按钮<br>详细信息块：文档名称、文档详细信息、所有收件人</p> <p><em>包含在部分审批时：</em><br>文档预览<br>自定义消息<br>暂存<br>项目</p> </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>已添加为批准者或审阅者</strong> </p> <p>您被添加为文档批准的批准者或查看者。</p> <p>即时通知电子邮件的主题是： <em>需要您审批（文档）</em></p> </td> 
   <td> <p>请求者<br>您的角色<br>团队<br>审批请求日期<br>到期日期<br>“前往审阅”按钮<br>详细信息块：文档名称、文档详细信息、所有收件人</p> <p><em>包含在部分审批时：</em><br>文档预览<br>自定义消息<br>暂存<br>项目</p> </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>已移除审批者或审阅者</strong> </p> <p>您会从文档审批中删除审批者或审阅者。</p> <p>即时通知电子邮件的主题是： <em>不再需要您审批（文档）</em></p> </td> 
   <td> <p>请求者<br>文档和版本<br>角色<br>团队（无按钮或详细信息块）</p> <p><em>包含在部分审批时：</em><br>文档预览<br>自定义消息</p> </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>角色已更改</strong> </p> <p>您的审批者或审阅者角色在文档审批时发生了更改。</p> <p>即时通知电子邮件的主题是： <em>您在（文档）上的角色已更改</em></p> </td> 
   <td> <p>请求者<br>文档和版本<br>角色更改方向<br>“前往审阅”按钮<br>详细信息块：文档名称、文档详细信息、所有收件人</p> <p><em>包含在部分审批时：</em><br>文档预览<br>阶段<br>项目</p> </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
 </tbody> 
</table>
