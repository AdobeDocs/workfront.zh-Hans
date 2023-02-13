---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: 使用增强的连接器校样链接的资产
description: 从Experience Manager Assets链接资产后，您可以创建校样并分配用户以审核资产并向资产添加评论。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d72ac84f-1865-4122-bc77-d8200a4d0f69
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# 使用增强的连接器校样链接的资产

从Experience Manager Assets链接资产后，您可以创建校样并分配用户以审核资产并向资产添加评论。 从链接的资产创建的校样将计入校样存储配额。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p> 任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>你一定有Experience Manager Assets·艾斯提亚。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看访问权限或更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

在开始之前，您必须

* 安装Workfront for Experience Manager增强连接器

## 创建校样

您可以创建静态校样、视频校样或交互式校样。

要创建校样，请执行以下操作：

1. 转到要校样的项目、任务或问题，然后单击 **文档** 中。
1. 将鼠标悬停在文档上，然后单击 **创建校样** 链接。

   >[!NOTE]
   >
   >如果 **上传文档时自动生成校样** 系统会在您的用户配置文件中启用，从而自动创建一个简单的校样。

1. 选择以下选项之一：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">简单校样</td> 
      <td>此选项会创建一个未附加工作流的校样，并应用默认校样设置。 您可以更新默认的校样设置，或在创建校样后添加工作流。 有关校样设置的更多信息，请参阅 <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">编辑校样设置</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">高级校样</td> 
      <td> <p>此选项允许您配置基本或高级工作流，并修改所创建校样的校样设置。 有关更多信息，请参阅 </p> 
       <ul> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">使用基本工作流创建高级校样</a> </p> </li> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">使用自动工作流创建高级校样</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

## 管理现有校样

创建校样后，您便可以执行

* 查看当前阶段活动
* 更新审阅人和截止日期
* 编辑工作流

有关如何管理现有校样的更多信息，请参阅 [在Adobe Workfront中管理校样](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md).

## 查看验证

指派的审阅人可以执行以下操作

* 查看资产并进行评论
* 向注释添加操作
* 比较版本
* 批准或拒绝校样

有关使用校对工具可执行的操作的更多信息，请参阅 [在Adobe Workfront中审阅校样](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).
