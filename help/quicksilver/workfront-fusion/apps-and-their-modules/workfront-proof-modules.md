---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Workfront校样模块
description: 在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!DNL Workfront Proof]，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion, Workfront Proof, Digital Content and Documents
exl-id: f5c6fb08-880d-4432-aef1-57db13b3ecdb
source-git-commit: a79c6b2fb2b651987f973bc0d74e0eeea312c5bc
workflow-type: tm+mt
source-wordcount: '2886'
ht-degree: 0%

---

# [!DNL Workfront Proof] 模块

在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!DNL Workfront Proof]，并将其连接到多个第三方应用程序和服务。

如果您需要执行校对内当前不支持的任务，则此功能非常有用 [!DNL Workfront] 或 [!DNL Workfront Proof]，例如根据某些事件更新校样并搜索校样的收件人。

的 [!DNL Workfront Proof] 连接器不计入贵组织可用的活动应用程序数。 所有方案，即使它们仅使用 [!DNL Workfront Proof] 应用程序时，请根据贵组织的总方案计数计算。

如果您需要有关创建方案的说明，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

有关模块的信息，请参阅 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## 访问要求

您必须具有以下访问权限才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td>
  <td> <p>[!UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td>
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p>  <p>[!UICONTROL [!DNL Workfront Fusion] （工作自动化）</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Workfront Proof] 模块及其字段

配置 [!DNL Workfront Proof] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!DNL Workfront Proof] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [触发器](#triggers)
* [操作](#actions)
* [搜索](#searches)

### 触发器

* [观看校样](#watch-proofs)
* [观看PDF摘要](#watch-for-pdf-summary)
* [[!UICONTROL 观看校样活动]](#watch-proof-activity)

#### [!UICONTROL 观看校样]

当某人创建或决定校样时，此计划触发器模块会执行一个方案。

该模块会返回在您指定的时间段内找到的所有记录的列表及其类型。 它还会返回您指定字段的值。 如果模块找到对校样做出的决策，则它会在单独的字段中同时包含先前值和当前值。 您可以在方案的后续模块中映射此信息。

这会在您指定的定期计划间隔内发生。

您必须拥有足够的权限才能在中访问校样或校样 [!DNL Workfront Proof] 以检索此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Workfront Proof] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">记录类型</td> 
   <td>选择 [!DNL Workfront Proof] 记录您希望模块监视的内容。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">输出</td> 
   <td> <p>选择要包含在此模块的输出包中的信息。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">限制</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 观看PDF摘要]

此即时触发模块在某人为校样创建PDF摘要时执行方案。

此模块中需要Webhook。

模块会返回与校样关联的所有标准字段，以及连接所访问的任何自定义字段和值。 它还会为PDF摘要创建新事件订阅，并输出有效载荷中发送的“pdf_url”属性的内容。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>有关连接 [!DNL Workfront Proof] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Webhook]</td> 
   <td>您可以选择现有网页挂接，也可以创建新网页挂接。 有关更多信息，请参阅 <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">中的即时触发器(Webhook) [!DNL Adobe Workfront Fusion]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL限制]</td> 
   <td>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 观看校样活动]

当在校样中发生指定的活动时，此触发器模块会执行一个方案。

模块会返回与校样关联的所有标准字段，以及连接所访问的任何自定义字段和值。 它还会为PDF摘要创建新事件订阅，并输出 `pdf_url` 属性。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>有关连接 [!DNL Workfront Proof] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Activity type]</td> 
   <td>选择您是要观看任何新决策（包括[!UICONTROL校样]状态更改），还是仅观看整体校样状态更改。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL限制]</td> 
   <td>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。</td> 
  </tr> 
 </tbody> 
</table>

### 操作

* [[!UICONTROL 创建校对]](#create-proof)
* [[!UICONTROL 自定义API调用]](#custom-api-call)
* [[!UICONTROL 下载校样]](#download-proof)
* [[!UICONTROL 读取记录]](#read-a-record)
* [[!UICONTROL 请求PDF摘要]](#request-pdf-summary)
* [[!UICONTROL 更新校样]](#update-proof)
* [[!UICONTROL 上传文件]](#upload-file)

#### [!UICONTROL 创建校对]

此操作模块会在中创建新校样或新版本的校样 [!DNL Workfront Proof].

如果要创建新版本，请指定新校样和源校样的参数。

该模块返回新校样或校样版本的ID。您可以在场景中的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>有关连接 [!DNL Workfront Proof] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL校样类型]</td> 
   <td> <p>指定您希望创建的校样具有基本工作流还是[!UICONTROL自动工作流]。</p> <p>然后，填写为所选校样类型显示的字段。 例如，如果您选择[!UICONTROL Automated Workflow]，请填写 <strong>[!UICONTROL工作流阶段]</strong> 字段来配置阶段。</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL允许下载原始文件]</td> 
   <td>选择是否允许下载从中创建校样的原始文件。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Classic校样查看器]</td> 
   <td>选择您是否在使用经典校样查看器。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL将所有文件合并到单个校样中]</td> 
   <td>启用此选项可将所有文件合并到一个多页校样中。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL创建新校样版本]</td> 
   <td>如果希望模块创建现有校样的新版本，请选择此选项。 然后，在 <strong>[!UICONTROL现有校样ID]</strong> 字段，用于显示、映射或输入校样的唯一ID。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL自定义链接标签]</td> 
   <td>输入或映射自定义校样链接的标签。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL自定义链接URL]</td> 
   <td>输入或映射自定义链接的URL。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL订阅者的默认电子邮件通知]</td> 
   <td>键入以下数字之一，以指示您要对所创建校样使用的以下默认电子邮件通知设置。
    <ul>
     <li><strong>1</strong>  — 所有新评论和回复</li>
     <li><strong>2</strong>  — 对我的评论的答复</li>
     <li><strong>3</strong>  — 每日摘要</li>
     <li><strong>4</strong>  — 每小时概要</li>
     <li><strong>5</strong>  — 仅决策</li>
     <li><strong>9</strong>  — 已禁用</li>
    </ul></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL禁用Excel摘要]</td> 
   <td>选择是否要禁用将校样注释下载到Excel文件的功能。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL禁用PDF摘要]</td> 
   <td>选择是否要禁用将校样注释下载到PDF文件的功能。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL禁用订阅电子邮件]</td> 
   <td>选择是否要禁用此校样的订阅电子邮件。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL启用嵌入播放器]</td> 
   <td>选择是否要为此校样启用嵌入式播放器。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL启用订阅]</td> 
   <td>选择是否允许非参与者的用户订阅校样。<br>如果选择此选项，则还可以为订阅者选择默认角色，如此表所述。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL启用订阅验证]</td> 
   <td>选择是否要启用订阅电子邮件验证。 如果启用了此功能，订阅者必须单击电子邮件中的链接才能访问校样。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL启用团队URL]</td> 
   <td>选择是希望创建的校样来隐藏还是显示团队URL。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL文件哈希] <span style="font-weight: normal;">或</span> [!UICONTROL文件哈希]</td> 
   <td>添加要从中创建校样或校样的文件的ID。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL文件名]</td> 
   <td>添加所创建校样的文件名或名称。这是必填字段。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL在做出所有必需决策时进行锁校样]</td> 
   <td>指定是否希望创建的校样在做出所有必需的决策后锁定。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL将此校样通知收件人]</td> 
   <td>选择一个选项，以指示您是否希望在创建校样时通知收件人。&gt;</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL校样名称]</td> 
   <td>键入所创建校样的名称。这是必填字段。 使用管道符号(|)分隔多个校样的名称。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL校样所有者ID]</td> 
   <td>输入或映射校样所有者的ID。 如果此字段留空，则校样所有者将设置为当前用户。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL引用ID]</td> 
   <td>输入校样的引用ID。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL需要电子签名]</td> 
   <td>选择您是否希望要求对证据作出决定的任何人提交电子签名。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL需要登录]</td> 
   <td> <p>指定是否希望创建的校样需要登录。 </p> <p>此设置与[!UICONTROL需要登录]设置相同，详见 <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">在中配置校样设置[!UICONTROL [!DNL Workfront Proof]</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Resolution ID]</td> 
   <td>输入要用于校样的分辨率ID。 有关分辨率ID的列表，请参阅 [!DNL Workfront Proof] <a href="http://api.proofhq.com/home/objects/soapworkflowproofobject">API文档</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROLSWF]</td> 
   <td>输入SWF校样的类型。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Show] [item]</td> 
   <td>对于每个项目，选择是否要在校样中显示它。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Workspace ID]</td> 
   <td>输入要在中创建校样的工作区的ID。 </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL收件人]</td> 
   <td>添加所创建校样的收件人的电子邮件地址。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Deadline]</td> 
   <td> <p>指定您希望创建校样的截止时间。 使用以下日期格式：</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 自定义API调用]

