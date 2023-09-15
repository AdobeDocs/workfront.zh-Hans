---
content-type: reference
navigation-topic: notifications
title: '通知：关于我赞助的项目的信息'
description: 以下通知会提醒您正在赞助的项目中发生的活动。
author: Lisa
feature: Get Started with Workfront
exl-id: b4c7c046-f15f-4e6e-9332-5232c7b7080b
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1314'
ht-degree: 6%

---

# 通知：关于我赞助的项目的信息

以下通知会提醒您正在赞助的项目中发生的活动。

有关配置接收哪些通知的信息，请参阅 [修改您自己的电子邮件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>在添加文档之后，发送电子邮件给项目发起人。</strong> </p> <p>在将文档添加到项目时，项目发起人会收到电子邮件通知。</p> <p>仅当项目状态为[！UICONTROL当前]且文档不是[！UICONTROL专用]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL文档已添加到] &lt;project name=""&gt;</em></p> <p>每日摘要通知的主题是：<em> [！UICONTROL您赞助的项目摘要] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 项目名称<br>Portfolio名称<br>文档参考号<br>添加文档的用户的名称<br>文档名称<br>添加日期<br>文档详细信息（格式、大小、版本号）<br>文档缩略图<br><strong>[！UICONTROL预览]</strong> 和 <strong>[！UICONTROL下载]</strong> 按钮<br>*项目名称<br>*项目参考号<br>*添加的文档总数<br>*文档名称<br>*添加文档的用户的名称<br>*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在完成里程碑任务之后，发送电子邮件给项目发起人。</strong> </p> <p>当项目发起人发起的项目中的里程碑任务完成后，项目发起人会收到电子邮件通知。</p> <p>仅当项目状态为[！UICONTROL当前]或[！UICONTROL计划]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL完成]： &lt;task name=""&gt; 日期 &lt;project name=""&gt;</em></p> <p>注意：如果任务更改为等于[！UICONTROL完成]的状态，则电子邮件主题仍显示“[！UICONTROL完成]”。<br></p> <p>每日摘要通知的主题是：<em> 您赞助的项目的摘要 &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 任务名称<br>项目名称<br>任务参考号<br>完成任务的用户的名称<br>新任务状态<br>完成任务的日期和时间<br>上一个任务状态<br><strong>[！UICONTROL查看更多详细信息]</strong> 按钮 <br>*项目名称<br>*项目参考号<br>*已完成任务的总数<br>*任务名称<br>*完成任务的用户的名称<br>*每日摘要的日期<br></td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>当项目从正进度状态 (按时) 更改为负进度状态 (延迟) 时，发送电子邮件给项目发起人</strong> </p> <p>当项目进度落后时，项目发起人会收到电子邮件通知。 当进度状态为“[！UICONTROL存在风险]”或“[！UICONTROL存在问题]”时，项目落后于计划。</p> <p>拥有[！UICONTROL Review]许可证的用户不会收到通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL项目进度更改]： &lt;project name=""&gt;</em></p> <p>每日摘要通知的主题是： <em>[！UICONTROL您赞助的项目摘要] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 项目名称<br>Portfolio名称<br>项目参考号<br>项目进度状态<br>项目[！UICONTROL计划开始日期]<br>项目[！UICONTROL计划完成日期]<br>项目[！UICONTROL预计开始日期]<br>项目[！UICONTROL预计完成日期]<br>项目完成百分比<br>项目状态<br>项目所有者<br>*项目名称<br>*项目参考号<br>*项目进度状态<br>*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在完成一项任务之后，发送电子邮件给项目发起人</strong> </p> <p>项目发起人会收到电子邮件通知。</p> <p>仅当项目状态为[！UICONTROL当前]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL完成]： &lt;task name=""&gt; 日期 &lt;project name=""&gt;</em></p> <p> <p>注意：如果任务更改为等于[！UICONTROL完成]的状态，则电子邮件主题仍显示“[！UICONTROL完成]”。</p> </p> <p>每日摘要通知的主题是：<em> 您赞助的项目的摘要 &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 任务名称<br>项目名称<br>任务参考号<br>完成任务的用户的名称<br>任务状态<br>任务状态更改的日期和时间<br>上一个任务状态<br><strong>查看更多详细信息</strong> 按钮<br>*项目名称<br>*项目参考号<br>*已完成任务的总数<br>*任务名称<br>*完成任务的用户的名称<br>*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>当任务从正进度状态 (按时) 更改为负进度状态 (延迟) 时，发送电子邮件给项目发起人</strong> </p> <p>当项目中的任务落后于预定计划时，项目发起人会收到电子邮件通知。 当进度状态为“[！UICONTROL有风险]”、“[！UICONTROL落后]”或“[！UICONTROL延迟]”时，任务进度落后于计划。</p> <p>仅当项目状态为[！UICONTROL当前]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL任务进度更改]： &lt;task name=""&gt;</em></p> <p>每日摘要通知的主题是：<em> [！UICONTROL您赞助的项目摘要] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 任务名称<br>项目名称<br>任务参考号<br>新任务进度状态<br>任务[！UICONTROL计划开始日期]<br>任务[！UICONTROL计划完成日期]<br>任务[！UICONTROL预计开始日期]<br>任务[！UICONTROL预计完成日期]<br>任务完成百分比<br>任务状态<br>分派至姓名<br>按名称输入<br>*项目名称<br>*项目参考号<br>*晚于计划的任务总数<br>*任务名称<br>*输入任务的用户的名称<br>*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在添加问题之后，发送电子邮件给项目发起人。</strong> </p> <p>在将问题添加到项目时，项目发起人会收到电子邮件通知。</p> <p>仅当项目状态为[！UICONTROL当前]或[！UICONTROL计划]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL问题已添加到] &lt;project name=""&gt;</em></p> <p>每日摘要通知的主题是： <em>[！UICONTROL您赞助的项目摘要] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 项目名称<br>Portfolio名称<br>问题参考号<br>添加问题的用户的名称<br>问题名称<br>问题类型<br>输入日期<br>问题优先级<br>分派至姓名 <br>问题状态<br>主要联系人<br>*项目名称<br>*项目参考号<br>*添加到项目的问题总数<br>*问题名称<br>*分配给问题的用户的名称<br>*每日摘要的日期<br><br></td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在完成问题之后，发送电子邮件给项目发起人</strong> </p> <p>项目发起人会收到电子邮件通知。</p> <p>仅当项目状态为[！UICONTROL当前]或[！UICONTROL计划]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL完成]： &lt;issue name=""&gt; 日期 &lt;project name=""&gt;</em></p> <p>每日摘要通知的主题是：<em> 您赞助的项目的摘要 &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 问题名称<br>项目名称<br>问题参考号<br>完成问题的用户的名称<br>问题状态<br>完成问题的日期和时间<br>上一个问题状态<br><strong>查看更多详细信息</strong> 按钮<br>*项目名称<br>*项目参考号<br>*已完成的问题总数<br>*问题名称<br>*分配给问题的用户的名称<br>*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在添加未分派的问题之后，发送电子邮件给项目发起人。</strong> </p> <p>当未分配的问题添加到项目时，项目发起人会收到电子邮件通知。</p> <p>仅当项目状态为[！UICONTROL当前]或[！UICONTROL计划]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL应分派到]上的此新问题的用户 &lt;project name=""&gt;？</em></p> <p>每日摘要通知的主题是：<em> [！UICONTROL您赞助的项目摘要] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 项目名称<br>Portfolio名称<br>问题参考号<br>添加问题的用户的名称<br>问题名称<br>问题类型<br>输入日期<br>问题优先级<br>指定给名称（空）<br>问题状态<br>主要联系人<br>*项目名称<br>*项目参考号<br>*添加的问题总数<br>*问题名称<br>*添加问题的用户的名称<br>*每日摘要的日期<br></td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>当项目赞助者更改或项目创建时，发送电子邮件给新分派赞助者</strong> </p> <p>当项目发起人设置为项目发起人时，项目发起人会收到电子邮件通知。<br></p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL项目发起人]： &lt;project name=""&gt;</em></p> <p>电子邮件通知正文中包含以下文本：</p> <p><em>[！UICONTROL Hi] &lt;your name=""&gt;，</em> </p> <p><em>&lt;name of="" the="" user="" who="" assigned="" you="" as="" the="" project="" sponsor=""&gt; [！UICONTROL使您成为] &lt;project name=""&gt;. [！UICONTROL作为项目发起人，您可能会收到有关项目活动的其他电子邮件通知或参与审批与项目相关的工作。 祝您使用愉快。</em> </p> <p>每日摘要通知的主题是： <em>您赞助的项目的摘要 &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>项目名称<br>Portfolio名称<br>项目参考号<br>项目计划完成日期<br>*项目名称<br>*项目参考号<br>*每日摘要日期</p> </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
 </tbody> 
</table>
