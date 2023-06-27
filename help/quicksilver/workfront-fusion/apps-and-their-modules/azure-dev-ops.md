---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Azure DevOps模块
description: 在 [!DNL Adobe Workfront Fusion] 场景，您可以自动执行使用 [!DNL Azure DevOps]，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: ecaa93c9-47bb-4fe1-87b4-d2e117cc68ae
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1797'
ht-degree: 0%

---

# [!DNL Azure DevOps] 模块

在 [!DNL Adobe Workfront Fusion] 场景，您可以自动执行使用 [!DNL Azure DevOps]，并将其连接到多个第三方应用程序和服务。

如果您需要有关创建方案的说明，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

有关模块的信息，请参见 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## 访问要求

您必须具有以下权限才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td>
  <td> <p>[！UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td>
   <td> <p>[！UICONTROL计划]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td> 
   <td>
   <p>当前许可证要求：否 [!DNL Workfront Fusion] 许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] 用于工作自动化和集成] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 计划，您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 计划。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关以下项的信息 [!DNL Adobe Workfront Fusion] 许可证，请参见 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 先决条件

使用 [!DNL Azure DevOps] 模块，您必须拥有 [!DNL Azure] DevOps帐户。

## Connect [!DNL Azure DevOps] 到 [!DNL Workfront Fusion] {#connect-azure-devops-to-workfront-fusion}

1. 添加 [!DNL Azure DevOps] 模块到您的场景。
1. 单击 **[!UICONTROL 添加]** 旁边的 [!UICONTROL 连接] 字段。
1. 在 [!UICONTROL 连接类型] 字段，选择 **[!DNL Azure DevOps]**.

   >[!IMPORTANT]
   >
   >此 [!UICONTROL [!DNL Azure DevOps] （请求所有范围）] 在不久的将来，连接类型将被弃用。 因此，我们不建议使用它。

1. 填写以下字段：

   <table style="table-layout:auto">
        <tr>
            <td>[！UICONTROL连接名称]</td>
            <td>输入正在创建的连接的名称。</td>
        </tr>
      <tr>
            <td>[！UICONTROL组织]</td>
            <td>输入您在其下创建 [!DNL Azure DevOps] 应用程序。</td>
        </tr>
    </table>

1. 单击 **[!UICONTROL 继续]** 以完成连接设置并继续创建场景。

## [!UICONTROL Azure DevOps] 模块及其字段

配置时 [!DNL Azure DevOps] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除此以外，还有 [!DNL Azure DevOps] 可能会显示字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [触发器](#triggers)
* [操作](#actions)
* [搜索](#searches)

### 触发器

#### [!UICONTROL 关注工作项]

此即时触发器模块执行在中添加、更新或删除记录时的场景 [!UICONTROL Azure DevOps].

该模块返回与记录关联的任何标准字段，以及连接访问的任何自定义字段和值。 您可以将此信息映射到场景中的后续模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Webhook]</td> 
   <td> <p>选择或添加模块的webhook。</p> <p>有关触发器模块中Webhook的更多信息，请参阅 <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">中的即时触发器(Webhook) [!DNL Adobe Workfront Fusion]</a>.</p> <p>有关如何创建webhook的信息，请参见 <a href="../../workfront-fusion/apps-and-their-modules/webhooks-updated.md" class="MCXref xref">Webhook</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 操作

* [自定义API调用](#custom-api-call)
* [读取记录](#read-record)
* [创建记录](#create-a-record)
* [更新工作项](#update-a-work-item)
* [[!UICONTROL 上传附件]](#upload-an-attachment)
* [下载附件](#download-an-attachment)
* [链接工作项]([!UICONTROL #link-work-items])

#### [!UICONTROL 自定义API调用]

通过此操作模块，您可以对 [!DNL Azure DevOps] API。 这样，您就可以创建一个其他人无法实现的数据流自动化 [!DNL Azure DevOps] 模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Azure DevOps] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] 到[！UICONTROL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL基本URL]</td> 
   <td> <p>选择或映射用于连接到 [!DNL Azure DevOps] 帐户</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL相对URL]</td> 
   <td> <p>输入为此API调用要连接的相对URL。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例: </b></span></span><code>{organization}/_apis[/{area}]/{resource}</code> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL API版本]</td> 
   <td>选择或映射 [!DNL Azure DevOps] 为此API调用要连接到的API。 如果未选择版本， [!DNL Workfront Fusion] 连接到 [!DNL Azure DevOps] API版本5.1。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查询字符串]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的查询。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL主体]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的正文内容。</p> <p>注释:  <p>使用条件语句(例如 <code>if</code> 在JSON中，将引号放在条件语句之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 读取记录]

该操作模块从中的单个记录读取数据 [!DNL Azure DevOps].

您指定记录的ID。

该模块返回记录的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以将此信息映射到场景中的后续模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Azure DevOps] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] 到[！UICONTROL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td> <p>选择您要读取项目还是工作项</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL项目]</strong>：选择要读取的项目……</p> </li> 
     <li> <p><strong>[！UICONTROL工作项]</strong>：选择包含要读取的工作项的项目，然后选择该工作项类型。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出]</td> 
   <td>选择要包含在此模块的输出包中的信息。 可用字段取决于工作项类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td>输入或映射要读取的记录的ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建记录]

