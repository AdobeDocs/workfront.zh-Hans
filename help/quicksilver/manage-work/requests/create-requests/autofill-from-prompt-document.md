---
title: 使用由AI提供支持的表单填写功能，使用提示或文档填写请求
content-type: reference
description: 可以通过输入提示或提供文档来使用AI自动填写请求字段。
author: Becky
feature: Get Started with Workfront
exl-id: 4a22f9ea-c9ee-4947-8683-9989c54903b1
source-git-commit: 3c319ff406ca7705e618f3159edcf87d27d8229e
workflow-type: tm+mt
source-wordcount: '1370'
ht-degree: 3%

---

# 使用由AI提供支持的表单填写功能，使用提示或文档填写请求

>[!NOTE]
>
>* 此功能将作为公开测试版在以下时间表中提供：
>
>   * 每月发布： 2025年9月11日
>   * 季度发布： 2025年10月16日
>
>* 要使用此功能，您的组织必须满足使用Workfront AI Assistant的要求。 有关详细信息，请参阅[AI助手先决条件](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant)。

AI表单填写可以帮助您根据输入的提示自动填写请求字段。 它还可以基于文本填写字段，例如电子邮件和上传的文档。 您可以在提交请求之前批准或拒绝这些建议。

AI表单填写不会覆盖您已填写的任何字段。

用户不会收到他们无权访问的数据建议。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>参与者或更高版本</p>
   <p>请求或更高版本</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对问题的访问权限</p>  </td> 
  </tr> 
   <td role="rowheader">对象权限</td> 
   <td><p>将请求添加到请求队列的权限</p> <p>查看现有请求或更高权限</p> <p>有关设置请求队列的信息，请参阅<a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">创建请求队列</a>。 </p> </td> 
  <tr>
  </tr>
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

若要使用AI表单填写功能通过提示或文档填写请求，必须应用以下的&#x200B;**所有**：

* 您的组织必须已迁移到Adobe IMS (Identity Management System)
* 必须启用Adobe Unified Experience
* 您的组织必须具有Select、Prime或Ultimate Workfront计划
* Adobe必须具有已签署的Adobe Gen AI协议

  有关签署协议的更多信息，请参阅AI助手概述一文中的[签署Adobe Gen AI协议](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)。
* 必须在组织的系统设置中启用AI助手。 此项由Workfront管理员管理。

  有关在系统设置中启用AI助手的详细信息，请参阅[启用或禁用AI助手](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md)。

## 从文本提示获取建议

AI表单填写可根据文本（如电子邮件）建议字段值。 将粘贴到文本块中，Workfront会处理文本以根据文本建议字段值。

例如，如果电子邮件包含“将于6月1日到期”，并且请求表单中存在截止日期的字段，则AI表单填写将建议在6月1日填写该字段值。

在填写表单时，Workfront还会检查以前对类似上下文的请求。 例如，如果提示提及请求是针对特定客户的，Workfront可以根据之前的请求自动查找并输入该客户的账单地址。

您可以粘贴要应用于整个表单或表单单个部分的文本。

要根据粘贴的文本提示使用建议，请执行以下操作：

1. 开始创建请求。

   有关说明，请参阅[创建并提交请求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)。

1. 要将文本提示应用于整个表单，请单击表单名称下的AI图标![AI图标](assets/request-prompt-icon.png)。

   或

   要为单个分区应用文本提示，请单击分区名称旁边的AI图标![AI图标](assets/request-prompt-icon.png)。

1. 将文本粘贴到提示框中。
1. 单击&#x200B;**填写表单**。

   Workfront会生成表单建议。
1. 对于每个字段建议，请为该字段选择&#x200B;**接受**&#x200B;或&#x200B;**拒绝**。

   ![接受或拒绝建议](assets/accept-reject-suggestion.png)

   或

   选择页面顶部的&#x200B;**全部接受**&#x200B;或&#x200B;**全部拒绝**&#x200B;以接受或拒绝所有建议。

   >[!NOTE]
   >
   >当您提交请求时，任何未审核的建议都将被自动接受。

### 文本提示示例

这些示例显示人工智能可引用其他项目的各种方式的提示。

#### 引用过去的客户营销活动

>[!BEGINSHADEBOX]

创建一个与我们在（客户公司）第2季度发布会上类似的促销活动请求，但这次是针对他们的汽车部门。 保留相同的可交付结果集和受众配置文件。

>[!ENDSHADEBOX]

#### 基于现有项目构建

>[!BEGINSHADEBOX]

使用我们在（项目名称）项目去年春季启动时所用的相同设置。 我想要开展一场以同一高管受众为目标的数字广告营销活动，并包含更新后的本季度日期。

>[!ENDSHADEBOX]

#### 重用过去交付项中的样式

>[!BEGINSHADEBOX]

准备类似于去年运行的（客户公司）夏季促销活动的请求。 专注于社交媒体资产，保持西班牙语作为主要语言，并将预算调整至75,000美元。

>[!ENDSHADEBOX]

#### 展开旧版营销活动类型

