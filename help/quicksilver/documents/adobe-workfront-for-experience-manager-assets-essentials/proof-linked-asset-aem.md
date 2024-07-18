---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 校对Experience Manager Assets或Assets Essentials的链接资源
description: 从Experience Manager Assets Essentials链接资源后，您可以创建验证并分配用户以查看该资源并向其添加评论。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abd641a1-081b-4b86-95ee-f0ed030d704c
source-git-commit: 3b063899c5c7992aad71d1eb8c8fafff7fda84c3
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 1%

---

# 校对Experience Manager Assets或Assets Essentials的链接资源

从Experience Manager Assets Essentials链接资源后，您可以创建验证并分配用户以查看该资源并向其添加评论。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p> 任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>工作或更高</p>
   <p>您必须为用户启用验证。</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>您必须具有Experience Manageras a Cloud Service或Assets Essentials，并且您必须在Admin Console中作为用户添加到产品中。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看访问权限或更高版本</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 先决条件

开始之前，

* 您的Workfront管理员必须配置Experience Manager集成。 有关详细信息，请参阅[配置Experience Manager Assetsas a Cloud Service集成](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)或[配置Experience Manager Assets Essentials集成](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)。

## 创建校样

您可以创建静态、视频或交互式校样。

要创建验证，请执行以下操作：

1. 转到要验证的项目、任务或问题，然后单击&#x200B;**文档**&#x200B;部分。
1. 将鼠标悬停在文档上，然后单击文档名称下方显示的&#x200B;**创建验证**&#x200B;链接。

   >[!NOTE]
   >
   >如果您在上传用户配置文件中启用了文档&#x200B;**时**&#x200B;自动生成验证，则系统会自动创建一个简单的验证。

1. 选择下列选项之一：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>简单校对</strong></td> 
      <td>此选项创建一个未附加工作流的验证，并应用默认验证设置。 您可以更新默认验证设置，或在创建验证后添加工作流。 有关校对设置的详细信息，请参阅<a href="../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">编辑校对设置</a>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>高级校对</strong></td> 
      <td> <p>利用此选项，可配置基本或高级工作流并修改所创建验证的验证设置。 有关更多信息，请参阅 </p> 
       <ul> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">使用基本工作流创建高级校对</a> </p> </li> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">使用自动化工作流创建高级校对</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

## 管理现有校对

创建验证后，您可以执行以下操作

* 查看当前阶段活动
* 更新审阅者和截止日期
* 编辑工作流

有关如何管理现有校样的更多信息，请参阅[在Adobe Workfront中管理校样](../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md)。

## 审查验证

分配的审阅人可执行如下操作

* 查看资源并进行评论
* 向评论添加操作
* 比较版本
* 批准或拒绝证明

有关可以使用校对工具执行的操作的更多信息，请参阅[在Adobe Workfront中查看校对](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md)。
