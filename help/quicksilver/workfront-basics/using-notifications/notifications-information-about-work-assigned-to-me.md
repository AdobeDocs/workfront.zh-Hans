---
content-type: reference
navigation-topic: notifications
title: '通知：有关分配给我的工作的信息'
description: 以下通知会提醒您有关分配给您的工作项上发生的活动。
author: Lisa
feature: Get Started with Workfront
exl-id: 5d7fdee8-cb5c-4ab8-bec3-beff9851b8f6
source-git-commit: 901605917347297a1ee077f00905b03427582650
workflow-type: tm+mt
source-wordcount: '2090'
ht-degree: 6%

---

# 通知：有关分配给我的工作的信息

以下通知会提醒您有关分配给您的工作项上发生的活动。

有关配置您收到的通知的信息，请参阅 [激活或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

另请参阅 [事件通知](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th> <p>包含的字段 </p> <p> *仅每日摘要字段</p> </th> 
   <th>默认状态</th> 
  </tr> 
 </thead> 
 <tbody>
  <tr> 
   <td> <p><strong>已完成分配到我团队中任务的某个前置任务</strong> </p> <p>当其任务的前置任务完成时，分配的团队会收到电子邮件通知。 </p> <p>拥有[！UICONTROL Review]或[！UICONTROL Requestor]许可证的用户不会收到通知。</p> <p>即时通知电子邮件的主题是： <em>完成： &lt;task name=""&gt;</em></p> <p> 每日摘要通知的主题是： <em> [！UICONTROL分配给您的工作摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>前置任务名称<br>前置任务项目<br>前置任务参考号<br>完成前置任务的用户的名称<br>前置任务状态<br>前置任务完成的日期和时间<br>前置任务的前一状态<br><strong>查看更多详细信息</strong> 按钮<br>*项目名称<br>*项目参考号<br>*已完成的前置任务总数<br>*任务名称<br>*完成任务的用户的名称<br>*每日摘要日期 </p> </td> 
   <td><strong>每日</strong> </td>
  </tr>
  <tr> 
   <td> <p><strong>在完成任务之后，通过电子邮件向主分派用户发送所有依赖任务</strong> </p> <p>当任务被分派人的任务之一的前置任务完成时，任务被分派人会收到电子邮件通知。 </p> <p>拥有[！UICONTROL Review]或[！UICONTROL Requestor]许可证的用户不会收到通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL完成]： &lt;task name=""&gt;</em></p> <p> 每日摘要通知的主题是： <em> [！UICONTROL分配给您的工作摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>前置任务名称<br>前置任务项目<br>前置任务参考号<br>完成前置任务的用户的名称<br>前置任务状态<br>前置任务完成的日期和时间<br>前置任务的前一状态<br><strong>[！UICONTROL查看更多详细信息]</strong> 按钮<br>*项目名称<br>*项目参考号<br>*已完成的前置任务总数<br>*任务名称<br>*完成任务的用户的名称<br>*每日摘要日期 </p> </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <!--
  <tr data-mc-conditions=""> 
   <td> <p><strong>A predecessor of one of my tasks is completed</strong> </p> <p>The task assignee receives an email notification when a predecessor of one of their tasks is completed. </p> <p>Users with a [!UICONTROL Review] or [!UICONTROL Requestor] license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Complete]: &lt;Task Name></em></p> <p> The subject of the daily digest notification is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest> </em></p> </td> 
   <td> <p>Assigned by</p> <p>Task Name</p> <p>[!UICONTROL View] button</p> <p>Parent tasks</p> <p>Assignees</p> <p>Task status</p> <p>Task description</p> <p>Task Reference Number</p> <p> <br>Completed predecessor tasks </p> <p>Name of the user who completed the predecessor task<br>Date when the predecessor was completed</p> <p>[!UICONTROL View] button<br>Option to add to the daily digest</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  -->
  <tr> 
   <td> <p><strong>在批准或拒绝批准任务之后，发送电子邮件给分派用户</strong> </p> <p>任务被分派人在任务被批准或拒绝时收到电子邮件通知。</p> <p>仅当项目状态为“当前”时，才会发送通知。</p> <p>拥有[！UICONTROL Review]或[！UICONTROL Requestor]许可证的用户不会收到通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL完成]： &lt;task name=""&gt; 日期 &lt;project name=""&gt;</em></p> <p> 每日摘要通知的主题是： <em> [！UICONTROL分配给您的工作摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 任务名称<br>项目名称<br>任务参考号<br>授予批准的用户的名称<br>新任务状态<br>批准或拒绝任务的日期和时间<br>上一个任务状态<br><strong>[！UICONTROL查看更多详细信息]</strong> 按钮<br>*项目名称<br>*项目参考号<br>*批准或拒绝的任务总数<br>*任务名称<br>*批准或拒绝任务的用户的名称<br>*批准决定（[！UICONTROL已批准]/[！UICONTROL已拒绝]）<br>*每日摘要的日期<br></td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p id="a-task-i-m-assigned-to-is-completed"><strong>在完成任务之后，发送电子邮件给分派用户</strong> </p> <p>任务被分派人在任务完成时收到电子邮件通知。</p> <p>仅当项目状态为[！UICONTROL当前]时，才会发送通知。</p> <p>拥有[！UICONTROL Review]或[！UICONTROL Requestor]许可证的用户不会收到通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL完成]： &lt;task name=""&gt; 日期 &lt;project name=""&gt;</em></p> <p> <p>注意：如果任务更改为等同于[！UICONTROL完成]的状态，则电子邮件主题仍显示“完成”。</p> </p> <p> 每日摘要通知的主题是： <em> [！UICONTROL分配给您的工作摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>任务名称<br>项目名称<br>任务参考号<br>完成任务的用户的名称<br>完成任务的日期和时间<br>上一个任务状态<br><strong>[！UICONTROL查看更多详细信息]</strong> 按钮<br>*项目名称<br>*项目参考号<br>*已完成任务的总数<br>*任务名称<br>*完成任务的用户的名称<br>*每日摘要的日期<br></p> </td> 
   <td><strong>每日</strong> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><strong>已完成分配到我团队中任务的所有前置任务</strong> </p> <p>当分配团队中某个任务的前置任务被标记为完成时，分配团队会收到电子邮件通知。</p> <p>具有“审阅”或“请求者”许可证的用户不会收到通知。</p> <p>即时通知电子邮件的主题是： <em>任务完成： &lt;name&gt;</em></p> <p> 每日摘要通知的主题是： <em> 分配给您的工作的摘要 &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 任务名称<br>任务项目<br>任务参考号<br>完成前置任务的用户的名称<br>前置任务状态<br>前置任务完成的日期和时间<br>前置任务的前一状态<br><strong>查看更多详细信息</strong> 按钮<br>*项目名称<br>*项目参考号<br>*已完成任务的总数<br>*任务名称<br>*完成任务的用户的名称<br>*每日摘要日期 </td>
   <td><strong>即时</strong> </td> 
  </tr>
  <!--
  <tr data-mc-conditions=""> 
   <td> <p><strong>All predecessors of a task assigned to my team are completed</strong> </p> <p>The assigned team receives an email notification when a predecessor of one of their tasks is marked complete.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Task Complete: &lt;Name&gt;</em></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>Assigned by</p> <p>Task Name</p> <p>View button</p> <p>Parent tasks</p> <p>Assignees</p> <p>Task status</p> <p>Task description</p> <p>Task Reference Number</p> <p> <br>Completed predecessor tasks </p> <p>Name of the user who completed the predecessor task<br>Date when the predecessor was completed</p> <p>View button<br>Option to add to the daily digest<br></p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p><strong>All predecessors of a task assigned to my team are completed</strong> </p> <p>The team assigned receives an email notification for each predecessor that is marked complete. </p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Complete: &lt;Task Name&gt;</em><br></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
    <td> Task Name<br>Task Project<br>Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </td> 
    <td><strong>Instant</strong> </td> 
   </tr>
  --> 
  <tr> 
   <td> <p><strong>在所有前置任务完成之后，通过电子邮件向主分派用户发送所有依赖任务</strong> </p> <p>任务被分派人会收到每个已完成前置任务的电子邮件通知。</p> <p>拥有[！UICONTROL Review]或[！UICONTROL Requestor]许可证的用户不会收到通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL完成]： &lt;task name=""&gt;</em><br></p> <p> 每日摘要通知的主题是： <em> [！UICONTROL分配给您的工作摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 任务名称<br>任务项目<br>任务参考号<br>完成前置任务的用户的名称<br>前置任务状态<br>前置任务完成的日期和时间<br>前置任务的前一状态<br><strong>[！UICONTROL查看更多详细信息]</strong> 按钮<br>*项目名称<br>*项目参考号<br>*已完成任务的总数<br>*任务名称<br>*完成任务的用户的名称<br>*每日摘要日期 </td> 
   <td><strong>即时</strong> </td> 
  </tr>
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p><strong>All predecessors of my tasks are completed</strong> </p> <p>The task assignee receives an email notification for each predecessor that is completed.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Complete: &lt;Task Name&gt;</em><br></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
    <td> Task Name<br>Task Project<br>Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </td> 
    <td><strong>Instant</strong> </td> 
   </tr>
  --> 
  <tr> 
   <td> <p><strong>在批准或拒绝问题之后，向被分派的用户发送电子邮件</strong> </p> <p>当做出批准决定（批准或拒绝）时，问题的被分派人会收到电子邮件通知。</p> <p>拥有[！UICONTROL Review]或[！UICONTROL Requestor]许可证的用户不会收到通知。</p> <p>即时通知电子邮件的主题是： <em>未决批准问题： &lt;planned start="" date=""&gt; &lt;issue reference="" number=""&gt; - &lt;issue name=""&gt; 在 &lt;project name=""&gt;</em></p> <p> 每日摘要通知的主题是： <em> 分配给您的工作的摘要 &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 问题名称<br>项目名称<br>问题参考号<br>批准或拒绝问题的用户的名称<br>批准决定（已批准或已拒绝）<br>问题状态<br>请求审批的用户的名称<br><strong>[！UICONTROL查看更多详细信息]</strong> 按钮<br>*项目名称<br>*项目参考号<br>*批准或拒绝的问题总数<br>*问题名称<br>*批准或拒绝问题的用户的名称<br>*批准决定（已批准或已拒绝）<br>*每日摘要的日期<br></td> 
   <td><strong>每日</strong> </td> 
  </tr>
  <tr> 
   <td> <p><strong>在完成问题之后，发送电子邮件给分派用户</strong> </p> <p>仅当项目状态为[！UICONTROL当前]或[！UICONTROL规划]时，才会发送通知。</p> <p>拥有[！UICONTROL Review]或[！UICONTROL Requestor]许可证的用户不会收到通知。</p> <p>即时通知电子邮件的主题是： <em>完成： &lt;issue name=""&gt; 日期 &lt;project name=""&gt;</em></p> <p><em> 每日摘要通知的主题是：分配给您的工作的摘要 &lt;date of="" daily="" digest=""&gt; </em> </p> </td> 
   <td> 问题名称<br>项目名称<br>问题参考号<br>完成问题的用户的名称<br>新问题状态<br>问题完成的日期和时间<br>上一个任务状态<br><strong>[！UICONTROL查看更多详细信息]</strong> 按钮<br>*项目名称<br>*项目参考号<br>*已完成的问题总数<br>*问题名称<br>*完成问题的用户的名称<br>*每日摘要的日期<br></td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在我的请求下上传或更改文档</strong> </p> <p>问题被分派人在上传文档或在其添加的问题上更改文档详细信息时收到电子邮件通知。</p> <p>如果触发问题的用户是问题受分配人，则不会发送电子邮件通知。</p> <p>仅当项目状态为[！UICONTROL当前]并且项目设置为帮助请求队列时（如中所述），才会发送通知 <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">创建请求队列</a>)。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL文档已添加到] &lt;request name=""&gt;</em></p> <p> 每日摘要通知的主题是： <em> [！UICONTROL分配给您的工作摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>请求名称<br>项目名称（请求队列名称）<br>文档参考号 <br>上传文档的用户的名称<br>文档名称 <br>添加日期<br>文档详细信息（格式、大小、版本号）<br>文档缩略图<br><strong>[！UICONTROL预览]</strong> 和 <strong>[！UICONTROL下载]</strong> 按钮<br>*项目名称<br>*项目参考号<br>*上传或更改的文档总数<br>*文档名称<br>*对象名称<br>*上传文档的用户的名称<br>*每日摘要日期</p> </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>当任务的计划完成日期改变时，向被分派的用户发送电子邮件</strong> </p> <p>当任务的[！UICONTROL规划完成日期]发生更改时，任务被分配人会收到电子邮件通知，除非更改规划完成日期的用户同时也是任务被分配人。</p> <p>仅当项目状态不是[！UICONTROL Planning]时，才发送通知。</p> <p>不会发送有关个人任务的通知。</p> <p> 具有“审阅”或“请求者”许可证的用户不会收到通知。 </p> <p> 即时通知电子邮件的主题是： <em>[！UICONTROL到期日期已更改。]</em></p> <p> 每日摘要通知的主题是： <em> [！UICONTROL分配给您的工作摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 任务名称<br>项目名称<br>任务参考号<br>新到期日期（[！UICONTROL计划完成日期]）<br>更改到期日期的日期和时间<br>更改到期日期的用户的名称<br>*项目名称<br>*项目参考号<br>*到期日期（计划完成日期）发生更改的任务总数<br>*任务名称<br>*新的计划完成日期<br>*更改到期日期的用户名称<br>*每日摘要日期 </td> 
   <td> <p><strong>即时</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>当问题的计划完成日期改变时，向被分派的用户发送电子邮件</strong> </p> <p>问题被分配人在[！UICONTROL规划完成日期]发生更改时收到电子邮件通知，除非更改[！UICONTROL规划完成日期]的用户也是被分配人。</p> <p>仅当项目状态不是[！UICONTROL Planning]时，才发送通知。</p> <p>拥有[！UICONTROL Review]或[！UICONTROL Requestor]许可证的用户不会收到通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL到期日期已更改]</em></p> <p> </p> <p> 每日摘要通知的主题是： <em> [！UICONTROL分配给您的工作摘要] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>问题名称<br>项目名称<br>问题参考号<br>新到期日期（[！UICONTROL计划完成日期]）<br>更改到期日期的日期和时间<br>更改到期日期的用户的名称<br>*项目名称<br>*项目参考号<br>*到期日期（[！UICONTROL规划完成日期]）发生更改的问题总数<br>*问题名称<br>*新的[！UICONTROL计划完成日期]<br>*更改到期日期的用户名称<br>*每日摘要的日期<br></p> </td> 
   <td> <p><strong>即时</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>有关我已分配到的任务的状态已更改</strong> <p>任务状态更改时，任务被分派人会收到电子邮件通知，除非更改状态的用户也是被分派人。</p> <p>注意：当任务状态更改为完成时，不会发送此通知。 已完成的任务会使用单独的通知。 参见 <a href="#a-task-i-m-assigned-to-is-completed" class="MCXref xref">在完成任务之后，发送电子邮件给分派用户</a>，在上。</p> <p>仅当项目状态为[！UICONTROL当前]时，才会发送通知。</p> <p>拥有[！UICONTROL Review]或[！UICONTROL Requestor]许可证的用户不会收到通知。</p> <p>即时通知电子邮件的主题是： <em>&lt;task name=""&gt; 起始日期 &lt;project name=""&gt; 是 &lt;new status=""&gt;</em></p> <p> </p> <p> 每日摘要通知的主题是： <em> [！UICONTROL分配给您的工作摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 任务名称<br>项目名称<br>任务参考号<br>更改状态的用户的名称<br>新状态<br>状态更改的日期和时间<br>预览状态<br><strong>[！UICONTROL查看更多详细信息]</strong> 按钮<br>*项目名称<br>*项目参考号<br>*状态更改的任务总数<br>*任务名称<br>*上一个任务状态<br>*新任务状态<br>*更改了状态的用户的名称<br>*每日摘要的日期<br></td> 
   <td><strong>[！UICONTROL日报]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我所工作的一个项目的状态发生了变化</strong> </p> <p>除非您自己更改状态，否则当分配至您的问题的状态发生更改时，您将收到电子邮件通知。 </p> <p>仅当项目状态为[！UICONTROL当前]时，才会发送通知。</p> <p>拥有[！UICONTROL Review]或[！UICONTROL Requestor]许可证的用户不会收到通知。</p> <p>即时通知电子邮件的主题是： <em>&lt;issue name=""&gt; 起始日期 &lt;project name=""&gt; 是 &lt;new status=""&gt;</em></p> <p> 每日摘要通知的主题是： <em> [！UICONTROL分配给您的工作摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 问题名称<br>项目名称<br>问题参考号<br>更改状态的用户的名称<br>新状态<br>状态更改的日期和时间<br>上一个问题状态<br><strong>查看更多详细信息</strong> 按钮<br>*项目名称<br>*项目参考号<br>*状态更改的问题总数<br>*任务名称<br>*上一个问题状态<br>*新问题状态<br>*更改了状态的用户的名称<br>*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
 </tbody> 
</table>
