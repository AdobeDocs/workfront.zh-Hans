---
filename: adobe-target-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Target模块
description: 在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!DNL Adobe Target], as well as connect it to multiple third-party applications and services. [!DNL Adobe Target] 模块允许您创建、读取、更新或删除记录，列出给定类型的所有记录，根据您指定的条件搜索记录，或对自定义API调用 [!DNL Adobe Target] API。
author: Becky
exl-id: 9597806b-d4bf-4627-b27d-30e24a1e6776
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2598'
ht-degree: 0%

---

# [!DNL Adobe Target] 模块

在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!DNL Adobe Target]，并将其连接到多个第三方应用程序和服务。 [!DNL Adobe Target] 利用模块，可创建、创建、读取、更新或删除记录、列出给定类型的所有记录、根据您指定的条件搜索记录，或对自定义API调用 [!DNL Adobe Target] API。


如果您需要有关创建方案的说明，请参阅 [创建方案](../../workfront-fusion/scenarios/create-a-scenario.md).

有关模块的信息，请参阅 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## 访问要求

您必须具有以下访问权限才能使用本文中的功能：

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 计划*</td>
      <td>
        <p>[!UICONTROL Pro]或更高版本</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td>
      <td>
        <p>[!UICONTROL Plan]、[!UICONTROL Work]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td>
      <td >
        <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成）</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">产品</td>
      <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td>
    </tr>
    </tr>
  </tbody>
</table>


要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 先决条件

在使用 [!DNL Adobe Target] 连接器中，必须确保满足以下先决条件：

* 您必须具有活动 [!DNL Adobe Target] 帐户。

## 创建连接 [!DNL Adobe Target]

为 [!DNL Adobe Target] 模块：

1. 单击 **[!UICONTROL 添加]** 中。

1. 填写以下字段：

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL连接名称]</td>
        <td>
          <p>输入此连接的名称。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL客户端ID]</td>
        <td>输入 [!DNL Adobe] 客户端ID。 此信息可在的[!UICONTROL凭据详细信息]部分中找到 [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL客户端密钥]</td>
        <td>输入 [!DNL Adobe] 客户端密钥。 此信息可在的[!UICONTROL凭据详细信息]部分中找到 [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL组织ID]</td>
        <td>输入 [!DNL Adobe] 组织ID。 此信息可在的[!UICONTROL凭据详细信息]部分中找到 [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL技术帐户ID]</td>
        <td>输入 [!DNL Adobe] 技术帐户ID。 此信息可在的[!UICONTROL凭据详细信息]部分中找到 [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL租户]</td>
        <td>
          <p> 要找到您的租户，请登录到 [!DNL Adobe Experience Cloud]，打开 [!DNL Target]，然后单击 [!DNL Target] 卡。 按照URL子域中所述，使用租户ID值。</p>
          <p>例如，如果您的URL在登录到 [!DNL Adobe Target] is <code>&lt;https://mycompany.experiencecloud.adobe.com/...></code> 则您的租户ID为“mycompany”。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL元范围]</td>
        <td>输入 <code>ent_marketing_sdk</code>       </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL私钥]</td>
        <td>
          <p>输入在中创建凭据时生成的私钥 [!DNL Adobe Developer Console]. </p>
          <p>要提取您的私钥或证书，请执行以下操作：</p>
          <ol>
            <li value="1">
              <p>单击 <b>[!UICONTROL Extract]</b>.</p>
            </li>
            <li value="2">
              <p>选择要提取的文件类型。</p>
            </li>
            <li value="3">
              <p>选择包含私钥或证书的文件。</p>
            </li>
            <li value="4">
              <p>输入文件的密码。</p>
            </li>
            <li value="5">
              <p>单击 <b>[!UICONTROL Save]</b> 以提取文件并返回到连接设置。</p>
            </li>
          </ol>
        </td>
      </tr>
    </tbody>
    </table>

1. 单击 **[!UICONTROL 继续]** 保存连接并返回到模块。

## [!DNL Adobe Target] 模块及其字段

