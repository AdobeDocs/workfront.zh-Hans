---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 在Experience Manager Assets Essentials集成中使用工作流
description: 在Experience Manager Assets Essentials集成中使用工作流
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
source-git-commit: 9080dfe7e46a3780d493b59c8f2a3c4efbc011e7
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 0%

---

# 在Experience Manager Assets集成中使用工作流

<span class="preview">此页面上的信息是指尚未普遍提供的功能。 它仅在“预览沙盒”环境中可用。</span>

工作流是一组将Workfront与Adobe Experience Manager as a Cloud Service连接的操作。 Workfront管理员可以在Workfront中配置工作流，然后将其分配给项目模板。 当使用分配了工作流的项目模板创建项目时，将触发工作流中定义的操作。

>[!NOTE]
>
>工作流仅在Adobe Experience Manager as a Cloud Service集成中可用。 它们在与Adobe Experience Manager Assets Essentials的集成中不可用。


## 访问要求

您必须具备以下条件：

<table>
  <tr>
   <td><strong>Adobe Workfront计划*</strong>
   </td>
   <td>任意
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront许可证*</strong>
   </td>
   <td>请求或更高版本
   </td>
  </tr>
  <tr>
   <td><strong>产品</strong>
   </td>
   <td><p>您必须具有Experience Manager Assetsas a Cloud Service或Assets Essentials，并且必须以Admin Console用户身份添加到产品中。</p><p>您必须对Adobe Experience Manager中的存储库具有写入权限，才能创建链接的文件夹。</p>&gt;
   </td>
  </tr>
  <tr>
   <td><strong>访问级别配置*</strong>
   </td>
   <td>编辑对文档的访问
<p>
<strong>注意： </strong>如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <strong>创建或修改自定义访问级别</strong>.
   </td>
  </tr>
  <tr>
   <td><strong>对象权限</strong>
   </td>
   <td>管理项目的访问权限或更高权限 
<p>
有关请求其他访问权限的信息，请参阅 <strong>请求对对象的访问 </strong>.
   </td>
  </tr>
</table>

## 先决条件

开始之前，

* 您的Workfront管理员必须在Adobe Experience Manager集成中配置工作流。 有关更多信息，请参阅 [配置Experience Manager Assetsas a Cloud Service集成](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).

## 向模板添加工作流

您可以向项目模板添加工作流。 该工作流将应用于使用该模板创建的任何项目。

1. <!-- main menu snippet??--> 通过单击 **模板** 在主菜单中，从列表中选择模板。
1. 单击 **Experience Manager Assets** 中。

   >[!NOTE]
   >
   >如果Experience Manager Assets部分在左侧导航中不可见，则表示您的Workfront管理员尚未为您的组织启用工作流。 <!--Is this right?-->

1. 在 **为自动化工作流字段选择集成**，选择要用于从此模板创建的项目的工作流的集成。
1. （可选）编辑要应用于从此模板创建的项目的任何工作流值。

   例如，要在默认值以外的位置创建链接文件夹，请输入链接文件夹的位置。

   只有已在“设置”的“Experience Manager”区域中激活的工作流才能在模板或项目中使用。

1. 您所做的更改会自动保存。 <!-- do they though??-->

## 向项目添加工作流

您可以在创建项目时添加工作流，也可以向现有项目添加工作流。 在这两种情况下，您都将使用项目模板来添加工作流。

### 创建项目时添加工作流

1. 开始创建项目。

   有关说明，请参阅 [使用模板创建项目](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

1. 选择项目的模板时，请选择包含要用于此项目的工作流的模板。
1. （可选）编辑项目的任何工作流值，如 [编辑项目中的工作流值](#edit-workflow-values-in-a-project).

   只有已在“设置”的“Experience Manager”区域中激活的工作流才能在模板或项目中使用。


### 向现有项目添加工作流

1. 开始向项目添加模板。

   有关说明，请参阅 [将模板附加到项目](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

1. 选择项目的模板时，请选择包含要用于此项目的工作流的模板。
1. （可选）编辑项目的任何工作流值，如 [编辑项目中的工作流值](#edit-workflow-values-in-a-project).

### 编辑项目中的工作流值

您可以在项目级别编辑工作流值。 项目级别的工作流值会覆盖在项目模板中设置的值，这会覆盖在Adobe Experience Manager Assets集成中设置的默认值。

所有工作流值均可在以下位置找到：

* 创建项目或编辑项目窗口的工作流部分。
* 左侧导航的Adobe Experience Manager部分。


   >[!NOTE]
   >
   >如果这些区域不可见，则表示您的Workfront管理员尚未为您的组织启用工作流。

#### 链接的文件夹

要编辑链接文件夹的工作流，请执行以下操作：

1. 切换 **[!UICONTROL 创建链接的文件夹]** 开。
1. 选择一个文件夹路径，以指示您希望将所有关联的文件夹关联到此集成的位置。
1. 如果使用“创建项目”或“编辑项目”窗口，请单击“保存”。

   或

   如果您位于Adobe Experience Manager区域，则所做的更改会自动保存。 <!--Do they though?-->