此操作模块创建新项目或工作项。

模块输出新创建工作项的对象ID，或新创建项目的URL和状态代码。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Azure DevOps] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] 到[！UICONTROL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td> <p>选择您要创建工作项还是项目。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL项目]</strong> </p> <p>填写以下字段：</p> 
      <ul> 
       <li> <p><strong>[！UICONTROL名称]</strong>：输入或映射新项目的名称。</p> </li> 
       <li> <p><strong>[！UICONTROL描述]</strong>：输入或映射新项目的描述。 </p> </li> 
       <li> <p><strong>[！UICONTROL可见性]</strong>：选择您希望项目是公共项目还是专用项目。 用户必须登录您的组织，并且必须已被授予项目访问权限，才能与专用项目交互。 未登录到贵组织的用户可看到公共项目。</p> </li> 
       <li> <p><strong>[！UICONTROL版本控制]</strong>：选择是否希望项目使用 [!DNL Git] 或[！UICONTROL Team Foundation版本控制(TFCV)]进行版本控制。</p> </li> 
       <li> <p><strong>[！UICONTROL工作项进程]</strong>：选择要用于项目的工作流程。 选项有[！UICONTROL Basic]、[！UICONTROL Scrum]、[！UICONTROL功能成熟度模型集成(CMMI)]和[！UICONTROL Agile]。</p> <p>有关的详细信息 [!DNL Azure DevOps] 进程，请参见 <a href="https://docs.microsoft.com/en-us/azure/devops/boards/work-items/guidance/choose-process?view=azure-devops&amp;tabs=basic-process">选择进程</a> 在 [!DNL Azure DevOps] 文档。</p> </li> 
      </ul> </li> 
     <li> <p><strong>[！UICONTROL工作项]</strong> </p> <p>填写以下字段：</p> 
      <ul> 
       <li> <p><strong>[！UICONTROL项目]</strong>：选择要创建工作项的项目。</p> </li> 
       <li> <p><strong>[！UICONTROL工作项类型]</strong>：选择要创建的工作项类型。</p> </li> 
       <li> <p><strong>[！UICONTROL其他字段]</strong>：在这些字段中，输入您希望工作项对于给定属性具有的值。 可用字段取决于工作项类型。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新工作项]

此操作模块使用其ID更新现有工作项。

模块返回已更新工作项的ID。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Azure DevOps] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] 到[！UICONTROL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL项目]</td> 
   <td>选择包含要更新的工作项的项目。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL工作项类型]</td> 
   <td> <p>选择要更新的工作项的类型。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL其他字段]</td> 
   <td>在每个字段中，输入您希望工作项对于给定属性具有的值。 可用字段取决于工作项类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL工作项ID]</td> 
   <td>输入或映射要更新的工作项的ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 上传附件]

此操作模块上传文件并将其附加到工作项。

模块将返回附件的附件ID和下载URL。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Azure DevOps] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] 到[！UICONTROL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL项目] </td> 
   <td> <p>选择要上载附件的项目。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL工作项ID]</td> 
   <td> <p>输入或映射要上载附件所在工作项的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL注释]</td> 
   <td>输入要添加到上传附件的注释文本。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL源文件] </td> 
   <td>从上一个模块中选择源文件，或者输入或映射源文件的名称和内容。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下载附件]

此操作模块下载附件。

模块将返回附件的文件内容。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Azure DevOps] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] 到[！UICONTROL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL附件URL]</td> 
   <td> <p>输入或映射要下载的附件的URL。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 链接工作项]

此操作模块链接两个工作项并定义它们之间的关系。

模块返回主工作项和任何关联字段的ID，以及连接访问的任何自定义字段和值。 您可以将此信息映射到场景中的后续模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Azure DevOps] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] 到[！UICONTROL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL工作项ID]</td> 
   <td>输入或映射要将其他工作项链接到的主工作项项的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL链接的工作项ID]</td> 
   <td>输入或映射要链接到主工作项的工作项的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL链接类型]</td> 
   <td> <p>定义要链接的工作项之间的关系。</p> <p>有关更多信息，请参阅 <a href="https://docs.microsoft.com/en-us/azure/devops/boards/queries/link-type-reference?view=azure-devops">链接类型引用</a> 在[！UICONTROL Azure DevOps]文档中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL注释]</td> 
   <td>输入或映射注释的文本。 这对于解释链接的推理或意图很有用。</td> 
  </tr> 
 </tbody> 
</table>

### 搜索

#### [!UICONTROL 列出工作项]

此操作模块可检索中特定类型的所有工作项 [!DNL Azure DevOps] 项目。

模块返回主工作项和任何关联字段的ID，以及连接访问的任何自定义字段和值。 您可以将此信息映射到场景中的后续模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Azure DevOps] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] 到[！UICONTROL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL项目]</td> 
   <td>选择要从中检索工作项的项目。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL工作项类型]</td> 
   <td> <p>选择要检索的工作项类型。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出]</td> 
   <td>选择要显示在模块输出中的属性。 可用字段取决于您要检索的工作项类型。 您必须至少选择一个属性。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>输入或映射最大工作项数，该最大工作项数 [!DNL Workfront Fusion] 在一个执行周期内返回。</td> 
  </tr> 
 </tbody> 
</table>