配置 [!DNL Adobe Target] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!DNL Adobe Target] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [操作](#actions)

* [搜索](#searches)


### 操作

* [[!UICONTROL 创建记录]](#create-a-record)

* [[!UICONTROL 进行自定义API调用]](#make-a-custom-api-call)

* [[!UICONTROL 删除记录]](#delete-a-record)

* [[!UICONTROL 读取记录]](#read-a-record)

* [[!UICONTROL 更新记录]](#update-a-record)


#### [!UICONTROL 创建记录]

此操作模块会创建AB或XT活动、选件或受众。

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL连接]</td>
    <td>有关创建与 [!DNL Adobe Target]，请参阅 <a href="#Create" class="MCXref xref" >创建连接 [!DNL Adobe Target]</a> 在本文中。</td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL记录类型]</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>选择要创建的记录类型。</p>
      <ul>
        <li>
          <p>[!UICONTROL AB活动]</p>
          <p>继续 <a href="#AB%C2%A0Activ" class="MCXref xref" >AB活动字段</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL XT Activity]</p>
          <p>继续 <a href="#XT" class="MCXref xref" >XT活动字段</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL选件]</p>
          <p>继续 <a href="#Offer" class="MCXref xref" >选件字段</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL Audience]</p>
          <p>继续 <a href="#Audience" class="MCXref xref" >受众字段</a>.</p>
        </li>
      </ul>
    </td>
  </tr>
</tbody>
</table>

##### AB活动字段

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL名称]</td>
      <td>输入或映射此活动的名称。 名称不得超过250个字符。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL选项]</td>
      <td>
        <p>对于要添加到活动的每个选项，单击 <b>[!UICONTROL添加项目]</b> 并填写以下字段：</p>
        <ul>
          <li>
            <p><b>[!UICONTROL选项本地ID]</b>
            </p>
            <p>输入或映射用于跨API请求跟踪选项的字符串。</p>
          </li>
          <li>
            <p><b>[!UICONTROL名称]</b>
            </p>
            <p>输入或映射选项的名称。 名称不得超过250个字符。</p>
          </li>
          <li>
            <p><b>[!UICONTROL选件ID]</b>
            </p>
          </li>
          <li>
            <p>选择或映射与选项关联的选件。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL位置]</td>
      <td>
        <p>对于要添加到活动的每个Mbox，单击 <b>[!UICONTROL添加项目]</b> 并填写以下字段：</p>
        <ul>
          <li>
            <p>[!UICONTROL受众ID]</p>
            <p>对于要添加到Mbox的每个受众，单击 <b>[!UICONTROL添加项目]</b> ，然后选择受众ID。</p>
          </li>
          <li>
            <p><b>[!UICONTROL位置本地ID]</b>
            </p>
            <p>输入或映射用于跨API请求跟踪位置的字符串。</p>
          </li>
          <li>
            <p><b>[!UICONTROL名称]</b>
            </p>
            <p>输入或映射位置的名称。 名称不得超过250个字符。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL体验]</td>
      <td>
        <p>提供内容选件的页面上的位置列表。 位置包含以下内容：
</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Experience Local ID]</b>
            </p>
            <p>输入或映射体验的ID</p>
          </li>
          <li>
            <p><b>[!UICONTROL名称]</b>
            </p>
            <p>输入或映射体验的名称

</p>
          </li>
          <li>
            <p><b>[!DNL Audience IDs]</b>
            </p>
            <p>对于要查看体验的每个受众，单击 <b>[!UICONTROL添加项目]</b> 并输入受众ID。

