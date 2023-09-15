---
content-type: reference
navigation-topic: notifications
title: '通知：我发出的请求'
description: 以下通知告知您已在Adobe Workfront中发出的请求。
author: Lisa
feature: Get Started with Workfront
exl-id: 42771f71-dbf8-4e73-9a0e-8efea612af4a
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1427'
ht-degree: 7%

---

# 通知：我已发出的请求

以下通知告知您在中发出的请求 [!DNL Adobe Workfront].

有关配置接收哪些通知的信息，请参阅 [修改您自己的电子邮件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

另请参阅 [事件通知](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td colspan="3"><strong>我已做出的请求</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>文档审批请求已完成</strong> </p> <p>请求审批文档的用户会在文档审批请求完成后收到电子邮件通知。</p> <p>即时通知电子邮件的主题是：<em> &lt;approver name=""&gt; 具有 &lt;approval decision="" uicontrol="" approved="" uicontrol="" approved="" with="" changes="" uicontrol="" rejected=""&gt; 本文档。</em></p> <p>注意：您无法为每日摘要电子邮件配置此通知。</p> </td> 
   <td> 文档名称<br>审批者姓名 </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>与我作为主要联系人的问题相关的文档已更改或上载</strong> </p> <p>在上传或更改有关问题的文档时，问题的主要联系人会收到电子邮件通知，除非上传或更改文档的用户同时也是主要联系人。</p> <p>仅当项目设置为[！UICONTROL帮助请求队列]（如中所述）时，才会发送通知 <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[！UICONTROL创建请求队列]</a>)。</p> <p>即时通知电子邮件的主题是： <em>文档已添加至 &lt;issue name=""&gt;</em></p> <p>每日摘要通知的主题是： <em>您的请求的摘要 &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> 文档上传到的对象名称<br>父对象名称<br>文档参考号<br>上传文档的用户的名称<br>文档名称<br>添加日期<br>文档详细信息（格式、大小、版本号）<br>文档缩略图<br><strong>[！UICONTROL预览]</strong> 和 <strong>[！UICONTROL下载]</strong> 按钮<br>*项目名称<br>*项目参考号<br>*上传的文档总数<br>*文档名称<br>*父对象名称<br>*添加文档的用户的名称<br>*每日摘要的日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>要求上传一份文档已实现</strong> </p> <p>文档请求者在完成文档上载请求时收到电子邮件通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL您的文档请求来自] &lt;user name=""&gt; 已完成</em></p> <p>注意：您无法为每日摘要电子邮件配置此通知。</p> </td> 
   <td> <p>上传文档的用户的名称<br>文档上传到的对象名称<br>文档名称<br><br></p> </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我已分配至某人的个人任务已完成</strong> </p> <p>当某个临时任务完成时，会向将该任务分配给其他人的用户发送通知。 </p> <p>有关临时任务的详细信息，请参阅 <a href="../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md" class="MCXref xref">从[！UICONTROL主页]区域创建工作项</a>.</p> <p>即时通知电子邮件的主题是： <em>任务完成： &lt;task name=""&gt;</em></p> <p> <p>注意：您无法为每日摘要电子邮件配置此通知。</p> </p> </td> 
   <td> 任务名称<br>默认项目名称（接收个人任务的用户的个人项目）<br>任务参考号<br>任务所有者名称<br>新任务状态<br>完成任务的日期和时间<br>上一个任务状态<br><strong>[！UICONTROL查看更多详细信息]</strong> 按钮<br><br><br></td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我是主要联系人的一个问题已完成。</strong> </p> <p>问题创建者会在问题完成时收到通知。</p> <p>仅当项目状态为[！UICONTROL当前]或[！UICONTROL计划]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL问题完成]： &lt;issue name=""&gt;</em></p> <p>每日摘要通知的主题是：<em> 您的请求的摘要 &lt;date of="" the="" daily="" digest=""&gt;</em></p> <p> </p> </td> 
   <td> 问题名称<br>项目名称<br>问题参考号<br>完成问题的用户的名称<br>新建状态<br>完成问题的日期和时间<br>上一个问题状态<br><strong>[！UICONTROL查看更多详细信息]</strong> 按钮 <br>*项目名称<br>*项目参考号<br>*已完成的问题总数<br>*问题名称<br>*完成问题的用户的名称<br>*每日摘要日期 </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我添加一个问题到项目。</strong> </p> <p>当问题的主要联系人添加问题到项目中时，他们会收到通知。</p> <p>仅当项目状态为[！UICONTROL当前]或[！UICONTROL计划]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL问题已提交]： &lt;issue name=""&gt; 日期 &lt;project name=""&gt;</em></p> <p>每日摘要通知的主题是：<em> 您的请求的摘要 &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> 项目名称<br>Portfolio名称<br>问题参考号<br>您的姓名<br>问题名称<br>输入日期<br>问题优先级<br>问题状态<br>分派至姓名<br>主要联系人<br>*项目名称<br>*项目参考号<br>*添加的问题总数<br>*问题名称<br>*每日摘要日期 </td> 
   <td> <p><strong>即时</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我提交请求 (确认)</strong> </p> <p>问题的主要联系人会在提交问题时收到电子邮件通知。</p> <p>仅当项目状态为[！UICONTROL当前]并且项目设置为[！UICONTROL帮助请求队列]（如中所述）时，才会发送通知 <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[！UICONTROL创建请求队列]</a>)。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL请求已提交]： &lt;request name=""&gt; 日期 &lt;project request="" queue="" name=""&gt;</em></p> <p>每日摘要通知的主题是：<em> 您的请求的摘要 &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>项目名称（请求队列名称）<br>Portfolio名称<br>问题参考号<br>问题名称<br>输入日期<br>问题优先级<br>问题状态<br>分派至姓名<br>主要联系人<br>*项目参考号<br>*项目名称<br>*提交的请求总数<br>*请求名称<br>*请求优先级<br>*每日摘要日期</p> </td> 
   <td> <p><strong>即时</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我的请求已关闭 (确认)</strong> </p> <p>当请求关闭时，问题的主要联系人会收到电子邮件通知。</p> <p>仅当项目状态为“当前”并且项目设置为[！UICONTROL帮助请求队列]（如中所述）时，才会发送通知 <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">创建请求队列</a>)。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL您的请求已关闭]："&lt;request name=""&gt;"</em></p> <p>每日摘要通知的主题是：<em> [！UICONTROL您的请求摘要] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> 请求名称<br>项目名称<br>请求参考号<br>关闭请求的用户的名称<br>问题状态<br>关闭请求的日期和时间<br>上一个请求状态<br><strong>[！UICONTROL查看更多详细信息]</strong> 按钮<br>*项目参考号<br>*项目名称<br>*已关闭的请求总数<br>*请求名称<br>*关闭请求的用户的名称<br>*每日摘要日期 </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>有人已分派到我的请求</strong> </p> <p>当用户被分配给问题时，除非主要联系人和分配的用户是同一个用户，否则问题的主要联系人会收到电子邮件通知。</p> <p>仅当项目状态为“当前”并且项目设置为[！UICONTROL帮助请求队列]（如中所述）时，才会发送通知 <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[！UICONTROL创建请求队列]</a>)。</p> <p>即时通知电子邮件的主题是： <em>&lt;name of="" the="" user="" who="" is="" assigned="" to="" your="" request=""&gt; [！UICONTROL已分配给您的请求]：“&lt;request name=""&gt;"</em></p> <p>每日摘要通知的主题是：<em> [！UICONTROL您的请求摘要] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>问题名称<br>项目名称<br>问题参考号<br>请求名称<br>请求类型<br>输入日期<br>问题优先级<br>主要联系人<br>计划完成日期<br>问题状态<br><strong>查看更多详细信息</strong> 按钮 <br>*项目名称<br>*项目参考号<br>*分配的请求总数<br>*请求名称<br>*指定给姓名<br>*每日摘要日期</p> </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我创建项目的状态更改</strong> </p> <p>项目状态更改时，创建项目的用户会收到电子邮件通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL项目状态更改]： &lt;project name=""&gt;</em></p> <p>每日摘要通知的主题是：<em> [！UICONTROL您的请求摘要] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>项目名称<br>Portfolio名称<br>项目参考号<br>更改状态的用户的名称<br>新建状态<br>项目状态更改的日期和时间<br>上一个项目状态<br><strong>[！UICONTROL查看更多详细信息]</strong> 按钮<br>*项目名称<br>*项目参考号<br>*项目新状态<br>*更改项目状态的用户的名称<br>*每日摘要日期</p> </td> 
   <td> <p><strong>即时</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我的请求上的状态更改</strong> </p> <p>问题主要联系人会在问题状态更改时收到电子邮件通知，除非更改状态的用户同时也是主要联系人。</p> <p>仅当项目状态为“当前”并且项目设置为[！UICONTROL帮助请求队列]（如中所述）时，才会发送通知 <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[！UICONTROL创建请求队列]</a>)。</p> <p>即时通知电子邮件的主题是： <em>&lt;request name=""&gt; 是 &lt;new status=""&gt;</em></p> <p>每日摘要通知的主题是：<em> 您的请求的摘要 &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> 请求名称<br>项目名称<br>请求参考号<br>更改请求状态的用户的名称<br>新建状态<br>请求状态更改的日期和时间<br>上一个请求状态<br><strong>[！UICONTROL查看更多详细信息]</strong> 按钮<br>*项目名称<br>*项目参考号<br>*状态已更改的请求总数<br>*请求名称<br>*上一个请求状态<br>*新请求状态<br>*更改了状态的用户的名称<br>*每日摘要的日期<br></td> 
   <td> <p><strong>每日</strong> </p> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>
