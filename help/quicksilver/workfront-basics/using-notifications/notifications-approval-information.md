---
content-type: reference
navigation-topic: notifications
title: “通知：审批信息'
description: 以下通知会提醒您有关涉及的工作项目中正在进行的批准活动。 有关配置接收的通知的信息，请参阅激活或停用您自己的事件通知。
author: Lisa
feature: Get Started with Workfront
exl-id: e152913e-de7e-405f-af63-827a9b91e2ae
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 6%

---

# 通知：审批信息

以下通知会提醒您有关涉及的工作项目中正在进行的批准活动。 有关配置接收的通知的信息，请参阅 [激活或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>已完成委托的问题审批请求</strong> </p> <p>您委派给其他用户的问题批准已被该用户批准或拒绝。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL发布批准/拒绝代表您发布] &lt;user name=""&gt;</em></p> <p>每日摘要通知的主题是：<em> [!UICONTROL审批信息摘要] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>问题名称<br>项目名称<br>问题参考编号<br>代表您批准/拒绝此问题的用户的名称<br>批准决定<br>问题状态<br>请求批准的用户的名称<br><strong>[!UICONTROL请参阅更多详细信息]</strong> 按钮<br>*项目参考编号<br>*项目名称<br>*委派的发行批准总数<br>*问题名称<br>*审批者姓名<br>*每日摘要的日期<br><br></p> </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>已完成委托的项目审批请求</strong> </p> <p>您委派给其他用户的项目批准已被该用户批准或拒绝。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL项目代表您批准/拒绝] &lt;user name=""&gt;</em></p> <p><em>每日摘要通知的主题是：[!UICONTROL审批信息摘要] &lt;date of="" daily="" digest=""&gt;</em> </p> </td> 
   <td> 项目名称<br>[!UICONTROLPortfolio名称]<br>[!UICONTROL项目引用编号]<br>代表您批准/拒绝项目的用户的名称<br>[!UICONTROL批准决策]<br>[!UICONTROL项目状态]<br>请求批准的用户的名称<br><strong>[!UICONTROL请参阅更多详细信息]</strong> 按钮<br>*项目参考编号<br>*项目名称<br>*审批者姓名<br>[!UICONTROL *每日摘要的日期]<br></td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>已完成委托的任务审批请求</strong> </p> <p>您委派给其他用户的任务批准已被该用户批准或拒绝。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL任务批准/拒绝由]代表您作出 &lt;user name=""&gt;</em></p> <p>每日摘要通知的主题是：<em> [!UICONTROL审批信息摘要] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 任务名称<br>项目名称<br>任务参考编号<br>代表您批准/拒绝任务的用户的名称<br>批准决定<br>任务状态<br>请求批准的用户的名称<br><strong>查看更多详细信息</strong> 按钮<br>*项目参考编号<br>*项目名称<br>*已委派任务批准的总数<br>*任务名称<br>*审批者姓名<br>*每日摘要的日期<br></td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>文档审批请求已取消</strong> </p> <p>文档的文档审批者在文档审批请求被取消时会收到电子邮件通知。</p> <p>即时通知电子邮件的主题是： <em>&lt;user name=""&gt; [!UICONTROL已取消文档批准请求]</em></p> <p> <p>注意：您无法为每日摘要电子邮件配置此通知。</p> </p> </td> 
   <td> 已取消批准请求的用户的名称<br>[!UICONTROL文档名称] </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我被委托为批准者</strong> </p> <p>如果某人向您委派了批准，您会收到电子邮件通知。 </p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL Delegated] &lt;object type=""&gt; [!UICONTROL批准 — 请查看] &lt;object name=""&gt;</em></p> <p> <p>注意：您无法为每日摘要电子邮件配置此通知。</p> </p> </td> 
   <td> <p>[!UICONTROL对象名称]<br>[!UICONTROL父对象名称]<br>[!UICONTROL对象引用编号]<br>提交对象以供审批的用户名称<br>您代表其批准对象的用户的名称<br>对象状态<br>请求批准的日期和时间<br>对象优先级<br>批准步骤名称<br>对象的[!UICONTROL计划完成日期]<br><strong>[!UICONTROL做出批准决策]</strong> 按钮</p> </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在接受和关闭工时表之后，发送电子邮件给用户</strong> </p> <p>您的时间表获得批准后，您会收到一封电子邮件通知。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL Timeske Approved]: &lt;timesheet start="" date=""&gt; - &lt;timesheet end="" date=""&gt;</em></p> <p> <p>注意：您无法为每日摘要电子邮件配置此通知。</p> </p> </td> 
   <td> 批准工时单的用户名称<br>时间表获得批准的日期和时间<br>时间表状态([!UICONTROL Approved])<br>工时单的开始日期和结束日期<br>工时单中记录的总时数<br>工时单中记录的超时时间 </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
 </tbody> 
</table>
