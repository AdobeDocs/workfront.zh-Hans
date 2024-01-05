---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Workfront Proof模块
description: 在 [!DNL Adobe Workfront Fusion] 方案，您可以自动执行使用 [!DNL Workfront Proof]，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion, Workfront Proof, Digital Content and Documents
exl-id: f5c6fb08-880d-4432-aef1-57db13b3ecdb
source-git-commit: 8764de907f49260908911ca393c1173b66dbb065
workflow-type: tm+mt
source-wordcount: '2934'
ht-degree: 0%

---

# [!DNL Workfront Proof] 模块

在 [!DNL Adobe Workfront Fusion] 方案，您可以自动执行使用 [!DNL Workfront Proof]，并将其连接到多个第三方应用程序和服务。

如果您需要执行校对中当前不支持的任务，这将很有用 [!DNL Workfront] 或 [!DNL Workfront Proof]，例如根据某些事件更新验证和搜索验证的收件人。

此 [!DNL Workfront Proof] 连接器不计入您的组织可用的活动应用程序数量。 所有方案，即使它们只使用 [!DNL Workfront Proof] 应用程序，确实计入贵组织的方案总数。

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
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] 对于工作自动化和集成]，[！UICONTROL [!DNL Workfront Fusion] 工作自动化]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 计划，您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 计划。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关的信息 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Workfront Proof] 模块及其字段