>[!BEGINSHADEBOX]

请参考第1季度的（营销活动名称）网络研讨会系列营销活动。 我想要相同的注册工作流程和资产，但这一次的主题是“财务规划中的人工智能”，观众是年轻的专业人士。

>[!ENDSHADEBOX]

#### 重复对其他产品的请求

>[!BEGINSHADEBOX]

设置营销活动请求，就像我们处理的（客户公司）品牌重塑项目一样，但将替换为（新客户公司）作为客户。 使所有交付项与公司品牌保持一致。

>[!ENDSHADEBOX]

#### 含隐式引用的叙述样式

>[!BEGINSHADEBOX]

我们正在策划一场类似于去年投放的假日社交广告的营销活动。 预算应约为5万，目标是创造潜在客户，交付成果应包括Instagram和TikTok资源。

>[!ENDSHADEBOX]


## 根据您上传的文档获取建议

由AI提供支持的表单填写功能可使用提示填写请求，或者文档可以根据您上传的文档建议字段值。

此类建议还会检查以前对类似上下文的请求。 例如，如果提示提及请求是针对特定客户的，Workfront可以根据之前的请求自动查找并输入该客户的账单地址。

### 文档上传护栏

#### 支持的文件类型

支持以下文件类型：

<table>
<tr style="border: 0;">
<td>
<ul>
<li>BMP</li>
<li>CSV</li>
<li>DOC</li>
<li>DOCX</li>
<li>GIF</li>
<li>JPEG</li>
</ul>
</td>
<td>
<ul>
<li>ODP</li>
<li>ODS</li>
<li>ODT</li>
<li>PDF</li>
<li>PNG</li>
<li>PPT</li>
</ul>
</td>
<td>
<ul>
<li>PPTX</li>
<li>RTF</li>
<li>TIFF</li>
<li>TXT</li>
<li>XLS</li>
<li>XLSX</li>
</ul>
</td>
</tr>
</table>

#### 支持的文件大小

每个文件的大小最多可达100 MB

#### 文件数

您最多可以上传50个文件（页面、幻灯片或工作表）。

>[!IMPORTANT]
>
>文档将转换为一系列图像，每个图像都被视为单独的文件。
>
>例如，您可以上传一个包含50张幻灯片的PowerPoint，或上传每个包含10页的5个Word文档。

#### 支持的字段类型

Workfront字段类型会影响给定字段是否可以自动填写。

<table>
<tr>
<td><b>受支持的</b><br>由AI提供支持的表单填写功能可以填写</td>
<td><b>不支持</b> <br>AI支持的表单填写未填写</td>
</tr>
<tr>
<td>
<ul>
<li>单行文本</li>
<li>文本区域或段落</li>
<li>日期字段</li>
<li>复选框</li>
<li>单选按钮</li>
<li>单选和多选下拉菜单</li>
</ul>
</td>
<td><li>键盘缓冲</li>
<li>外部查找</li>
<li>内部查找</li>
<li>参考</li>
<li>WF Planning嵌入字段</li>
</ul>
</td>
</tr>
</table>

#### 其他最佳实践

将文档上传到AI表单填写时请考虑以下事项：

* AI表单填充当前已针对拉丁字母进行了优化。
* 我们建议使用8点或更大的文本大小。
* AI表单填充可能难以处理文档中的图像，例如旋转或扭曲的图像、图形以及计数图像中的对象或使用空间原因。
* 与往常一样，我们建议在提交请求之前检查结果的准确性。

### 上传文档以自动填写请求

您可以上载要应用于整个表单或表单单个部分的文档。

1. 开始创建请求。

   有关说明，请参阅[创建并提交请求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)。

1. 要将文档应用于整个表单，请单击表单名称下的AI图标![AI图标](assets/request-prompt-icon.png)。

   或

   若要将文档应用于单个分区，请单击分区名称旁边的AI图标![AI图标](assets/request-prompt-icon.png)。

1. 单击&#x200B;**上载文件**，然后从文件管理器中选择该文件。

   或

   将文档从文件管理器拖到&#x200B;**上载文件以自动填写请求表单**&#x200B;框。
1. 单击&#x200B;**填写表单**，共&#x200B;**填写部分**。

   Workfront会生成表单建议。
1. 对于每个字段建议，请为该字段选择&#x200B;**接受**&#x200B;或&#x200B;**拒绝**。

   ![接受或拒绝建议](assets/accept-reject-suggestion.png)

   或

   选择页面顶部的&#x200B;**全部接受**&#x200B;或&#x200B;**全部拒绝**&#x200B;以接受或拒绝所有建议。

   >[!NOTE]
   >
   >当您提交请求时，任何未审核的建议都将被自动接受。

## 故障排除

如果您没有获得预期的建议，可能是由于以下原因之一：

* 您必须在系统中拥有至少一个月的请求数据，然后才能建议来自先前请求的字段值。
* 在上传文档以从中提取建议时，您可能没有遵循文档上传护栏。 有关详细信息，请参阅本文中的[文档上传护栏](#document-upload-guardrails)。
