---
content-type: reference
navigation-topic: notifications
title: “通知：有关我拥有的项目的信息
description: 以下通知会提醒您有关在您拥有的项目中发生的活动。 有关配置接收的通知的信息，请参阅激活或停用您自己的事件通知。
author: Lisa
feature: Get Started with Workfront
exl-id: cf605849-bcc0-4982-b8fa-f69eef7a4fb6
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1713'
ht-degree: 6%

---

# 通知：有关我拥有的项目的信息

以下通知会提醒您有关在您拥有的项目中发生的活动。 有关配置接收的通知的信息，请参阅 [激活或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>在添加文档之后，发送电子邮件给项目所有者。</strong> </p> <p>在将文档添加到项目时，项目所有者会收到电子邮件通知，除非添加文档的用户也是项目所有者。</p> <p>仅当项目状态为[!UICONTROL当前]且文档不是私有时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL文档已添加到] &lt;project name=""&gt;</em></p> <p> 每日摘要通知的主题是： <em> [！您拥有的项目的UICONTROL摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 项目名称<br>Portfolio名称<br>项目参考编号<br>添加文档的用户的名称<br>文档名称<br>添加日期<br>文档详细信息（格式、大小、版本号）<br><strong>[!UICONTROL预览]</strong> 和 <strong>[!UICONTROL下载]</strong> 按钮<br>*项目名称<br>*项目参考编号<br>*添加的文档总数<br>*文档名称<br>*添加文档的用户名称<br>*每日摘要的日期<br></td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在完成里程碑任务之后，发送电子邮件给项目所有者。</strong> </p> <p>仅当项目状态为[!UICONTROL Current]或[!UICONTROL Planning]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL Complete]: &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p>注意：如果任务更改为等于[!UICONTROL Complete]的状态，则电子邮件的主题仍显示“[!UICONTROL Complete]”。</p> <p> 每日摘要通知的主题是： <em> [！您拥有的项目的UICONTROL摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 任务名称<br>项目名称<br>任务参考编号<br>完成任务的用户的名称<br>新任务状态<br>任务完成的日期和时间<br>上一任务状态<br><strong>[!UICONTROL请参阅更多详细信息]</strong> 按钮<br>*项目名称<br>*项目参考编号<br>*完成的任务总数<br>*任务名称<br>*完成任务的用户名<br>*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>当项目从正进度状态 (按时) 更改为负进度状态 (延迟) 时，发送电子邮件给项目所有者</strong> </p> <p>当项目超出计划时，项目所有者会收到电子邮件通知。 当进度状态为“[!UICONTROL At Risk]”、“[!UICONTROL Beind]”或“[!UICONTROL Late]”时，项目将落后于计划。</p> <p>最佳做法是保持此通知处于活动状态。 </p> <p>拥有[!UICONTROL Review]许可证的用户不会收到通知。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL项目进度更改]: &lt;project name=""&gt;</em></p> <p> 每日摘要通知的主题是： <em> [！您拥有的项目的UICONTROL摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>项目名称<br>Portfolio名称<br>项目参考编号<br>项目进度状态<br>项目[!UICONTROL计划开始日期]<br>项目[!UICONTROL计划完成日期]<br>项目[!UICONTROL预计开始日期]<br>项目[!UICONTROL预计完成日期]<br>项目完成百分比<br>项目状态<br>项目所有者<br>*项目名称<br>*项目参考编号<br>*项目进度状态<br>*每日摘要的日期<br></p> </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在添加问题之后，发送电子邮件给项目所有者。</strong> </p> <p>在向项目添加问题时，项目所有者会收到电子邮件通知。</p> <p>仅当项目状态为[!UICONTROL Current]或[!UICONTROL Planning]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL问题已添加到] &lt;project name=""&gt;</em></p> <p> </p> <p> 每日摘要通知的主题是： <em> [！您拥有的项目的UICONTROL摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>项目名称<br>Portfolio名称<br>问题参考编号<br>添加问题的用户的名称<br>问题名称<br>问题类型<br>输入日期<br>问题优先级<br>分配给名称 <br>问题状态<br>主要联系人<br>*项目名称<br>*项目参考编号<br>*项目中添加的问题总数<br>*问题名称<br>*添加了问题的用户的名称<br>*每日摘要日期</p> </td> 
   <td> <p><strong>即时</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在完成任务之后，发送电子邮件给项目所有者</strong> </p> <p>当任务完成时，项目所有者会收到通知。</p> <p>仅当项目状态为[!UICONTROL Current]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL Complete]: &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p> <p>注意：如果任务更改为等于[!UICONTROL Complete]的状态，则电子邮件的主题仍显示“[!UICONTROL Complete]”。</p> </p> <p> 每日摘要通知的主题是： <em> [！您拥有的项目的UICONTROL摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 任务名称<br>项目名称<br>任务参考编号<br>完成任务的用户的名称 <br>任务状态<br>任务完成的日期和时间<br>上一任务状态<br><strong>[!UICONTROL请参阅更多详细信息]</strong> 按钮<br>*项目名称<br>*项目参考编号<br>*完成的任务总数 <br>*任务名称<br>*完成任务的用户名<br>*每日摘要的日期<br></td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>当任务从正进度状态 (按时) 更改为负进度状态 (延迟) 时，发送电子邮件给项目所有者</strong> </p> <p>当项目上的任务滞后于计划时，项目所有者会收到电子邮件通知。 当进度状态为“[!UICONTROL At Risk]”、“[!UICONTROL Beind]”或“[!UICONTROL Late]”时，任务将滞后于计划。</p> <p>仅当项目状态为[!UICONTROL Current]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL任务进度更改]: &lt;task name=""&gt;</em></p> <p> 每日摘要通知的主题是： <em> [！您拥有的项目的UICONTROL摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 任务名称<br>项目名称<br>任务参考编号<br>新任务进度状态<br>任务[!UICONTROL计划开始日期]<br>任务[!UICONTROL计划完成日期]<br>任务[!UICONTROL预计开始日期]<br>任务[!UICONTROL预计完成日期]<br>任务完成百分比<br>任务状态<br>分配给名称<br>按名称输入<br>*项目名称<br>*项目参考编号<br>*延迟计划的任务总数<br>*任务名称<br>*分配给名称<br>*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在完成问题之后，发送电子邮件给项目所有者</strong> </p> <p>当项目所有者的项目出现问题时，他们会收到一封电子邮件通知。</p> <p>仅当项目状态为[!UICONTROL Current]或[!UICONTROL Planning]时，才会发送通知。</p> <p>拥有[!UICONTROL Review]许可证的用户不会收到通知。 </p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL Complete]: &lt;issue name=""&gt; on &lt;project name=""&gt;</em></p> <p> 每日摘要通知的主题是： <em> [！您拥有的项目的UICONTROL摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 问题名称<br>项目名称<br>问题参考编号<br>完成问题的用户的名称<br>问题状态<br>问题完成的日期和时间<br>上一问题状态<br><strong>[!UICONTROL请参阅更多详细信息]</strong> 按钮 <br>*项目名称<br>*项目参考编号<br>*完成的问题总数<br>*问题名称<br>*分配给问题的用户的名称<br>*每日摘要的日期<br></td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在添加未分配问题之后，发送电子邮件给项目所有者。</strong> </p> <p>在将未分配的问题添加到项目时，项目所有者会收到电子邮件通知。</p> <p>仅当项目状态为[!UICONTROL Current]或[!UICONTROL Planning]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL应在上为谁分配此新问题] &lt;project name=""&gt;?</em></p> <p> </p> <p> 每日摘要通知的主题是： <em> 您拥有的项目摘要 &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>项目名称<br>Portfolio名称<br>问题参考编号<br>添加问题的用户的名称<br>问题名称<br>问题类型<br>输入日期<br>问题优先级<br>分配给名称（空）<br>问题状态<br>主要联系人<br>*项目名称<br>*项目参考编号<br>*添加的问题总数<br>*问题名称<br>*添加了问题的用户的名称<br>*每日摘要的日期<br></p> </td> 
   <td> <p><strong>即时</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>当项目所有者更改或项目创建时，发送电子邮件给新分派所有者</strong> </p> <p>当用户被分配为项目的所有者时，该用户会收到电子邮件通知。</p> <p>如果项目所有者是进行分配的同一用户，则不会发送电子邮件通知。</p> <p>拥有[!UICONTROL Review]许可证的用户不会收到通知。</p> <p>打开这个，因为他们被分配到了某个东西。 </p> <p> 分配某些内容，共享某些内容，获取某些内容的访问权限。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL您现在是项目所有者] &lt;project name=""&gt;</em></p> <p>电子邮件通知正文中包含以下文本：<em><br></em></p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;,<br></em><em>&lt;name of="" the="" user="" who="" assigned="" you="" as="" the="" project="" owner=""&gt; [!UICONTROL使您成为]的所有者 &lt;project name=""&gt;. [!UICONTROL作为项目所有者，您可能会收到有关项目活动的其他电子邮件通知、批准项目所需的时间或参与批准与项目相关的工作。 都是你的。]</em> </p> <p> 每日摘要通知的主题是： <em> [！您拥有的项目的UICONTROL摘要] &lt;date of="" daily="" digest=""&gt; </em></p> <p> </p> </td> 
   <td> <p>项目名称<br>Portfolio名称<br>项目参考编号<br>项目完成日期<br>*项目名称<br>*项目参考编号<br>*每日摘要日期</p> </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>当任务的提交日期改变时，向项目所有者发送电子邮件</strong> </p> <p>当项目上某项任务的“提交日期”发生更改时，项目所有者会收到一封电子邮件通知，除非更改“提交日期”的用户也是项目所有者。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL的提交日期] &lt;task name=""&gt; [!UICONTROL现在为] &lt;new commit="" date=""&gt;</em></p> <p> 每日摘要通知的主题是： <em> 您拥有的项目摘要 &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>任务名称<br>项目名称<br>任务参考编号<br>更改提交日期的用户的名称<br>新提交日期<br>任务[!UICONTROL计划完成日期]<br>有关项目时间轴如何受此更改影响的信息<br>分配给名称<br>按名称输入<br>项目所有者<br><strong>[!UICONTROL请参阅更多详细信息]</strong> 按钮<br>*项目名称<br>*项目参考编号<br>*提交日期已更改的任务总数<br>*任务名称<br>*每日摘要的日期<br></p> </td> 
   <td> <p><strong>即时</strong> </p> <p><strong>和[!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>当问题的提交日期改变时，向项目所有者发送电子邮件</strong> </p> <p>当项目上的问题的提交日期发生更改时，项目所有者会收到电子邮件通知，除非更改提交日期的用户与项目所有者的用户相同。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL的提交日期] &lt;issue name=""&gt; [!UICONTROL现在为] &lt;new commit="" date=""&gt;</em></p> <p> 每日摘要通知的主题是： <em> [！您拥有的项目的UICONTROL摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>问题名称<br>项目名称<br>问题参考编号<br>更改提交日期的用户的名称<br>新提交日期<br>发行计划完成日期<br>分配给名称<br>按名称输入<br>项目所有者<br><strong>[!UICONTROL请参阅更多详细信息]</strong> 按钮<br>*项目名称<br>*项目参考编号<br>*提交日期已更改的问题总数<br>*问题名称<br>*每日摘要的日期<br></p> </td> 
   <td> <p><strong>即时</strong> </p> <p><strong>和[!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