配置时 [!DNL Workfront Proof] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除此以外，还有 [!DNL Workfront Proof] 字段可能会显示，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [触发器](#triggers)
* [操作](#actions)
* [搜索](#searches)

### 触发器

* [观看校样](#watch-proofs)
* [观看PDF摘要](#watch-for-pdf-summary)
* [[!UICONTROL Watch Proof活动]](#watch-proof-activity)

#### [!UICONTROL 观看校样]

当有人创建验证或做出决策时，此计划触发器模块执行场景。

该模块会返回一个列表，列出在指定的时间段内找到的所有记录及其类型。 它还会返回您指定的字段值。 如果模块发现对验证做出了决策，则会在单独的字段中包含之前值和当前值。 您可以在场景的后续模块中映射此信息。

此操作在您指定的定期计划间隔内进行。

您必须具有足够的权限才能访问中的验证 [!DNL Workfront Proof] 以检索此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关连接 [!DNL Workfront Proof] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与的连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">记录类型</td> 
   <td>选择类型 [!DNL Workfront Proof] 录制您希望模块观看的内容。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">输出</td> 
   <td> <p>选择要包含在此模块的输出捆绑包中的信息。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">限制</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 观看PDF摘要]

当有人为校对创建PDF摘要时，此即时触发模块会执行场景。

此模块中需要webhook。

模块返回与验证关联的所有标准字段，以及连接访问的任何自定义字段和值。 它还为PDF摘要创建新的事件预订，并输出有效负载中发送的“pdf_url”属性中的内容。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>有关连接 [!DNL Workfront Proof] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与的连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Webhook]</td> 
   <td>您可以选择现有的webhook或创建新一个。 有关更多信息，请参阅 <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">中的即时触发器(Webhook) [!DNL Adobe Workfront Fusion]</a>. </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL限制]</td> 
   <td>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Watch Proof活动]

此触发器模块执行对验证验证执行指定活动时的场景。

模块返回与验证关联的所有标准字段，以及连接访问的任何自定义字段和值。 它还为PDF摘要创建新的事件预订，并从以下位置输出内容 `pdf_url` 在有效负载中发送的属性。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>有关连接 [!DNL Workfront Proof] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与的连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL活动类型]</td> 
   <td>选择您是要观看任何新决策（包括[！UICONTROL proof]状态更改），还是只观看整体验证状态更改。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL限制]</td> 
   <td>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</td> 
  </tr> 
 </tbody> 
</table>

### 操作

* [[!UICONTROL 创建校对]](#create-proof)
* [[!UICONTROL 自定义API调用]](#custom-api-call)
* [[!UICONTROL 下载校对]](#download-proof)
* [[!UICONTROL 读取记录]](#read-a-record)
* [[!UICONTROL 请求PDF摘要]](#request-pdf-summary)
* [[!UICONTROL 更新校对]](#update-proof)
* [[!UICONTROL 上传文件]](#upload-file)

#### [!UICONTROL 创建校对]

此操作模块在中创建新验证或新版本的验证 [!DNL Workfront Proof].

如果要创建新版本，请为新验证和源验证指定参数。

模块会返回新验证或验证版本的ID。您可以将此信息映射到场景中的后续模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>有关连接 [!DNL Workfront Proof] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与的连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL校对类型]</td> 
   <td> <p>指定您希望创建的验证具有基本工作流还是[！UICONTROL自动工作流]。</p> <p>然后，填写为您选择的验证类型显示的字段。 例如，如果您选择[！UICONTROL自动工作流]，请填写 <strong>[！UICONTROL工作流暂存]</strong> 用于配置暂存的字段。</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL允许下载原始文件]</td> 
   <td>选择是否允许下载从中创建校对的原始文件。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL经典校对查看器]</td> 
   <td>选择是否使用经典校样查看器。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL将所有文件合并为单个校对]</td> 
   <td>启用此选项可将所有文件合并到单个多页验证中。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL创建新验证版本]</td> 
   <td>如果希望模块创建现有校对的新版本，请选择此选项。 然后，在 <strong>[！UICONTROL现有校对ID]</strong> 显示、映射或输入验证的唯一ID的字段。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL自定义链接标签]</td> 
   <td>输入或映射自定义验证链接的标签。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL自定义链接URL]</td> 
   <td>输入或映射自定义链接的URL。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL订阅者的默认电子邮件通知]</td> 
   <td>键入以下数字之一，以指示要将以下哪些默认电子邮件通知设置用于已创建的验证。
    <ul>
     <li><strong>1</strong>  — 所有新评论和回复</li>
     <li><strong>2</strong>  — 回复我的评论</li>
     <li><strong>3</strong>  — 每日摘要</li>
     <li><strong>4</strong>  — 每小时摘要</li>
     <li><strong>5</strong>  — 仅决策</li>
     <li><strong>9</strong>  — 已禁用</li>
    </ul></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL禁用Excel摘要]</td> 
   <td>选择是否要禁用将验证评论下载到Excel文件的功能。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL禁用PDF摘要]</td> 
   <td>选择是否要禁用将校对注释下载到PDF文件的功能。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL禁用订阅电子邮件]</td> 
   <td>选择是否要为此验证禁用订阅电子邮件。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL启用嵌入播放器]</td> 
   <td>选择是否要为此验证启用嵌入的播放器。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL启用订阅]</td> 
   <td>选择是否允许非参与者订阅验证。<br>如果选择此选项，您还可以为订阅者选择默认角色，如本表所述。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL启用订阅验证]</td> 
   <td>选择是否要启用订阅电子邮件验证。 如果启用此项，订阅者必须单击电子邮件中的链接才能访问验证。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL启用团队URL]</td> 
   <td>选择您希望创建的校对隐藏还是显示团队URL。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL文件哈希] <span style="font-weight: normal;">或</span> [！UICONTROL文件散列]</td> 
   <td>添加要从中创建验证的一个或多个文件的ID。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL文件名]</td> 
   <td>为创建的验证添加一个或多个文件名这是必填字段。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL完成所有必需的决策时锁定校对]</td> 
   <td>指定您是否希望在做出所有必需的决策后锁定创建的验证。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL将此证明通知收件人]</td> 
   <td>选择一个选项，以指示您是否希望在创建验证时通知收件人。&gt;</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL校对名称]</td> 
   <td>为创建的验证键入名称。这是必填字段。 使用管道符号(|)为多个校样分隔名称。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL校对所有者ID]</td> 
   <td>输入或映射验证所有者的ID。 如果此字段留空，则验证所有者将设置为当前用户。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL引用ID]</td> 
   <td>输入验证的参考ID。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL需要电子签名]</td> 
   <td>选择您是否希望要求决定证明的任何人提交电子签名。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL需要登录]</td> 
   <td> <p>指定您是否希望创建的验证需要登录。 </p> <p>这与中说明的[！UICONTROL需要登录]设置相同 <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">中的[！UICONTROL配置校对设置] [!DNL Workfront Proof]</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL分辨率ID]</td> 
   <td>输入要用于校对的分辨率ID。 有关分辨率ID的列表，请参见 [!DNL Workfront Proof] <a href="https://api.proofhq.com/home/objects/soapworkflowproofobject.html">API文档</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROLSWF]</td> 
   <td>输入SWF验证的类型。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL Show] [item]</td> 
   <td>对于每个项目，选择是否要将其显示在验证中。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL工作区ID]</td> 
   <td>输入要在其中创建验证的工作区的ID。 </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL收件人]</td> 
   <td>为创建的验证添加所需收件人的电子邮件地址。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL截止日期]</td> 
   <td> <p>指定您希望创建的验证的截止日期。 使用以下日期格式：</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 自定义API调用]

