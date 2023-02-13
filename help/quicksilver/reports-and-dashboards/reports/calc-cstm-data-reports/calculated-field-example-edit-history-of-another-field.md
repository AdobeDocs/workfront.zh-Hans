---
content-type: reference
product-area: reporting
keywords: 审核，跟踪，自定义，字段
navigation-topic: calculate-custom-data-reports
title: “计算的自定义字段示例：显示字段的编辑历史记录”
description: 如果用户定期更新自定义字段，并且您想要捕获对字段所做的所有更改的日志以及更改发生的日期，则可以在计算的自定义字段中捕获此信息。
author: Nolan
feature: Reports and Dashboards
exl-id: e233ef28-c95a-42a1-b2eb-448dad5feddb
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '666'
ht-degree: 0%

---

# 计算的自定义字段示例：显示字段的编辑历史记录

如果用户定期更新自定义字段，并且您想要捕获对字段所做的所有更改的日志以及更改发生的日期，则可以在计算的自定义字段中捕获此信息。

以下示例向您展示了如何构建 *说明编辑历史记录* 计算字段，用于捕获对名为的单行文本字段所做的所有更改 *说明*.

>[!TIP]
>
>您可以对所有类型的自定义字段遵循此示例，而不仅仅是单行文本字段。

此操作将执行以下操作： 

* 限制 *说明编辑历史记录* 字段，以保留在Workfront数据库限制内。
* 检查 *说明* 字段与 *说明编辑历史记录* 值；它将其假定为空，如果不为空，则会执行以下操作： 

   * 如果匹配，则会将 *说明编辑历史记录* 原样；
   * 如果二者不匹配，它会将 *说明编辑历史记录* 的 *说明* 字段中，后跟括号、垂直条和上一个 *说明编辑历史记录*，这会保留先前的值和输入日期。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <caption style="text-align: left;"> 
  <p>*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。</p> 
 </caption> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront计划*</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td> <p>Workfront许可证*</p> </td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td><strong>访问级别配置*</strong> </td> 
   <td> <p>对自定义Forms的管理访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>对象权限</strong> </p> </td> 
   <td> <p>管理自定义表单的权限 </p> <p>有关更多信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">共享自定义表单</a>.<br></p> </td> 
  </tr> 
 </tbody> 
</table>

## 先决条件

要向自定义表单添加显示字段编辑历史记录的计算字段，您必须先：

* 创建自定义表单
* 将要捕获其历史记录的字段添加到自定义表单

## 显示字段的编辑历史记录

1. 转到要添加计算字段的自定义表单。

1. 例如，要创建单行文本自定义字段，请执行以下操作：

   1. 单击 **单行文本字段**.
   1. 指定 **标签** (例如 *说明*.
   1. 单击 **阿普利耶**.

1. 选择 **添加字段**，然后选择 **已计算** 向表单中添加计算的自定义字段。
1. 指定 **标签** ，例如 *说明编辑历史记录*.

   此字段将捕获对您创建的第一个字段(*说明*)。

1. 单击 **保存并关闭**.
1. 单击表单的名称，您现在已在其中添加两个字段以重新将其打开。
1. 单击计算的自定义字段 *说明编辑历史记录，* 然后，在“计算”框中复制并粘贴以下内容：
1. 在 **计算** 字段，为自定义字段指定以下计算：

   ```
   LEFT(IF(LEFT({DE:Instructions Edit History},LEN(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})))={DE:Instructions},{DE:Instructions Edit History},CONCAT(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})," (",$$NOW,") | ",{DE:Instructions Edit History})),2000)
   ```

1. （推荐）在 **说明** 字段。
1. 确保  **文本** 的 **格式** 字段，将计算的自定义字段格式设置为文本。

   这是默认设置。

1. 单击 **保存并关闭**.

   现在，当您将自定义表单附加到对象，然后有人在 *说明* 字段中， *说明编辑历史记录”字段显示最新值，后跟括号中的当前日期，并显示一个垂直条。 如果进行了进一步更改，则会以相同方式将这些更改添加到此信息中。

   在上述计算中，您可以将 *说明* ，其中包含您要跟踪其历史记录的单行文本字段的确切名称，以及 *说明编辑历史记录* ，其确切名称为计算字段。
