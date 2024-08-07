---
content-type: release-notes
navigation-topic: 2019-4-release-activity
title: 2019.4年其他增强功能
description: 本页介绍了2019.4版本中的各种增强功能。 它将在2019年11月11日这一周的生产环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: ed7488f1-2076-4160-97f3-a3da25cccd0f
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---

# 2019.4年其他增强功能

本页介绍了2019.4版本中的各种增强功能。 它将在2019年11月11日这一周的生产环境中提供。

有关2019.4中所做所有更改的列表，请参阅[2019.4版本概述](../../../../product-announcements/product-releases/quarterly-release-archive/2019.4-release-activity/2019-4-release-activity-overview.md)。

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td> <strong>从AdobeCC文档启动自动验证工作流</strong> <p>无需离开Adobe抄送，即可为已创建的Adobe抄送文档启动自动验证工作流。 有关详细信息，请参阅<a href="../../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md" class="MCXref xref" xrefformat="{para}">使用Illustrator和InDesign的Illustrator扩展</a>中的章节<a href="../../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md#generate" class="MCXref xref" xrefformat="{para}">从Workfront或InDesign生成校对</a>。</p> </td> 
  </tr> 
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td><strong>Workfront G Suite add-on</strong> <p>Now you can manage Workfront objects directly from Gmail, Google Calendar, and Google Drive.</p> <p>When you open a Workfront notification email, instantly view all information about the associated object and take actions, such as reviewing content or updating a status, without leaving your Inbox.</p> <p>When you open a non-Workfront email:</p> 
     <ul> 
      <li>Convert it into a task or issue.</li> 
      <li>Associate it with a project.</li> 
      <li>Assign it as a work item.</li> 
      <li>Add it to a work item as an update.</li> 
      <li>Upload its attachments to Workfront.</li> 
     </ul> <p>Manage Workfront objects without leaving G Suite:</p> 
     <ul> 
      <li>Post updates and replies to comments.</li> 
      <li>View and manage documents associated with a task or issue.</li> 
     </ul> <p>Access and work with object details:</p> 
     <ul> 
      <li>Read the description</li> 
      <li>View the parent object</li> 
      <li>Change the status</li> 
      <li>Access custom data</li> 
      <li>Mark it as complete.</li> 
     </ul> <p>And access your Workfront Home content, including tasks, issues, approvals, and access requests, without leaving G Suite.</p> <p>For more information, see <a href="../../../../workfront-integrations-and-apps/workfront-for-g-suite/workfront-for-gsuite.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront for G Suite</a>.</p> </td> 
   </tr>
  --> 
  <tr> 
   <td> <strong>防止电子邮件地址重复</strong> <p>在Workfront中创建多个用户时，您无法再使用相同的电子邮件地址，即使这些电子邮件地址因情况而异。 例如，您不能创建一个电子邮件地址为JohnDoe@example.com的用户，而创建另一个电子邮件地址为johndoe@example.com的用户。 </p> <p>在此更改之前，支持创建具有匹配电子邮件地址的用户，这些电子邮件地址仅因大小写而异。 </p> <p>注意：如果现有用户的匹配电子邮件地址仅因大小写而异，则将来需要更新这些用户。 如果您的Workfront实例中的用户具有匹配的电子邮件地址，这些地址仅因大小写而异，则Workfront将在需要更新这些地址时为您提供其他信息和时间表。</p> </td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <strong>自定义表单中预输入字段可用的其他对象类型</strong> 
     <p>现在，当您创建“预输入”自定义字段时，可以将以下对象类型与该字段相关联：用户、公司、组、工作角色、Portfolio、项目群和模板。</p> 
     <p>以前，您只能将用户对象类型与预输入自定义字段相关联。</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td> <strong>显示的最新版本文档的文件名</strong> <p>现在，当您上载文件名不同于现有版本的文档版本时，新文件名将显示在Workfront中。</p> <p>以前，当您添加具有不同文件名的新版本时，Workfront中将继续显示以前版本的文件名。</p> <p>有关详细信息，请参阅<a href="../../../../documents/managing-documents/upload-new-document-version.md" class="MCXref xref" xrefformat="{para}">上载文档的新版本</a>。</p> </td> 
  </tr> 
  <tr> 
   <td> <strong>将筛选器添加到自定义表单中的预输入字段</strong> <p>现在，当您向自定义表单添加预输入字段时，可以添加过滤器以限制有人使用该字段时可用的对象。 例如，您可以限制该字段，以便用户只能选择贵组织中的营销和销售团队的成员。</p> <p>有关更多信息，请参阅创建自定义Forms一文中的创建和添加新字段。</p> </td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <strong>更改自定义表单中字段的显示类型</strong> 
     <p>现在，您可以更改自定义表单中字段的显示类型。</p> 
     <p>例如，如果您已创建复选框字段，则可以将其更改为下拉列表字段或单选按钮字段。 这三种字段显示类型可以互换。</p> 
     <p>或者，如果您已创建单行文本字段，则可以将其更改为段落文本字段。 这两种字段显示类型可以互换。</p> 
     <p>以前，要更改自定义字段的显示类型，您必须创建新字段并删除旧字段。 这需要传输数据，而这通常非常耗时。</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <strong>创建休息时间日历和报告</strong> 
     <p>您现在可以看到用户的休息时间，以便更好地规划和执行。 您还可以将新的休息时间报告和日历添加到功能板，以便实时查看用户可用性。</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>