通过此操作模块，您可以对 [!DNL Workfront Proof] API。 这样，您就可以创建另一个无法实现的数据流自动化 [!DNL Workfront Proof] 模块。

模块会返回状态代码、标题和正文。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>有关连接 [!DNL Workfront Proof] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与的连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL方法]</td> 
   <td>为API调用设置操作。 有关可用的操作，请参阅 <a href="https://api.proofhq.com/">Proof API文档</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL正文(XML)]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的正文内容。</p> <p>注意：  <p>使用条件语句(例如 <code>if</code> 在JSON中，将引号放在条件语句之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**示例：**
>
>![](assets/wfp-api-module-example-350x586.png)

#### [!UICONTROL 下载校对]

此操作模块下载您使用其ID识别的特定验证的源文件。

您指定校样的ID。

模块会返回用于创建验证的源文件的内容。您可以在场景的后续模块中映射此信息。

您必须具有足够的权限才能访问中的记录 [!DNL Workfront Proof] 以检索此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>有关连接 [!DNL Workfront Proof] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与的连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL校对ID]</td> 
   <td> <p>键入在[！UICONTROL验证详细信息]页面上找到的验证的唯一ID。 有关更多信息，请参阅 <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">在中管理校对详细信息 [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 读取记录]

此操作模块从中的单个验证读取数据 [!DNL Workfront Proof].

您可以指定校样的ID以及您想要从校样中获得的信息。

模块会返回您为验证选择的字段的值及其类型。 您可以在场景的后续模块中映射此信息。

您必须具有足够的权限才能访问中的记录 [!DNL Workfront Proof] 以检索此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>有关连接 [!DNL Workfront Proof] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与的连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL记录类型]</td> 
   <td>选择您要读取校样、校样评论还是校样审阅者。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL输出]</td> 
   <td> <p>选择要包含在此模块的输出捆绑包中的信息。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL ID]</td> 
   <td>输入或映射唯一的 [!DNL Workfront Proof] 您希望模块读取的记录的ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 请求PDF摘要]

该操作模块在中请求特定验证的PDF摘要 [!DNL Workfront Proof].

您指定校样的ID。

该模块返回PDF摘要信息。 您可以在场景的后续模块中映射此信息。

您必须具有足够的权限才能访问中的记录 [!DNL Workfront Proof] 以检索此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>有关连接 [!DNL Workfront Proof] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与的连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL校对ID]</td> 
   <td> <p>输入唯一值 [!DNL Workfront Proof] 您要请求PDF摘要的校对ID。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL回调URL]</td> 
   <td>输入或映射要发送PDF摘要的URL。</td> 
  </tr> 
 </tbody> 
</table>

##### 可能存在的错误

* **错误**： &quot;[!UICONTROL 您没有执行此请求的特权。 阶段必须至少包含一个收件人。]&quot;
* **解决方案**：确保您不是唯一一个分配到工作流暂存阶段的人。 必须为工作流的阶段分配另一个用户。

#### [!UICONTROL 更新校对]

此操作模块更新中的现有校对 [!DNL Workfront Proof].

您可以指定校样的ID和记录类型以及要包含在输出中的字段。

该模块会返回与记录关联的任何标准字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

