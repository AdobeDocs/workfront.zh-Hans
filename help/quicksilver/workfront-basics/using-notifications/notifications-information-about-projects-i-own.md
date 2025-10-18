---
content-type: reference
navigation-topic: notifications
title: 通知：关于我拥有的项目的信息
description: 以下通知会提醒您有关在您拥有的项目中发生的活动。 有关配置您收到的通知的信息，请参阅修改您自己的电子邮件通知。
author: Courtney
feature: Get Started with Workfront
exl-id: cf605849-bcc0-4982-b8fa-f69eef7a4fb6
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '1709'
ht-degree: 0%

---

# 通知：关于我拥有的项目的信息

以下通知会提醒您有关在您拥有的项目中发生的活动。 有关配置您收到的通知的信息，请参阅[修改您自己的电子邮件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。

另请参阅[事件通知](../../workfront-basics/using-notifications/event-notifications.md)。

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
   <td> <p><strong>向我拥有的项目添加了文档</strong> </p> <p>将文档添加到项目时，项目所有者会收到电子邮件通知，除非添加该文档的用户也是项目所有者。</p> <p>仅当项目状态为[！UICONTROL当前]且文档不是“私有”时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL文档已添加到] &lt;项目名称&gt;</em></p> <p> 每日摘要通知的主题是：<em> [！UICONTROL您拥有的项目摘要] &lt;每日摘要的日期&gt; </em></p> </td> 
   <td> 项目名称<br>Portfolio名称<br>项目参考编号<br>添加文档的用户的名称<br>文档名称<br>已于日期添加<br>文档详细信息（格式、大小、版本号）<br><strong>[！UICONTROL预览]</strong>和<strong>[！UICONTROL下载]</strong>按钮<br>*项目名称<br>*项目参考编号<br>*添加的文档总数<br>*文档名称<br>*添加用户的名称文档<br>*每日摘要的日期<br></td> 
   <td><strong>每天</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在完成里程碑任务之后，发送电子邮件给项目所有者</strong> </p> <p>仅当项目状态为[！UICONTROL当前]或[！UICONTROL计划]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： &lt;项目名称&gt;<em>上的</em>[！UICONTROL完成]： &lt;任务名称&gt;</p> <p>注意：如果任务更改为等于[！UICONTROL完成]的状态，则电子邮件主题仍显示“[！UICONTROL完成]”。</p> <p> 每日摘要通知的主题是：<em> [！UICONTROL您拥有的项目摘要] &lt;每日摘要的日期&gt; </em></p> </td> 
   <td> 任务名称<br>项目名称<br>任务参考编号<br>完成任务的用户的名称<br>新任务状态<br>完成任务的日期和时间<br>上一任务状态<br><strong>[！UICONTROL查看更多详细信息]</strong>按钮<br>*项目名称<br>*项目参考编号<br>*已完成任务的任务总数<br>*任务名称<br>*完成任务的用户的名称<br>*每日摘要的日期 </td> 
   <td><strong>每天</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我拥有的项目落后</strong> </p> <p>当项目落后于计划时，项目所有者会收到电子邮件通知。 当进度状态为“[！UICONTROL有风险]”、“[！UICONTROL落后]”或“[！UICONTROL延迟]”时，项目进度落后于计划。</p> <p>最佳实践是保持此通知处于活动状态。 </p> <p>拥有[！UICONTROL Review]许可证的用户不会收到通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL项目进度更改]： &lt;项目名称&gt;</em></p> <p> 每日摘要通知的主题是：<em> [！UICONTROL您拥有的项目摘要] &lt;每日摘要的日期&gt; </em></p> </td> 
   <td> <p>项目名称<br>Portfolio名称<br>项目参考编号<br>项目进度状态<br>项目[！UICONTROL计划开始日期]<br>项目[！UICONTROL计划完成日期]<br>项目[！UICONTROL预计开始日期]<br>项目[！UICONTROL预计完成日期]<br>项目完成百分比<br>项目状态<br>项目所有者<br>*项目名称<br>*项目参考编号number<br>*项目进度状态<br>*每日摘要的日期<br></p> </td> 
   <td><strong>每天</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>向我拥有的项目添加了一个问题</strong> </p> <p>在将问题添加到项目时，项目所有者会收到电子邮件通知。</p> <p>仅当项目状态为[！UICONTROL当前]或[！UICONTROL计划]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL问题已添加到] &lt;项目名称&gt;</em></p> <p> </p> <p> 每日摘要通知的主题是：<em> [！UICONTROL您拥有的项目摘要] &lt;每日摘要的日期&gt; </em></p> </td> 
   <td> <p>项目名称<br>Portfolio名称<br>问题参考编号<br>添加问题的用户名称<br>问题名称<br>问题类型<br>输入的日期<br>问题优先级<br>分配给名称<br>问题状态<br>主要联系人<br>*项目名称<br>*项目参考编号<br>*添加到项目的问题总数<br>*问题名称<br>*添加问题的用户名称<br>*每日摘要日期</p> </td> 
   <td> <p><strong>即时</strong> </p> <p><strong>和每天</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在完成任务之后，发送电子邮件给项目所有者</strong> </p> <p>项目所有者会在任务完成其项目时收到通知。</p> <p>仅当项目状态为[！UICONTROL当前]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： &lt;项目名称&gt;<em>上的</em>[！UICONTROL完成]： &lt;任务名称&gt;</p> <p> <p>注意：如果任务更改为等于[！UICONTROL完成]的状态，则电子邮件主题仍显示“[！UICONTROL完成]”。</p> </p> <p> 每日摘要通知的主题是：<em> [！UICONTROL您拥有的项目摘要] &lt;每日摘要的日期&gt; </em></p> </td> 
   <td> 任务名称<br>项目名称<br>任务参考编号<br>完成任务的用户的名称<br>任务状态<br>完成任务的日期和时间<br>上一任务状态<br><strong>[！UICONTROL查看更多详细信息]</strong>按钮<br>*项目名称<br>*项目参考编号<br>*完成任务的用户的任务总数<br>*任务名称<br>*完成任务的用户的名称<br>*每日摘要的日期<br></td> 
   <td><strong>每天</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我拥有的项目中的任务落后</strong> </p> <p>当项目中的任务落后于计划时，项目所有者会收到电子邮件通知。 当进度状态为“[！UICONTROL有风险]”、“[！UICONTROL落后]”或“[！UICONTROL延迟]”时，任务进度落后于计划。</p> <p>仅当项目状态为[！UICONTROL当前]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL任务进度更改]： &lt;任务名称&gt;</em></p> <p> 每日摘要通知的主题是：<em> [！UICONTROL您拥有的项目摘要] &lt;每日摘要的日期&gt; </em></p> </td> 
   <td> 任务名称<br>项目名称<br>任务参考编号<br>新任务进度状态<br>任务[！UICONTROL计划开始日期]<br>任务[！UICONTROL计划完成日期]<br>任务[！UICONTROL预计开始日期]<br>任务[！UICONTROL预计完成日期]<br>任务完成百分比<br>任务状态<br>分配给名称<br>由名称<br>*输入的项目名称<br>*项目参考编号<br>*落后于预定计划的任务总数<br>*任务名称<br>*分配给名称<br>*每日摘要日期 </td> 
   <td><strong>每天</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在完成问题之后，发送电子邮件给项目所有者</strong> </p> <p>项目所有者在其项目上完成问题后会收到电子邮件通知。</p> <p>仅当项目状态为[！UICONTROL当前]或[！UICONTROL计划]时，才会发送通知。</p> <p>拥有[！UICONTROL Review]许可证的用户不会收到通知。 </p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL完成]： &lt;项目名称&gt;</em>上的&lt;问题名称&gt;</p> <p> 每日摘要通知的主题是：<em> [！UICONTROL您拥有的项目摘要] &lt;每日摘要的日期&gt; </em></p> </td> 
   <td> 问题名称<br>项目名称<br>问题参考编号<br>完成问题的用户名称<br>问题状态<br>完成问题的日期和时间<br>上一个问题状态<br><strong>[！UICONTROL查看更多详细信息]</strong>按钮<br>*项目名称<br>*项目参考编号<br>*完成的问题总数<br>*问题名称<br>*分配给问题的用户名称<br>*每日摘要的日期<br></td> 
   <td><strong>每天</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>向我拥有的项目添加了未分配问题</strong> </p> <p>当未分配的问题添加到项目时，项目所有者会收到电子邮件通知。</p> <p>仅当项目状态为[！UICONTROL当前]或[！UICONTROL计划]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL谁应被分配到] &lt;项目名称&gt;？</em>上的此新问题</p> <p> </p> <p> 每日摘要通知的主题是： <em>您拥有的项目摘要&lt;每日摘要的日期&gt; </em></p> </td> 
   <td> <p>项目名称<br>Portfolio名称<br>问题参考编号<br>添加问题的用户名称<br>问题名称<br>问题类型<br>输入的日期<br>问题优先级<br>分配给名称（空）<br>问题状态<br>主要联系人<br>*项目名称<br>*项目参考编号<br>*添加的问题总数<br>*问题名称<br>*添加问题的用户名称<br>*每日摘要的日期<br></p> </td> 
   <td> <p><strong>即时</strong> </p> <p><strong>和每天</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我被设置为新项目的所有者</strong> </p> <p>当用户被指定为项目所有者时，该用户会收到电子邮件通知。</p> <p>如果项目所有者是进行分配的同一个用户，则不会发送电子邮件通知。</p> <p>拥有[！UICONTROL Review]许可证的用户不会收到通知。</p> <p>打开此功能，因为它们已分派到某个项目。 </p> <p> 分配某些内容，共享某些内容，获取某些内容的访问权限。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL您现在是] &lt;项目名称&gt;</em>的项目所有者</p> <p>电子邮件通知正文中包含以下文本：<em><br></em></p> <p><em>[！UICONTROL Hi] &lt;您的名称&gt;，<br></em><em>&lt;将您分配为项目所有者的用户的名称&gt; [！UICONTROL使您成为] &lt;项目名称&gt;的所有者。 [！UICONTROL作为项目所有者，您可能会收到有关项目活动的其他电子邮件通知，需要您审批项目小时数，或参与审批与项目相关的工作。 都是你的。]</em> </p> <p> 每日摘要通知的主题是：<em> [！UICONTROL您拥有的项目摘要] &lt;每日摘要的日期&gt; </em></p> <p> </p> </td> 
   <td> <p>项目名称<br>Portfolio名称<br>项目参考编号<br>项目完成日期<br>*项目名称<br>*项目参考编号<br>*每日摘要日期</p> </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>当任务的提交日期更改时，向项目所有者发送电子邮件</strong> </p> <p>当项目上任务的提交日期更改时，项目所有者会收到电子邮件通知，除非更改提交日期的用户也是项目所有者。</p> <p>即时通知电子邮件的主题为： <em>[！UICONTROL提交日期] &lt;任务名称&gt; [！UICONTROL现在为] &lt;新提交日期&gt;</em></p> <p> 每日摘要通知的主题是： <em>您拥有的项目摘要&lt;每日摘要的日期&gt; </em></p> </td> 
   <td> <p>任务名称<br>项目名称<br>任务引用编号<br>更改提交日期的用户名称<br>新提交日期<br>任务[！UICONTROL计划完成日期]<br>有关此更改对项目时间线有何影响的信息<br>分配给名称<br>由名称<br>项目所有者<br><strong>[！UICONTROL输入查看更多详细信息]</strong>按钮<br>*项目名称<br>*项目引用数字<br>*提交日期已更改的任务总数<br>*任务名称<br>*每日摘要的日期<br></p> </td> 
   <td> <p><strong>即时</strong> </p> <p><strong>和[！UICONTROL Daily]</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>当问题的提交日期更改时，向项目所有者发送电子邮件</strong> </p> <p>当项目问题的提交日期更改时，项目所有者会收到电子邮件通知，除非更改提交日期的用户与项目所有者是同一用户。</p> <p>即时通知电子邮件的主题为： <em>[！UICONTROL提交日期] &lt;问题名称&gt; [！UICONTROL现在为] &lt;新提交日期&gt;</em></p> <p> 每日摘要通知的主题是：<em> [！UICONTROL您拥有的项目摘要] &lt;每日摘要的日期&gt; </em></p> </td> 
   <td> <p>问题名称<br>项目名称<br>问题引用编号<br>更改提交日期的用户名称<br>新提交日期<br>问题计划完成日期<br>分配给名称<br>由名称<br>项目所有者<br><strong>[！UICONTROL输入查看更多详细信息]</strong>按钮<br>*项目名称<br>*项目引用编号<br>*提交日期已更改的问题总数<br>*问题问题name<br>*每日摘要的日期<br></p> </td> 
   <td> <p><strong>即时</strong> </p> <p><strong>和[！UICONTROL Daily]</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
