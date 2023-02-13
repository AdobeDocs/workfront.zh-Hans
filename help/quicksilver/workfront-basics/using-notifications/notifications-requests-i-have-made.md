---
content-type: reference
navigation-topic: notifications
title: “通知：我提出的请求'
description: 以下通知可告知您在Adobe Workfront中发出的请求。
author: Lisa
feature: Get Started with Workfront
exl-id: 42771f71-dbf8-4e73-9a0e-8efea612af4a
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1429'
ht-degree: 6%

---

# 通知：我提出的请求

以下通知可告知您在 [!DNL Adobe Workfront].

有关配置接收的通知的信息，请参阅 [激活或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>文档审批请求已完成</strong> </p> <p>在文档批准请求完成时，请求对文档进行批准的用户会收到电子邮件通知。</p> <p>即时通知电子邮件的主题是：<em> &lt;approver name=""&gt; has &lt;approval decision="" uicontrol="" approved="" uicontrol="" approved="" with="" changes="" uicontrol="" rejected=""&gt; 本文档。</em></p> <p>注意：您无法为每日摘要电子邮件配置此通知。</p> </td> 
   <td> 文档名称<br>审批者姓名 </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>与我作为主要联系人的问题相关的文档已更改或上载</strong> </p> <p>在文档上传或更改时，问题的主要联系人会收到电子邮件通知，除非上传或更改文档的用户也是主要联系人。</p> <p>仅当项目设置为[!UICONTROL帮助请求队列]时，才会发送通知(如 <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL创建请求队列]</a>)。</p> <p>即时通知电子邮件的主题是： <em>文档已添加到 &lt;issue name=""&gt;</em></p> <p>每日摘要通知的主题是： <em>请求摘要 &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> 对象上传文档的名称<br>父对象名称<br>文档参考编号<br>上传文档的用户的名称<br>文档名称<br>添加日期<br>文档详细信息（格式、大小、版本号）<br>文档缩略图<br><strong>[!UICONTROL预览]</strong> 和 <strong>[!UICONTROL下载]</strong> 按钮<br>*项目名称<br>*项目参考编号<br>*上传的文档总数<br>*文档名称<br>*父对象名称<br>*添加文档的用户名称<br>*每日摘要的日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>要求上传一份文档已实现</strong> </p> <p>文档请求者在文档上传请求得到满足时会收到电子邮件通知。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL从]发出文档请求 &lt;user name=""&gt; 已完成</em></p> <p>注意：您无法为每日摘要电子邮件配置此通知。</p> </td> 
   <td> <p>上传文档的用户的名称<br>对象上传文档的名称<br>文档名称<br><br></p> </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我已分配至某人的个人任务已完成</strong> </p> <p>当该任务完成时，系统会向为其他人分配临时任务的用户发出通知。 </p> <p>有关临时任务的更多信息，请参阅 <a href="../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md" class="MCXref xref">从[!UICONTROL Home]区域创建工作项</a>.</p> <p>即时通知电子邮件的主题是： <em>任务完成： &lt;task name=""&gt;</em></p> <p> <p>注意：您无法为每日摘要电子邮件配置此通知。</p> </p> </td> 
   <td> 任务名称<br>默认项目名称（接收个人任务的用户的个人项目）<br>任务参考编号<br>任务所有者名称<br>新任务状态<br>任务完成的日期和时间<br>上一任务状态<br><strong>[!UICONTROL请参阅更多详细信息]</strong> 按钮<br><br><br></td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在完成问题之后，发送电子邮件给问题创建者。</strong> </p> <p>问题的主要联系人在问题完成时会收到通知。</p> <p>仅当项目状态为[!UICONTROL Current]或[!UICONTROL Planning]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL问题完成]: &lt;issue name=""&gt;</em></p> <p>每日摘要通知的主题是：<em> 请求摘要 &lt;date of="" the="" daily="" digest=""&gt;</em></p> <p> </p> </td> 
   <td> 问题名称<br>项目名称<br>问题参考编号<br>完成问题的用户的名称<br>新状态<br>问题完成的日期和时间<br>上一问题状态<br><strong>[!UICONTROL请参阅更多详细信息]</strong> 按钮 <br>*项目名称<br>*项目参考编号<br>*已完成的问题总数<br>*问题名称<br>*完成问题的用户的姓名<br>*每日摘要日期 </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在添加问题之后，发送电子邮件给问题创建者。</strong> </p> <p>当某个问题的主要联系人在项目中添加问题时，该联系人会收到通知。</p> <p>仅当项目状态为[!UICONTROL Current]或[!UICONTROL Planning]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL问题已提交]: &lt;issue name=""&gt; on &lt;project name=""&gt;</em></p> <p>每日摘要通知的主题是：<em> 请求摘要 &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> 项目名称<br>Portfolio名称<br>问题参考编号<br>您的姓名<br>问题名称<br>输入日期<br>问题优先级<br>问题状态<br>分配给名称<br>主要联系人<br>*项目名称<br>*项目参考编号<br>*添加的问题总数<br>*问题名称<br>*每日摘要日期 </td> 
   <td> <p><strong>即时</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我提交请求 (确认)</strong> </p> <p>问题的主要联系人在提交问题时会收到电子邮件通知。</p> <p>仅当项目状态为[!UICONTROL Current]且项目设置为[!UICONTROL帮助请求队列]时(如 <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL创建请求队列]</a>)。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL请求已提交]: &lt;request name=""&gt; on &lt;project request="" queue="" name=""&gt;</em></p> <p>每日摘要通知的主题是：<em> 请求摘要 &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>项目名称（请求队列名称）<br>Portfolio名称<br>问题参考编号<br>问题名称<br>输入日期<br>问题优先级<br>问题状态<br>分配给名称<br>主要联系人<br>*项目参考编号<br>*项目名称<br>*提交的请求总数<br>*请求名称<br>*请求优先级<br>*每日摘要日期</p> </td> 
   <td> <p><strong>即时</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我的请求已关闭 (确认)</strong> </p> <p>请求关闭后，问题的主要联系人会收到电子邮件通知。</p> <p>仅当项目状态为“当前”且项目设置为[!UICONTROL帮助请求队列]时(如 <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">创建请求队列</a>)。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL您的请求已关闭]:"&lt;request name=""&gt;"</em></p> <p>每日摘要通知的主题是：<em> [!UICONTROL请求摘要] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> 请求名称<br>项目名称<br>请求引用编号<br>关闭请求的用户的名称<br>问题状态<br>请求关闭的日期和时间<br>上一个请求状态<br><strong>[!UICONTROL请参阅更多详细信息]</strong> 按钮<br>*项目参考编号<br>*项目名称<br>*已结束的请求总数<br>*请求名称<br>*关闭请求的用户的名称<br>*每日摘要日期 </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>分派某人给我的请求</strong> </p> <p>问题的主要联系人在将用户分配到问题时会收到电子邮件通知，除非主要联系人和分配的用户是同一用户。</p> <p>仅当项目状态为“当前”且项目设置为[!UICONTROL帮助请求队列]时(如 <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL创建请求队列]</a>)。</p> <p>即时通知电子邮件的主题是： <em>&lt;name of="" the="" user="" who="" is="" assigned="" to="" your="" request=""&gt; [!UICONTROL已分配给您的请求]:"&lt;request name=""&gt;"</em></p> <p>每日摘要通知的主题是：<em> [!UICONTROL请求摘要] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>问题名称<br>项目名称<br>问题参考编号<br>请求名称<br>请求类型<br>输入日期<br>问题优先级<br>主要联系人<br>计划完成日期<br>问题状态<br><strong>查看更多详细信息</strong> 按钮 <br>*项目名称<br>*项目参考编号<br>*分配的请求总数<br>*请求名称<br>*分配给名称<br>*每日摘要日期</p> </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>当项目状态更改时，向输入项目的用户发送电子邮件</strong> </p> <p>创建项目的用户在项目状态发生更改时会收到电子邮件通知。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL项目状态更改]: &lt;project name=""&gt;</em></p> <p>每日摘要通知的主题是：<em> [!UICONTROL请求摘要] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>项目名称<br>Portfolio名称<br>项目参考编号<br>更改了状态的用户的名称<br>新状态<br>项目状态更改的日期和时间<br>上一个项目状态<br><strong>[!UICONTROL请参阅更多详细信息]</strong> 按钮<br>*项目名称<br>*项目参考编号<br>*项目新状态<br>*更改项目状态的用户名称<br>*每日摘要日期</p> </td> 
   <td> <p><strong>即时</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我的请求上的状态更改</strong> </p> <p>问题的主要联系人在问题状态发生更改时会收到电子邮件通知，除非更改了状态的用户也是主要联系人。</p> <p>仅当项目状态为“当前”且项目设置为[!UICONTROL帮助请求队列]时，才会发送通知(如 <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL创建请求队列]</a>)。</p> <p>即时通知电子邮件的主题是： <em>&lt;request name=""&gt; is &lt;new status=""&gt;</em></p> <p>每日摘要通知的主题是：<em> 请求摘要 &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> 请求名称<br>项目名称<br>请求引用编号<br>更改请求状态的用户的名称<br>新状态<br>请求状态发生更改的日期和时间<br>上一个请求状态<br><strong>[!UICONTROL请参阅更多详细信息]</strong> 按钮<br>*项目名称<br>*项目参考编号<br>*状态发生更改的请求总数<br>*请求名称<br>*以前的请求状态<br>*新请求状态<br>*更改了状态的用户名称<br>*每日摘要的日期<br></td> 
   <td> <p><strong>每日</strong> </p> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>
