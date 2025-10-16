---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: 共享文档文件夹
description: 您可以从文档区域共享文件夹及其内容。
author: Alina
feature: Get Started with Workfront
exl-id: c0d318a8-b1cf-4522-b478-acf092687658
source-git-commit: 4ae96f67b15838403ffce32317d871d6904d6d95
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 0%

---

# 共享文档文件夹

您可以从文档区域共享文件夹及其内容。

>[!NOTE]
>
>* 文件夹必须位于对象上文件夹层次结构的前五个级别中。 第六级或更低级别的每个文件夹都从其正上方的文件夹继承其共享配置。
>
>  有关添加子文件夹以创建文件夹层次结构的信息，请参阅文章[创建文档文件夹](../../documents/organizing-documents/create-documents-folder.md#creating-folders)中的[创建文件夹和子文件夹](../../documents/organizing-documents/create-documents-folder.md)部分。
>
>* 无法共享智能文件夹。
>* 如果为模板中的文档文件夹配置共享选项，然后有人从该模板创建项目，则共享配置不会传输到新项目中的文档文件夹。
>* 如果为工作项中的文档文件夹配置共享选项，然后复制该工作项，则共享配置不会转移到新工作项中的文档文件夹。
>

## 访问要求

<!--drafted for P&P
(I am putting Contributor and higher here because this is what I found in testing. Normally, Review equals Light but I found out that Contributor can also have manage rights to documents and can share them.)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Contributor or higher</p> 
   Or
   <p>Legacy license: Review or higher</p>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access to Documents</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View access to an object</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>浅色或更高</p> 
   <p>审核或更高</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>查看对文档的访问权限</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看对对象的访问权限</p>  </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 共享文件夹

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)，然后单击&#x200B;**文档**。

   或

   打开Workfront对象后，单击左侧面板中的&#x200B;**文档**。

1. 选择文件夹，然后单击工具栏中的共享图标![](assets/share-icon.png)。

   文件夹必须位于对象上文件夹层次结构的前五个级别中，并且不能是智能文件夹。

1. 在显示的框中，在&#x200B;**将文件夹访问权限授予**&#x200B;下，开始键入要与其共享文件夹的用户、团队、工作角色、组或公司的名称，然后在名称显示时按&#x200B;**Enter**。
1. 要调整您刚刚添加的用户、团队、工作角色、组或公司的访问权限，请单击名称右侧的下拉菜单，然后配置以下任一可用选项及其任何高级设置：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">查看它</td> 
      <td> <p>能够查看文件夹及其内容。</p> <p>单击<strong>高级设置</strong>以指定是否允许以下设置：</p> 
       <ul> 
        <li><strong>下载</strong>：能够将文件夹及其内容下载为ZIP文件</li> 
        <li> <p><strong>共享</strong>：能够与系统中的其他人共享文件夹</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">管理它</td> 
      <td> <p>能够查看和编辑文件夹及其内容</p> <p>单击<strong>高级设置</strong>以指定是否允许用户执行以下操作：</p> 
       <ul> 
        <li><strong>删除</strong>：从系统中删除文件夹及其内容</li> 
        <li><b>下载</b>：以ZIP文件格式下载文件夹及其内容</li> 
        <li><strong>共享</strong>：与系统中的其他用户共享文件夹及其内容</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可选）重复步骤3 - 4以向列表中添加其他名称并配置其选项。
1. （可选）如果希望系统中的每个人都可以查看文件夹及其内容，请单击共享框右上角的齿轮图标![](assets/gear-icon-settings-with-dn-arrow.jpg)，然后单击&#x200B;**使其在系统范围内可见。**

   如果您改变主意，可以单击&#x200B;**删除系统范围访问权限**（默认选项）。

## 用户如何访问与其共享的文件夹的内容

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Delete these 2 paragraphs when the story &nbsp;<a href="https://hub.workfront.com/task/622f8d6f000897c9a4a11bdfd9b2cf34/overview">Handle email notification content when a folder is shared</a> goes to Preview:</p>
-->

目前，当您共享文件夹时，收件人在其“文档”区域中看不到该文件夹。 但是，他们可以通过运行文档报告来访问其文档。

有关运行报表的信息，请参阅[了解Adobe Workfront中的对象](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects)一文中的[对象报表](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)部分。 另请参阅[创建自定义报表](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

<!--
<div class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Workfront sends a notification email when someone shares a document folder on an object with a user or a team. To access the folder from the email, recipients can click the folder title or the "See it in Workfront" link.</p> <note type="note">
<ul class="preview">
<li> <p>The email notification "Someone shares an object with me" or "Someone shares an object with my team" must be enabled in order for a user or team to receive a notification email about a shared folder.</p> </li>
<li> <p>When someone shares a document folder from the global Documents area, the links in the notification email take the recipient to the global Documents area. Because folders in this area are private, the shared folder is not displayed there, but the recipient can access its documents by creating a document report. </p> <p>For information about running a report, see the section <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects" class="MCXref xref">Report on objects</a> in the article <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>. Also see <a href="../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.</p> </li>
<li> <p>Currently, it is not possible to share folders with external users.</p> </li>
</ul>
</note>
</div>
-->

## 共享包含文件夹的对象时继承的权限

当您共享具有文档文件夹的对象时，收件人还可以访问该文件夹：

* 如果您授予收件人查看父对象的权限，则他们将拥有对文件夹的查看权限。
* 如果您授予收件人Contribute或Manage对父对象的访问权限，则他们将拥有对文件夹的Manage访问权限。
* 如果您向父对象授予一种类型的访问权限（查看、贡献或管理），向文件夹授予另一种类型的访问权限，则您的收件人对该文件夹中的文档具有最高两种类型的访问权限

  例如，如果您共享具有“查看”访问权限的父对象，而文件夹具有“管理”访问权限，则收件人对该文件夹中的文档具有“管理”权限。

  >[!NOTE]
  >
  >附加的文档仅从其附加的对象继承权限。 如果在对象上创建文件夹并将文档移动到该文件夹中，它会继承该文件夹的权限。 但是，如果您在父对象或祖父对象上创建文件夹，并将文档移动到该文件夹中，则它不会继承该文件夹的权限。

* 如果在收件人的访问级别中启用了“从不从项目、任务、问题等继承文档访问权限”选项，则他们不会继承您与他们共享的文件夹中文档的权限。 要授予他们访问文件夹中文档的权限，您必须共享该文档。

  有关“从不继承”选项的信息，请参阅[配置对Adobe Workfront的访问权限](../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)。

  有关共享文档的信息，请参阅[共享文档](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md)。
