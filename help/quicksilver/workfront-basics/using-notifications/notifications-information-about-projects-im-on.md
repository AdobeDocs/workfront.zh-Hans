---
content-type: reference
navigation-topic: notifications
title: “通知：有关我正在执行的项目的信息”
description: 以下通知会提醒您正在处理的项目中发生的活动。
author: Lisa
feature: Get Started with Workfront
exl-id: c4cf84eb-8911-4bff-a548-7f0e6d8aa7b5
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1588'
ht-degree: 6%

---

# 通知：有关我正在执行的项目的信息

以下通知会提醒您正在处理的项目中发生的活动。

有关配置接收的通知的信息，请参阅 [激活或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

另请参阅 [事件通知](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th> <p>包含的字段 </p> <p> *仅限每日摘要字段</p> </th> 
   <th>默认状态</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>在添加文档之后，发送电子邮件给团队。</strong> </p> <p>在将文档添加到项目时，项目团队成员会收到一封电子邮件通知，添加文档的用户除外。</p> <p>仅当项目状态为[!UICONTROL当前]且文档不是私有时，才会发送通知。</p> <p>即时通知电子邮件的主题是 <em>[!UICONTROL文档已添加到] &lt;project name=""&gt;</em></p> <p>每日摘要通知的主题是 <em>[!UICONTROL Digest of Projects You On] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 项目名称<br>Portfolio名称<br>文档参考编号<br>添加文档的用户的名称<br>文档名称<br>添加日期<br>文档详细信息（格式、大小、版本号）<br>文档缩略图<br><strong>[!UICONTROL预览]</strong> 和 <strong>[!UICONTROL下载]</strong> 按钮<br>*项目名称<br>*项目参考编号<br>*添加的文档总数<br>*文档名称<br>*上传文档的用户名<br>*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在完成里程碑任务之后，发送电子邮件给团队。</strong> </p> <p>当项目上的里程碑任务完成时，项目团队成员会收到通知。 完成个人任务时不会发送通知。</p> <p>仅当项目状态为[!UICONTROL Current]或[!UICONTROL Planning]时，才会发送通知。</p> <p>主题行是 <em>[!UICONTROL Complete]: &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p>每日摘要通知的主题是 <em> [!UICONTROL Digest of Projects You On] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 任务名称<br>项目名称<br>任务参考编号<br>完成任务的用户的名称<br>任务状态<br>任务完成的日期和时间<br>上一任务状态<br><strong>[!UICONTROL请参阅更多详细信息]</strong> 按钮 <br>*项目名称<br>*项目参考编号<br>*完成的任务总数<br>*任务名称<br>*完成任务的用户名<br>*每日摘要的日期<br></td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>当项目状态从 idea/approved/rejected/requested/planning 更改为当前，发送电子邮件给团队</strong> </p> <p>当项目状态设置为[!UICONTROL Current]时，项目团队的成员会收到一封电子邮件通知。</p> <p>注意：当项目状态设置为[!UICONTROL Current]时，用户必须列在项目的“人员配备”选项卡上才能收到通知。 有关将用户添加到项目团队的信息，请参阅 <a href="../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">管理项目团队</a>.</p> <p>即时通知电子邮件的主题是 <em>&lt;project name=""&gt; [!UICONTROL为当前 — 转到您的项目并查看您的任务！]</em></p> <p> 每日摘要通知的主题是 <em> [!UICONTROL Digest of Projects You On] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>项目名称<br>Portfolio名称<br>项目参考编号<br>项目状态<br>项目[!UICONTROL计划完成日期]<br>项目所有者<br>分配给您、您的某个工作角色或您的某个团队的任务列表<br><strong>[!UICONTROL请参阅更多详细信息]</strong> 按钮<br>*项目名称<br>*项目参考编号<br>*项目状态<br>*每日摘要日期</p> </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>我的团队所处理的项目成为活动状态</strong> <p>当项目处于活动状态时，团队成员会收到一封电子邮件通知。 必须将团队分配给至少一个任务才能接收通知。</p><p>如果为单个用户和团队分配了项目上的任务。 团队将不会收到通知。</p><p>即时通知电子邮件的主题是 <i>&lt;project name=""&gt; [!UICONTROL处于活动状态 — 转到您的项目并查看您的任务！]</i></p><p>每日摘要通知的主题是 <em> [!UICONTROL Digest of Projects You On] &lt;date of="" daily="" digest=""&gt; </em></p></td> 
   <td>项目名称<br>Portfolio名称<br>项目参考编号<br>项目状态<br>项目[!UICONTROL计划完成日期]<br>项目所有者<br>分配给您的团队的任务列表<br><strong>[!UICONTROL请参阅更多详细信息]</strong> 按钮<br>*项目名称<br>*项目参考编号<br>*项目状态<br>*每日摘要日期</td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在完成项目之后，发送电子邮件给团队</strong> </p> <p>当项目状态为[!UICONTROL完成]时，项目团队的成员会收到一封电子邮件通知。</p> <p>提示：如果项目是定期完成的，则启用此选项可以为在许多项目中任务数量有限的用户创建大量电子邮件。</p> <p>即时通知电子邮件的主题是 <em>[!UICONTROL项目状态更改]: &lt;project name=""&gt;</em></p> <p> 每日摘要通知的主题是 <em> [!UICONTROL Digest of Projects You On] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 项目名称<br>Portfolio名称<br>项目参考编号<br>完成项目的用户的名称<br>项目状态<br>项目完成的日期和时间<br>上一个项目状态<br><strong>[!UICONTROL请参阅更多详细信息]</strong> 按钮<br>*项目名称<br>*项目参考编号<br>*项目状态<br>*每日摘要的日期<br></td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在完成任务之后，发送电子邮件给团队</strong> </p> <p>当项目任务完成时，项目团队成员会收到一封电子邮件通知。 <br>有关项目团队的更多信息，请参阅 <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">项目团队概述</a>.</p> <p>仅当项目状态为[!UICONTROL Current]时，才会发送通知。</p> <p>即时通知电子邮件的主题是 <em>[!UICONTROL Complete]: &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p> <p>注意：如果任务更改为等于[!UICONTROL Complete]的状态，则电子邮件的主题仍显示“[!UICONTROL Complete]”。</p> </p> <p><em> 每日摘要通知的主题是：[!UICONTROL Digest of Projects You On] &lt;date of="" daily="" digest=""&gt; </em> </p> </td> 
   <td> <p>任务名称<br>项目名称<br>任务参考编号<br>完成任务的用户的名称<br>任务状态<br>更改任务状态的日期和时间<br>上一任务状态<br><strong>查看更多详细信息</strong> 按钮<br>*项目名称<br>*项目参考编号<br>*完成的任务总数<br>*任务名称<br>*完成任务的用户名<br>*每日摘要的日期<br></p> </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在添加问题之后，发送电子邮件给团队。</strong> </p> <p>在向项目添加问题时，项目团队成员会收到一封电子邮件通知。</p> <p>仅当项目状态为“当前”时，才会发送通知。</p> <p>即时通知电子邮件的主题是 <em>[!UICONTROL问题已添加到] &lt;project name=""&gt;</em></p> <p> </p> <p> 每日摘要通知的主题是 <em> [!UICONTROL Digest of Projects You On] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 项目名称<br>Portfolio名称<br>问题参考编号<br>添加问题的用户的名称<br>问题类型<br>问题名称<br>输入日期<br>问题优先级<br>分配给名称 <br>问题状态<br>主要联系人<br>*项目名称<br>*项目参考编号<br>*项目中添加的问题总数<br>*问题名称<br>*分配给问题的用户的名称<br>*每日摘要日期 </td> 
   <td> <p><strong>即时</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在完成问题之后，发送电子邮件给团队</strong> </p> <p>当项目团队的项目出现问题时，其成员会收到一封电子邮件通知。<br>有关项目团队的更多信息，请参阅 <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">项目团队概述</a>.</p> <p>仅当项目状态为[!UICONTROL Current]或[!UICONTROL Planning]时，才会发送通知。</p> <p>即时通知电子邮件的主题是 <em>[!UICONTROL Complete]: &lt;issue name=""&gt; on &lt;project name=""&gt;</em></p> <p> 每日摘要通知的主题是 <em> [!UICONTROL Digest of Projects You On] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 问题名称<br>项目名称<br>完成问题的用户的名称<br>问题状态<br>问题完成的日期和时间<br>上一问题状态<br><strong>[!UICONTROL请参阅更多详细信息]</strong> 按钮<br>*项目名称<br>*项目参考编号<br>*完成的问题总数<br>*问题名称<br>*分配给问题的用户的名称<br>*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在添加未分配问题之后，发送电子邮件给团队。</strong> </p> <p>在将未分配的问题添加到项目时，项目团队成员会收到一封电子邮件通知。</p> <p>仅当项目状态为[!UICONTROL Current]时，才会发送通知。</p> <p>即时通知电子邮件的主题是 <em>[!UICONTROL应在上为谁分配此新问题] &lt;project name=""&gt;?</em></p> <p> 每日摘要通知的主题是 <em> [!UICONTROL Digest of Projects You On] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 项目名称<br>Portfolio名称<br>问题参考编号<br>添加问题的用户的名称<br>问题名称<br>问题类型<br>输入日期<br>问题优先级<br>分配给名称（空） <br>问题状态<br>主要联系人<br>*项目名称<br>*项目参考编号<br>*添加的问题总数<br>*问题名称<br>*添加了问题的用户的名称<br>*每日摘要的日期<br></td> 
   <td> <p><strong>即时</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>当项目团队中添加了一个用户时，发送电子邮件给用户</strong> </p> <p>被添加到项目的用户在被添加时会收到一封电子邮件通知，除非该用户自行添加到项目中。</p> <p>仅当项目状态为[!UICONTROL Current]时，才会发送通知。</p> <p>即时通知电子邮件的主题是 <em>[!UICONTROL您已添加到项目] &lt;project name=""&gt;</em></p> <p> 每日摘要通知的主题是 <em> [!UICONTROL Digest of Projects You On] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>项目名称<br>Portfolio名称<br>项目参考编号<br>将您添加到项目的用户的名称<br>项目[!UICONTROL计划开始日期]<br>项目[!UICONTROL计划完成日期]<br>项目完成百分比<br>项目上其他人的姓名 <br>项目所有者<br><strong>查看更多详细信息</strong> 按钮<br>*项目名称<br>*项目参考编号<br>*每日摘要日期</p> </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>当项目状态更改时，发送电子邮件给团队</strong> </p> <p>当项目状态发生更改时，项目团队成员会收到一封电子邮件通知。 <br>有关项目团队的更多信息，请参阅 <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">项目团队概述</a>.</p> <p>即时通知电子邮件的主题是 <em>[!UICONTROL项目状态更改]: &lt;project name=""&gt;</em></p> <p> 每日摘要通知的主题是 <em> [!UICONTROL Digest of Projects You On] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 项目名称<br>Portfolio名称<br>项目参考编号<br>更改项目状态的用户的名称<br>新建项目状态<br>项目状态更改的日期和时间<br>上一个项目状态<br><strong>[!UICONTROL请参阅更多详细信息]</strong> 按钮<br>*项目名称<br>*项目参考编号<br>*项目状态<br>*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
 </tbody> 
</table>
