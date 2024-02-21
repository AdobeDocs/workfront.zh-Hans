---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Adobe Workfront中可用的事件通知
description: 事件通知是由对象（如项目、任务和问题）上的各种类型事件触发的电子邮件。 本文列出并描述了可用的事件通知类型。
author: Lisa, Nolan
feature: System Setup and Administration
role: Admin
exl-id: de7a995d-ff1e-4631-91f7-4dc895a87c94
source-git-commit: 738286fdcd19d1db648da220778d1041a0010cff
workflow-type: tm+mt
source-wordcount: '5127'
ht-degree: 8%

---

# Adobe Workfront中可用的事件通知

<!-- Audited: 1/2024 -->

事件通知是由对象（如项目、任务和问题）上的各种类型事件触发的电子邮件，如中所述 [事件通知](../../../workfront-basics/using-notifications/event-notifications.md).

可以在系统和组级别配置这些通知：

* 有关在系统级别配置事件通知的信息，请参见 [为系统中的每个人配置事件通知](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
* 有关在组级别配置事件通知的信息，请参见 [查看和配置组的事件通知](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

个人用户还可以在个人配置文件中激活和取消激活其个人事件通知。 有关更多信息，请参阅 [修改您自己的电子邮件通知](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

下表列出了所有Adobe Workfront事件通知、事件的简短描述以及默认情况下事件是处于活动状态还是非活动状态。

## 需要操作

另请参阅 [通知：需要操作](../../../workfront-basics/using-notifications/notifications-action-needed.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>对象类型</th> 
   <th>事件</th> 
   <th>收件人</th> 
   <th>描述</th> 
   <th>默认状态</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>用户</p> </td> 
   <td> <p>访问请求</p> </td> 
   <td> <p>用户</p> </td> 
   <td> <p>有人向我请求访问权限。</p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>文档</p> <p> </p> </td> 
   <td> <p>文档请求添加</p> </td> 
   <td> <p>请求该文档的用户</p> </td> 
   <td> <p>有人请求我上传文档。</p> <p>文档请求者在收到上传文档的请求时会收到电子邮件通知。</p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>文档</p> </td> 
   <td> <p>待审批文档</p> </td> 
   <td> <p>审批者</p> </td> 
   <td> <p>我需要审批一个文档。</p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>问题</p> </td> 
   <td> <p>问题分配</p> </td> 
   <td> <p>问题分派到的用户</p> </td> 
   <td> <p>我被分派到一个问题。</p> <p>仅当项目的状态为“当前”并且问题的状态不是“已关闭”或等同于“已关闭”的状态时，问题受理人才会收到电子邮件通知。</p> <p>拥有轻度许可、参与者许可、审查许可或请求许可的用户不会收到通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>问题</p> </td> 
   <td> <p>未决批准的问题</p> </td> 
   <td> <p>审批者</p> </td> 
   <td> <p>我需要批准一个问题。</p> <p>哪些用户会收到此事件的电子邮件通知取决于“不要求审批者加入项目团队（对于包括角色的审批流程）”设置是否已启用（如中所述） <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">配置全局审批设置</a>)。 </p> <p>如果已启用此选项</strong>，会向系统中具有“审批者”工作角色的所有用户发送电子邮件通知。</p> <p>如果禁用此选项</strong>，则只有具有“审批者”工作角色的项目团队成员会收到电子邮件通知。</p> <p>如果项目处于“计划”或“当前”状态，则会发送通知。 </p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>问题</p> </td> 
   <td> <p>未决批准的问题</p> </td> 
   <td> <p>已委托的审批者</p> </td> 
   <td> <p>我需要回顾委托给我的问题审批。</p> <p>当有人将问题审批委派给另一个用户时，将通知该用户。 </p> <p>仅当项目处于当前状态时，才会发送通知。</p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>项目</p> </td> 
   <td> <p>未决批准的项目</p> </td> 
   <td> <p>审批者</p> </td> 
   <td> <p>我需要审批一个项目。</p> <p>哪些用户会收到此事件的电子邮件通知取决于“不要求审批者加入项目团队（对于包括工作角色的审批流程）”设置是否已启用（如所述） <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">配置全局审批设置</a>)。</p> <p>如果已启用此选项</strong>，会向系统中具有“审批者”工作角色的所有用户发送电子邮件通知。</p> <p>如果禁用此选项</strong>，则只有具有“审批者”工作角色的项目团队成员会收到电子邮件通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td>项目</td> 
   <td>未决批准的项目</td> 
   <td>已委托的审批者</td> 
   <td> <p>我需要回顾委托给我的项目审批。</p> </td> 
   <td> 活动</td> 
  </tr> 
  <tr> 
   <td> <p>任务</p> </td> 
   <td> <p>任务分派</p> </td> 
   <td> <p>任务被分派到的用户</p> </td> 
   <td> <p>我被设置为任务的主要被分配人。</p> <p>如果任务被分配人是任务的主要被分配人，则任务被分配人会收到电子邮件通知，除非被分配人是进行分配的用户。</p> <p>如果项目状态为“当前”且任务未标记为“完成”，则会发送通知。</p> <p>拥有“Light”或“Review”许可证的用户不会收到通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务</p> </td> 
   <td> <p>未决批准的任务</p> </td> 
   <td> <p>审批者</p> </td> 
   <td> <p>我需要批准一项任务。</p> <p>哪些用户会收到此事件的电子邮件通知取决于“不要求审批者加入项目团队（对于包括角色的审批流程）”设置是否已启用（如中所述） <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">配置全局审批设置</a>)。 </p> <p>如果已启用此选项</strong>，会向系统中具有“审批者”工作角色的所有用户发送电子邮件通知。</p> <p>如果禁用此选项</strong>，则只有具有“审批者”工作角色的项目团队成员会收到电子邮件通知。</p> <p>仅当请求时的项目状态为“当前”时，才会发送通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务</p> </td> 
   <td> <p>未决批准的任务</p> </td> 
   <td> <p>已委托的审批者</p> </td> 
   <td> <p>我需要回顾委托给我的任务审批。</p> <p>当有人将问题审批委派给另一个用户时，将通知该用户。 </p> <p>仅当请求时的项目状态为“当前”时，才会发送通知。</p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>时间表</p> </td> 
   <td> <p>重新开立的工时表</p> </td> 
   <td> <p>时间表所属的用户</p> </td> 
   <td> <p>我的工时表已重新开立。</p> <p>除非重新打开时间表的用户同时也是时间表的所有者，否则时间表所有者会在时间表重新打开时收到电子邮件通知。</p> <p>仅当时间表状态为“打开”时，才会发送电子邮件通知。</p> <p>拥有“Light”或“Review”许可证的用户不会收到通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>时间表</p> </td> 
   <td> <p>拒绝时间表</p> </td> 
   <td> <p>时间表所属的用户</p> </td> 
   <td> <p>我的工时表被拒绝。</p> <p>时间表所有者会在时间表被拒绝时收到电子邮件通知，除非拒绝时间表的用户同时也是所有者。</p> <p>仅当时间表状态为“被拒绝”时，才会发送电子邮件通知。</p> <p>拥有“Light”或“Review”许可证的用户不会收到通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>时间表</p> </td> 
   <td> <p>工时表提交</p> </td> 
   <td> <p>审批者</p> </td> 
   <td> <p>我需要审批工时表。</p> <p>在提交需要审批的时间表后，时间表审批者会收到电子邮件通知，除非提交时间表的用户也是时间表审批者。</p> <p>仅当时间表状态为“已提交”时，才会发送通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务</p> </td> 
   <td> <p>工作项请求</p> </td> 
   <td> <p>项目所针对的团队成员</p> </td> 
   <td> <p>我的团队获得了新的工作请求。</p> <p>当团队收到新的工作请求时，团队成员会收到电子邮件通知。 （如果提交请求的用户是团队成员，则不会收到通知。）</p> <p>仅当发出工作请求时的项目状态为“当前”且工作请求状态为“新建”时，才会发送通知。</p> <p>拥有“Light”或“Review”许可证的用户不会收到通知。</p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务</p> </td> 
   <td> <p>工作项请求</p> </td> 
   <td> <p>请求工作项的用户</p> </td> 
   <td> <p>我收到新的工作请求。</p> <p>工作项的被分派人会收到电子邮件通知，除非提出请求的用户也是被分派人。 </p> <p>如果任务状态为“完成”或问题状态为“已关闭”，则不会发送通知。</p> <p>仅当请求时的项目状态为“当前”时，才会发送通知。</p> <p>拥有“Light”或“Review”许可证的用户不会收到通知。</p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
 </tbody> 
</table>

## 我已提出的请求

另请参阅 [通知：我已发出的请求](../../../workfront-basics/using-notifications/notifications-requests-i-have-made.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>对象类型</th> 
   <th>事件</th> 
   <th>收件人</th> 
   <th>描述</th> 
   <th> 默认状态</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>文档</p> </td> 
   <td> <p>文档审批状态更改</p> </td> 
   <td> <p>请求人</p> </td> 
   <td> <p>文档审批请求已完成。</p> <p>文档审批请求完成后，文档请求者会收到电子邮件通知。</p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>文档</p> </td> 
   <td> <p>文档请求完成</p> </td> 
   <td> <p>请求人</p> </td> 
   <td> <p>已履行文档上传请求。</p> <p>当上传文档的请求得到满足时，文档请求者会收到电子邮件通知。</p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>问题</p> </td> 
   <td> <p>问题添加</p> </td> 
   <td> <p>问题创建者</p> </td> 
   <td> <p>我在项目中添加了一个问题。</p> <p>当问题创建者向项目中添加问题时，问题创建者会收到通知。</p> <p>仅当项目状态为“当前”或“计划”时，才会发送通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td>问题</td> 
   <td>问题分配</td> 
   <td>问题创建者</td> 
   <td> <p>有人被分配到我是主要联系人的问题。</p> <p>将问题分配给用户后，问题的主要联系人会收到通知。 </p> <p>仅当项目状态为“当前”或“计划”时，才会发送通知。</p> </td> 
   <td> 非活动</td> 
  </tr> 
  <tr> 
   <td> <p>问题</p> </td> 
   <td> <p>问题完成</p> </td> 
   <td> <p>问题创建者</p> </td> 
   <td> <p>在完成问题之后，发送电子邮件给问题创建者。</p> <p>仅当项目状态为“当前”或“计划”时，才会发送通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>项目</p> </td> 
   <td> <p>项目状态更改</p> </td> 
   <td> <p>创建项目的用户（输入者）</p> </td> 
   <td> <p>当项目状态更改时，向输入项目的用户发送电子邮件。</p> <p>项目状态更改时，创建项目的用户会收到电子邮件通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>问题</p> </td> 
   <td> <p>请求添加</p> </td> 
   <td> <p>问题创建者</p> </td> 
   <td> <p>我提交请求（确认）。</p> <p>问题的主要联系人会在提交问题时收到电子邮件通知。</p> <p>仅当项目状态为“当前”并且项目使用“是技术支持”视图时，才会发送通知。</p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>问题</p> </td> 
   <td> <p>请求分配</p> </td> 
   <td> <p>问题创建者</p> </td> 
   <td> <p>有人已分配给我的请求。</p> <p>当用户被分配给问题时，除非主要联系人和分配的用户是同一个用户，否则问题的主要联系人会收到电子邮件通知。</p> <p>仅当项目状态为“当前”并且项目使用“是技术支持”视图时，才会发送通知。</p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>问题</p> </td> 
   <td> <p>请求已关闭</p> </td> 
   <td> <p>问题创建者</p> </td> 
   <td> <p>我的请求已关闭（确认）。</p> <p>当请求关闭时，问题的主要联系人会收到电子邮件通知。</p> <p>仅当项目状态为“当前”并且项目使用“是技术支持”视图时，才会发送通知。</p> <p>如果启用了“问题完成”通知，它们将始终触发，而不是“向问题主要联系人关闭的请求”。 如果要触发此通知，则必须取消激活“问题完成”通知。</p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>文档</p> </td> 
   <td> <p>请求文档添加</p> </td> 
   <td> <p>问题创建者</p> </td> 
   <td> <p>在我是主要联系人的问题上更改或上传文档。</p> <p>在上传或更改有关问题的文档时，问题的主要联系人会收到电子邮件通知，除非上传或更改文档的用户同时也是主要联系人。</p> <p>仅当项目状态为“当前”，且项目在“队列设置”选项卡上启用了“作为帮助请求队列发布”时，才会发送通知。</p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>问题</p> </td> 
   <td> <p>请求状态更改</p> </td> 
   <td> <p>问题创建者</p> </td> 
   <td> <p>我的请求上的状态已更改。</p> <p>问题主要联系人会在问题状态更改时收到电子邮件通知，除非更改状态的用户同时也是主要联系人。</p> <p>仅当项目状态为“当前”并且项目使用“是技术支持”视图时，才会发送通知。</p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE:
       For more information on publishing a project as a Help Request Queue, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.-->

## 通信

另请参阅 [通知：通信](../../../workfront-basics/using-notifications/notifications-communication.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>对象类型</th> 
   <th>事件</th> 
   <th>收件人</th> 
   <th>描述</th> 
   <th> 默认状态</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>文档</p> </td> 
   <td> <p>文档评论</p> </td> 
   <td> <p>文档所有者</p> </td> 
   <td> <p>在我的文档中添加了一个评论。</p> <p>Workfront中文档的所有者会在文档上发布评论时收到电子邮件通知，除非发布评论的用户同时也是文档所有者。</p> <p>任何直接包含在评论中的用户都会收到电子邮件通知。</p> <p>仅当项目状态为“当前”时，才会发送通知。 </p> <p>即时通知电子邮件的主题是： <em>评论 &lt;request name=""&gt; 日期 &lt;project name=""&gt; (参考编号 &lt;request reference="" number=""&gt;)</em></p> <p> 每日摘要通知的主题是：<em> 通信的摘要 &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>活动 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>注释</p> </td> 
   <td> <p>请求注释添加</p> </td> 
   <td> <p>问题创建者</p> </td> 
   <td> <p>在请求上发布评论时，通过电子邮件将问题发送给主要联系人。</p> <p>当在请求上发布评论时，问题的主要联系人会收到电子邮件通知，除非发布评论的用户也是问题的主要联系人。</p> <p>任何直接包含在评论中的用户都会收到电子邮件通知。</p> <p>仅当项目状态为“当前”时，才会发送通知。</p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>用户</p> </td> 
   <td>定向更新</td> 
   <td>用户</td> 
   <td> <p>有人将我列入定向更新。</p> <p>定向更新是指用户明确在更新中包含另一个用户的情况，如中所述 <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">为其他人标记更新</a>.</p> <p>在这种情况下，定向更新中包含的用户会收到有关更新的电子邮件通知。</p> <p>仅当用户具有对象的访问权限并在其配置文件中将其保持启用时，才会发送电子邮件通知。  </p> <p>默认情况下，此事件通知处于激活状态，无法取消激活。</p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>团队</p> </td> 
   <td> <p>定向更新</p> </td> 
   <td> <p>团队成员</p> </td> 
   <td> <p>有人将我的团队列入定向更新。</p> <p>定向更新是指用户明确在更新中包含另一个用户的情况，如中所述 <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">为其他人标记更新</a>.</p> <p>在这种情况下，定向更新中包括的团队的任何成员都会收到有关更新的电子邮件通知。</p> <p>电子邮件通知仅发送给对更新对象具有访问权限的用户。</p> <p>如果发送定向更新的用户是所包含的团队的成员，则发送更新的用户不会收到电子邮件通知。</p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>注释</p> </td> 
   <td> <p>工作项注释</p> </td> 
   <td> <p>跟帖参与者</p> </td> 
   <td> <p>某人备注我所在的跟帖。</p> <p>当用户在线程中发表评论时，线程中的参与者和直接消息中包含的用户会收到电子邮件通知。</p> <p>用户必须具有查看权限才能接收通知。</p> <p>以下用户未收到通知：</p> 
    <ul> 
     <li> <p>直接消息中包含的团队</p> </li> 
     <li> <p>注释的所有者</p> </li> 
     <li> <p>主要联系人</p> </li> 
    </ul> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>注释</p> </td> 
   <td> <p>工作项注释</p> </td> 
   <td> <p>工作项分派人</p> </td> 
   <td> <p>某人备注我的工作项之一。</p> <p>工作项的被分派人在用户向工作项添加更新时收到电子邮件通知，除非添加更新的用户也是被分派人。</p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>注释</p> </td> 
   <td> <p>工作请求回复</p> </td> 
   <td> <p> 工作请求者</p> </td> 
   <td> <p>有人回复了我的请求。</p> <p>当用户提交请求且另一个用户回复该请求后，提交请求的用户会收到电子邮件通知。</p> <p>如果出现以下情况，则不发送电子邮件通知：</p> 
    <ul> 
     <li> <p>回复的用户是发出请求的同一个用户</p> </li> 
     <li> <p>用户无权查看注释</p> </li> 
    </ul> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: for the directed update above, it also mentions:
        ... and is not the same user that enters the update-->

## 审批信息

另请参阅 [通知：审批信息](../../../workfront-basics/using-notifications/notifications-approval-information.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>对象类型</th> 
   <th>事件</th> 
   <th>收件人</th> 
   <th>描述</th> 
   <th> 默认状态</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>用户</p> </td> 
   <td> <p>审批委托</p> </td> 
   <td> <p>用户</p> </td> 
   <td> <p>我被委托为批准者。</p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>问题</p> </td> 
   <td> <p>委派问题审批的状态更改</p> </td> 
   <td> <p>委托审批的用户</p> </td> 
   <td> <p>已完成委托的问题审批请求。 </p> <p>当您将问题审批委托给其他人时，您会在他们完成该审批时收到电子邮件通知（无论他们是否批准或拒绝问题审批）。 </p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>项目</p> </td> 
   <td> <p>委派项目审批的状态更改</p> </td> 
   <td> <p>委托审批的用户</p> </td> 
   <td> <p>已完成委托的项目审批请求。</p> <p>当您将项目审批委托给其他人时，您会在他们完成该审批时收到电子邮件通知（无论他们是否批准或拒绝项目审批）。</p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务</p> </td> 
   <td> <p>委派任务审批的状态更改</p> </td> 
   <td> <p>委托审批的用户</p> </td> 
   <td> <p>委托的任务审批状态已完成。</p> <p>当您将任务审批委托给其他人时，您会在他们完成该审批时收到电子邮件通知（无论他们是否批准或拒绝任务审批）。</p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>文档</p> </td> 
   <td> <p>“文档审批取消”到“审批者”</p> </td> 
   <td> <p>委托审批的用户</p> </td> 
   <td> <p>文档审批请求已取消。</p> <p>文档审批请求被取消时，文档的文档审批者会收到电子邮件通知。</p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>时间表</p> </td> 
   <td> <p>工时表批准</p> </td> 
   <td> <p>时间表所属的用户</p> </td> 
   <td> <p>我的工时表已被批准。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
 </tbody> 
</table>

## 有关分派给我的工作的信息

另请参阅 [通知：有关分配给我的工作的信息](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>对象类型</th> 
   <th>事件</th> 
   <th>收件人</th> 
   <th>描述</th> 
   <th> 默认状态</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>任务</td> 
   <td>所有前置任务完成</td> 
   <td>分配给依赖任务的团队成员</td> 
   <td> <p>已完成团队任务的所有前置任务。</p> <p>任务被分派人（团队的所有成员）都会收到电子邮件通知。</p> <p>拥有“Light”或“Review”许可证的用户不会收到通知。</p> </td> 
   <td>非活动</td> 
  </tr> 
  <tr> 
   <td> <p>任务</p> </td> 
   <td> <p>所有前置任务完成</p> </td> 
   <td> <p>分配给依赖任务的用户</p> </td> 
   <td> <p>我的任务的所有前置任务都已完成。</p> <p>任务被分派人收到电子邮件通知。</p> <p>拥有“Light”或“Review”许可证的用户不会收到通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>问题</p> </td> 
   <td> <p>批准决定</p> </td> 
   <td> <p>问题分派到的用户</p> </td> 
   <td> <p>在批准或拒绝问题之后，向被分派的用户发送电子邮件。</p> <p>在作出（批准或拒绝）批准决策时，问题的被分派人会收到电子邮件通知。</p> <p>拥有“Light”或“Review”许可证的用户不会收到通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务</p> </td> 
   <td> <p>批准决定</p> </td> 
   <td> <p>任务分派到的用户</p> </td> 
   <td> <p>我完成的任务已被批准或拒绝。</p> <p>当任务被批准或拒绝时，任务被分派人会收到电子邮件通知。</p> <p>仅当项目状态为“当前”时，才会发送通知。</p> <p>拥有“Light”或“Review”许可证的用户不会收到通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>问题</p> </td> 
   <td> <p>问题完成</p> </td> 
   <td> <p>问题分派到的用户</p> </td> 
   <td> <p>在完成问题之后，发送电子邮件给分派用户。</p> <p>仅当项目状态为“当前”或“计划”时，才会发送通知。</p> <p>拥有“Light”或“Review”许可证的用户不会收到通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>问题</p> </td> 
   <td> <p>问题计划完成日期已更改</p> </td> 
   <td> <p>问题分派到的用户</p> </td> 
   <td> <p>当问题的截止日期改变时，向被分派的用户发送电子邮件。</p> <p>问题被分配人在计划完成日期更改时收到电子邮件通知，除非更改计划完成日期的用户也是被分配人。</p> <p>仅当项目状态不是Planning时才发送通知。</p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>问题</p> </td> 
   <td> <p>问题状态更改</p> </td> 
   <td> <p>问题分派到的用户</p> </td> 
   <td> <p>我的工作项之一的状态发生更改。</p> <p>除非更改状态的用户同时也是受让人，否则问题的受让人在状态更改时收到电子邮件通知。</p> <p>仅当项目状态为“当前”时，才会发送通知。</p> <p>拥有“Light”或“Review”许可证的用户不会收到通知。</p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>文档</p> </td> 
   <td> <p>请求文档添加</p> </td> 
   <td> <p>问题分派到的用户</p> </td> 
   <td> <p>在我的请求下上传或更改文档。</p> <p>在上传或更改其添加问题的文档时，问题被分派人会收到电子邮件通知。</p> <p>如果输入问题的用户是问题受分配人，则不会发送电子邮件通知。</p> <p>仅当项目状态为“当前”，且项目在“队列设置”选项卡上启用了“作为帮助请求队列发布”时，才会发送通知。</p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务</p> </td> 
   <td> <p>任务完成</p> </td> 
   <td> <p>任务分派到的用户</p> </td> 
   <td> <p>在完成任务之后，发送电子邮件给分派用户。</p> <p>任务被分派人在任务完成时收到电子邮件通知。 个人任务完成后，不会发送通知。</p> <p>仅当项目状态为“当前”时，才会发送通知。</p> <p>拥有轻度许可、参与者许可、审查许可或请求者许可的用户不会收到通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务</p> </td> 
   <td> <p>任务完成</p> </td> 
   <td> <p>分配给依赖任务的用户</p> </td> 
   <td> <p>我的任务之一的前置任务已完成。</p> <p>当任务的前置任务之一完成时，任务被分派人会收到电子邮件通知。</p> <p>拥有“Light”或“Review”许可证的用户不会收到通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务</p> </td> 
   <td> <p>任务计划完成日期已更改</p> </td> 
   <td> <p>任务分派到的用户</p> </td> 
   <td> <p>当任务的到期日期改变时，向被分派的用户发送电子邮件。</p> <p>当任务的计划完成日期更改时，任务被分配人会收到电子邮件通知，除非更改计划完成日期的用户也是任务被分配人。</p> <p>仅当项目状态不是Planning时才发送通知。</p> <p>不会发送有关个人任务的通知。</p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务</p> </td> 
   <td> <p>任务状态更改</p> </td> 
   <td> <p>任务分派到的用户</p> </td> 
   <td> <p>当任务状态更改时，向被分派的用户发送电子邮件。</p> <p>任务被分配人会在任务状态更改时收到电子邮件通知，除非更改状态的用户也是被分配人。</p> <p>仅当项目状态为“当前”时，才会发送通知。</p> <p>拥有“Light”或“Review”许可证的用户不会收到通知。 </p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: from the Request document add to issue assigned to: 
        For more information on publishing a project as a Help Request Queue, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>. -->

## 有关我参与的项目的信息

另请参阅 [通知：关于我参与的项目的信息](../../../workfront-basics/using-notifications/notifications-information-about-projects-im-on.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>对象类型</th> 
   <th>事件</th> 
   <th>收件人</th> 
   <th>描述</th> 
   <th> 默认状态</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>项目</p> </td> 
   <td> <p>当前项目状态</p> </td> 
   <td> <p>项目团队成员</p> </td> 
   <td> <p>当项目处于活动状态时，发送电子邮件给团队。</p> <p>项目用户会在项目变为活动状态时收到电子邮件通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>文档</p> </td> 
   <td> <p>文档添加</p> </td> 
   <td> <p>项目团队成员</p> </td> 
   <td> <p>在添加文档之后，发送电子邮件给团队。</p> <p>将文档添加到项目时，项目团队中的用户会收到电子邮件通知，但添加该文档的用户除外。</p> <p>仅当项目状态为“当前”且文档不是“专用”时，才会发送通知。 </p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>问题</p> </td> 
   <td> <p>问题添加</p> </td> 
   <td> <p>项目团队成员</p> </td> 
   <td> <p>在添加问题之后，发送电子邮件给团队。</p> <p>在将问题添加到项目时，项目中的用户会收到电子邮件通知。</p> <p>仅当项目状态为“当前”时，才会发送通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>问题</p> </td> 
   <td> <p>问题完成</p> </td> 
   <td> <p>项目团队成员</p> </td> 
   <td> <p>在完成问题之后，发送电子邮件给团队。</p> <p>项目中的任何用户都会收到通知。</p> <p>仅当项目状态为“当前”或“计划”时，才会发送通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务</p> </td> 
   <td> <p>里程碑任务完成</p> </td> 
   <td> <p>项目团队成员</p> </td> 
   <td> <p>在完成里程碑任务之后，发送电子邮件给团队。</p> <p>当里程碑任务完成后，项目团队中的所有用户都会收到通知。 </p> <p>仅当项目状态为“当前”或“计划”时，才会发送通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>项目</p> </td> 
   <td> <p>项目完成</p> </td> 
   <td> <p>项目团队成员</p> </td> 
   <td> <p>在完成项目之后，发送电子邮件给团队。</p> <p>当项目状态为完成时，项目团队中的用户会收到电子邮件通知。</p> <p>提示：如果项目定期完成，则启用此选项可能会为在许多项目上任务数量有限的用户创建大量电子邮件。 </p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>项目</p> </td> 
   <td> <p>项目状态更改</p> </td> 
   <td> <p>项目团队成员</p> </td> 
   <td> <p>当项目状态更改时，发送电子邮件给团队。</p> <p>当项目状态更改时，项目团队中的用户会收到电子邮件通知。 </p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>项目用户</p> </td> 
   <td> <p>添加项目用户</p> </td> 
   <td> <p>项目团队成员</p> </td> 
   <td> <p>我被添加到一个项目。</p> <p>添加到项目的用户会在添加时收到电子邮件通知，除非该用户已自行添加到项目中。</p> <p>仅当项目状态为“当前”时，才会发送通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务</p> </td> 
   <td> <p>任务完成</p> </td> 
   <td> <p>项目团队成员</p> </td> 
   <td> <p>在完成任务之后，发送电子邮件给团队。</p> <p>项目团队成员会收到电子邮件通知。</p> <p>仅当项目状态为“当前”时，才会发送通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>问题</p> </td> 
   <td> <p>已添加未分配问题</p> </td> 
   <td> <p>项目团队成员</p> </td> 
   <td> <p>在添加未分配问题之后，发送电子邮件给团队。</p> <p>将未分配的问题添加到项目时，项目用户会收到电子邮件通知。</p> <p>仅当项目状态为“当前”时，才会发送通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
 </tbody> 
</table>

## 有关我拥有的项目的信息

另请参阅 [通知：关于我拥有的项目的信息](../../../workfront-basics/using-notifications/notifications-information-about-projects-i-own.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>对象类型</th> 
   <th>事件</th> 
   <th>收件人</th> 
   <th>描述</th> 
   <th> 默认状态</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>文档</p> </td> 
   <td> <p>文档添加</p> </td> 
   <td> <p>项目所有者</p> </td> 
   <td> <p>在添加文档之后，发送电子邮件给项目所有者。</p> <p>将文档添加到项目时，项目所有者会收到电子邮件通知，除非添加该文档的用户也是项目所有者。</p> <p>仅当项目状态为“当前”且文档不是“专用”时，才会发送通知。</p> <p>拥有“Light”或“Review”许可证的用户不会收到通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>问题</p> </td> 
   <td> <p>问题添加</p> </td> 
   <td> <p>项目所有者</p> </td> 
   <td> <p>在添加问题之后，发送电子邮件给项目。</p> <p>在将问题添加到项目时，项目所有者会收到电子邮件通知。</p> <p>仅当项目状态为“当前”或“计划”时，才会发送通知。</p> <p>拥有“Light”或“Review”许可证的用户不会收到通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>问题</p> </td> 
   <td> <p>问题提交日期更改</p> </td> 
   <td> <p>项目所有者</p> </td> 
   <td> <p>当问题的提交日期改变时，向项目所有者发送电子邮件。</p> <p>当项目问题的提交日期更改时，项目所有者会收到电子邮件通知，除非更改提交日期的用户与项目所有者是同一用户。</p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>问题</p> </td> 
   <td> <p>问题完成</p> </td> 
   <td> <p>项目所有者</p> </td> 
   <td> <p>在完成问题之后，发送电子邮件给项目所有者。</p> <p>项目所有者会收到电子邮件通知。</p> <p>仅当项目状态为“当前”或“计划”时，才会发送通知。</p> <p>拥有“Light”或“Review”许可证的用户不会收到通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务</p> </td> 
   <td> <p>里程碑任务完成</p> </td> 
   <td> <p>项目所有者</p> </td> 
   <td> <p>在完成里程碑任务之后，发送电子邮件给团队。</p> <p>仅当项目状态为“当前”或“计划”时，才会发送通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>项目</p> </td> 
   <td> <p>项目所有者工作</p> </td> 
   <td> <p>项目所有者</p> </td> 
   <td> <p>当项目所有者更改或项目创建时，发送电子邮件给新分派所有者。</p> <p>当用户被指定为项目所有者时，该用户会收到电子邮件通知。</p> <p>如果项目所有者是进行分配的同一个用户，则不会发送电子邮件通知</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>项目</p> </td> 
   <td> <p>项目进度更改</p> </td> 
   <td> <p>项目所有者</p> </td> 
   <td> <p>我拥有的一个项目落在了后面。</p> <p>当项目进度落后时，项目所有者会收到电子邮件通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务</p> </td> 
   <td> <p>任务提交日期更改</p> </td> 
   <td> <p>项目所有者</p> </td> 
   <td> <p>当任务的提交日期改变时，向项目所有者发送电子邮件。</p> <p>当项目上任务的提交日期更改时，项目所有者会收到电子邮件通知，除非更改提交日期的用户也是项目所有者。</p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务</p> </td> 
   <td> <p>任务完成</p> </td> 
   <td> <p>项目所有者</p> </td> 
   <td> <p>在完成任务之后，发送电子邮件给项目所有者。</p> <p>项目所有者会收到通知。 </p> <p>仅当项目状态为“当前”时，才会发送通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务</p> </td> 
   <td> <p>任务进度更改</p> </td> 
   <td> <p>项目所有者</p> </td> 
   <td> <p>当任务从正进度状态（按时）更改为负进度状态（延迟）时，发送电子邮件给项目所有者。</p> <p>当项目中的任务落后于计划时，项目所有者会收到电子邮件通知。</p> <p>仅当项目状态为“当前”时，才会发送通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>问题</p> </td> 
   <td> <p>未分配问题添加</p> </td> 
   <td> <p>项目所有者</p> </td> 
   <td> <p>在添加未分配问题之后，发送电子邮件给项目所有者。</p> <p>当未分配的问题添加到项目时，项目所有者会收到电子邮件通知。</p> <p>仅当项目状态为“当前”或“计划”时，才会发送通知。</p> <p>拥有“Light”或“Review”许可证的用户不会收到通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
 </tbody> 
</table>

## 关于我赞助的项目的信息

另请参阅 [通知：关于我赞助的项目的信息](../../../workfront-basics/using-notifications/notifications-information-about-projects-i-sponsor.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>对象类型</th> 
   <th>事件</th> 
   <th>收件人</th> 
   <th>描述</th> 
   <th> 默认状态</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>文档</p> </td> 
   <td> <p>文档添加</p> </td> 
   <td> <p>项目赞助者</p> </td> 
   <td> <p>在添加文档之后，发送电子邮件给项目发起人。</p> <p>在将文档添加到项目时，项目发起人会收到电子邮件通知，除非该文档由项目发起人添加。</p> <p>仅当项目状态为“当前”且文档不是“专用”时，才会发送通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>问题</p> </td> 
   <td> <p>问题添加</p> </td> 
   <td> <p>项目赞助者</p> </td> 
   <td> <p>在添加问题之后，发送电子邮件给项目发起人。</p> <p>在将问题添加到项目时，项目发起人会收到电子邮件通知。</p> <p>仅当项目状态为“当前”或“计划”时，才会发送通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>问题</p> </td> 
   <td> <p>问题完成</p> </td> 
   <td> <p>项目赞助者</p> </td> 
   <td> <p>在完成问题之后，发送电子邮件给项目发起人。</p> <p>项目发起人会收到电子邮件通知。</p> <p>仅当项目状态为“当前”或“计划”时，才会发送通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务</p> </td> 
   <td> <p>里程碑任务完成</p> </td> 
   <td> <p>项目赞助者</p> </td> 
   <td> <p>在完成里程碑任务之后，发送电子邮件给项目发起人。</p> <p>项目发起人在其发起的项目上完成里程碑任务时会收到电子邮件通知。</p> <p>仅当项目状态为“当前”或“计划”时，才会发送通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>项目</p> </td> 
   <td> <p>项目进度更改</p> </td> 
   <td> <p>项目赞助者</p> </td> 
   <td> <p>我赞助的项目落后。</p> <p>当项目进度落后时，项目发起人会收到电子邮件通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>项目</p> </td> 
   <td> <p>项目发起人工作</p> </td> 
   <td> <p>项目赞助者</p> </td> 
   <td> <p>当项目赞助者更改或项目创建时，发送电子邮件给新分派赞助者。</p> <p>当项目发起人设置为项目发起人时，项目发起人会收到电子邮件通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务</p> </td> 
   <td> <p>任务完成</p> </td> 
   <td> <p>项目赞助者</p> </td> 
   <td> <p>在完成任务之后，发送电子邮件给项目发起人。</p> <p>项目发起人会收到电子邮件通知。</p> <p>仅当项目状态为“当前”时，才会发送通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务</p> </td> 
   <td> <p>任务进度更改</p> </td> 
   <td> <p>项目赞助者</p> </td> 
   <td> <p>当任务从正进度状态（按时）更改为负进度状态（延迟）时，发送电子邮件给项目发起人。</p> <p>当项目中的任务落后于预定计划时，项目发起人会收到电子邮件通知。</p> <p>仅当项目状态为“当前”时，才会发送通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>问题</p> </td> 
   <td> <p>未分配问题添加</p> </td> 
   <td> <p>项目赞助者</p> </td> 
   <td> <p>在添加未分配问题之后，发送电子邮件给项目发起人。</p> <p>当未分配的问题添加到项目时，项目发起人会收到电子邮件通知。</p> <p>仅当项目状态为“当前”或“计划”时，才会发送通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
 </tbody> 
</table>

## 其他信息

另请参阅 [通知：其他信息](../../../workfront-basics/using-notifications/notifications-misc-information.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>对象类型</th> 
   <th>事件</th> 
   <th>收件人</th> 
   <th>描述</th> 
   <th> 默认状态</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>公告</td> 
   <td> <p>已添加公告</p> </td> 
   <td> <p></p> </td> 
   <td> <p>将向公告中心发送一条消息。</p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>文档</p> </td> 
   <td> <p>文档请求取消</p> </td> 
   <td> <p>请求该文档的用户</p> </td> 
   <td> <p>取消我发送的文档上传请求。</p> <p>文档请求被取消时，文档请求者会收到电子邮件通知。</p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>错误通知</p> </td> 
   <td> <p></p> </td> 
   <td> <p>发现需要您注意的错误。</p> <p>Workfront尝试连接到POP帐户失败后，会生成电子邮件通知。 尝试25次后，Workfront会禁用与POP帐户的连接以保留资源，并会发送通知。 </p> <p>如果POP电子邮件与请求队列关联，则电子邮件通知将发送给项目所有者；如果POP帐户与电子邮件设置中的“接收邮件”功能关联，则电子邮件通知将发送给Workfront管理员。
   </p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>问题</p> </td> 
   <td> <p>问题分配</p> </td> 
   <td> <p>资源所有者</p> </td> 
   <td> <p>问题分配更改影响了我的一名人员。</p> <p>当更改影响被分配人管理的用户时，问题被分配人管理器会收到电子邮件通知。</p> <p>仅当项目状态为“当前”或“计划”时，才会发送通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>用户</p> </td> 
   <td> <p>新建用户</p> </td> 
   <td> <p>用户</p> </td> 
   <td> <p>在Workfront中创建新用户时，发送电子邮件给用户。</p> <p>创建新用户后，该用户会收到电子邮件邀请，通知他们已创建Workfront帐户，并提示他们设置密码。</p> <p>创建新用户时，用户可以选择“向此人发送邀请电子邮件”选项（如中所述） <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">添加用户</a><span style="font-weight: 400;">)。 但是，全局启用“新用户至用户”选项后，无论是否选择“向此人发送邀请电子邮件”选项，所有新用户都会收到电子邮件邀请。</span></p> </td> 
   <td> 非活动 </td> 
  </tr> 
  <tr> 
   <td> <p>团队</p> </td> 
   <td> <p>对象共享</p> </td> 
   <td> <p>共享该对象的团队成员</p> </td> 
   <td> <p>有人与我的团队共享对象。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>用户</p> </td> 
   <td> <p>对象共享</p> </td> 
   <td> <p>与对象共享的用户</p> </td> 
   <td> <p>有人与我共享对象。</p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>项目用户</p> </td> 
   <td> <p>添加项目用户</p> </td> 
   <td> <p>资源所有者</p> </td> 
   <td> <p>我的一个人员已添加到项目中。</p> <p>当经理的其中一个直接报告添加到项目时，经理会收到电子邮件通知。</p> <p>拥有“Light”或“Review”许可证的用户不会收到通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>项目</p> </td> 
   <td> <p>“项目添加”到“项目组合或项目群”</p> </td> 
   <td> <p>Portfolio或项目群所有者</p> </td> 
   <td> <p>有人将项目添加到我拥有的项目组合或程序。</p> </td> 
   <td> <p>活动</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务</p> </td> 
   <td> <p>任务分派</p> </td> 
   <td> <p>资源所有者</p> </td> 
   <td> <p>任务分配更改影响了我的一名人员。</p> <p>任务受让人的经理会收到电子邮件通知。</p> <p>仅当项目状态为“当前”时，才会发送通知。</p> </td> 
   <td> <p>非活动</p> </td> 
  </tr> 
  <tr> 
   <td> 项目 <br>任务 <br>问题</td> 
   <td>新建更新</td> 
   <td>订阅者 </td> 
   <td> <p class="p1"><span class="s1 wysiwyg-font-size-medium">向我订阅的任务、问题或项目进行更新时会发送电子邮件。</span> </p> </td> 
   <td>活动</td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: from Error notification above: 
      
       <br>For more information on how to associate a request queue with a POP account, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.
       For more information on how to enable a POP account for incoming mail, see .
      -->

## 委派

另请参阅 [通知：委派](../../../workfront-basics/using-notifications/notifications-delegation.md).

| 对象类型 | 事件 | 收件人 | 描述 | 默认状态 |
|------------------|------|---------------------------------------------|--------------------------------------------------------------|---------------|
| 任务和问题 | 任务和问题委派 | 被分派人 | 我委派我的任务和问题（确认） | 活动 |
| 任务和问题 | 停止任务和问题委派 | 被分派人 | 我停止委派我的任务和问题（确认） | 活动 |
| 任务和问题 | 任务和问题委派 | 委派 | 有人将其任务和问题委派给我 | 活动 |
| 任务和问题 | 停止任务和问题委派 | 委派 | 有人停止将其任务和问题委派给我 | 活动 |
