---
content-type: reference
navigation-topic: notifications
title: “通知：通信'
description: 以下通知会提醒您有关涉及的工作项目中发生的通信（如更新评论）。 有关配置接收的通知的信息，请参阅激活或停用您自己的事件通知。
author: Lisa
feature: Get Started with Workfront
exl-id: 473e1760-f85a-4622-beff-9431046d655e
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1546'
ht-degree: 4%

---

# 通知：通信

以下通知会提醒您有关涉及的工作项目中发生的通信（如更新评论）。 有关配置接收的通知的信息，请参阅 [激活或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>这些通知会提醒您已在特定项目上发布的所有评论。 因此，您必须同时选择或取消选择所有通知，以便在每日摘要电子邮件中发送。 如果希望仅在发生某些评论时收到有关这些评论的通知，则可以指定要立即发送的单个通知。

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
   <td> <p><strong>有人将我列入定向更新</strong> </p> <p>定向更新是指当用户在更新中专门包括另一个用户时，如 <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">[!UICONTROL在上标记其他人]更新</a>.</p> <p>在这种情况下，被包含在定向更新中的用户会收到有关该更新的电子邮件通知。</p> <p>仅当用户具有对对象的访问权限时，才会发送电子邮件通知。</p> <p>即时通知电子邮件的主题是： <em>&lt;name of="" the="" user="" who="" included="" you="" in="" the="" update=""&gt; [!UICONTROL希望您知道]</em></p> <p>每日摘要通知的主题是： <em>[!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 对象进行更新的名称<br>父对象名称<br>对象引用编号<br>定向更新中包含的所有用户和团队的名称<br>进行更新的日期和时间<br>定向更新文本<br><strong>[!UICONTROL注释]</strong> 按钮<br>*收到的评论总数<br>*收到的每个对象的注释数<br>*<strong>[!UICONTROL请参阅所有通知]</strong> 按钮<br>*每日摘要的日期<br></td> 
   <td> <p><strong>即时</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>用户回复工作请求时，向请求工作的人发送电子邮件。</strong> </p> <p>在用户提交工作请求并且另一用户回复该工作请求后，提交该请求的用户会收到电子邮件通知。</p> <p>在以下情况下，不会发送电子邮件通知：</p> 
    <ul> 
     <li> <p>回复的用户与发出请求的用户相同</p> </li> 
     <li> <p>用户无权查看注释</p> </li> 
    </ul><strong>即时通知电子邮件的主题是： <em>[!UICONTROL注释] &lt;request name=""&gt; on &lt;project name=""&gt; （参考#） &lt;request reference="" number=""&gt;)</em></strong> 每日摘要通知的主题是：<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></td> 
   <td> 请求名称<br>项目名称<br>参考编号<br>回复了您请求的用户的名称<br>评论的日期和时间<br>对您的请求发表的评论文本<br>*收到的评论总数<br>*每个请求收到的评论数<br>*<strong>[!UICONTROL请参阅所有通知]</strong> 按钮<br>*每日摘要的日期<br></td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>注释已被贴到的请求上</strong> </p> <p>当在[!UICONTROL帮助台]请求中发布评论时，问题的主要联系人会收到电子邮件通知，除非发布评论的用户也是问题的主要联系人。</p> <p>直接包含在评论中的任何用户也会收到电子邮件通知。</p> <p>仅当项目状态为[!UICONTROL Current]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL注释] &lt;request name=""&gt; on &lt;project name=""&gt; （参考#） &lt;request reference="" number=""&gt;)</em></p> <p>每日摘要通知的主题是：<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 请求名称<br>项目名称<br>参考编号<br>回复了您请求的用户的名称<br>评论的日期和时间<br>对您的请求发表的评论文本<br>*收到的评论总数<br>*每个请求收到的评论数<br>*项目名称<br>*<strong>[!UICONTROL请参阅所有通知]</strong> 按钮<br>*每日摘要的日期<br></td> 
   <td> <p><strong>即时</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在我的文档中添加了一个评论</strong> </p> <p>中文档的所有者 [!DNL Adobe Workfront] 在文档上发布评论时，会收到电子邮件通知，除非发布评论的用户也是文档所有者。</p> <p>直接包含在评论中的任何用户也会收到电子邮件通知。</p> <p>仅当项目状态为[!UICONTROL Current]时，才会发送通知。 </p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL注释] &lt;request name=""&gt; on &lt;project name=""&gt; （参考#） &lt;request reference="" number=""&gt;)</em></p> <p> 每日摘要通知的主题是：<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td>文档名称<br>项目、任务或问题名称<br>参考编号<br>回复了您请求的用户的名称<br>评论的日期和时间<br>对文档的评论文本</td> 
   <td> <p><strong>即时</strong> </p> <p><strong>和每日</strong> </p> <p><strong></strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>当某人备注跟帖，向备注该跟帖的每个人发送电子邮件</strong> </p> <p>当用户在线程中发表评论时，线程中的参与者和包含在私信中的用户会收到电子邮件通知。</p> <p>用户必须具有[!UICONTROL视图]访问权限才能接收通知。</p> <p>以下用户不会收到通知：</p> 
    <ul> 
     <li>包含在私信中的团队</li> 
     <li>票据的所有者</li> 
     <li>主要联系人</li> 
    </ul> <p><strong>即时通知电子邮件的主题是： <em>[!UICONTROL RE:评论] &lt;object name=""&gt;&lt;object type=""&gt; on &lt;project name=""&gt;（参考#） &lt;object reference="" number=""&gt;</em>)</strong> </p> <p><strong> 每日摘要通知的主题是：<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></strong> </p> </td> 
   <td> 对象名称<br>父对象名称<br>对线程发表评论的用户的名称<br>在线程上发表的注释文本<br>评论的日期和时间<br>*收到的评论总数<br>*收到的每个对象的注释数<br>*项目名称<br>*<strong>[!UICONTROL请参阅所有通知]</strong> 按钮<br>*每日摘要日期 </td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>某人备注我的工作项之一</strong> </p> <p>工作项的被分派人在用户向工作项添加更新时随时会收到电子邮件通知，除非添加更新的用户也是被分派人。 </p> <p>在请求上发布评论时，通过电子邮件将问题主要联系人发送给。</p> <p>问题的主要联系人在请求中发布评论时会收到电子邮件通知，除非发布评论的用户也是问题的主要联系人。</p> <p>直接包含在评论中的任何用户也会收到电子邮件通知。</p> <p>仅当项目状态为[!UICONTROL Current]时，才会发送通知。</p> <p>即时通知电子邮件的主题是： <em>[!UICONTROL注释] &lt;work item="" name=""&gt; on &lt;project name="" ref="" work="" item="" reference="" number=""&gt;)</em></p> <p> 每日摘要通知的主题是：<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 工作项名称<br>项目名称<br>工作项参考编号<br>对工作项发表评论的用户的名称<br>对工作项目的评论文本<br>评论的日期和时间<br>*收到的评论总数<br>*收到的每个对象的注释数<br>*项目名称<br>*<strong>[!UICONTROL请参阅所有通知]</strong> 按钮<br>*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>有人将我的团队列入定向更新</strong> </p> <p>定向更新是指当用户在更新中专门包括另一个用户时，如 <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">更新时标记其他人</a>.</p> <p>在这种情况下，包含在定向更新中的团队的任何成员都会收到有关该更新的电子邮件通知。</p> <p>电子邮件通知仅发送给具有对象访问权限的用户。</p> <p>如果发送定向更新的用户是被包括的团队的成员，则发送更新的用户不会收到电子邮件通知。</p> <p>即时通知电子邮件的主题是：[!UICONTROL注释] &lt;object name=""&gt; on &lt;parent object="" name=""&gt; （参考#） &lt;object reference="" number=""&gt;)</p> <p> 每日摘要通知的主题是：<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>对象名称<br>父对象名称<br>对象引用编号<br>进行定向更新的用户的名称<br>定向更新中包含的所有团队和用户的名称<br>进行定向更新的日期和时间<br>定向更新的文本<br><strong>[!UICONTROL注释]</strong> 按钮<br>*收到的评论总数<br>*收到的每个对象的注释数<br>*项目名称<br>*<strong>[!UICONTROL请参阅所有通知]</strong> 按钮<br>*每日摘要日期 </p> </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>给用户添加了评论时</strong> </p> <p>您可以在用户对象的[!UICONTROL更新]选项卡中对用户进行评论。 在编辑用户的设置时，您还可以对用户进行评论。 评论所依据的用户会收到一封电子邮件，通知他们此评论。 </p> <p>您必须至少拥有用户的[!UICONTROL视图]权限，才能在用户的[!UICONTROL更新]选项卡上输入更新。 您必须对用户具有[!UICONTROL Edit]权限，才能编辑用户的设置。 </p> <p>有关在“更新”选项卡中对用户进行评论的更多信息，请参阅 <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">更新工作</a>.</p> <p>有关在编辑用户设置时在用户上输入评论的详细信息，请参阅 <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">配置我的设置</a>.</p> <p>即时通知电子邮件的主题是： <em>&lt;user name=""&gt; [!UICONTROL希望您知道]</em></p> <p>每日摘要通知的主题是：<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 您的用户名<br>添加评论的用户的名称<br>注释文本<br>评论的日期和时间<br>*收到的评论总数<br>*收到的每个对象的注释数<br>*<strong>[!UICONTROL请参阅所有通知]</strong> 按钮<br>*每日摘要日期 </td> 
   <td> <p><strong>即时</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
