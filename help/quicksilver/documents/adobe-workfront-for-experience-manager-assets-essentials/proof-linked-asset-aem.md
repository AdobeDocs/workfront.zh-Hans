---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 校对针对Experience Manager Assets或Assets Essentials的链接资源
description: 从Experience Manager Assets Essentials链接资源后，您可以创建验证并分配用户以查看该资源并向其添加评论。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abd641a1-081b-4b86-95ee-f0ed030d704c
source-git-commit: 430751f0e38c6c45145c965398990ee3652f36fe
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 2%

---

# 校对针对Experience Manager Assets或Assets Essentials的链接资源

从Experience Manager Assets Essentials链接资源后，您可以创建验证并分配用户以查看该资源并向其添加评论。

## 访问要求

<!-- Audited: 4/2025 -->

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p> 任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>标准</p>
   <p>工作或更高</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">其他产品</td> 
   <td>您必须安装了Experience Manager as a Cloud Service或Assets Essentials，并且您必须作为用户添加到Admin Console的产品中。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对文档的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看访问权限或更高版本</p>  </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

开始之前：

* 您的Workfront管理员必须配置Experience Manager集成。 有关详细信息，请参阅[配置Experience Manager Assets as a Cloud Service集成](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)或[配置Experience Manager Assets Essentials集成](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)。

## 创建校样

您可以创建静态、视频或交互式校样。

要创建验证，请执行以下操作：

1. 转到要验证的项目、任务或问题，然后单击&#x200B;**文档**&#x200B;部分。
1. 将鼠标悬停在文档上，然后单击文档名称下方显示的&#x200B;**创建验证**&#x200B;链接。

   >[!NOTE]
   >
   >如果您在上传用户配置文件中启用了文档&#x200B;**时**&#x200B;自动生成验证，则系统会自动创建一个简单的验证。

1. 从下拉列表中选择以下选项之一：

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
      <td> <p>利用此选项，可配置基本或高级工作流并修改所创建验证的验证设置。 有关更多信息，请参阅： </p> 
       <ul> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">使用基本工作流创建高级校对</a> </p> </li> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">使用自动化工作流创建高级校对</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

## 管理现有校对

创建验证后，您可以执行以下操作：

* 查看当前阶段活动
* 更新审阅者和截止日期
* 编辑工作流

有关如何管理现有校样的更多信息，请参阅[在Adobe Workfront中管理校样：文章索引](../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md)。

## 审阅校对

分配的审阅人可以执行以下操作：

* 查看资源并进行评论
* 向评论添加操作
* 比较版本
* 批准或拒绝证明

有关可以使用校对工具执行的操作的更多信息，请参阅[在Adobe Workfront中查看校对：文章索引](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md)。
