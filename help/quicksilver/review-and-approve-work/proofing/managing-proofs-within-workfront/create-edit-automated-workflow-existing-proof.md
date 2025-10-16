---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 为现有验证创建或编辑自动工作流
description: 如果您的流程比较复杂，或者您经常将内容发送给同一人员组，则使用自动工作流可以更轻松地管理审核流程。 使用自动工作流创建验证时，验证会从阶段转移到阶段，直到最终批准。 轮到参与者查看文档时，会通知他们。
author: Courtney
feature: Digital Content and Documents
exl-id: 852f960f-1b57-4a8a-a928-407ad52418e6
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '1142'
ht-degree: 1%

---

# 为现有验证创建或编辑自动工作流

如果您的流程比较复杂，或者您经常将内容发送给同一人员组，则使用自动工作流可以更轻松地管理审核流程。 使用自动工作流创建验证时，验证会从阶段转移到阶段，直到最终批准。 轮到参与者查看文档时，会通知他们。

有关为新验证创建自动化工作流的信息，请参阅[使用自动化工作流创建高级验证](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>
   <p>标准</p>
   <p>工作或计划</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校样权限配置文件 </td> 
   <td>经理或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对文档的访问权限</p></td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 为现有验证创建或编辑自动工作流：

1. 将鼠标悬停在文档区域中的文档上，然后单击校对工作流。

   或

   如果您正在验证查看器中查看验证，请单击左侧面板中的&#x200B;**工作流** ![工作流图标](assets/workflow-icon-proofing-viewer.png)，然后单击“编辑”图标![编辑图标](assets/edit-icon-proofing-viewer.png)以打开验证的自动工作流设置。

1. （视情况而定）如果验证当前正在使用基本工作流（不带暂存），请在显示的屏幕中单击&#x200B;**转换为自动工作流**。

   >[!NOTE]
   >
   >从基本工作流转换为自动工作流时，无法编辑第一个阶段，但可以添加和配置新阶段。

1. （视情况而定）要使用您的Adobe Workfront管理员创建并与您共享的自动工作流模板，请单击&#x200B;**添加模板**，在显示的框中选择该模板，然后单击&#x200B;**添加模板**。

   有关详细信息，请参阅本文中的[关于使用自动化工作流模板](#about-using-automated-workflow-templates)。

1. 向自动工作流添加阶段：

   1. 单击右上角附近的&#x200B;**新阶段**。
   1. 在出现的框中，键入阶段的&#x200B;**名称**。
   1. （可选）设置阶段的截止日期。
   1. 在&#x200B;**激活阶段**&#x200B;部分中，选择您希望阶段激活的方式：


      <table>
      <tbody>
      <tr>
      <td><strong>创建验证时</strong></td>
      <td>该阶段会自动变为活动状态，因为已创建验证。</td>
      </tr>
      <tr>
      <td><strong>当上一个阶段的截止日期过去时</strong></td>
      <td>单击<strong>父阶段</strong>下拉列表中的上一个阶段。</td>
      </tr>
      <tr>
      <td><strong>在特定日期和时间</strong></td>
      <td>单击<strong>日期</strong>框以选择日期，然后单击右侧的框以选择时间。</td>
      </tr>
      <tr>
      <td><strong>所有决策均为“已批准”或“已批准”，且更改位于父阶段</strong></td>
      <td>单击<strong>父阶段</strong>下拉列表中的父阶段。</td>
      </tr>
      <tr>
      <td><strong>所有决策都在父级阶段批准</strong></td>
      <td>单击<strong>父阶段</strong>下拉列表中的父阶段。</td>
      </tr>
      <tr>
      <td><strong>所有决策都已作出</strong></td>
      <td>单击<strong>父阶段</strong>下拉列表中的父阶段。</td>
      </tr>
      </tbody>
      </table>


   1. 输入联系人姓名或电子邮件地址，并配置阶段审阅人的设置。

      有关添加审阅人的信息，请参阅本文中的[关于将审阅人添加到阶段](#about-adding-reviewers-to-a-stage)。

   1. 使用以下任一选项进一步配置暂存：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader"><strong>截止日期选项</strong> </td>
         <td><p>要设置阶段的截止日期，请单击<strong>截止日期选项</strong>下拉列表中的选项。 然后，在<strong>Deadline</strong>下，执行以下操作之一：</p>
          <ul>
           <li>如果您选择<strong>设置特定日期</strong>：请选择所需的截止日期和时间。</li>
           <li>如果您选择<strong>从阶段激活日期计算</strong>：请选择要添加到阶段激活日期的工作日数以确定截止日期。</li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">锁定阶段</td>
         <td>指定可以锁定舞台的时间。 </td>
        </tr>
        <tr>
         <td role="rowheader">主要决策者</td>
         <td><p>选择阶段上的主要决策者（仅在您将至少一名具有“审批者”或更高验证角色的人员添加到阶段后可用）。 如果选择主要决策者，则在此阶段上禁用<strong>仅需要一个决策</strong>选项。</p></td>
        </tr>
        <tr>
         <td role="rowheader">只需一个决策</td>
         <td>当决策者做出决策时，结束整个审核过程。<p>如果您在<strong>主要决策者</strong>下拉菜单中指定了用户，则此选项不可用。</p></td>
        </tr>
        <tr>
         <td role="rowheader">专用阶段</td>
         <td>仅允许以下人员查看在此阶段所做的评论和决策：主管、Adobe Workfront管理员和Workfront Proof管理员</td>
        </tr>
        <tr>
         <td role="rowheader">通过电子邮件通知用户</td>
         <td>轮到审阅人处理验证时，通过电子邮件通知他们。</td>
        </tr>
       </tbody>
      </table>

   1. 单击&#x200B;**添加阶段**。

1. 根据需要重复上一步添加更多阶段。

   将阶段添加到自动工作流时，屏幕上会出现一个图表来表示这些阶段：

   ![工作流程图](assets/workflow-diagram-existing-proof-qs-350x215.png)

1. 完成添加阶段后，单击&#x200B;**完成**。

## 关于使用自动工作流模板 {#about-using-automated-workflow-templates}

使用自动工作流模板时，请考虑以下事项：

1. 自动工作流模板的设置确定您可以使用自动工作流执行哪些操作以进行验证。 例如，如果在模板中禁用了添加暂存按钮，则当您使用验证的自动工作流设置时，该按钮将不可见。
1. 当有人在自动工作流模板中被添加到阶段，但也以审阅者身份出现在验证中时，应用模板会将审阅者从阶段中删除。 如果不将其他审阅人添加到阶段，则会显示一条消息，提示您添加审阅人。
1. 能否修改自动工作流模板取决于Workfront管理员配置的模板设置，如中所述。 如果禁用了修改模板的功能，则只有模板所有者可以修改模板。

## 关于向阶段添加审阅者 {#about-adding-reviewers-to-a-stage}

将审阅者添加到阶段时，请考虑以下事项：

* 将用户添加到阶段后，您可以为该用户在验证上配置设置，如验证角色和他们应具有的任何其他权限，以及当人们对验证做出评论和决策时将收到的电子邮件警报类型。
* 您可以将一个或多个用户从一个阶段拖到另一个阶段。 您可以将用户直接拖到另一个阶段，也可以将用户拖到&#x200B;**阶段**&#x200B;图上的阶段。 要选择多个用户，请按Shift+Ctrl键（在Windows上）或Shift+Command键(在Mac上)。
* 您只能将查看者添加到验证一次，这意味着您无法将同一人员添加到验证上的多个阶段。
* 未添加到专用阶段的审阅人无法在验证上看到该阶段，也无法在该阶段中做出评论。
* 默认情况下，将用户添加到阶段会授予该用户从创建验证之时起查看验证的权限。

  在工作流进入添加用户的阶段之前，Workfront管理员可以限制用户访问验证。 有关更多信息，请参阅  中的。