通过此操作模块，您可以对 [!DNL Workfront Proof] API。 这样，您就可以创建数据流自动化，而另一个数据流无法实现 [!DNL Workfront Proof] 模块。

模块会返回状态代码、标头和正文。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>有关连接 [!DNL Workfront Proof] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL方法]</td> 
   <td>设置API调用的操作。 有关可用的操作，请参阅 <a href="http://api.proofhq.com/">校样API文档</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL主体(XML)]</td> 
   <td> <p>以标准JSON对象的形式为API调用添加正文内容。</p> <p>注释:  <p>使用条件语句时，例如 <code>if</code> 在JSON中，将引号放置在条件语句的外部。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**示例:**
>
>![](assets/wfp-api-module-example-350x586.png)

#### [!UICONTROL 下载校样]

此操作模块会下载您使用其ID标识的特定校样的源文件。

您指定校样的ID。

该模块返回用于创建校样的源文件的内容。您可以在方案的后续模块中映射此信息。

您必须拥有足够的权限才能访问 [!DNL Workfront Proof] 以检索此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>有关连接 [!DNL Workfront Proof] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL校样ID]</td> 
   <td> <p>键入校样的唯一ID，该ID位于[!UICONTROL校样详细信息]页面上。 有关更多信息，请参阅 <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">在中管理校样详细信息 [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 读取记录]

