---
content-type: reference
navigation-topic: notifications
title: '通知：审批信息'
description: 以下通知提醒您有关您参与的工作项中发生的批准活动。 有关配置您收到的通知的信息，请参阅修改您自己的电子邮件通知。
author: Lisa
feature: Get Started with Workfront
exl-id: e152913e-de7e-405f-af63-827a9b91e2ae
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 0%

---

# 通知：审批信息

以下通知提醒您有关您参与的工作项中发生的批准活动。 有关配置您收到的通知的信息，请参阅[修改您自己的电子邮件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。

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
   <td> <p><strong>委托的问题审批请求已完成</strong> </p> <p>您委托给另一个用户的问题批准已被该用户批准或拒绝。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL 由] &lt;用户名&gt;</em>代表您作出的问题批准/拒绝</p> <p>每日摘要通知的主题是：<em> [!UICONTROL 审批信息摘要] &lt;每日摘要的日期&gt;</em></p> </td> 
   <td> <p>问题名称<br>项目名称<br>问题参考编号<br>代表您批准/拒绝问题的用户名称<br>批准决定<br>问题状态<br>请求批准的用户的名称<br><strong>[!UICONTROL 查看更多详细信息]</strong>按钮<br>*项目参考编号<br>*项目名称<br>*委托的问题审批总数<br>*问题名称<br>*审批者名称<br>*每日摘要的日期<br><br></p> </td> 
   <td><strong>每天</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>委托的项目审批请求已完成</strong> </p> <p>您委托给另一个用户的项目审批已被该用户批准或拒绝。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL 由] &lt;用户名&gt;</em>代表您作出的项目批准/拒绝</p> <p><em>每日摘要通知的主题是：[!UICONTROL 审批信息摘要] &lt;每日摘要的日期&gt;</em> </p> </td> 
   <td> 项目名称<br>[!UICONTROL Portfolio名称]<br>[!UICONTROL 项目参考编号]<br>代表您批准/拒绝项目的用户名称<br>[!UICONTROL 批准决定]<br>[!UICONTROL 项目状态]<br>请求批准的用户名称<br><strong>[!UICONTROL 查看更多详细信息]</strong> button<br>*项目参考编号<br>*项目名称<br>*批准者名称<br> 1&rbrace;[!UICONTROL *每日摘要的日期]<br></td> 
   <td><strong>每天</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>委托的任务审批请求已完成</strong> </p> <p>您委托给另一个用户的任务审批已被该用户批准或拒绝。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL 由] &lt;用户名&gt;</em>代表您作出的任务批准/拒绝</p> <p>每日摘要通知的主题是：<em> [!UICONTROL 审批信息摘要] &lt;每日摘要的日期&gt;</em></p> </td> 
   <td> 任务名称<br>项目名称<br>任务参考编号<br>代表您批准/拒绝任务的用户的名称<br>批准决定<br>任务状态<br>请求批准的用户的名称<br><strong>查看更多详细信息</strong>按钮<br>*项目参考编号<br>*项目名称<br>*委托任务审批总数<br>*任务名称<br>*批准者姓名<br>*每日摘要日期<br></td> 
   <td><strong>每天</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>文档审批请求已取消</strong> </p> <p>文档审批请求被取消时，文档的文档审批者会收到电子邮件通知。</p> <p>即时通知电子邮件的主题是： <em>&lt;用户名&gt; [!UICONTROL 已取消文档审批请求]</em></p> <p> <p>注意：您无法为每日摘要电子邮件配置此通知。</p> </p> </td> 
   <td> 取消审批请求的用户的名称<br>[!UICONTROL 文档名称] </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我被委托为批准者</strong> </p> <p>如果有人向您委托审批，您将收到电子邮件通知。 </p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL Delegated] &lt;Object Type&gt; [!UICONTROL Approval - Please Review] &lt;Object Name&gt;</em></p> <p> <p>注意：您无法为每日摘要电子邮件配置此通知。</p> </p> </td> 
   <td> <p>[!UICONTROL 对象名称]<br>[!UICONTROL 父对象名称]<br>[!UICONTROL 对象参考编号]<br>提交对象以供审批的用户名称<br>您代表其审批对象的用户名称<br>对象状态<br>请求审批的日期和时间<br>对象优先级<br>审批步骤名称<br>[!UICONTROL 规划完成日期]对象<br><strong>[!UICONTROL 进行审批决策]</strong>按钮</p> </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我的工时表已被批准</strong> </p> <p>您的时间表获得批准后，您将收到电子邮件通知。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL 已批准工时表]：&lt;工时表开始日期&gt; - &lt;工时表结束日期&gt;</em></p> <p> <p>注意：您无法为每日摘要电子邮件配置此通知。</p> </p> </td> 
   <td> 批准您的时间表的用户的名称<br>批准时间表的日期和时间<br>时间表状态（[!UICONTROL 已批准]）<br>时间表的开始日期和结束日期<br>时间表记录的总小时数<br>时间表记录的加班小时数 </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
 </tbody> 
</table>