</p>
          </li>
          <li>
            <p><b>[!UICONTROL访客百分比]</b>
            </p>
            <p>输入或映射分配给体验的访客百分比</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL量度]</td>
      <td> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL第三方ID]</td>
      <td>输入或映射ID以标识此活动。 您可以选择此ID。 此ID不得与其他活动相同，且不得超过250个字符。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL开始于]</td>
      <td>以格式输入或映射开始活动的日期和时间 <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL结束于]</td>
      <td>以格式输入或映射结束活动的日期和时间 <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL State]</td>
      <td>
        <p>输入或映射活动的状态。</p>
        <ul>
          <li>
            <p>[!UICONTROL Approved]</p>
          </li>
          <li>
            <p>[!UICONTROL已停用]</p>
          </li>
          <li>
            <p>[!UICONTROL已暂停]</p>
          </li>
          <li>
            <p>[!UICONTROL已保存] </p>
          </li>
          <li>
            <p>[!UICONTROL已删除]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL优先级]</td>
      <td>输入定义活动优先级的数字。 数字越高，优先级越高。 此值必须介于0到999之间。 默认值为5。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL自动分配流量]</td>
      <td>
        <p>启用此选项可自动分配流量。 自动分配会向更成功的体验发送更多流量。</p>
        <p>选择或映射用于判断哪个体验更成功的评估标准。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>输入或映射与活动关联的工作区</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL属性ID] </td>
      <td>对于要添加到活动的每个资产，单击 <b>[!UICONTROL添加项目]</b> ，然后选择或映射属性的ID。</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL报表受众]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>对于要添加到活动的每个报表受众，单击[!UICONTROL添加项目]，然后输入以下信息：</p>
        <ul>
          <li>
            <p><b>[!UICONTROL报表受众本地ID]</b>
            </p>
            <p>输入或映射用于跨API请求跟踪报表受众的字符串。</p>
          </li>
          <li>
            <p><b>[!UICONTROL Audience ID]</b>
            </p>
            <p>输入或映射要用于报表的区段</p>
          </li>
          <li>
            <p><b>[!UICONTROL量度本地ID]</b>
            </p>
            <p>输入或映射用于跨API请求跟踪量度的字符串。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### XT活动字段

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL名称]</td>
      <td>输入或映射此活动的名称。 名称不得超过250个字符。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL选项]</td>
      <td>
        <p>对于要添加到活动的每个选项，单击 <b>[!UICONTROL添加项目]</b> 并填写以下字段：</p>
        <ul>
          <li>
            <p><b>[!UICONTROL选项本地ID]</b>
            </p>
            <p>输入或映射用于跨API请求跟踪选项的字符串。</p>
          </li>
          <li>
            <p><b>[!UICONTROL名称]</b>
            </p>
            <p>输入或映射选项的名称。 名称不得超过250个字符。</p>
          </li>
          <li>
            <p><b>[!UICONTROL选件ID]</b>
            </p>
          </li>
          <li>
            <p>选择或映射与选项关联的选件。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL位置]</td>
      <td>
        <p>对于要添加到活动的每个Mbox，单击 <b>[!UICONTROL添加项目]</b> 并填写以下字段：</p>
        <ul>
          <li>
            <p>[!UICONTROL受众ID]</p>
            <p>对于要添加到Mbox的每个受众，单击 <b>[!UICONTROL添加项目]</b> ，然后选择受众ID。</p>
          </li>
          <li>
            <p><b>[!UICONTROL位置本地ID]</b>
            </p>
            <p>输入或映射用于跨API请求跟踪位置的字符串。</p>
          </li>
          <li>
            <p><b>[!UICONTROL名称]</b>
            </p>
            <p>输入或映射位置的名称。 名称不得超过250个字符。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL体验]</td>
      <td>
        <p>提供内容选件的页面上的位置列表。 位置包含以下内容：
</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Experience Local ID]</b>
            </p>
            <p>输入或映射体验的ID</p>
          </li>
          <li>
            <p><b>[!UICONTROL名称]</b>
            </p>
            <p>输入或映射体验的名称

</p>
          </li>
          <li>
            <p><b>[!DNL Audience IDs]</b>
            </p>
            <p>对于要查看体验的每个受众，单击 <b>[!UICONTROL添加项目]</b> 并输入受众ID。

</p>
          </li>
          <li>
            <p><b>[!UICONTROL访客百分比]</b>
            </p>
            <p>输入或映射分配给体验的访客百分比</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL量度]</td>
      <td> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL第三方ID]</td>
      <td>输入或映射ID以标识此活动。 您可以选择此ID。 此ID不得与其他活动相同，且不得超过250个字符。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL开始于]</td>
      <td>以格式输入或映射开始活动的日期和时间 <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL结束于]</td>
      <td>以格式输入或映射结束活动的日期和时间 <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL State]</td>
      <td>
        <p>输入或映射活动的状态。</p>
        <ul>
          <li>
            <p>[!UICONTROL Approved]</p>
          </li>
          <li>
            <p>[!UICONTROL已停用]</p>
          </li>
          <li>
            <p>[!UICONTROL已暂停]</p>
          </li>
          <li>
            <p>[!UICONTROL已保存] </p>
          </li>
          <li>
            <p>[!UICONTROL已删除]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL优先级]</td>
      <td>输入定义活动优先级的数字。 数字越高，优先级越高。 此值必须介于0到999之间。 默认值为5。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL自动分配流量]</td>
      <td>
        <p>启用此选项可自动分配流量。 自动分配会向更成功的体验发送更多流量。</p>
        <p>选择或映射用于判断哪个体验更成功的评估标准。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>输入或映射与活动关联的工作区</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL属性ID] </td>
      <td>对于要添加到活动的每个资产，单击 <b>[!UICONTROL添加项目]</b> ，然后选择或映射属性的ID。</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL报表受众]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>对于要添加到活动的每个报表受众，单击[!UICONTROL添加项目]，然后输入以下信息：</p>
        <ul>
          <li>
            <p><b>[!UICONTROL报表受众本地ID]</b>
            </p>
            <p>输入或映射用于跨API请求跟踪报表受众的字符串。</p>
          </li>
          <li>
            <p><b>[!UICONTROL Audience ID]</b>
            </p>
            <p>输入或映射要用于报表的区段</p>
          </li>
          <li>
            <p><b>[!UICONTROL量度本地ID]</b>
            </p>
            <p>输入或映射用于跨API请求跟踪量度的字符串。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### 选件字段

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL名称]</td>
      <td>输入或映射此活动的名称。 名称不得超过250个字符。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL内容]</td>
      <td>
        <p>输入或映射将向用户显示的选件内容。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>
        <p>输入或映射与选件关联的工作区的ID。 如果留空，则选件将与帐户的默认工作区关联。 此功能仅适用于 [!DNL Target] 高级帐户。</p>
      </td>
    </tr>
  </tbody>
