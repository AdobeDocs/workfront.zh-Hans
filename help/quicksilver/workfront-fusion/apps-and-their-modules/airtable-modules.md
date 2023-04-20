---
filename: airtable-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: 可放气模块
description: Adobe Workfront Fusion除了需要Adobe Workfront许可证之外，还需要Adobe Workfront Fusion许可证。
author: Becky
hidefromtoc: true
source-git-commit: 6955c979d504adb6514ae64bf5108174d7a90ce4
workflow-type: tm+mt
source-wordcount: '1863'
ht-degree: 2%

---


# 可放气模块


使用 [!DNL Airtable] 连接器 [!DNL Adobe Workfront Fusion]，则可以根据 [!DNL Airtable] 帐户、创建、上传和更新记录、搜索记录，以及对Airtable API进行自定义API调用。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 先决条件

您必须拥有Airtable帐户才能使用本文中的功能。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see the tutorial .</p>
-->

## 将Airtable连接到Workfront Fusion {#connect-airtable-to-workfront-fusion}

<!--

1. Log in to your Airtable account.
1. Open your account overview and generate the API key.
-->
1. 打开Workfront Fusion和 **创建连接** 对话框。
1. 输入连接的名称。
1. （可选）单击显示高级设置，然后输入可放置的客户端ID和客户端密钥。
1. 单击 **继续** 按钮以创建连接并返回到模块。

## 可飞行模块及其字段

### 记录