此操作模块从 [!DNL Workfront Proof].

您可以指定校样的ID以及校样中需要的信息。

模块会返回您为校样选择的字段值及其类型。 您可以在方案的后续模块中映射此信息。

您必须拥有足够的权限才能访问 [!DNL Workfront Proof] 以检索此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>有关连接 [!DNL Workfront Proof] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL记录类型]</td> 
   <td>选择要阅读校样、校样注释还是校样审阅人。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL输出]</td> 
   <td> <p>选择要包含在此模块的输出包中的信息。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>输入或映射唯一 [!DNL Workfront Proof] 您希望模块读取的记录的ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 请求PDF摘要]

此操作模块会请求PDF摘要，以获取 [!DNL Workfront Proof].

您指定校样的ID。

该模块返回PDF摘要信息。 您可以在方案的后续模块中映射此信息。

您必须拥有足够的权限才能访问 [!DNL Workfront Proof] 以检索此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>有关连接 [!DNL Workfront Proof] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL校样ID]</td> 
   <td> <p>输入唯一 [!DNL Workfront Proof] 要为其请求PDF摘要的校样的ID。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL回调URL]</td> 
   <td>输入或映射要将PDF摘要发送到的URL。</td> 
  </tr> 
 </tbody> 
</table>

##### 可能的错误

* **错误**:&quot;[!UICONTROL 您没有执行此请求的权限。 舞台必须至少包含一个收件人。]&quot;
* **解决方案**:确保您不是分配给工作流各个阶段的唯一用户。 必须有另一个用户被分配到工作流的各个阶段。

#### [!UICONTROL 更新校样]

此操作模块会更新 [!DNL Workfront Proof].

您可以指定校样的ID和记录类型以及要包含在输出中的字段。

模块会返回与记录关联的任何标准字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