</table>

##### 受众字段

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL名称]</td>
      <td>输入或映射此受众的名称。 名称不得超过250个字符。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL内容]</td>
      <td>
        <p>输入或映射此受众的描述。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Target规则]</td>
      <td>
        <p>启用切换开关以使规则变为“与”，即必须应用所有规则。</p>
        <p>对于要应用于受众的每个规则，单击 <b>[!UICONTROL添加项目]</b> 并输入要应用的规则的JSON。 </p>
        <div class="example"><span class="autonumber"><span><b>示例: </b></span></span>
          <p>示例:</p>
          <p ><code>&lbrace;</code></p>
                    <p ><code>                "page": "url",</code>
                    </p>
                    <p><code>                "equals":&lbrack;</code>
                    </p>
                    <p ><code>                    "http://www.myhomepage.com/"</code>
                    </p>
                    <p><code>                &rbrack;</code>
                    </p>
                    <p ><code>            &rbrace;,</code>
                    </p>
                    <p ><code>            &lbrace;</code>
                    </p>
                    <p><code>                "geo": "region",</code>
                    </p>
                    <p><code>                "matches": &lbrack;</code>
                    </p>
                    <p ><code>                    "california"</code>
                    </p>
                    <p ><code>                &rbrack;</code>
                    </p>
                    <p ><code>            &rbrace;</code>
                    </p>
      </td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Workspace]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>输入或映射与受众关联的工作区ID。 如果留空，则选件将与帐户的默认工作区关联。 此功能仅适用于 [!DNL Target Premium] 帐户。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 进行自定义API调用]

此模块对 [!DNL Adobe Target] API

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL连接]</td>
      <td>有关创建与 [!DNL Adobe Target]，请参阅 <a href="#Create" class="MCXref xref" >创建连接 [!DNL Adobe Target]</a> 在本文中。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL [!DNL Target] 基本URL]</td>
      <td>输入或映射 [!DNL Target] 基本URL。</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL路径]</p>
      </td>
      <td>
        <p>输入相对于{baseURL}/的路径</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL方法]</p>
      </td>
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL标头]</td>
      <td>
        <p>以标准JSON对象的形式添加请求的标头。</p>
        <p>例如， <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] 自动添加授权标头和x-api-key标头。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL查询字符串]  </td>
      <td>
        <p>输入请求查询字符串。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL主体]</td>
   <td> <p>以标准JSON对象的形式为API调用添加正文内容。</p> <p>注释:  <p>使用条件语句时，例如 <code>if</code> 在JSON中，将引号放置在条件语句的外部。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL 删除记录]

此操作模块会删除单个AB活动、XT活动、选件或受众。

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL连接]</td>
    <td>有关创建与 [!DNL Adobe Target]，请参阅 <a href="#Create" class="MCXref xref" >创建连接 [!DNL Adobe Target]</a> 在本文中。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL记录类型]</td>
    <td>选择要删除的记录类型。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL记录ID]</td>
    <td>输入或映射要删除的记录的ID。</td>
  </tr>
</tbody>
</table>

#### [!UICONTROL 读取记录]

