---
content-type: reference
navigation-topic: notifications
title: '通知：需要操作'
description: 通过下面的通知，您可以了解是否需要针对工作项采取行动。 有关配置您收到的通知的信息，请参阅修改您自己的电子邮件通知。
author: Lisa
feature: Get Started with Workfront
exl-id: dd383bd4-da30-45ea-889e-e6b49416974b
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '2442'
ht-degree: 0%

---

# 通知：[!UICONTROL 需要操作]

通过下面的通知，您可以了解是否需要针对工作项采取行动。 有关配置您收到的通知的信息，请参阅[修改您自己的电子邮件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。

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
   <td> <p><strong>我获得新工作请求</strong> </p> <p>工作项的被分派人会收到电子邮件通知，除非提出请求的用户也是被分派人。 </p> <p>如果任务状态为[！UICONTROL完成]或问题状态为[！UICONTROL已关闭]，则不会发送通知。</p> <p>拥有[！UICONTROL Review]或[！UICONTROL Requestor]许可证的用户不会收到通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL新工作请求]： &lt;请求名称&gt;</em></p> <p>每日摘要通知的主题是： <em>[！UICONTROL需要操作的摘要] &lt;每日摘要的日期&gt;</em></p> </td> 
   <td> <p>任务名称</p> <p>[！UICONTROL计划完成日期]</p> <p>父项</p> <p>分配者</p> <p>任务负责人</p> <p>[！UICONTROL状态]</p> <p>[！UICONTROL描述]</p> <p>[！UICONTROL视图]按钮<br>添加到每日摘要的选项</p> <br> </td> 
   <td><strong>即时和</strong> <strong>每日</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>我需要审批文档</strong> </p> <p>当文档审批者被列为审批者时，他们将收到通知。</p> <p>即时通知电子邮件的主题是： <em>&lt;提交审批的用户名称&gt; [！UICONTROL要求您在[!DNL Adobe Workfront]中审批文档。]</em></p> <p>每日摘要通知的主题是：<em> [！UICONTROL需要操作的摘要] &lt;每日摘要的日期&gt;</em></p> </td> 
   <td> 项目名称<br>Portfolio名称<br>提交审批的用户名称<br>文档名称<br>文档参考编号<br>请求的审批日期和时间<br>文档详细信息（格式、大小、版本号）<br><strong>[！UICONTROL作出审批决定]</strong> button<br>*待审批文档审批总数<br>*链接到<strong>[！UICONTROL文档审批</strong>*<strong>查看所有审批]</strong> button<br>*日期每日摘要<br></td> 
   <td><strong>即时和每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我需要审批一个项目</strong> </p> <p>在审批工作角色时，哪些用户会收到此事件的电子邮件通知，这取决于“[！UICONTROL审批者不需要位于项目团队中（对于包含角色的审批流程）]”设置是否已启用（如<a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">配置全局审批设置</a>中所述）。 </p> <p><strong>如果已启用此选项</strong>，则会向系统中具有与该批准关联的工作角色的所有用户发送电子邮件通知。 </p> <p><strong>如果禁用此选项</strong>，则只有具有与审批流程关联的工作角色的项目团队成员会收到电子邮件通知。</p> <p>如果批准与某个用户相关联，则该用户会收到通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL待审批项目]： &lt;项目名称&gt;</em></p> <p> 每日摘要通知的主题是： <em> [！UICONTROL需要操作的摘要] &lt;每日摘要的日期&gt; </em></p> </td> 
   <td> <p>项目名称<br>Portfolio名称<br>项目参考编号<br>提交审批的用户名称<br>待审批状态<br>请求的审批日期和时间<br>项目优先级<br>待审批的审批步骤<br>等待审批的决策数<br>审批者姓名（仅限用户）<br>[！UICONTROL项目计划完成日期] <br><strong>[！UICONTROL作出审批决定]</strong>按钮<br>*待审批项目审批的总数{13 <strong>[！UICONTROL项目审批]</strong><br>*<strong>[！UICONTROL查看所有审批]</strong>按钮<br>*每日摘要的日期<br></p> </td> 
   <td><strong>即时和每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我需要批准任务</strong> </p> <p>在审批工作角色时，哪些用户会收到此事件的电子邮件通知，这取决于“[！UICONTROL审批者不需要位于项目团队中（对于包含角色的审批流程）]”设置是否已启用（如<a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">配置全局审批设置</a>中所述）。 </p> <p><strong>如果已启用此选项</strong>，则会向系统中具有与该批准关联的工作角色的所有用户发送电子邮件通知。 </p> <p><strong>如果禁用此选项</strong>，则只有具有与审批流程关联的工作角色的项目团队成员会收到电子邮件通知。</p> <p>如果批准与某个用户相关联，则该用户会收到通知。 </p> <p>仅当项目状态为[！UICONTROL当前]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL未决批准任务]： &lt;任务名称&gt;</em></p> <p> 每日摘要通知的主题是： <em> [！UICONTROL需要操作的摘要] &lt;每日摘要的日期&gt; </em></p> </td> 
   <td> <p>任务名称<br>项目名称<br>提交审批的用户名称<br>待审批状态<br>请求的审批日期和时间<br>任务优先级<br>审批阶段名称<br>审批者名称<br>[！UICONTROL任务计划完成日期]<br><strong>[！UICONTROL作出审批决定]</strong>按钮<br>*待审批任务审批总数<br>*链接到<strong>[！UICONTROL任务审批*请参阅所有审批]</strong>按钮<strong></strong>*每日摘要的日期<br></p> </td> 
   <td><strong>即时和每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我需要审批时间表</strong> </p> <p>在提交需要审批的时间表后，时间表审批者会收到电子邮件通知，除非提交时间表的用户也是时间表审批者。</p> <p>仅当时间表状态为[！UICONTROL已提交]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL已提交工时表]：&lt;工时表所有者&gt;，&lt;工时表开始日期&gt; - &lt;工时表结束日期&gt;</em></p> <p> 每日摘要通知的主题是： <em> [！UICONTROL需要操作的摘要] &lt;每日摘要的日期&gt; </em></p> </td> 
   <td> 提交时间表以供审批的用户名称<br>提交时间表的日期和时间<br>时间表状态<br>时间表的开始和结束日期<br>时间表上记录的小时数<br>时间表上记录的加班小时数<br><strong>[！UICONTROL审阅]</strong>和<strong>[！UICONTROL批准]</strong>按钮<br>*待处理时间表批准的总数<br>*链接到<strong>[！UICONTROL icontrol时间表审批]</strong><br><strong>[！UICONTROL *查看所有审批]</strong>按钮<br>*每日摘要的日期 </td> 
   <td><strong>即时和</strong> <strong>每日</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>我需要审批问题</strong> </p> <p>在审批工作角色时，哪些用户会收到此事件的电子邮件通知取决于“[！UICONTROL审批者不需要位于项目团队中（对于包含角色的审批流程）]”设置是否已启用（如<a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">[！UICONTROL配置全局审批]设置</a>中所述）。 </p> <p><strong>如果已启用此选项</strong>，则会向系统中具有与该批准关联的工作角色的所有用户发送电子邮件通知。 </p> <p><strong>如果禁用此选项</strong>，则只有具有与审批流程关联的工作角色的项目团队成员会收到电子邮件通知。</p> <p>如果批准与某个用户相关联，则该用户会收到通知。 </p> <p>仅当项目状态为[！UICONTROL当前]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL问题未决批准]： &lt;问题名称&gt;</em></p> <p> 每日摘要通知的主题是： <em> [！UICONTROL需要操作的摘要] &lt;每日摘要的日期&gt; </em></p> </td> 
   <td> 问题名称<br>项目名称<br>问题参考编号<br>提交问题以供审批的用户名称<br>待审批状态<br>请求的审批日期和时间<br>问题优先级<br>审批阶段<br>审批者姓名<br>[！UICONTROL问题计划完成日期]<br>[！UICONTROL主要联系人]<br><strong>[！UICONTROL作出审批决定]</strong>按钮<br>*待审批问题的总数<br>*链接到<strong>[！UICONTROL问题审批]</strong><br><strong>[！UICONTROL *查看所有审批]</strong>按钮<br>*每日摘要的日期 </td> 
   <td><strong>即时和</strong> <strong>每日</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>我需要回顾委托给我的项目审批</strong> </p> <p>项目审批委托给您，您需要对其进行审核。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL委托项目审批 — 请审核] &lt;项目名称&gt;</em></p> <p><em>每日摘要通知的主题是：[！UICONTROL需要操作的摘要] &lt;每日摘要的日期&gt;</em> </p> </td> 
   <td> 项目名称<br>Portfolio名称<br>项目参考编号<br>请求审批的用户名称<br>您代表其审批项目的用户名称<br>待审批状态<br>请求的审批日期和时间<br>项目优先级<br>审批步骤<br>审批者姓名<br>[！UICONTROL项目计划完成日期]<br><strong>[！UICONTROL作出审批决定]</strong>按钮<br>*待审批项目审批总数<br> 3}*链接到<strong>[！UICONTROL项目审批*查看所有审批]</strong>按钮<br>*每日摘要的日期 </td> 
   <td><strong>即时和每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我需要回顾委托给我的任务审批</strong> </p> <p>任务审批委托给您，您需要对其进行审核。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL委托任务审批 — 请查看]&lt;任务名称&gt;</em></p> <p>每日摘要通知的主题是：<em> [！UICONTROL需要操作的摘要] &lt;每日摘要的日期&gt;</em></p> </td> 
   <td> 任务名称<br>项目名称<br>任务参考编号<br>请求审批的用户名称<br>您代表其审批任务的用户的名称<br>待审批状态<br>请求的审批日期和时间<br>任务优先级<br>审批阶段<br>审批者姓名<br>[！UICONTROL任务计划完成日期]<br><strong>[！UICONTROL作出审批决定]</strong>按钮<br>*待审批任务的总数<br> 3}*链接到<strong>[！UICONTROL任务审批*查看所有审批]</strong>按钮<br>*每日摘要的日期 </td> 
   <td><strong>即时和每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我需要回顾委托给我的问题审批</strong> </p> <p>问题审批委托给您，您需要对其进行审核。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL委托问题审批 — 请查看] &lt;问题名称&gt;</em></p> <p>每日摘要通知的主题是：<em> [！UICONTROL需要操作的摘要] &lt;每日摘要的日期&gt;</em></p> </td> 
   <td> 问题名称<br>项目名称<br>问题参考编号<br>请求审批的用户名称<br>您代表其审批问题的用户名称<br>待审批状态<br>请求的审批日期和时间<br>问题优先级<br>审批阶段<br>审批者姓名<br>问题计划完成日期<br>主要联系人<br><strong>[！UICONTROL作出审批决定]</strong>按钮<br>*待审批问题总数{14 <strong>[！UICONTROL问题批准的链接]</strong><br><strong>[！UICONTROL *查看所有批准]</strong>按钮<br>*每日摘要的日期<br><br></td> 
   <td><strong>即时和每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我已分配到问题</strong> </p> <p>问题被分派人收到电子邮件通知。 如果问题的状态为或相当于[！UICONTROL已关闭]，则问题被分派人不会收到电子邮件。</p> <p>拥有[！UICONTROL Review]或[！UICONTROL Requestor]许可证的用户不会收到通知。</p> <p>仅当项目状态为[！UICONTROL当前]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL新工作请求]： &lt;问题名称&gt;</em></p> <p>每日摘要通知的主题是：<em> [！UICONTROL需要操作的摘要] &lt;每日摘要的日期&gt;</em></p> </td> 
   <td> <p>问题名称<br>项目名称<br>[！UICONTROL问题参考编号]<br>您的名称<br>问题到期日期（[！UICONTROL计划完成日期]）<br>将问题分配给您的用户名称<br><strong>[！UICONTROL处理该问题]</strong>按钮<br>*分配总数<br>*分配给您的任务和问题总数<br>*链接到<strong>[！UICONTROL工作请求]</strong><br>*日期每日摘要<br></p> </td> 
   <td><strong>即时和每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我被设置为任务的主要被分配人</strong> </p> <p>如果任务被分配人是任务的主要被分配人，则任务被分配人会收到电子邮件通知，除非被分配人是进行分配的用户。</p> <p>如果项目状态为[！UICONTROL当前]，并且任务未标记为[！UICONTROL完成]，则会发送通知。</p> <p>拥有[！UICONTROL Review]或[！UICONTROL Requestor]许可证的用户不会收到通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL新工作请求]： &lt;任务名称&gt;</em></p> <p>每日摘要通知的主题是：<em> [！UICONTROL需要操作的摘要] &lt;每日摘要的日期&gt;</em></p> </td> 
   <td> 任务名称<br>项目名称<br>任务参考编号<br>您的名称<br>任务到期日期（[！UICONTROL计划完成日期]）<br>分配给您的任务的用户名称<br><strong>[！UICONTROL处理该任务]</strong>按钮<br>*分配给您的任务和问题总数<br>*链接到<strong>[！UICONTROL工作请求]</strong>*每日摘要日期 </td> 
   <td><strong>即时和每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我的团队获得了新工作请求</strong> </p> <p>当团队收到新的工作请求时，团队成员会收到电子邮件通知。 （如果提交请求的用户是团队成员，则不会收到通知。）</p> <p>仅当项目状态为[！UICONTROL当前]且工作请求状态为[！UICONTROL新建]时，才会发送通知。</p> <p>拥有[！UICONTROL Review]许可证的用户不会收到通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL新工作请求]： &lt;请求名称&gt;</em></p> <p>每日摘要通知的主题是： <em>[！UICONTROL需要操作的摘要] &lt;每日摘要的日期&gt;</em></p> </td> 
   <td> <p> 问题名称<br>项目名称（请求队列名称）<br>问题参考编号<br>团队名称<br>问题到期日期（计划完成日期）<br>提交请求的用户的名称<br><strong>[！UICONTROL处理此请求]</strong>按钮<br>*分配给您团队的请求总数</p> <p>*工作请求名称</p> <p>[！UICONTROL *计划完成日期]</p> <p>*提交请求的用户名称<br>*链接到<strong>[！UICONTROL团队请求]</strong><br>*每日摘要的日期 </p> <p><span class="preview">*团队分配</span> </p> </td> 
   <td><strong>即时和每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我的工时表已重新打开</strong> </p> <p>除非重新打开时间表的用户同时也是时间表的所有者，否则时间表所有者会在时间表重新打开时收到电子邮件通知。</p> <p>仅当时间表状态为[！UICONTROL打开]时，才会发送电子邮件通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL时间表重新打开]： &lt;时间表开始日期&gt; - &lt;时间表结束日期&gt;</em></p> <p>注意：您无法为每日摘要电子邮件配置此通知。</p> </td> 
   <td> 重新打开时间表的用户的名称<br>重新打开时间表的日期和时间<br>时间表状态（[！UICONTROL重新打开]）<br>时间表上记录的总小时数<br>时间表上记录的加班小时数<br><strong>[！UICONTROL审阅]</strong>按钮 </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我的工时表被拒绝</strong> </p> <p>时间表所有者会在时间表被拒绝时收到电子邮件通知，除非拒绝时间表的用户同时也是所有者。</p> <p>仅当时间表状态为[！UICONTROL已拒绝]时，才会发送电子邮件通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL已拒绝时间表]：&lt;时间表开始日期&gt; - &lt;时间表结束日期&gt;</em></p> <p>注意：您无法为每日摘要电子邮件配置此通知。</p> </td> 
   <td> 拒绝时间表的用户名称<br>时间表状态（[！UICONTROL已拒绝]）<br>时间表被拒绝的日期和时间<br><strong>[！UICONTROL审阅]</strong>按钮 </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>某人向我请求访问权限</strong> </p> <p>叫我做点什么，所以打开电源。</p> <p>创建项目的人员有权访问该项目。</p> <p>这就是当有人请求访问时，用户获得通知的原因。</p> <p>即时通知电子邮件的主题是： <em>&lt;请求访问的用户名&gt; [！UICONTROL需要访问] &lt;对象名&gt;</em></p> <p>每日摘要通知的主题是：<em> [！UICONTROL需要操作的摘要] &lt;每日摘要的日期&gt;</em></p> </td> 
   <td> <p>对象名称<br>父对象名称<br>对象引用编号<br>请求访问的用户的名称<br>用户请求的访问类型<br><strong>[！UICONTROL授权] &lt;请求的访问的名称&gt;访问</strong>和<strong>[！UICONTROL授权不同的访问]</strong>按钮<br>*待处理访问请求审批总数<br>*链接到<strong>[！UICONTROL访问请求]</strong>审批<br>*每日摘要日期</p> </td> 
   <td><strong>即时和每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>有人请求我上传文档</strong> </p> <p>当用户收到上传文档的请求时，文档请求者会收到电子邮件通知。</p> <p>即时通知电子邮件的主题是： <em>&lt;请求文档的用户的名称&gt; [！UICONTROL需要您在[!DNL Workfront]中提供的文档。]</em></p> <p> <p>注意：您无法为每日摘要电子邮件配置此通知。</p> </p> </td> 
   <td> 请求文档的用户的名称<br>应该将文档上载到的对象的名称<br><strong>[！UICONTROL将其附加到此处]</strong>链接 </td> 
   <td><strong>即时</strong> </td> 
  </tr> 
 </tbody> 
</table>
