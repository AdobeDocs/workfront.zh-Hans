---
content-type: reference
navigation-topic: notifications
title: “通知：所需操作'
description: 以下通知可告知您是否需要对工作项执行操作。 有关配置接收的通知的信息，请参阅激活或停用您自己的事件通知。
author: Lisa
feature: Get Started with Workfront
exl-id: dd383bd4-da30-45ea-889e-e6b49416974b
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '2446'
ht-degree: 4%

---

# 通知： [!UICONTROL 所需操作]

以下通知可告知您是否需要对工作项执行操作。 有关配置接收的通知的信息，请参阅 [激活或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>我获得新工作请求</strong> </p> <p>工作项的被分派人会收到电子邮件通知，除非提出请求的用户也是被分派人。 </p> <p>如果任务状态为[!UICONTROL Complete]或问题状态为[!UICONTROL Closed]，则不会发送通知。</p> <p>拥有[!UICONTROL Review]或[!UICONTROL Requestor]许可证的用户不会收到通知。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL New Work Request]: &lt;request name=""&gt;</em></p> <p>每日摘要通知的主题是： <em>[!UICONTROL所需操作摘要] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>任务名称</p> <p>[!UICONTROL计划完成日期]</p> <p>父项</p> <p>分配者</p> <p>任务负责人</p> <p>[!UICONTROL状态]</p> <p>[!UICONTROL描述]</p> <p>[!UICONTROL视图]按钮<br>添加到每日摘要的选项</p> <br> </td> 
   <td><strong>即时和</strong> <strong>每日</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>我需要审批一个文档</strong> </p> <p>文档的审批者在列为审批者时会收到通知。</p> <p>即时通知电子邮件的主题是： <em>&lt;name of="" the="" user="" who="" submitted="" the="" approval=""&gt; [!UICONTROL要求您批准 [!DNL Adobe Workfront].]</em></p> <p>每日摘要通知的主题是：<em> [!UICONTROL所需操作摘要] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> 项目名称<br>Portfolio名称<br>提交批准的用户的名称<br>文档名称<br>文档参考编号<br>请求的批准日期和时间<br>文档详细信息（格式、大小、版本号）<br><strong>[!UICONTROL做出批准决策]</strong> 按钮<br>*待批准文档的总数<br>*链接至 <strong>[!UICONTROL文档批准</strong>*<strong>请参阅所有批准]</strong> 按钮<br>*每日摘要的日期<br></td> 
   <td><strong>即时和每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>当一个项目未决批准时，发送电子邮件给批准者</strong> </p> <p>在作业角色审批时，哪些用户会收到此事件的电子邮件通知取决于是否启用了“[!UICONTROL审批者不需要加入项目团队（对于包含角色的审批流程）]”设置(如 <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">配置全局批准设置</a>)。 </p> <p><strong>如果已启用此选项</strong>，则会向系统中具有与批准关联作业角色的所有用户发送电子邮件通知。 </p> <p><strong>如果禁用此选项</strong>，则只有具有与批准流程关联的作业角色的项目团队成员才会收到电子邮件通知。</p> <p>如果批准与用户关联，则该用户将收到通知。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL项目待批准]: &lt;project name=""&gt;</em></p> <p> 每日摘要通知的主题是： <em> [!UICONTROL所需操作摘要] &lt;date of="" the="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>项目名称<br>Portfolio名称<br>项目参考编号<br>提交批准的用户名<br>待批准状态<br>请求的批准日期和时间<br>项目优先级<br>审批步骤待批<br>等待批准的决定数<br>批准者名称（仅限用户）<br>[!UICONTROL项目计划完成日期] <br><strong>[!UICONTROL做出批准决策]</strong> 按钮<br>*待批项目总数 <br>*链接至 <strong>[!UICONTROL项目批准]</strong><br>*<strong>[!UICONTROL查看所有批准]</strong> 按钮<br>*每日摘要的日期</p> </td> 
   <td><strong>即时和每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>当一个任务未决批准时，发送电子邮件给批准者</strong> </p> <p>在作业角色审批时，哪些用户会收到此事件的电子邮件通知取决于是否启用了“[!UICONTROL审批者不需要加入项目团队（对于包含角色的审批流程）]”设置(如 <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">配置全局批准设置</a>)。 </p> <p><strong>如果已启用此选项</strong>，则会向系统中具有与批准关联作业角色的所有用户发送电子邮件通知。 </p> <p><strong>如果禁用此选项</strong>，则只有具有与批准流程关联的作业角色的项目团队成员才会收到电子邮件通知。</p> <p>如果批准与用户关联，则该用户将收到通知。 </p> <p>仅当项目状态为[!UICONTROL Current]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL任务待批准]: &lt;task name=""&gt;</em></p> <p> 每日摘要通知的主题是： <em> [!UICONTROL所需操作摘要] &lt;date of="" the="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>任务名称<br>项目名称<br>提交批准的用户的名称<br>待批准状态<br>请求的批准日期和时间<br>任务优先级<br>批准阶段名称<br>批准者名称<br>[!UICONTROL任务计划完成日期]<br><strong>[!UICONTROL做出批准决策]</strong> 按钮<br>*待批准任务的总数<br>*链接至<strong>[!UICONTROL任务批准*请参阅所有批准]</strong> 按钮<strong></strong>*每日摘要的日期<br></p> </td> 
   <td><strong>即时和每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在提交工时表之后，发送电子邮件给批准者</strong> </p> <p>在提交需要批准的时间表时，时间表审批者会收到电子邮件通知，除非提交时间表的用户也是时间表审批者。</p> <p>仅当时间表的状态为[!UICONTROL Submitted]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL已提交时间表]: &lt;timesheet owner=""&gt;, &lt;timesheet start="" date=""&gt; - &lt;timesheet end="" date=""&gt;</em></p> <p> 每日摘要通知的主题是： <em> [!UICONTROL所需操作摘要] &lt;date of="" the="" daily="" digest=""&gt; </em></p> </td> 
   <td> 提交工时单以供审批的用户的名称<br>提交时间表的日期和时间<br>时间表的状态<br>工时单的开始和结束日期<br>工时单上记录的小时数<br>工时单上记录的超时小时数<br><strong>[!UICONTROL Review]</strong> 和 <strong>[!UICONTROL Approve]</strong> 按钮<br>*待处理时间表审批的总数<br>*链接至 <strong>[!UICONTROL时间表批准]</strong><br><strong>[!UICONTROL *请参阅“所有批准”]</strong> 按钮<br>*每日摘要的日期 </td> 
   <td><strong>即时和</strong> <strong>每日</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>当一个问题未决批准时，发送电子邮件给批准者</strong> </p> <p>在作业角色审批时，哪些用户会收到此事件的电子邮件通知取决于是否启用了“[!UICONTROL审批者不需要加入项目团队（对于包含角色的审批流程）]”设置(如 <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">[!UICONTROL配置全局批准]设置</a>)。 </p> <p><strong>如果已启用此选项</strong>，则会向系统中具有与批准关联作业角色的所有用户发送电子邮件通知。 </p> <p><strong>如果禁用此选项</strong>，则只有具有与批准流程关联的作业角色的项目团队成员才会收到电子邮件通知。</p> <p>如果批准与用户关联，则该用户将收到通知。 </p> <p>仅当项目状态为[!UICONTROL Current]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL问题待批准]: &lt;issue name=""&gt;</em></p> <p> 每日摘要通知的主题是： <em> [!UICONTROL所需操作摘要] &lt;date of="" the="" daily="" digest=""&gt; </em></p> </td> 
   <td> 问题名称<br>项目名称<br>问题参考编号<br>提交问题以供审批的用户的名称<br>待批准状态<br>请求的批准日期和时间<br>问题优先级<br>审批阶段<br>批准者的名称<br>[!UICONTROL问题计划完成日期]<br>[!UICONTROL主要联系人]<br><strong>[!UICONTROL做出批准决策]</strong> 按钮<br>*待批准问题的总数<br>*链接至 <strong>[!UICONTROL Issue Approvals]</strong><br><strong>[!UICONTROL *请参阅“所有批准”]</strong> 按钮<br>*每日摘要的日期 </td> 
   <td><strong>即时和</strong> <strong>每日</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>我需要回顾委托给我的项目审批</strong> </p> <p>项目批准已委派给您，您需要对其进行审核。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL委派项目批准 — 请查看] &lt;project name=""&gt;</em></p> <p><em>每日摘要通知的主题是：[!UICONTROL所需操作摘要] &lt;date of="" the="" daily="" digest=""&gt;</em> </p> </td> 
   <td> 项目名称<br>Portfolio名称<br>项目参考编号<br>请求批准的用户的名称<br>您代表其批准项目的用户的名称<br>待批准状态<br>请求的批准日期和时间<br>项目优先级<br>批准步骤<br>批准者的名称<br>[!UICONTROL项目计划完成日期]<br><strong>[!UICONTROL做出批准决策]</strong> 按钮<br>*待批项目总数<br>*链接至 <strong>[!UICONTROL项目批准*请参阅所有批准]</strong> 按钮 <br>*每日摘要的日期 </td> 
   <td><strong>即时和每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我需要回顾委托给我的任务审批</strong> </p> <p>已将任务批准委派给您，您需要对其进行审核。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL委派任务批准 — 请查看]&lt;task name=""&gt;</em></p> <p>每日摘要通知的主题是：<em> [!UICONTROL所需操作摘要] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> 任务名称<br>项目名称<br>任务参考编号<br>请求批准的用户的名称<br>您代表其批准任务的用户的名称<br>待批准状态<br>请求的批准日期和时间<br>任务优先级<br>审批阶段<br>批准者的名称<br>[!UICONTROL任务计划完成日期]<br><strong>[!UICONTROL做出批准决策]</strong> 按钮 <br>*待批准任务的总数<br>*链接至 <strong>[!UICONTROL任务批准*请参阅所有批准]</strong> 按钮<br>*每日摘要的日期 </td> 
   <td><strong>即时和每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我需要回顾委托给我的问题审批</strong> </p> <p>已将问题批准委派给您，您需要对其进行审核。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL委派的问题批准 — 请查看] &lt;issue name=""&gt;</em></p> <p>每日摘要通知的主题是：<em> [!UICONTROL所需操作摘要] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> 问题名称<br>项目名称<br>问题参考编号<br>请求批准的用户的名称<br>您代表其批准问题的用户的名称<br>待批准状态<br>请求的批准日期和时间<br>问题优先级<br>审批阶段<br>批准者的名称<br>发行计划完成日期<br>主要联系人<br><strong>[!UICONTROL做出批准决策]</strong> 按钮<br>*待批准问题的总数<br>*链接至 <strong>[!UICONTROL Issue Approvals]</strong><br><strong>[!UICONTROL *请参阅“所有批准”]</strong> 按钮<br>*每日摘要的日期<br></td> 
   <td><strong>即时和每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在问题分派更改之后，发送电子邮件给新分派用户</strong> </p> <p>问题代理人收到电子邮件通知。 如果问题的状态与[!UICONTROL Closed]相等，则问题代理人不会收到电子邮件。</p> <p>拥有[!UICONTROL Review]或[!UICONTROL Requestor]许可证的用户不会收到通知。</p> <p>仅当项目状态为[!UICONTROL Current]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL New Work Request]: &lt;issue name=""&gt;</em></p> <p>每日摘要通知的主题是：<em> [!UICONTROL所需操作摘要] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>问题名称<br>项目名称<br>[!UICONTROL问题参考编号]<br>您的姓名<br>发出到期日期（[!UICONTROL计划完成日期]）<br>将问题分配给您的用户的名称<br><strong>[!UICONTROL Work It]</strong> 按钮<br>*分配总数<br>*分配给您的任务和问题总数<br>*链接至 <strong>[!UICONTROL工作请求]</strong><br>*每日摘要的日期<br></p> </td> 
   <td><strong>即时和每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在任务主分派更改之后，发送电子邮件给新分派用户</strong> </p> <p>如果任务受分配人被设为任务的主要受分配人，则任务受分配人会收到电子邮件通知，除非该受分配人是进行分配的用户。</p> <p>如果项目状态为[!UICONTROL Current]且该任务未标记为[!UICONTROL Complete]，则会发送通知。</p> <p>拥有[!UICONTROL Review]或[!UICONTROL Requestor]许可证的用户不会收到通知。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL New Work Request]: &lt;task name=""&gt;</em></p> <p>每日摘要通知的主题是：<em> [!UICONTROL所需操作摘要] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> 任务名称<br>项目名称<br>任务参考编号<br>您的姓名<br>任务到期日期（[!UICONTROL计划完成日期]）<br>将任务分配给您的用户的名称<br><strong>[!UICONTROL Work It]</strong> 按钮<br>*分配给您的任务和问题总数<br>*链接至 <strong>[!UICONTROL工作请求]</strong>*每日摘要的日期 </td> 
   <td><strong>即时和每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我的团队获得了新的工作请求</strong> </p> <p>团队成员在团队收到新的工作请求时会收到电子邮件通知。 （如果提交请求的用户是团队成员，则该用户不会收到通知。）</p> <p>仅当项目状态为[!UICONTROL Current]且工作请求状态为[!UICONTROL New]时，才会发送通知。</p> <p>拥有[!UICONTROL Review]许可证的用户不会收到通知。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL New Work Request]: &lt;request name=""&gt;</em></p> <p>每日摘要通知的主题是： <em>[!UICONTROL所需操作摘要] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p> 问题名称<br>项目名称（请求队列名称）<br>问题参考编号<br>团队名称<br>发行到期日（计划完成日期）<br>提交请求的用户的名称<br><strong>[!UICONTROL Work It]</strong> 按钮<br>*分配给您的团队的请求总数</p> <p>*工作请求名称</p> <p>[!UICONTROL *计划完成日期]</p> <p>*提交请求的用户名<br>*链接至 <strong>[!UICONTROL团队请求]</strong><br>*每日摘要的日期 </p> <p><span class="preview">*团队分配</span> </p> </td> 
   <td><strong>即时和每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我的工时表已重新开立</strong> </p> <p>重新打开时间表时，“时间表所有者”会收到一封电子邮件通知，除非重新打开时间表的用户也是时间表的所有者。</p> <p>仅当时间表状态为[!UICONTROL Open]时，才会发送电子邮件通知。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL重新打开时间表]: &lt;timesheet start="" date=""&gt; - &lt;timesheet end="" date=""&gt;</em></p> <p>注意：您无法为每日摘要电子邮件配置此通知。</p> </td> 
   <td> 重新打开工时单的用户的名称<br>重新打开工时单的日期和时间<br>时间表的状态（[!UICONTROL重新打开]）<br>工时单上记录的总小时数<br>工时单上记录的超时小时数<br><strong>[!UICONTROL Review]</strong> 按钮 </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在拒绝工时表之后，发送电子邮件给用户</strong> </p> <p>工时单所有者在工时单被拒绝时会收到电子邮件通知，除非拒绝工时单的用户也是所有者。</p> <p>仅当时间表状态为[!UICONTROL Rejected]时，才会发送电子邮件通知。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL已拒绝时间表]:&lt;start date="" of="" the="" timesheet=""&gt; - &lt;end date="" of="" the="" timesheet=""&gt;</em></p> <p>注意：您无法为每日摘要电子邮件配置此通知。</p> </td> 
   <td> 拒绝工时单的用户的名称<br>时间表的状态([!UICONTROL Rejected])<br>拒绝时间表的日期和时间<br><strong>[!UICONTROL Review]</strong> 按钮 </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>某人向我请求访问权限</strong> </p> <p>让我做点事，那就打开。</p> <p>项目创建者有权访问该项目。</p> <p>这是当用户请求访问时，用户收到通知的原因。</p> <p>即时通知电子邮件的主题是： <em>&lt;name of="" user="" who="" requested="" the="" access=""&gt; [!UICONTROL需要访问] &lt;object name=""&gt;</em></p> <p>每日摘要通知的主题是：<em> [!UICONTROL所需操作摘要] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>对象名称<br>父对象名称<br>对象引用编号<br>请求访问的用户的名称<br>用户请求的访问类型<br><strong>[!UICONTROL授予] &lt;name of="" the="" access="" requested=""&gt; 访问</strong> 和 <strong>[!UICONTROL授予不同的访问权限]</strong> 按钮<br>*待批准访问请求的总数<br>*链接至 <strong>[!UICONTROL访问请求]</strong> 批准<br>*每日摘要日期</p> </td> 
   <td><strong>即时和每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>有人要求我上传一份文档</strong> </p> <p>当用户收到上载文档的请求时，文档请求会收到电子邮件通知。</p> <p>即时通知电子邮件的主题是： <em>&lt;name of="" the="" user="" requesting="" the="" document=""&gt; [!UICONTROL需要您在 [!DNL Workfront].]</em></p> <p> <p>注意：您无法为每日摘要电子邮件配置此通知。</p> </p> </td> 
   <td> 请求文档的用户的名称<br>应将文档上载到的对象的名称<br><strong>[!UICONTROL将其附加到此处]</strong> 链接 </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
 </tbody> 
</table>
