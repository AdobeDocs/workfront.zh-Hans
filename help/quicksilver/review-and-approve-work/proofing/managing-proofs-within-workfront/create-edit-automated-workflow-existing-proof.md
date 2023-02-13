---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 创建或编辑现有校样的自动化工作流
description: 如果您的流程复杂或您定期向同一批人员发送内容以供审阅，则通过自动化工作流可以更轻松地管理审阅流程。 使用自动工作流创建校样时，校样会从阶段移动到最终批准。 当参与者需要审阅文档时，会通知他们。
author: Courtney
feature: Digital Content and Documents
exl-id: 852f960f-1b57-4a8a-a928-407ad52418e6
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1225'
ht-degree: 1%

---

# 创建或编辑现有校样的自动化工作流

如果您的流程复杂或您定期向同一批人员发送内容以供审阅，则通过自动化工作流可以更轻松地管理审阅流程。 使用自动工作流创建校样时，校样会从阶段移动到最终批准。 当参与者需要审阅文档时，会通知他们。

有关为新校样创建自动工作流的信息，请参阅 [使用自动工作流创建高级校样](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>当前计划：Pro或更高版本</p> <p>或</p> <p>旧版计划：Premium</p> <p>有关使用不同计划校对访问权限的更多信息，请参阅 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的校对功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>当前计划：工作或计划</p> <p>旧版计划：任意（必须为用户启用校样）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校对权限配置文件 </td> 
   <td>经理或更高级别</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、角色或校样权限配置文件，请联系您的Workfront或Workfront校样管理员。

## 为现有校样创建或编辑自动工作流：

1. 将鼠标悬停在“文档”区域中的文档上，然后单击“校对工作流”。

   或

   如果要在校对查看器中查看校样，请单击 **工作流** ![](assets/workflow-icon-proofing-viewer.png) 在左侧面板中，单击编辑图标 ![](assets/edit-icon-proofing-viewer.png) 以打开校样的自动工作流设置。

1. （视情况而定）如果校样当前使用的基本工作流（无阶段），请单击 **转换为自动化工作流** 在显示的屏幕中。

   >[!NOTE]
   >
   >在从基本工作流转换为自动工作流时，您无法编辑第一个阶段，但可以添加和配置新阶段。

1. 视情况而定)要使用由Adobe Workfront管理员创建并与您共享的自动工作流模板，请单击 **添加模板**，在显示的框中选择模板，然后单击 **添加模板**.

   有关更多信息，请参阅 [关于使用自动化工作流模板](#about-using-automated-workflow-templates) 在本文中。

1. 向自动工作流添加阶段：

   1. 单击 **新阶段** 在右上角附近。
   1. 在显示的框中，键入 **名称** 为舞台准备。
   1. （可选）设置阶段的截止时间。
   1. 在 **激活阶段** 部分中，选择您希望舞台激活的方式：


      <table>
      <tbody>
      <tr>
      <td><strong>论校样创建</strong></td>
      <td>由于已创建校样，因此阶段会自动变为活动状态。</td>
      </tr>
      <tr>
      <td><strong>当上一个阶段的截止日期过去时</strong></td>
      <td>单击 <strong>父阶段</strong> 下拉列表。</td>
      </tr>
      <tr>
      <td><strong>特定日期和时间</strong></td>
      <td>单击 <strong>开</strong> 框选择日期，然后单击右侧的框以选择时间。</td>
      </tr>
      <tr>
      <td><strong>所有决策均为“已批准”或“已批准”，并在父级进行更改</strong></td>
      <td>单击 <strong>父阶段</strong> 下拉列表。</td>
      </tr>
      <tr>
      <td><strong>所有决策在父级上均获得批准</strong></td>
      <td>单击 <strong>父阶段</strong> 下拉列表。</td>
      </tr>
      <tr>
      <td><strong>所有决定都做出</strong></td>
      <td>单击 <strong>父阶段</strong> 下拉列表。</td>
      </tr>
      </tbody>
      </table>


   1. 输入联系人姓名或电子邮件地址，并为舞台的审阅人配置设置。

      有关添加审阅人的信息，请参阅 [关于将审阅人添加到舞台](#about-adding-reviewers-to-a-stage) 在本文中。

   1. 使用以下任意选项进一步配置舞台：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader"><strong>截止日期选项</strong> </td>
         <td><p>要设置阶段的截止时间，请单击 <strong>截止日期选项</strong> 下拉列表。 然后，在 <strong>截止时间</strong>，执行下列操作之一：</p>
          <ul>
           <li>如果您选择 <strong>设置特定日期</strong>:选择所需的截止日期和时间。</li>
           <li>如果您选择 <strong>从阶段激活日期计算</strong>:选择要添加到阶段激活日期的工作天数，以确定截止日期。</li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">锁台</td>
         <td>指定舞台可以锁定的时间。 </td>
        </tr>
        <tr>
         <td role="rowheader">主要决策者</td>
         <td><p>在舞台上选择主要决策者（只有在您向舞台中添加至少一名具有“审批者”或更高“校样”角色的人员后才可用）。 如果选择“主要决策者”，则 <strong>只需要一个决定</strong> 选项。</p></td>
        </tr>
        <tr>
         <td role="rowheader">只需一个决定</td>
         <td>当某个决策者做出决策时，结束整个审查过程。<p>如果您在 <strong>主要决策者</strong> 下拉菜单。</p></td>
        </tr>
        <tr>
         <td role="rowheader">私人舞台</td>
         <td>仅允许以下人员查看在此阶段做出的评论和决策：主管、Adobe Workfront管理员和Workfront校样管理员</td>
        </tr>
        <tr>
         <td role="rowheader">通过电子邮件通知用户</td>
         <td>轮到审阅人处理校样时通过电子邮件通知他们。</td>
        </tr>
       </tbody>
      </table>

   1. 单击 **添加阶段**.

1. 根据需要重复上一步骤以添加更多阶段。

   在向自动化工作流中添加阶段时，屏幕上会显示一个用于表示这些阶段的图表表单：

   ![](assets/workflow-diagram-existing-proof-qs-350x215.png)

1. 完成添加阶段后，单击 **完成**.

## 关于使用自动化工作流模板 {#about-using-automated-workflow-templates}

使用自动化工作流模板时，请考虑以下事项：

1. 自动工作流模板的设置决定了您可以使用自动工作流进行校样的操作。 例如，如果模板中禁用了添加阶段按钮，则当您使用校样的自动工作流设置时，该按钮将不可见。
1. 当某人在自动工作流模板中添加到页面，但已作为校样的审阅人存在时，应用该模板会将审阅人从舞台中删除。 如果不将其他审阅人添加到舞台，则会显示一条消息，提示您添加一个审阅人。
1. 您能否修改自动工作流模板取决于由Workfront管理员配置的模板设置，如中所述。 如果禁用了修改模板的功能，则只有模板的所有者才能修改模板。

## 关于将审阅人添加到舞台 {#about-adding-reviewers-to-a-stage}

在将审阅人添加到阶段时，请考虑以下事项：

* 在将用户添加到舞台后，您可以在校样上为该用户配置设置，例如校样角色和他们应具有的任何其他权限，以及当用户对校样进行评论和决策时他们将收到的电子邮件警报类型。
* 您可以将一个或多个用户从一个阶段拖到另一个阶段。 您可以将用户直接拖到另一个舞台，也可以将用户拖到 **阶段** 图表。 要选择多个用户，请按Shift+Ctrl（在Windows上）或Shift+Command(在Mac上)。
* 您只能向校样添加一次审阅人，这意味着您无法将同一人添加到校样的多个阶段。
* 未添加到专用舞台的审阅人无法在该舞台中进行校样或评论。
* 默认情况下，将用户添加到舞台会授予用户从创建校样开始查看校样的权限。

   您的Workfront管理员可以限制用户访问校样，直到工作流进入添加用户的阶段。 有关更多信息，请参阅中的。