* [创建记录](#create-a-record)
* [删除记录](#delete-a-record)
* [获取记录](#get-a-record)
* [搜索记录](#search-records)
* [更新记录](#update-a-record)
* [更新记录](#upsert-a-record)
* [监视记录](#watch-records)
* [监视响应](#watch-responses)
* [进行API调用](#make-an-api-call)

#### 创建记录 {#create-a-record}

此操作模块会创建新记录。

您可以指定要在记录中保存的数据以及要将其存储的位置。

模块会返回与记录关联的任何标准字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>连接 </td> 
   <td> <p>有关将Airtable帐户连接到Workfront Fusion的说明，请参阅 <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">将Airtable连接到Workfront Fusion</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>库 </td> 
   <td> <p>选择新记录所属的基础。</p> </td> 
  </tr> 
  <tr> 
   <td>表 </td> 
   <td> <p>选择新记录所属的表。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>记录</p> </td> 
   <td> <p>输入新记录的值。 可用字段基于您选择的表。</p> <!--<p>For more information on field types, search for "Supported field types" in the Airtable documentation.</p> 
    <ul> 
     <li> <p><strong>Text</strong>: string</p> <p>A single line of text.</p> </li> 
     <li> <p><strong>Long text</strong>: string</p> <p>Multiple lines of text, which may contain "mention tokens", for example:</p><pre>&lt;airtable:mention id="menE1i9oBaGX3DseR"&gt;@Alex&lt;/airtable:mention&gt;</pre> </li> 
     <li><strong>Attachment</strong> : Add the attachment. Airtable will download the file from the provided <code>url</code> and keep its own copy of it. If the File name field is left empty, Airtable generates the name automatically.</li> 
     <li><strong>Checkbox</strong>: Select one of the options.</li> 
     <li><strong>Multiple select</strong>: Select multiple options in the checklist.</li> 
     <li><strong>Single select</strong>: Select one option from the drop-down menu.</li> 
     <li><strong>Collaborator</strong>: Enter the email that uniquely identifies a user in Airtable who this base is shared with.</li> 
     <li><strong>Date</strong>: UTC date, for example, 2019-09-05 (ISO 8601 formatted date)</li> 
     <li>Phone number:</li> 
     <li><strong>Emails</strong>: A valid email address.</li> 
     <li><strong>URL</strong>: A valid URL (for example, airtable.com or https://airtable.com/universe).</li> 
     <li><strong>Number</strong>: Enter a number.</li> 
     <li><strong>Currency</strong>: Currency value.</li> 
     <li><strong>Percent</strong>: A percentage value. Must be higher than or equal to 0.</li> 
     <li><strong>Duration</strong>: Enter the duration time. If you need help, see the information about the duration field type in the Airtable support documentation. </li> 
     <li><strong>Rating</strong>: Enter the number. For example, "3 stars" is 3. A rating cannot be 0.</li> 
     <li><strong>Link</strong>: Enter the linked records IDs from the table. The order of record IDs will be reversed compared to what you see in the app.</li> 
     <li><strong>Rollup</strong>: Computed value: COUNT(values)</li> 
     <li><strong>Lookup</strong>: Array of long text fields</li> 
     <li><strong>Autonumber</strong>: Automatically incremented unique counter for each record.</li> 
     <li> <p><strong>Barcode</strong>: The barcode object may contain the following two properties, both of which are optional.</p> <p>Barcode data (text)</p> <p>Barcode symbology, for example, "upce" or "code39" (type)</p> </li> 
    </ul> --></td> 
  </tr> 
  <tr> 
   <td>智能链接</td> 
   <td> <p>启用此选项，可在链接到其他表的字段中输入名称，而不是记录ID。 如果没有匹配项，则在链接的表中自动创建记录。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 删除记录 {#delete-a-record}

此操作模块会删除特定记录。

您可以指定记录的ID和位置。

模块会返回记录的ID和任何关联字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>连接 </td> 
   <td> <p>有关将Airtable帐户连接到Workfront Fusion的说明，请参阅 <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">将Airtable连接到Workfront Fusion</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>库 </td> 
   <td> <p>选择包含要删除的记录的基。</p> </td> 
  </tr> 
  <tr> 
   <td>表 </td> 
   <td> <p>选择包含要删除的记录的表。</p> </td> 
  </tr> 
  <tr> 
   <td>记录ID</td> 
   <td> <p>输入或映射您希望删除模块的记录的唯一可播放ID。 例如，您可以使用搜索记录模块检索ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 获取记录 {#get-a-record}

此操作模块检索记录详细信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>连接 </td> 
   <td> <p>有关将Airtable帐户连接到Workfront Fusion的说明，请参阅 <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">将Airtable连接到Workfront Fusion</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>库 </td> 
   <td> <p>选择包含要检索记录的表的基。</p> </td> 
  </tr> 
  <tr> 
   <td>表</td> 
   <td> <p> 选择包含要检索其详细信息的记录的表。</p> </td> 
  </tr> 
  <tr> 
   <td>记录ID</td> 
   <td> <p> 输入或映射要检索详细信息的记录的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 搜索记录 {#search-records}

此搜索模块在Airtable中查找与您指定的搜索查询匹配的对象中的记录。

您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>连接 </td> 
   <td> <p>有关将Airtable帐户连接到Workfront Fusion的说明，请参阅 <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">将Airtable连接到Workfront Fusion</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>库 </td> 
   <td> <p>选择要搜索记录的基数。</p> </td> 
  </tr> 
  <tr> 
   <td>表 </td> 
   <td> <p>选择要搜索记录的表。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>公式</p> </td> 
   <td> <p>用于筛选记录的公式。 将为每个记录计算公式，如果结果不是 <code>0</code>, <code>false</code>, <code>""</code>, <code>NaN</code>, <code>[]</code>或 <code>#Error!</code> 该记录包含在响应中。</p> <p>如果与 <code>view</code>，则只返回该视图中满足公式的记录。</p> <p>例如，要仅包含名称不为空的记录，请传入：<code> NOT({Name} = '')</code></p> <p>要了解更多信息，请在Airtable支持文档中搜索有关公式字段引用的信息。</p> </td> 
  </tr> 
  <tr> 
   <td>排序 </td> 
   <td> <p>选择排序方向和要按排序结果的字段。</p> </td> 
  </tr> 
  <tr> 
   <td>查看 </td> 
   <td> <p>选择要搜索记录的视图。</p> </td> 
  </tr> 
  <tr> 
   <td>限制</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 更新记录 {#update-a-record}

此操作模块更新特定记录。

您指定记录的ID以及您希望它包含的新数据。

模块会返回与记录关联的任何标准字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>连接 </td> 
   <td> <p>有关将Airtable帐户连接到Workfront Fusion的说明，请参阅 <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">将Airtable连接到Workfront Fusion</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>库 </td> 
   <td> <p>选择包含要更新的记录的基。</p> </td> 
  </tr> 
  <tr> 
   <td>表 </td> 
   <td> <p>选择包含要更新的记录的表。</p> </td> 
  </tr> 
  <tr> 
   <td>记录ID </td> 
   <td> <p>输入或映射您希望更新模块的记录的唯一可播放ID。 例如，您可以使用搜索记录模块检索ID。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>记录</p> </td> 
   <td> <p>输入新记录的值。 可用字段取决于您选择的表。</p> <!--<p>In order to delete the content of the field, use the erase function. </p>  <p>Field types (via airtable.com/api):</p> 
    <ul> 
     <li> <p><strong>Text</strong>: string</p> <p>A single line of text.</p> </li> 
     <li> <p><strong>Long text</strong>: string</p> <p>The string can contain multiple lines of text with "mention tokens." For example:</p><pre>&lt;airtable:mention id="menE1i9oBaGX3DseR"&gt;@Alex&lt;/airtable:mention&gt;</pre> </li> 
     <li><strong>Attachment</strong>: Add the attachment. Airtable will download the file from the provided url and keep its own copy of it. If the File name field is left empty, Airtable will generate the name automatically.</li> 
     <li><strong>Checkbox</strong>: Select one of the options.</li> 
     <li><strong>Multiple select</strong>: Select multiple options in the checklist.</li> 
     <li><strong>Single select</strong>: Select one option from the drop-down menu.</li> 
     <li><strong>Collaborator</strong>: Enter the email that uniquely identifies a user in Airtable who this base is shared with.</li> 
     <li><strong>Date</strong>: UTC date, for example, 2019-09-05. (ISO 8601 formatted date)</li> 
     <li><strong>Phone number</strong>: A telephone number, for example, (415) 555-9876.</li> 
     <li><strong>Email</strong>valid email address.</li> 
     <li><strong>URL</strong>: lid URL such as airtable.com or https://airtable.coiverse.</li> 
     <li><strong>Number</strongnter a number.</li> 
     <li><strong>Currency</stro Currency value.</li> 
     <li><strong>Percent</stronA percentage value; must be equal to or more than 0i> 
     <li><strong>Duration</strong>: Enter the duration time. If you need help, see the information about the duration field type in the Airtable support documentation.</li> 
     <li><strong>Rating</strong>: Enter the number. For example, "3 stars" is 3. A rating cannot be 0.</li> 
     <li><strong>Link</strong>: Enter the linked records IDs from the table. The order of record IDs is reversed compared to what you see in the app.</li> 
     <li><strong>Rollup</strong>: Computed value: COUNT(values)</li> 
     <li><strong>Lookup</strong>: Array of long text fields</li> 
     <li><strong>Autonumber</strong>: Automatically incremented unique counter for each record.</li> 
     <li> <p><strong>Barcode</strong>: The barcode object may contain the following two properties, both of which are optional.</p> <p>Barcode data (text)</p> <p>Barcode symbology, for example, "upce" or "code39" (type)</p> </li> 
    </ul> --></td> 
  </tr> 
  <tr> 
   <td>智能链接</td> 
   <td> <p>在链接到其他表的字段中输入名称，而不是记录ID。 如果没有匹配项，则在链接的表中自动创建记录。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 更新记录

此操作模块更新或插入特定记录。

您指定记录的ID以及您希望它包含的新数据。

模块会返回与记录关联的任何标准字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>连接 </td> 
   <td> <p>有关将Airtable帐户连接到Workfront Fusion的说明，请参阅 <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">将Airtable连接到Workfront Fusion</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>库 </td> 
   <td> <p>选择包含要更新的记录的基。</p> </td> 
  </tr> 
  <tr> 
   <td>表 </td> 
   <td> <p>选择包含要更新的记录的表。</p> </td> 
  </tr> 
  <tr> 
   <td>记录ID </td> 
   <td> <p>如果要更新记录，请输入或映射希望模块更新的记录的唯一可播放ID。 例如，您可以使用搜索记录模块检索ID。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>记录</p> </td> 
   <td> <p>输入新记录的值。 可用字段取决于您选择的表。</p> <!-- <p>In order to delete the content of the field, use the erase function. </p>  <p>Field types (via airtable.com/api):</p> 
    <ul> 
     <li> <p><strong>Text</strong>: string</p> <p>A single line of text.</p> </li> 
     <li> <p><strong>Long text</strong>: string</p> <p>The string can contain multiple lines of text with "mention tokens." For example:</p><pre>&lt;airtable:mention id="menE1i9oBaGX3DseR"&gt;@Alex&lt;/airtable:mention&gt;</pre> </li> 
     <li><strong>Attachment</strong>: Add the attachment. Airtable will download the file from the provided url and keep its own copy of it. If the File name field is left empty, Airtable will generate the name automatically.</li> 
     <li><strong>Checkbox</strong>: Select one of the options.</li> 
     <li><strong>Multiple select</strong>: Select multiple options in the checklist.</li> 
     <li><strong>Single select</strong>: Select one option from the drop-down menu.</li> 
     <li><strong>Collaborator</strong>: Enter the email that uniquely identifies a user in Airtable who this base is shared with.</li> 
     <li><strong>Date</strong>: UTC date, for example, 2019-09-05. (ISO 8601 formatted date)</li> 
     <li><strong>Phone number</strong>: A telephone number, for example, (415) 555-9876.</li> 
     <li><strong>Email</strong>valid email address.</li> 
     <li><strong>URL</strong>: lid URL such as airtable.com or https://airtable.coiverse.</li> 
     <li><strong>Number</strongnter a number.</li> 
     <li><strong>Currency</stro Currency value.</li> 
     <li><strong>Percent</stronA percentage value; must be equal to or more than 0i> 
     <li><strong>Duration</strong>: Enter the duration time. If you need help, see the information about the duration field type in the Airtable support documentation.</li> 
     <li><strong>Rating</strong>: Enter the number. For example, "3 stars" is 3. A rating cannot be 0.</li> 
     <li><strong>Link</strong>: Enter the linked records IDs from the table. The order of record IDs is reversed compared to what you see in the app.</li> 
     <li><strong>Rollup</strong>: Computed value: COUNT(values)</li> 
     <li><strong>Lookup</strong>: Array of long text fields</li> 
     <li><strong>Autonumber</strong>: Automatically incremented unique counter for each record.</li> 
     <li> <p><strong>Barcode</strong>: The barcode object may contain the following two properties, both of which are optional.</p> <p>Barcode data (text)</p> <p>Barcode symbology, for example, "upce" or "code39" (type)</p> </li> 
    </ul> --></td> 
  </tr> 
  <tr> 
   <td>智能链接</td> 
   <td> <p>在链接到其他表的字段中输入名称，而不是记录ID。 如果没有匹配项，则在链接的表中自动创建记录。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 监视记录 {#watch-records}

当在指定的表中创建或更新记录时，此触发器模块会启动一个方案。

>[!NOTE]
>
>要使用此模块，必须在表中创建“创建时间”字段或“上次修改时间”字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>连接 </td> 
   <td> <p>有关将Airtable帐户连接到Workfront Fusion的说明，请参阅 <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">将Airtable连接到Workfront Fusion</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>库 </td> 
   <td> <p>选择要监视新记录的基数。</p> </td> 
  </tr> 
  <tr> 
   <td>表 </td> 
   <td> <p>选择要监视新记录的表。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>触发器配置</p> </td> 
   <td> <p>触发器字段</p> <p>A <code>Created Time</code> 或 <code>Last Modified Time</code> 用于对记录进行排序的字段。 如果您没有 <code>Created Time</code> 或 <code>Last Modified Time</code> 字段，则需要创建一个。 </p> <p>标签字段</p> <p>用作记录标签的字段，例如，在“选择开始位置”对话框中。</p> </td> 
  </tr> 
  <tr> 
   <td>限制</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期中监视的最大记录数。</p> </td> 
  </tr> 
  <tr> 
   <td>查看</td> 
   <td> <p>选择要使用的视图。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>公式</p> </td> 
   <td> <p>用于筛选记录的公式。 将为每个记录计算公式，如果结果不是 <code>0</code>, <code>false</code>, <code>""</code>, <code>NaN</code>, <code>[]</code>或 <code>#Error!</code> 该记录包含在响应中。</p> <p>如果与 <code>view</code>，则只返回该视图中满足公式的记录。</p> <p>例如，要仅包含名称不为空的记录，请传入：<code> NOT({Name} = '')</code></p> <p>要了解更多信息，请参阅Airtable支持文档中有关公式字段引用的信息。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 监视响应

此触发器模块会在提交表单时启动一个方案。

>[!NOTE]
>
>此功能仅适用于付费的Airtable Pro计划。

需要在Workfront Fusion中生成Webhook URL，然后将其添加到Airtable中的表单配置。

1. 将Watch新响应模块添加到您的Workfront Fusion方案中。
1. 生成并复制Webhook URL。

   有关说明，请参阅 [Adobe Workfront Fusion中的即时触发器(Webhook)](../../workfront-fusion/webhooks/instant-triggers-webhooks.md).

1. 登录到Airtable帐户。
1. 打开要用于表单的基本和表，然后创建表单视图。
1. 根据需要设置表单，向下滚动表单，并启用在表单提交后重定向到URL选项。
1. 在显示的对话框中输入步骤2中生成的Webhook URL，并在Webhook URL之后添加？record_id={record_id}以在模块的输出中包含记录ID，然后单击“保存”。 例如，生成的URL将如下所示：
1. 返回到您的Workfront Fusion方案并运行“监视响应”模块，以便仅从Airtable加载字段，并能够将这些字段映射到其他模块。
1. 在表格中提交表单，其中启用了提交表单后重定向到URL选项并添加了Webhook URL（上面的步骤6）。

   触发“监视响应”模块并加载所需数据。

1. 紧跟“可播放”>“监视响应”模块添加“可播放”>“获取记录”模块，并将record_id映射到“记录ID”字段。

现在，每次提交表单时，都会触发Workfront Fusion场景中的“监视响应”模块，并且“获取记录”模块会返回提交的表单详细信息。

#### 进行API调用

#### 自定义API调用

通过此操作模块，您可以对 [!DNL Airtable] API。 这样，您就可以创建数据流自动化，而另一个数据流无法实现 [!DNL Airtable] 模块。

该操作基于您指定的实体类型（Allocida对象类型）。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>连接</p> </td> 
   <td> <p>有关将Airtable帐户连接到Workfront Fusion的说明，请参阅 <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">将Airtable连接到Workfront Fusion</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>输入相对于 <code>https://api.airtable.com/}</code>. 示例: <code>v0/{base}/{table}</code> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">方法</td> 
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">标题</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 为您添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">查询字符串</td> 
   <td> <p>以键和值的形式为API调用添加查询</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">正文</td> 
   <td> <p>以标准JSON对象的形式为API调用添加正文内容。</p> <p>注释:  <p>使用条件语句时，例如 <code>if</code> 在JSON中，将引号放置在条件语句的外部。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
