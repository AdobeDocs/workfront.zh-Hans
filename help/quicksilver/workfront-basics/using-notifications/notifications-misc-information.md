---
content-type: reference
navigation-topic: notifications
title: '通知：其他信息'
description: 以下通知会提醒您正在赞助的项目中发生的活动。
author: Lisa
feature: Get Started with Workfront
exl-id: fd93a48b-ef09-4489-b93d-5328240ffed6
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '966'
ht-degree: 8%

---

# 通知：其他信息

以下通知会提醒您正在赞助的项目中发生的活动。

有关配置接收哪些通知的信息，请参阅 [修改您自己的电子邮件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

另请参阅 [事件通知](../../workfront-basics/using-notifications/event-notifications.md).

>[!NOTE]
>
>您无法启用或禁用每日通知，并且不会收到此类别中事件的每日摘要电子邮件。 您可以为启用或禁用单个即时通知 [!UICONTROL 其他] 类别。

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
   <td> <p><strong>将向[！UICONTROL公告中心]发送消息</strong> </p> <p>在将新消息发送到[！UICONTROL公告中心]后，您将收到电子邮件通知。 </p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL [!DNL Adobe Workfront] 公告]： &lt;subject of="" the="" announcement=""&gt;</em></p> </td> 
   <td> 公告主题<br>公告中包含的信息文本<br>附加文档<br>发送公告的用户的名称<br>发送公告的日期和时间 </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在更改任务的主要分配之后，发送电子邮件给资源所有者</strong> </p> <p>当指定为经理的用户的直接下属之一被分配给新任务时，经理会收到有关该分配的电子邮件。 </p> <p>仅当项目状态为[！UICONTROL当前]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL任务资源分配]： &lt;task name=""&gt;</em></p> </td> 
   <td>项目名称<br>任务名称<br>创建任务的日期和时间<br>创建任务的用户的名称<br>任务名称<br>到期日期（计划完成日期）<br>任务状态<br></td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>接到上传一份文档的要求后，该要求被取消</strong> </p> <p>文档请求被取消时，文档请求者会收到电子邮件通知。</p> <p>即时通知电子邮件的主题是： <em>&lt;name of="" the="" user="" who="" canceled="" the="" request=""&gt; 已取消文档请求。 </em></p> <p>电子邮件通知正文中包含以下文本：</p> <p><em>[！UICONTROL Hi] &lt;your name=""&gt;， <br><br>&lt;name of="" the="" user="" who="" canceled="" the="" request=""&gt;[！UICONTROL不再需要您上传与您之前收到的请求有关的任何内容。 我们只是想让您知道。 ]</em> </p> </td> 
   <td>取消请求的用户的名称<br>原始文档上载请求的文本<br>原始文档请求上方的“[！UICONTROL CANCELED]”横幅<br>原始文档请求的日期和时间<br></td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>发现一个需要我关注的错误</strong> </p> <p>通过电子邮件回复评论的用户会在回复无法传递时收到电子邮件通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL无法处理] &lt;subject of="" original="" message=""&gt;</em></p> <p>有关使用电子邮件回复评论的信息，请参阅。<strong></strong></p> </td> 
   <td> </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在更改问题工作之后，发送电子邮件给资源所有者</strong> </p> <p>将某个用户从问题中移除或将其分配给某个问题时，分配给该用户的经理会收到电子邮件通知。 </p> <p>仅当项目状态为“当前”或“计划”时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>问题分配： &lt;issue name=""&gt;</em></p> </td> 
   <td> <p>问题名称<br>项目名称<br>问题参考号<br>进行分配的用户的名称<br>问题类型<br>分配给问题的用户的名称<br>输入的问题日期<br>问题优先级<br>主要联系人<br>问题[！UICONTROL计划完成日期]<br>问题状态<br><strong>[！UICONTROL查看更多详细信息]</strong> 按钮</p> </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>当项目团队中添加了一个用户时，发送电子邮件给资源所有者</strong> </p> <p>当经理的一个用户被添加到项目时，经理会收到电子邮件通知。 无论项目的状态如何，都会发送此通知。 </p> <p>拥有[！UICONTROL Review]许可证的用户不会收到通知。</p> <p>电子邮件的主题是： <em>项目工作： &lt;user name=""&gt;[&lt;project guid=""&gt;_ &lt;user guid=""&gt;]</em></p> </td> 
   <td> <p>项目名称<br>Portfolio名称<br>项目参考号<br>将人员添加到项目的用户的名称<br>添加到项目的用户的名称<br>项目[！UICONTROL计划开始日期]<br>项目[！UICONTROL计划完成日期]<br>项目完成百分比<br>项目中的其他人的姓名<br>项目状态<br>项目所有者<br><strong>[！UICONTROL查看更多详细信息]</strong> 按钮<br><br><br></p> </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>默认向我拥有的项目组合或程序添加项目</strong> </p> <p>当新项目添加到项目组合或项目群时，项目组合和/或项目群所有者会收到通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL项目已添加到] &lt;portfolio name=""&gt;[项目GUID]</em></p> </td> 
   <td> Portfolio名称<br>项目参考号<br>将项目添加到项目组合/项目的用户的名称<br><br></td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>其他人与我共享对象</strong> </p> <p>当有人将您添加到对象权限的[！UICONTROL共享]列表时，您会收到电子邮件通知。</p> <p>即时通知电子邮件的主题是： <em>已授予[！UICONTROL访问权限]： &lt;object name=""&gt;</em></p> <p>仅当项目处于[！UICONTROL当前]状态时，才会发送通知。</p> </td> 
   <td> 对象名称<br>父对象名称<br>对象参考号<br>对对象的原始访问权限<br>授予对象的新访问权限<br>授予访问权限的日期和时间 <br>授予访问权限的用户的名称 </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>其他人与我的团队共享对象</strong> </p> <p>当有人将您的团队添加到对象权限的“共享”列表时，您会收到电子邮件通知。</p> <p>即时通知电子邮件的主题是： <em>已授予[！UICONTROL访问权限]： &lt;object name=""&gt; [访问规则GUID]</em></p> </td> 
   <td> 对象名称<br>父对象名称<br>对象参考号<br>旧访问权限<br>新建访问权限<br>授予访问权限的日期和时间<br>您的团队的名称<br>授予访问权限的用户的名称 </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我订阅的任务、问题或项目已更新</strong> </p> <p>当有人对您订阅的项目发表评论时，您将收到电子邮件通知。</p> <p>订阅电子邮件的主题是： <em>[！UICONTROL]已更新 &lt;object type=""&gt; 您已订阅： &lt;object name=""&gt;</em></p> </td> 
   <td> 对象名称<br> 对象参考号<br> 对订阅项目发表评论的用户名称<br> 发表评论的日期<br> 已添加备注到订阅的项目  </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
 </tbody> 
</table>
