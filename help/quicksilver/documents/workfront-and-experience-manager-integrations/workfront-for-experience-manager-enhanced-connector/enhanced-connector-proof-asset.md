---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: 验证具有增强连接器的链接资产
description: 从Experience Manager Assets链接资源后，您可以创建验证并分配用户以进行审核并向资源添加评论。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d72ac84f-1865-4122-bc77-d8200a4d0f69
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# 验证具有增强连接器的链接资产

从Experience Manager Assets链接资源后，您可以创建验证并分配用户以进行审核并向资源添加评论。 从链接资产创建的验证计入您的验证存储配额。

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
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>您必须安装了Experience Manager Assets Essentials。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看访问权限或更高版本</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 先决条件

在开始之前，您必须

* 安装Workfront for Experience Manager增强型连接器

## 创建验证

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
      <td role="rowheader">简单校对</td> 
      <td>此选项创建一个未附加工作流的验证，并应用默认验证设置。 您可以更新默认验证设置，或在创建验证后添加工作流。 有关校对设置的详细信息，请参阅<a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">编辑校对设置</a>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">高级校对</td> 
      <td> <p>利用此选项，可配置基本或高级工作流并修改所创建验证的验证设置。 有关更多信息，请参阅 </p> 
       <ul> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">使用基本工作流创建高级校对</a> </p> </li> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">使用自动化工作流创建高级校对</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

## 管理现有校对

创建验证后，您可以执行以下操作

* 查看当前阶段活动
* 更新审阅者和截止日期
* 编辑工作流

有关如何管理现有校样的更多信息，请参阅[在Adobe Workfront中管理校样](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md)。

## 审查验证

分配的审阅人可执行如下操作

* 查看资源并进行评论
* 向评论添加操作
* 比较版本
* 批准或拒绝证明

有关可以使用校对工具执行的操作的更多信息，请参阅[在Adobe Workfront中查看校对](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md)。
