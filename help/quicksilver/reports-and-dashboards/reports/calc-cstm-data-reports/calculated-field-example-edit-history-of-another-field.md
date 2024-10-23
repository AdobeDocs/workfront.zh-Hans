---
content-type: reference
product-area: reporting
keywords: 审核，跟踪，自定义，字段
navigation-topic: calculate-custom-data-reports
title: “计算自定义字段示例：显示字段的编辑历史记录”
description: 如果用户定期更新自定义字段，并且您希望捕获对字段所做的所有更改的日志以及发生更改的日期，则可以在计算的自定义字段中捕获此信息。
author: Nolan
feature: Reports and Dashboards
exl-id: e233ef28-c95a-42a1-b2eb-448dad5feddb
source-git-commit: ecafbd693237427d727b15dd22afd485b4e59c72
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 0%

---

# 计算自定义字段示例：显示字段的编辑历史记录

如果用户定期更新自定义字段，并且您希望捕获对字段所做的所有更改的日志以及发生更改的日期，则可以在计算的自定义字段中捕获此信息。

以下示例说明如何构建“说明编辑历史记录”计算字段，以捕获对名为“说明”的单行文本字段所做的所有更改。

>[!TIP]
>
>您可以按照此示例，查看所有类型的自定义字段，而不仅仅是单行文本字段。

此操作如下：

* 将“说明编辑历史记录”字段限制为最近2000个字符，以保持在Workfront数据库限制之内。
* 检查指令字段的当前值是否与指令编辑历史记录值的前面匹配；它假定为空白，否则将执行以下操作：

   * 如果二者匹配，则将“指令编辑历史记录”保留不变；
   * 如果它们不匹配，它将用指令字段中的最新值替换指令编辑历史记录，后跟括号中的当前日期、垂直栏和先前的指令编辑历史记录，从而保留先前的值和输入时的日期。

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
   <td>任何</td> 
  </tr> 
  <tr> 
   <td> <p>Workfront许可证*</p> </td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td><strong>访问级别配置*</strong> </td> 
   <td> <p>对自定义Forms的管理访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>对象权限</strong> </p> </td> 
   <td> <p>管理自定义表单的权限 </p> <p>有关详细信息，请参阅<a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">共享自定义表单</a>。<br></p> </td> 
  </tr> 
 </tbody> 
</table>

## 先决条件

要将显示字段编辑历史记录的计算字段添加到自定义表单，您必须首先：

* 创建自定义表单
* 将您要捕获其历史记录的字段添加到自定义表单

## 显示字段的编辑历史记录

1. 转到要添加计算字段的自定义表单。

1. 例如，要创建单行文本自定义字段，请执行以下操作：

   1. 单击&#x200B;**单行文本**。
   1. 为自定义字段指定&#x200B;**标签**。 例如，您可以将其命名为“Instructions”。
   1. 单击&#x200B;**应用**。

1. 单击&#x200B;**已计算**&#x200B;以将已计算的自定义字段添加到表单。
1. 为计算的自定义字段指定&#x200B;**标签**。 例如，您可以将其命名为“Instructions Edit History”。

   该字段将捕获对您创建的第一个字段（“说明”）所做的任何更改。

1. 单击&#x200B;**保存并关闭**。
1. 单击已添加两个字段的表单名称以重新打开它。
1. 单击计算自定义字段&#x200B;**指令编辑历史记录**，然后将以下内容复制并粘贴到&#x200B;**计算**&#x200B;框中：

   ```
   LEFT(IF(LEFT({DE:Instructions Edit History},LEN(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})))={DE:Instructions},{DE:Instructions Edit History},CONCAT(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})," (",$$NOW,") | ",{DE:Instructions Edit History})),2000)
   ```

1. （推荐）将相同的计算粘贴到表单上计算字段的&#x200B;**说明**&#x200B;字段中。
1. 确保在&#x200B;**格式**&#x200B;字段中选择&#x200B;**文本**，以将计算的自定义字段设置为文本格式。

   这是默认设置。

1. 单击&#x200B;**保存并关闭**。

   现在，当您将自定义表单附加到对象，然后有人更改了&#x200B;**指令**&#x200B;字段中的信息时，**指令编辑历史记录**&#x200B;字段显示最新值，后跟括号中的当前日期，以及垂直条。 如果进行了进一步的更改，则会以相同的方式将这些更改添加到此信息中。

   在上述计算中，您可以将&#x200B;*指令*&#x200B;替换为要跟踪其历史记录的单行文本字段的准确名称，将&#x200B;**指令编辑历史记录**&#x200B;替换为计算字段的准确名称。