此操作模块可检索单个活动、选件、受众、属性或报表的数据。

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL连接]</td>
    <td>有关创建与 [!DNL Adobe Target]，请参阅 <a href="#Create" class="MCXref xref" >创建连接 [!DNL Adobe Target]</a> 在本文中。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL记录类型]</td>
    <td>选择要读取的记录类型。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL记录ID]</td>
    <td>输入或映射要读取的记录的ID。</td>
  </tr>
</tbody>
</table>

#### [!UICONTROL 更新记录]

此操作模块可更新活动、选件或受众。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL连接]</td>
      <td>有关创建与 [!DNL Adobe Target]，请参阅 <a href="#Create" class="MCXref xref" >创建连接 [!DNL Adobe Target]</a> 在本文中。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL记录类型]</td>
      <td>
        <p>选择要更新的记录类型。</p>
        <ul>
          <li>
            <p><b>[!UICONTROL AB活动]</b>
            </p>
            <p>请参阅 <a href="#AB%C2%A0Activ" class="MCXref xref" >AB活动字段</a> 在 <a href="#Create2" class="MCXref xref" >创建记录</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL XT Activity]</b>
            </p>
            <p>请参阅 <a href="#XT" class="MCXref xref" >XT活动字段</a> 在 <a href="#Create2" class="MCXref xref" >创建记录</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL其他活动]</b>
            </p>
            <p>选择要更新值的字段，然后为该字段输入新值。</p>
          </li>
          <li>
            <p><b>[!UICONTROL选件]</b>
            </p>
            <p>请参阅 <a href="#Offer" class="MCXref xref" >选件字段</a> 在 <a href="#Create2" class="MCXref xref" >创建记录</a>.</p>
          </li>
          <li>
            <p><b>[!DNL Audience]</b>
            </p>
            <p>请参阅 <a href="#Audience" class="MCXref xref" >受众字段</a> 在 <a href="#Create2" class="MCXref xref" >创建记录</a>.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL记录ID]</td>
      <td>输入或映射要更新的记录的ID。</td>
    </tr>
  </tbody>
</table>

### 搜索

* [[!UICONTROL 获取记录]](#get-records)

* [[!UICONTROL 搜索]](#search)


#### [!UICONTROL 获取记录]

此搜索模块检索所选类型的记录列表。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL连接]</td>
      <td>有关创建与 [!DNL Adobe Target]，请参阅 <a href="#Create" class="MCXref xref" >创建连接 [!DNL Adobe Target]</a> 在本文中。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL记录类型]</td>
      <td>选择要更新的记录类型。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL排序依据]</td>
      <td>对于要排序的每个字段，单击 <b>[!UICONTROL添加项目]</b> 并选择字段以及返回的结果应升序还是降序。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL开始于]</td>
      <td>
        <p>输入要检索记录的最早日期。 </p>
        <p>有关支持的日期和时间格式的列表，请参阅 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在中键入强制 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL结束于]</td>
      <td>
        <p>输入要检索记录的最新日期。 </p>
        <p>有关支持的日期和时间格式的列表，请参阅 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在中键入强制 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 搜索]

此搜索模块会根据您指定的条件搜索“活动”、“选件”或“受众”。

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL连接]</td>
    <td>有关创建与 [!DNL Adobe Target]，请参阅 <a href="#Create" class="MCXref xref" >创建连接 [!DNL Adobe Target]</a> 在本文中。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL记录类型]</td>
    <td>选择要更新的记录类型。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL排序依据]</td>
    <td>对于要排序的每个字段，单击 <b>[!UICONTROL添加项目]</b> 并选择字段以及返回的结果应升序还是降序。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL搜索标准]</td>
    <td>对于要设置的每个规则，选择字段、运算符和值。 单击 <b>[!UICONTROL Add AND Rule]</b> 创建其他规则。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Offset]</td>
    <td>
      <p>输入您希望模块返回的第一个响应的编号。 第一个返回的响应的偏移为 <code>0</code>. 将此字段与[!UICONTROL返回结果的最大数]字段结合使用，可将响应分页。</p>
      <p>例如，要查看第三页响应，如果每页有10个响应，请将[!UICONTROL Offset]设置为20，将[!UICONTROL Maximum number of returned]结果设置为10。</p>
    </td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL返回结果的最大数]</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。 将此字段与[!UICONTROL Offset]字段结合使用，可对响应进行分页。</p>
      <p>例如，要查看第三页响应，如果每页有10个响应，请将[!UICONTROL Offset]设置为20，将[!UICONTROL Maximum number of returned]结果设置为10。</p>
    </td>
  </tr>
</tbody>
</table>
