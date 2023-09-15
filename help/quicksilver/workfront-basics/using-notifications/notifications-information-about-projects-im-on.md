---
content-type: reference
navigation-topic: notifications
title: “通知：关于我参与的项目的信息”
description: 以下通知提醒您正在处理的项目中发生的活动。
author: Lisa
feature: Get Started with Workfront
exl-id: c4cf84eb-8911-4bff-a548-7f0e6d8aa7b5
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1586'
ht-degree: 6%

---

# 通知：关于我参与的项目的信息

以下通知提醒您正在处理的项目中发生的活动。

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
   <td> <p><strong>我参与的项目添加了一个文档</strong> </p> <p>将文档添加到项目时，项目团队成员会收到电子邮件通知，但添加该文档的用户除外。</p> <p>仅当项目状态为[！UICONTROL当前]且文档不是“私有”时，才会发送通知。</p> <p>即时通知电子邮件的主题是 <em>[！UICONTROL文档已添加到] &lt;project name=""&gt;</em></p> <p>每日摘要通知的主题是 <em>[！UICONTROL您参与的项目摘要] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 项目名称<br>Portfolio名称<br>文档参考号<br>添加文档的用户的名称<br>文档名称<br>添加日期<br>文档详细信息（格式、大小、版本号）<br>文档缩略图<br><strong>[！UICONTROL预览]</strong> 和 <strong>[！UICONTROL下载]</strong> 按钮<br>*项目名称<br>*项目参考号<br>*添加的文档总数<br>*文档名称<br>*上传文档的用户的名称<br>*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我参与的项目中的一个里程碑任务已完成</strong> </p> <p>项目团队成员在项目中的里程碑任务完成时收到通知。 个人任务完成后，不会发送通知。</p> <p>仅当项目状态为[！UICONTROL当前]或[！UICONTROL计划]时，才会发送通知。</p> <p>主题行是 <em>[！UICONTROL完成]： &lt;task name=""&gt; 日期 &lt;project name=""&gt;</em></p> <p>每日摘要通知的主题是 <em> [！UICONTROL您参与的项目摘要] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 任务名称<br>项目名称<br>任务参考号<br>完成任务的用户的名称<br>任务状态<br>完成任务的日期和时间<br>上一个任务状态<br><strong>[！UICONTROL查看更多详细信息]</strong> 按钮 <br>*项目名称<br>*项目参考号<br>*已完成任务的总数<br>*任务名称<br>*完成任务的用户的名称<br>*每日摘要的日期<br></td> 
   <td><strong>[！UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我参与的一个项目成为活动状态</strong> </p> <p>当项目状态设置为[！UICONTROL当前]时，项目团队成员会收到电子邮件通知。</p> <p>注意：当项目状态设置为[！UICONTROL当前]时，用户必须在项目的“员工”选项卡上列出才能接收通知。 有关将用户添加到项目团队的信息，请参阅 <a href="../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">管理项目团队</a>.</p> <p>即时通知电子邮件的主题是 <em>&lt;project name=""&gt; [！UICONTROL是最新的 — 转到您的项目并查看您的任务！]</em></p> <p> 每日摘要通知的主题是 <em> [！UICONTROL您参与的项目摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>项目名称<br>Portfolio名称<br>项目参考号<br>项目状态<br>项目[！UICONTROL计划完成日期]<br>项目所有者<br>分配给您、工作角色或团队的任务列表<br><strong>[！UICONTROL查看更多详细信息]</strong> 按钮<br>*项目名称<br>*项目参考号<br>*项目状态<br>*每日摘要日期</p> </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>我的团队所处理的项目成为活动状态</strong> <p>当项目变为活动状态时，团队成员会收到电子邮件通知。 必须为团队分配至少一个任务才能接收通知。</p><p>如果单个用户和团队均被分配到项目中的任务，则。 团队将不会收到通知。</p><p>即时通知电子邮件的主题是 <i>&lt;project name=""&gt; [！UICONTROL处于活动状态 — 转到您的项目并查看您的任务！]</i></p><p>每日摘要通知的主题是 <em> [！UICONTROL您参与的项目摘要] &lt;date of="" daily="" digest=""&gt; </em></p></td> 
   <td>项目名称<br>Portfolio名称<br>项目参考号<br>项目状态<br>项目[！UICONTROL计划完成日期]<br>项目所有者<br>分配给您团队的任务列表<br><strong>[！UICONTROL查看更多详细信息]</strong> 按钮<br>*项目名称<br>*项目参考号<br>*项目状态<br>*每日摘要日期</td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我参与的一个项目已完成</strong> </p> <p>当项目状态为[！UICONTROL完成]时，项目团队成员会收到电子邮件通知。</p> <p>提示：如果项目定期完成，则启用此选项可能会为在许多项目上任务数量有限的用户创建大量电子邮件。</p> <p>即时通知电子邮件的主题是 <em>[！UICONTROL项目状态更改]： &lt;project name=""&gt;</em></p> <p> 每日摘要通知的主题是 <em> [！UICONTROL您参与的项目摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 项目名称<br>Portfolio名称<br>项目参考号<br>完成项目的用户的名称<br>项目状态<br>项目完成的日期和时间<br>上一个项目状态<br><strong>[！UICONTROL查看更多详细信息]</strong> 按钮<br>*项目名称<br>*项目参考号<br>*项目状态<br>*每日摘要的日期<br></td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我参与的项目中的一个任务已完成</strong> </p> <p>项目团队成员在其项目上完成任务后会收到电子邮件通知。 <br>有关项目团队的详细信息，请参阅 <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">项目团队概述</a>.</p> <p>仅当项目状态为[！UICONTROL当前]时，才会发送通知。</p> <p>即时通知电子邮件的主题是 <em>[！UICONTROL完成]： &lt;task name=""&gt; 日期 &lt;project name=""&gt;</em></p> <p> <p>注意：如果任务更改为等于[！UICONTROL完成]的状态，则电子邮件主题仍显示“[！UICONTROL完成]”。</p> </p> <p><em> 每日摘要通知的主题是：[！UICONTROL您参与的项目摘要] &lt;date of="" daily="" digest=""&gt; </em> </p> </td> 
   <td> <p>任务名称<br>项目名称<br>任务参考号<br>完成任务的用户的名称<br>任务状态<br>任务状态更改的日期和时间<br>上一个任务状态<br><strong>查看更多详细信息</strong> 按钮<br>*项目名称<br>*项目参考号<br>*已完成任务的总数<br>*任务名称<br>*完成任务的用户的名称<br>*每日摘要的日期<br></p> </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我参与的项目已添加一个问题</strong> </p> <p>在将问题添加到项目时，项目团队成员会收到电子邮件通知。</p> <p>仅当项目状态为“当前”时，才会发送通知。</p> <p>即时通知电子邮件的主题是 <em>[！UICONTROL问题已添加到] &lt;project name=""&gt;</em></p> <p> </p> <p> 每日摘要通知的主题是 <em> [！UICONTROL您参与的项目摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 项目名称<br>Portfolio名称<br>问题参考号<br>添加问题的用户的名称<br>问题类型<br>问题名称<br>输入日期<br>问题优先级<br>分派至姓名 <br>问题状态<br>主要联系人<br>*项目名称<br>*项目参考号<br>*添加到项目的问题总数<br>*问题名称<br>*分配给问题的用户的名称<br>*每日摘要日期 </td> 
   <td> <p><strong>即时</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我参与的一个项目已完成一个问题</strong> </p> <p>项目团队成员在其项目上完成某个问题后会收到电子邮件通知。<br>有关项目团队的详细信息，请参阅 <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">项目团队概述</a>.</p> <p>仅当项目状态为[！UICONTROL当前]或[！UICONTROL计划]时，才会发送通知。</p> <p>即时通知电子邮件的主题是 <em>[！UICONTROL完成]： &lt;issue name=""&gt; 日期 &lt;project name=""&gt;</em></p> <p> 每日摘要通知的主题是 <em> [！UICONTROL您参与的项目摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 问题名称<br>项目名称<br>完成问题的用户的名称<br>问题状态<br>完成问题的日期和时间<br>上一个问题状态<br><strong>[！UICONTROL查看更多详细信息]</strong> 按钮<br>*项目名称<br>*项目参考号<br>*已完成的问题总数<br>*问题名称<br>*分配给问题的用户的名称<br>*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我参与的项目添加了一个未分派问题</strong> </p> <p>将未分配的问题添加到项目后，项目团队成员会收到电子邮件通知。</p> <p>仅当项目状态为[！UICONTROL当前]时，才会发送通知。</p> <p>即时通知电子邮件的主题是 <em>[！UICONTROL应分派到]上的此新问题的用户 &lt;project name=""&gt;？</em></p> <p> 每日摘要通知的主题是 <em> [！UICONTROL您参与的项目摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 项目名称<br>Portfolio名称<br>问题参考号<br>添加问题的用户的名称<br>问题名称<br>问题类型<br>输入日期<br>问题优先级<br>指定给名称（空） <br>问题状态<br>主要联系人<br>*项目名称<br>*项目参考号<br>*添加的问题总数<br>*问题名称<br>*添加问题的用户的名称<br>*每日摘要的日期<br></td> 
   <td> <p><strong>即时</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我被添加到了一个项目</strong> </p> <p>添加到项目的用户会在添加时收到电子邮件通知，除非该用户将自己添加到项目中。</p> <p>仅当项目状态为[！UICONTROL当前]时，才会发送通知。</p> <p>即时通知电子邮件的主题是 <em>[！UICONTROL您已被添加到项目] &lt;project name=""&gt;</em></p> <p> 每日摘要通知的主题是 <em> [！UICONTROL您参与的项目摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>项目名称<br>Portfolio名称<br>项目参考号<br>将您添加到项目的用户的名称<br>项目[！UICONTROL计划开始日期]<br>项目[！UICONTROL计划完成日期]<br>项目完成百分比<br>项目中的其他人的姓名 <br>项目所有者<br><strong>查看更多详细信息</strong> 按钮<br>*项目名称<br>*项目参考号<br>*每日摘要日期</p> </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我参与的项目的状态更改了</strong> </p> <p>当项目状态更改时，项目团队成员会收到电子邮件通知。 <br>有关项目团队的详细信息，请参阅 <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">项目团队概述</a>.</p> <p>即时通知电子邮件的主题是 <em>[！UICONTROL项目状态更改]： &lt;project name=""&gt;</em></p> <p> 每日摘要通知的主题是 <em> [！UICONTROL您参与的项目摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 项目名称<br>Portfolio名称<br>项目参考号<br>更改项目状态的用户的名称<br>新建项目状态<br>项目状态更改的日期和时间<br>上一个项目状态<br><strong>[！UICONTROL查看更多详细信息]</strong> 按钮<br>*项目名称<br>*项目参考号<br>*项目状态<br>*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
 </tbody> 
</table>
