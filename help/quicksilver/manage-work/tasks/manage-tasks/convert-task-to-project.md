---
product-area: projects
navigation-topic: manage-tasks
title: 将任务转换为项目
description: 当项目中的任务需要完成的工作量比最初计划的要大时，您可以将其转换为项目。
author: Alina
feature: Work Management
exl-id: a45f0af4-1768-4f20-80d4-912e6fe0fc03
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# 将任务转换为项目

当项目中的任务需要完成的工作量比最初计划的要大时，您可以将其转换为项目。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对任务和项目的访问权限</p> <p>使用模板转换为项目时，查看或更高程度地访问模板</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理任务的权限</p> <p>查看模板的权限（如果使用模板转换为项目）</p> <p>创建项目后，您将拥有该项目的“管理”权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 将任务转换为项目的注意事项

* 将删除原始任务。
* 任务批准将被删除。
* 所有子任务、问题和注释汇总到新项目。
* 文档、文档版本和校样将移到新项目中。
* 所有子任务和问题的状态和完成百分比将保留。
* 任务的共享用户将成为项目上的共享用户。
* 项目开始日期设置为任务的开始日期。
* 如果任务状态为“新建”，则项目状态将设置为“计划”。
* 如果任务状态为“进行中”，则项目状态将设置为“当前”。
* 如果任务状态为“完成”，则项目状态将设置为“完成”。

## 将任务转换为项目

1. 转到要转换为项目的任务。
1. 单击 **更多** 图标 ![](assets/more-icon.png)，则 **转换为项目**.
1. 选择以下选项之一：

   * **新项目**
   * 中的模板 **从模板中选择** 部分

      ![](assets/convert-task-to-project-template-option-dropdown-nwe-350x209.png)

1. 单击 **继续** 在显示的通知中。
1. 在 **转换为项目** 框中，指定以下内容：

   * **名称**:为项目命名。 默认名称是任务的名称。
   * （可选） **描述**:描述此项目的用途。
   * （可选和视情况而定）如果您选择从模板创建项目，请更新 **转换为项目** 对话框。

      有关编辑项目字段的更多信息，请参阅 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md).

      >[!TIP]
      >
      >要更新“转换为项目”框中“财务”部分中的字段，您必须在访问级别拥有对财务数据的编辑访问权限。 如果您在访问级别具有查看财务数据的访问权限，则模板中的所有财务信息都会传输到新项目，并且在转换问题时无法对其进行编辑。 有关信息，请参阅 [授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) 和 [共享模板](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * （可选）添加 **自定义Forms** 到新项目。

      >[!TIP]
      如果将附加到任务的多对象自定义表单配置为与任务和项目一起使用，则在您进行转换时，表单中保存的所有信息都将保留。
      如果您使用模板进行转换，并且附加到模板的自定义表单包含自定义字段，该自定义字段也可在附加到任务的自定义表单中找到，则任务中的字段值将用于新项目。 但是，如果任务上的自定义字段为空，则会使用模板中的值。

1. 单击 **保存更改**.
