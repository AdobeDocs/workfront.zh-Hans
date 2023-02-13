---
content-type: reference
navigation-topic: notifications
title: “通知：其他信息'
description: 以下通知会提醒您所赞助项目中正在发生的活动。
author: Lisa
feature: Get Started with Workfront
exl-id: fd93a48b-ef09-4489-b93d-5328240ffed6
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '968'
ht-degree: 8%

---

# 通知：其他信息

以下通知会提醒您所赞助项目中正在发生的活动。

有关配置接收的通知的信息，请参阅 [激活或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

另请参阅 [事件通知](../../workfront-basics/using-notifications/event-notifications.md).

>[!NOTE]
>
>您无法启用或禁用每日通知，并且不会收到此类别中事件的每日摘要电子邮件。 您可以为 [!UICONTROL 其他] 类别。

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
   <td> <p><strong>消息将发送到[!UICONTROL公告中心]</strong> </p> <p>当有新消息发送到[!UICONTROL公告中心]时，您会收到一封电子邮件通知。 </p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL [!DNL Adobe Workfront] 公告]: &lt;subject of="" the="" announcement=""&gt;</em></p> </td> 
   <td> 公告的主体<br>公告中所载报文的文本<br>附加的文档<br>发送公告的用户的名称<br>发送公告的日期和时间 </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在更改任务的主要分配之后，发送电子邮件给资源所有者</strong> </p> <p>当指派为经理的用户的一个直接报告被指派给新任务时，经理会收到有关该分配的电子邮件。 </p> <p>仅当项目状态为[!UICONTROL Current]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL任务资源分配]: &lt;task name=""&gt;</em></p> </td> 
   <td>项目名称<br>任务名称<br>创建任务的日期和时间<br>创建任务的用户的名称<br>分配名称<br>到期日（计划完成日期）<br>任务状态<br></td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>接到上传一份文档的要求后，该要求被取消</strong> </p> <p>文档请求在取消文档请求时会收到电子邮件通知。</p> <p>即时通知电子邮件的主题是： <em>&lt;name of="" the="" user="" who="" canceled="" the="" request=""&gt; 已取消文档请求。 </em></p> <p>电子邮件通知正文中包含以下文本：</p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;, <br><br>&lt;name of="" the="" user="" who="" canceled="" the="" request=""&gt;[!UICONTROL不再需要您上传有关您之前获得的请求的任何内容。 我们只想告诉你。</em> </p> </td> 
   <td>取消请求的用户的名称<br>原始文档上传请求的文本<br>原始文档请求上方的“[!UICONTROL CANCELED]”横幅<br>原始文档请求的日期和时间<br></td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>发现一个需要我关注的错误</strong> </p> <p>通过电子邮件回复评论的用户在回复未能送达时会收到电子邮件通知。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL无法处理] &lt;subject of="" original="" message=""&gt;</em></p> <p>有关使用电子邮件回复评论的信息，请参阅。<strong></strong></p> </td> 
   <td> </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在更改问题工作之后，发送电子邮件给资源所有者</strong> </p> <p>分配给问题的用户的经理在从问题中删除该用户或将其分配给问题时，会收到电子邮件通知。 </p> <p>仅当项目状态为“当前”或“计划”时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>问题分配： &lt;issue name=""&gt;</em></p> </td> 
   <td> <p>问题名称<br>项目名称<br>问题参考编号<br>完成分配的用户的名称<br>问题类型<br>分配给问题的用户的名称<br>输入的发行日期<br>问题优先级<br>主要联系人<br>问题[!UICONTROL计划完成日期]<br>问题状态<br><strong>[!UICONTROL请参阅更多详细信息]</strong> 按钮</p> </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>当项目团队中添加了一个用户时，发送电子邮件给资源所有者</strong> </p> <p>将经理的某个用户添加到项目后，经理会收到一封电子邮件通知。 无论项目状态如何，都会发送此通知。 </p> <p>拥有[!UICONTROL Review]许可证的用户不会收到通知。</p> <p>电子邮件的主题是： <em>项目分配： &lt;user name=""&gt;[&lt;project guid=""&gt;_ &lt;user guid=""&gt;]</em></p> </td> 
   <td> <p>项目名称<br>Portfolio名称<br>项目参考编号<br>将人员添加到项目的用户的名称<br>已添加到项目的用户的名称<br>项目[!UICONTROL计划开始日期]<br>项目[!UICONTROL计划完成日期]<br>项目完成百分比<br>项目上其他人的姓名<br>项目状态<br>项目所有者<br><strong>[!UICONTROL请参阅更多详细信息]</strong> 按钮<br><br><br></p> </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>默认向我拥有的项目组合或程序添加项目</strong> </p> <p>当将新项目添加到项目组合或项目群时，项目组合和/或项目群所有者会收到通知。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL项目已添加到] &lt;portfolio name=""&gt;[项目GUID]</em></p> </td> 
   <td> Portfolio名称<br>项目参考编号<br>将项目添加到项目组合/项目群的用户的名称<br><br></td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>其他人与我共享对象</strong> </p> <p>当有人将您添加到对象的[!UICONTROL共享]权限列表时，您会收到电子邮件通知。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL已授予访问权限]: &lt;object name=""&gt;</em></p> <p>仅当项目处于[!UICONTROL Current]状态时，才会发送通知。</p> </td> 
   <td> 对象名称<br>父对象名称<br>对象引用编号<br>对对象的原始访问<br>授予对象的新访问权限<br>授予访问权限的日期和时间 <br>授予访问权限的用户的名称 </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>其他人与我的团队共享对象</strong> </p> <p>当有人将您的团队添加到对象权限的共享列表时，您会收到一封电子邮件通知。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL已授予访问权限]: &lt;object name=""&gt; [访问规则GUID]</em></p> </td> 
   <td> 对象名称<br>父对象名称<br>对象引用编号<br>旧访问<br>新访问<br>授予访问权限的日期和时间<br>团队的名称<br>授予访问权限的用户的名称 </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我订阅的任务、发行或项目已进行更新</strong> </p> <p>当某人对您订阅的项目发表评论时，您会收到电子邮件通知。</p> <p>订阅电子邮件的主题是： <em>[!UICONTROL对]进行了更新 &lt;object type=""&gt; 您订阅了： &lt;object name=""&gt;</em></p> </td> 
   <td> 对象名称<br> 对象引用编号<br> 对订阅项目发表评论的用户的名称<br> 日期评论<br> 已向订阅项目添加评论  </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
 </tbody> 
</table>
