---
content-type: reference
navigation-topic: notifications
title: '通知：通信'
description: 以下通知会提醒您有关您参与的工作项中发生的通信（如更新评论）。 有关配置您收到的通知的信息，请参阅修改您自己的电子邮件通知。
author: Lisa
feature: Get Started with Workfront
exl-id: 473e1760-f85a-4622-beff-9431046d655e
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1530'
ht-degree: 0%

---

# 通知：通信

以下通知会提醒您有关您参与的工作项中发生的通信（如更新评论）。 有关配置您收到的通知的信息，请参阅[修改您自己的电子邮件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。

>[!NOTE]
>
>这些通知会提醒您有关特定项目发布的所有评论。 因此，您必须同时选择或取消选择要在每日摘要电子邮件中传送的所有通知。 如果您希望仅在某些注释发生时才会收到通知，则可以指定各个通知以便即时发送。

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
   <td> <p><strong>有人将我包含在定向更新中</strong> </p> <p>定向更新是指用户明确将另一个用户包含在更新中，如<a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">[！UICONTROL在]更新</a>上标记其他用户中所述。</p> <p>在这种情况下，定向更新中包含的用户会收到有关更新的电子邮件通知。</p> <p>仅当用户具有对象的访问权限时，才会发送电子邮件通知。</p> <p>即时通知电子邮件的主题是： <em>&lt;将您包含在更新中的用户的名称&gt; [！UICONTROL希望您知道]</em></p> <p>每日摘要通知的主题是： <em>[！UICONTROL通信摘要] &lt;每日摘要的日期&gt;</em></p> </td> 
   <td> 进行更新的对象名称<br>父对象名称<br>对象参考编号<br>定向更新中包含的所有用户和团队的名称<br>进行更新的日期和时间<br>定向更新的文本<br><strong>[！UICONTROL注释]</strong> button<br>*收到的注释总数<br>*每个对象收到的注释数<br>*<strong>[！UICONTROL查看所有通知]</strong>按钮<br>*每日摘要的日期<br></td> 
   <td> <p><strong>即时</strong> </p> <p><strong>和每天</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>有人回复我的请求</strong> </p> <p>当用户提交工作请求且另一个用户回复该工作请求后，提交请求的用户会收到电子邮件通知。</p> <p>如果出现以下情况，则不发送电子邮件通知：</p> 
    <ul> 
     <li> <p>回复的用户是发出请求的同一个用户</p> </li> 
     <li> <p>用户无权查看注释</p> </li> 
    </ul><strong>即时通知电子邮件的主题是： <em>[！UICONTROL评论，位于] &lt;请求名称&gt;，位于&lt;项目名称&gt; （ref# &lt;请求参考编号&gt;）</em></strong>每日摘要通知的主题是：<em> [！UICONTROL通信摘要] &lt;每日摘要的日期&gt;</em></td> 
   <td> 请求名称<br>项目名称<br>参考编号<br>回复您的请求的用户名称<br>做出评论的日期和时间<br>对您的请求做出评论的文本<br>*收到的评论总数<br>*每个请求收到的评论数<br>*<strong>[！UICONTROL查看所有通知]</strong>按钮<br>*每日摘要的日期<br></td> 
   <td><strong>每天</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我的请求上已张贴了一个评论</strong> </p> <p>在[！UICONTROL技术支持]请求上发布评论时，问题主要联系人会收到电子邮件通知，除非发布评论的用户也是问题的主要联系人。</p> <p>任何直接包含在评论中的用户都会收到电子邮件通知。</p> <p>仅当项目状态为[！UICONTROL当前]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL Comment on] &lt;Request Name&gt; on &lt;Project Name&gt; (ref# &lt;Request Reference Number&gt;)</em></p> <p>每日摘要通知的主题是：<em> [！UICONTROL通信摘要] &lt;每日摘要的日期&gt;</em></p> </td> 
   <td> 请求名称<br>项目名称<br>参考编号<br>回复您的请求的用户名称<br>做出评论的日期和时间<br>对您的请求做出评论的文本<br>*收到的评论总数<br>*每个请求收到的评论数<br>*项目名称<br>*<strong>[！UICONTROL查看所有通知]</strong>按钮<br>*每日摘要的日期<br></td> 
   <td> <p><strong>即时</strong> </p> <p><strong>和每天</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我的文档中添加了评论</strong> </p> <p>[!DNL Adobe Workfront]中文档的所有者会在文档上发布评论时收到电子邮件通知，除非发布评论的用户也是文档所有者。</p> <p>任何直接包含在评论中的用户都会收到电子邮件通知。</p> <p>仅当项目状态为[！UICONTROL当前]时，才会发送通知。 </p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL Comment on] &lt;Request Name&gt; on &lt;Project Name&gt; (ref# &lt;Request Reference Number&gt;)</em></p> <p> 每日摘要通知的主题是：<em> [！UICONTROL通信摘要] &lt;每日摘要的日期&gt;</em></p> </td> 
   <td>文档名称<br>项目、任务或问题名称<br>参考编号<br>回复您的请求的用户的名称<br>发表评论的日期和时间<br>对文档发表的评论文本</td> 
   <td> <p><strong>即时</strong> </p> <p><strong>和每天</strong> </p> <p><strong></strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>某人备注我所在的线程</strong> </p> <p>当用户在线程中发表评论时，线程中的参与者和直接消息中包含的用户会收到电子邮件通知。</p> <p>用户必须具有[！UICONTROL视图]权限才能接收通知。</p> <p>以下用户未收到通知：</p> 
    <ul> 
     <li>直接消息中包含的团队</li> 
     <li>注释的所有者</li> 
     <li>主要联系人</li> 
    </ul> <p><strong>即时通知电子邮件的主题是： <em>[！UICONTROL RE： Comment on] &lt;Object Name&gt;&lt;Object Type&gt; on &lt;Project Name&gt;(ref# &lt;Object Reference Number&gt;</em>)</strong> </p> <p><strong>每日摘要通知的主题是：<em> [！UICONTROL Digest of Communication] &lt;每日摘要的日期&gt;</em></strong> </p> </td> 
   <td> 对象名称<br>父对象名称<br>对线程发表评论的用户名称<br>对线程发表评论的文本<br>发表评论的日期和时间<br>*收到的评论总数<br>*每个对象收到的评论数<br>*项目名称<br>*<strong>[！UICONTROL查看所有通知]</strong>按钮<br>*每日摘要日期 </td> 
   <td><strong>[！UICONTROL每日]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>某人备注我的工作项之一</strong> </p> <p>工作项的被分派人在用户向工作项添加更新时收到电子邮件通知，除非添加更新的用户也是被分派人。 </p> <p>在请求上发布评论时，通过电子邮件将问题发送给主要联系人。</p> <p>当在请求上发布评论时，问题的主要联系人会收到电子邮件通知，除非发布评论的用户也是问题的主要联系人。</p> <p>任何直接包含在评论中的用户都会收到电子邮件通知。</p> <p>即时通知电子邮件的主题是： <em>[！UICONTROL Comment on] &lt;Work Item Name&gt; on &lt;Project Name (ref# &lt;Work Item Reference Number&gt;)</em></p> <p> 每日摘要通知的主题是：<em> [！UICONTROL通信摘要] &lt;每日摘要的日期&gt;</em></p> </td> 
   <td> 工作项名称<br>项目名称<br>工作项引用编号<br>对工作项发表评论的用户名称<br>对工作项发表评论的文本<br>发表评论的日期和时间<br>*收到的评论总数<br>*每个对象收到的评论数<br>*项目名称<br>*<strong>[！UICONTROL查看所有通知]</strong>按钮<br>*每日摘要的日期 </td> 
   <td><strong>每天</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>有人将我的团队列入定向更新</strong> </p> <p>定向更新是指用户明确将另一个用户包含在更新中，如<a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">在更新上标记其他用户</a>中所述。</p> <p>在这种情况下，定向更新中包含的团队的任何成员都会收到有关更新的电子邮件通知。</p> <p>电子邮件通知仅发送给具有对象访问权限的用户。</p> <p>如果发送定向更新的用户是所包含的团队的成员，则发送更新的用户不会收到电子邮件通知。</p> <p>即时通知电子邮件的主题是： [！UICONTROL Comment on] &lt;Object name&gt; on &lt;Parent Object Name&gt; (ref# &lt;Object Reference Number&gt;)</p> <p> 每日摘要通知的主题是：<em> [！UICONTROL通信摘要] &lt;每日摘要的日期&gt;</em></p> </td> 
   <td> <p>对象名称<br>父对象名称<br>对象引用编号<br>进行定向更新的用户名称<br>定向更新中包含的所有团队和用户的名称<br>进行定向更新的日期和时间<br>定向更新的文本<br><strong>[！UICONTROL注释]</strong> button<br>*收到的注释总数<br>*每个对象收到的注释数<br>*项目名称<br>*<strong>[！UICONTROL查看所有通知]</strong>按钮14}*每日摘要日期<br> </p> </td> 
   <td><strong>每天</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>向用户</strong>添加评论时 </p> <p>您可以在用户对象的[！UICONTROL Updates]选项卡中对用户进行评论。 您还可以在编辑用户的设置时对用户进行评论。 作为评论对象的用户会收到一封电子邮件，用于通知他们此评论。 </p> <p>您必须具有至少[！UICONTROL视图]用户的权限，才能在用户的[！UICONTROL更新]选项卡中输入更新。 您必须具有用户的[！UICONTROL编辑权限]才能编辑用户的设置。 </p> <p>有关在“更新”选项卡中对用户发表评论的更多信息，请参阅<a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">更新工作</a>。</p> <p>有关在编辑用户的设置时输入用户评论的更多信息，请参阅<a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">配置我的设置</a>。</p> <p>即时通知电子邮件的主题是： <em>&lt;用户名&gt; [！UICONTROL希望您知道]</em></p> <p>每日摘要通知的主题是：<em> [！UICONTROL通信摘要] &lt;每日摘要的日期&gt;</em></p> </td> 
   <td> 您的用户名<br>添加注释的用户名<br>注释的文本<br>创建注释的日期和时间<br>*收到的注释总数<br>*每个对象收到的注释数<br>*<strong>[！UICONTROL查看所有通知]</strong>按钮<br>*每日摘要的日期 </td> 
   <td> <p><strong>即时</strong> </p> <p><strong>和每天</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