您必须拥有足够的权限才能访问 [!DNL Workfront Proof] 以检索此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>有关连接 [!DNL Workfront Proof] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL校样ID]</td> 
   <td> <p>键入校样的唯一ID，该ID位于[!UICONTROL校样详细信息]页面上。 有关更多信息，请参阅 <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">在中管理校样详细信息 [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Deadline]</td> 
   <td> <p>指定您希望创建校样的截止时间。 使用以下日期格式：</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL订阅者的默认电子邮件通知]</td> 
   <td>选择您要用于所创建校样的以下默认电子邮件通知设置中的哪个。
    <ul>
     <li> [!UICONTROL所有新评论和回复]</li>
     <li>[!UICONTROL对我的评论的回复]</li>
     <li>[!UICONTROL每日摘要]</li>
     <li> [!UICONTROL每小时摘要]</li>
     <li> [！仅UICONTROL决策]</li>
     <li> [!UICONTROL Disabled]</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL默认角色]</td> 
   <td>选择校样的默认角色。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL禁用订阅电子邮件]</td> 
   <td>选择是否要禁用此校样的订阅电子邮件。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL启用订阅]</td> 
   <td>选择是否允许非参与者的用户订阅校样。<br>如果选择此选项，则还可以为订阅者选择[!UICONTROL默认角色]，如此表所述。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL启用订阅验证]</td> 
   <td>选择是否要启用订阅电子邮件验证。 如果启用了此功能，订阅者必须单击电子邮件中的链接才能访问校样。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL启用团队URL]</td> 
   <td>选择是希望创建的校样来隐藏还是显示团队URL。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL在做出所有必需决策时进行锁校样]</td> 
   <td>指定是否希望创建的校样在做出所有必需的决策后锁定。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL消息]</td> 
   <td>输入或映射要随校样一起显示的消息。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL校样ID] </td> 
   <td>输入或映射要更新校样的ID。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL校样名称]</td> 
   <td>输入或映射要更新的校样的名称。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL需要登录]</td> 
   <td> <p>指定是否希望创建的校样需要登录。 </p> <p>此设置与[!UICONTROL需要登录]设置相同，详见 <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">在中配置校样设置[!UICONTROL [!DNL Workfront Proof]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL显示版本，如]</td> 
   <td>选择是否要显示指向此校样其他版本的链接。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL主题]</td> 
   <td>输入或映射校样的主题</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 上传文件]

此操作模块上传文件以与 [!UICONTROL 创建校样] 模块 [!DNL Workfront Proof].

该模块会返回已上传文件的哈希ID。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>有关连接 [!DNL Workfront Proof] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL源文件]</td> 
   <td> <p>从前一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 搜索

* [[!UICONTROL 搜索]](#search)
* [[!UICONTROL 列出工作流模板]](#list-workflow-templates)

#### [!UICONTROL 搜索]

此搜索模块在 [!DNL Workfront Proof] 与您指定的搜索查询匹配。

如果模块正在搜索校样，则会返回校样的ID。 或者，如果正在搜索收件人，则返回收件人的用户ID、电子邮件、名称、位置和电子邮件别名。您可以在方案的后续模块中映射此信息。

您必须拥有足够的权限才能访问 [!DNL Workfront Proof] 以检索此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>有关连接 [!DNL Workfront Proof] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>搜索</td> 
   <td> <p>Se[!UICONTROL ]选择您希望模块搜索的记录类型。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL校样]</strong> </p> <p>输入要搜索的校样的校样名称。</p> </li> 
     <li> <p><strong>[!UICONTROL Recipient]</strong> </p> <p>输入要搜索的收件人的电子邮件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL结果集]</td> 
   <td>指示模块是否将搜索 <strong>[!UICONTROL所有匹配记录]</strong> 或仅 <strong>[!UICONTROL第一条匹配记录]</strong>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL排序依据]</td> 
   <td>选择要按对结果排序的字段。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL排序方向]</td> 
   <td> <p>选择是升序排序还是降序排序结果。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出工作流模板]

此搜索模块列出了所有可用的工作流模板。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>有关连接 [!DNL Workfront Proof] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL输出]</td> 
   <td> <p>选择要包含在此模块的输出包中的信息。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期期间返回的最大模板数。</p> </td> 
  </tr> 
 </tbody> 
</table>