您必须具有足够的权限才能访问中的记录 [!DNL Workfront Proof] 以检索此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>有关连接 [!DNL Workfront Proof] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与的连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL校对ID]</td> 
   <td> <p>键入在[！UICONTROL验证详细信息]页面上找到的验证的唯一ID。 有关更多信息，请参阅 <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">在中管理校对详细信息 [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL截止日期]</td> 
   <td> <p>指定您希望创建的验证的截止日期。 使用以下日期格式：</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL订阅者的默认电子邮件通知]</td> 
   <td>选择您希望为创建的验证使用的以下默认电子邮件通知设置之一。
    <ul>
     <li> [！UICONTROL所有新评论和回复]</li>
     <li>[！UICONTROL回复我的评论]</li>
     <li>[！UICONTROL每日摘要]</li>
     <li> [！UICONTROL小时摘要]</li>
     <li> [！UICONTROL仅决策]</li>
     <li> [！UICONTROL已禁用]</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL默认角色]</td> 
   <td>选择验证的默认角色。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL禁用订阅电子邮件]</td> 
   <td>选择是否要为此验证禁用订阅电子邮件。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL启用订阅]</td> 
   <td>选择是否允许非参与者订阅验证。<br>如果选择此选项，您还可以为订阅者选择[！UICONTROL默认角色]，如本表所述。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL启用订阅验证]</td> 
   <td>选择是否要启用订阅电子邮件验证。 如果启用此项，订阅者必须单击电子邮件中的链接才能访问验证。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL启用团队URL]</td> 
   <td>选择您希望创建的校对隐藏还是显示团队URL。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL完成所有必需的决策时锁定校对]</td> 
   <td>指定您是否希望在做出所有必需的决策后锁定创建的验证。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Message]</td> 
   <td>输入或映射要与校样一起显示的消息。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL校对ID] </td> 
   <td>输入或映射要更新的校对ID。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL校对名称]</td> 
   <td>输入或映射要更新的校对的名称。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL需要登录]</td> 
   <td> <p>指定您是否希望创建的验证需要登录。 </p> <p>这与中说明的[！UICONTROL需要登录]设置相同 <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">中的[！UICONTROL配置校对设置] [!DNL Workfront Proof]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL显示类似版本]</td> 
   <td>选择是否要显示此校对的其他版本的链接。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL主题]</td> 
   <td>输入或映射验证的主题</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 上传文件]

此操作模块上传文件以用于 [!UICONTROL 创建校对] 中的模块 [!DNL Workfront Proof].

模块会返回已上传文件的哈希ID。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>有关连接 [!DNL Workfront Proof] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与的连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL源文件]</td> 
   <td> <p>从上一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 搜索

* [[!UICONTROL 搜索]](#search)
* [[!UICONTROL 列出工作流模板]](#list-workflow-templates)

#### [!UICONTROL 搜索]

此搜索模块查找对象中的记录 [!DNL Workfront Proof] 匹配您指定的搜索查询的规则。

如果正在搜索验证，模块将返回验证的ID。 如果正在搜索收件人，则它会返回收件人的用户ID、电子邮件、名称、位置和电子邮件别名。您可以将此信息映射到场景中的后续模块。

您必须具有足够的权限才能访问中的记录 [!DNL Workfront Proof] 以检索此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>有关连接 [!DNL Workfront Proof] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与的连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>搜索</td> 
   <td> <p>选择[！UICONTROL ]您希望模块搜索的记录类型。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL Proof]</strong> </p> <p>输入要搜索的校对的校对名称。</p> </li> 
     <li> <p><strong>[！UICONTROL收件人]</strong> </p> <p>输入要搜索的收件人的电子邮件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL结果集]</td> 
   <td>指示模块是否会搜索 <strong>[！UICONTROL所有匹配记录]</strong> 或仅 <strong>[！UICONTROL第一个匹配记录]</strong>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL排序方式]</td> 
   <td>选择要作为结果排序依据的字段。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL排序方向]</td> 
   <td> <p>选择要按升序或降序对结果进行排序。</p> </td> 
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
   <td> <p>有关连接 [!DNL Workfront Proof] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与的连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL输出]</td> 
   <td> <p>选择要包含在此模块的输出捆绑包中的信息。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL限制]</td> 
   <td> <p>输入或映射每个方案执行周期中您希望模块返回的最大模板数。</p> </td> 
  </tr> 
 </tbody> 
</table>
