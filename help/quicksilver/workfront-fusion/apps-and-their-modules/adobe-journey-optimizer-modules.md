---
filename: adobe-journey-optimizer-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Journey Optimizer模块
description: 在 [!DNL Adobe Workfront Fusion] 方案，您可以自动执行使用 [!DNL Adobe Journey Optimizer]，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: 2c1aea46-edbf-42a3-a6e9-f8aea042a48d
source-git-commit: 50078aec71a4173a67c386ae5a8a4b5ba6cf3ade
workflow-type: tm+mt
source-wordcount: '1602'
ht-degree: 0%

---

# [!DNL Adobe Journey Optimizer] 模块

<!--
Becky: pull from main, add to TOCs, then push to merge.
-->

在 [!DNL Adobe Workfront Fusion] 方案，您可以自动执行使用 [!DNL Adobe Journey Optimizer]，并将其连接到多个第三方应用程序和服务。 [!DNL Adobe Journey Optimizer] 通过模块，您可以创建、读取、更新或删除记录，或对 [!DNL Adobe Journey Optimizer] API。


如果您需要有关创建方案的说明，请参阅 [创建方案](../../workfront-fusion/scenarios/create-a-scenario.md).

有关模块的信息，请参见 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## 访问要求

您必须具有以下权限才能使用本文中的功能：

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 计划*</td>
      <td>
        <p>[！UICONTROL Pro]或更高版本</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td>
      <td>
        <p>[！UICONTROL计划]，[！UICONTROL工作]</p>
      </td>
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
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 计划，您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 计划。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</p>
   </td>
    </tr>
  </tbody>
</table>


要了解您拥有的计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关的信息 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 先决条件

在使用 [!DNL Adobe Journey Optimizer] 连接器时，必须确保满足以下先决条件：

* 您必须拥有有效的 [!DNL Adobe Journey Optimizer] 帐户。

## 创建与的连接 [!DNL Adobe Journey Optimizer]

要为创建连接，请执行以下操作 [!DNL Adobe Journey Optimizer] 模块：

1. 在任何 [!DNL Adobe Journey Optimizer] 模块，单击 **[!UICONTROL 添加]** ，位于“Connection（连接）”框旁。

1. 填写以下字段：

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[！UICONTROL连接名称]</td>
          <td>
            <p>输入此连接的名称。</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL客户端ID]</td>
          <td>输入您的 [!DNL Adobe] [！UICONTROL客户端ID]。 可在[！UICONTROL凭据详细信息]部分中找到此凭据。 [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL客户端密钥]</td>
          <td>输入您的 [!DNL Adobe] [！UICONTROL客户端密钥]。 可在[！UICONTROL凭据详细信息]部分中找到此凭据。 [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL技术帐户ID]</td>
          <td>输入您的 [!DNL Adobe] [！UICONTROL技术帐户ID]。 可在[！UICONTROL凭据详细信息]部分中找到此凭据。 [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL组织ID]</td>
          <td>输入您的 [!DNL Adobe] [！UICONTROL组织ID]。 可在[！UICONTROL凭据详细信息]部分中找到此凭据。 [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL元范围]</td>
          <td>
            输入连接所需的任何元范围。
          </td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL私钥]</td>
          <td>
            <p>输入在中创建凭据时生成的私钥 [!DNL Adobe Developer Console]. </p>
            <p>要提取您的私钥或证书，请执行以下操作：</p>
            <ol>
              <li value="1">
                <p>单击 <b>[！UICONTROL Extract]</b>.</p>
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
                <p>单击 <b>[！UICONTROL保存]</b> 以提取文件并返回到连接设置。</p>
              </li>
            </ol>
          </td>
        </tr>
      </tbody>
    </table>
1. 单击 **[!UICONTROL 继续]** 以保存连接并返回到模块。

## [!DNL Adobe Journey Optimizer] 模块及其字段

配置时 [!DNL Adobe Journey Optimizer] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除此以外，还有 [!DNL Adobe Journey Optimizer] 字段可能会显示，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [操作](#actions)
* [搜索](#searches)

### 操作

* [[!UICONTROL 创建记录]](#create-a-record)
* [[!UICONTROL 进行自定义API调用]](#make-a-custom-api-call)
* [[!UICONTROL 删除记录]](#delete-a-record)
* [[!UICONTROL 更新记录]](#update-a-record)

#### [!UICONTROL 创建记录]

此操作模块可创建投放位置、决策规则、标记、个性化优惠、收藏集或备用优惠。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
     <td>有关创建与的连接 [!DNL Adobe Journey Optimizer]，请参见 <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >创建与的连接 [!DNL Adobe Journey Optimizer]</a> 本文章中。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [！UICONTROL记录类型]
      </td>
      <td>
        选择要创建的记录类型
        <ul>
        <li><b>[！UICONTROL位置]</b>：继续执行 <a href="#placement-fields" >[！UICONTROL Placement]字段</a>.</li>
        <li><b>[！UICONTROL决策规则]</b>：继续执行 <a href="#decision-rule-fields" >[！UICONTROL Decision rule]字段</a>.</li>
        <li><b>[！UICONTROL决策]</b>：继续执行 <a href="#decision-fields" >[！UICONTROL Decision]字段</a>.</li>
        <li><b>[！UICONTROL标记]</b>：继续执行 <a href="#tag-fields" >[！UICONTROL标记]字段</a>.</li>
        <li><b>[！UICONTROL收藏集]</b>：继续执行 <a href="#collection-fields" >[！UICONTROL Collection]字段</a>.</li>
        <li><b>[！UICONTROL后备优惠]</b>：继续执行 <a href="#fallback-offer-fields" >[！UICONTROL后备优惠]字段</a>.</li>
        <li><b>[！UICONTROL个性化优惠]</b>：继续执行 <a href="#personalized-offer-fields" >[！UICONTROL个性化优惠]字段</a>.</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL 投放] 字段

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL名称]</td>
     <td>输入或映射投放位置的名称。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [！UICONTROL描述]
      </td>
      <td>输入或映射投放位置的描述。
      </td>
    </tr>
  </tbody>
</table>


##### [!UICONTROL 决策规则] 字段

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL名称]</td>
     <td>输入或映射描述规则的名称。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [！UICONTROL描述]
      </td>
      <td>输入或映射决策规则的描述。
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [！UICONTROL条件]
      </td>
      <td>输入或映射条件作为决策规则。
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL 决策] 字段

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL名称]</td>
     <td>输入或映射描述规则的名称。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL状态]</td>
      <td>选择决策的状态。
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL开始日期]</td>
      <td><p>输入或映射决策的开始日期。</p><p>有关支持的日期格式的列表，请参阅 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">键入强制 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[！UICONTROL结束日期]</td>
      <td><p>输入或映射决策的结束日期。</p><p>有关支持的日期格式的列表，请参阅 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">键入强制 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[！UICONTROL Placements]</td>
      <td>选择要添加到此决策中的投放位置
      </td>
    </tr>
   <tr>
      <td role="rowheader">[！UICONTROL收藏集]</td>
      <td>选择优惠收藏集，其中包含此决策将考虑的优惠。
      </td>
    </tr>
   <tr>
      <td role="rowheader">[！UICONTROL后备优惠]</td>
      <td>选择将向不符合此决策规则的客户呈现的备用优惠。
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL 标记] 字段

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL名称]</td>
     <td>输入或映射标记的名称。</td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL 收藏集] 字段

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL名称]</td>
     <td>输入或映射收藏集的名称。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [！UICONTROL筛选器类型]
      </td>
      <td>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [！UICONTROL Elements]
      </td>
      <td>选择要包含在集合中的标记。
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL 后备优惠] 字段

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL名称]</td>
     <td>输入或映射后备优惠的名称。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [！UICONTROL状态]
      </td>
      <td> 选择后备优惠的状态。
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [！UICONTROL位置]
      </td>
      <td>输入或映射后备优惠的位置。
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL 个性化优惠] 字段

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL名称]</td>
     <td>输入或映射描述规则的名称。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL状态]</td>
      <td>选择决策的状态。
      </td>
    </tr>
    <tr>
      <td role="rowheader">投放位置</td>
      <td>选择个性化优惠的投放位置。
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL开始日期]</td>
      <td><p>输入或映射个性化优惠的开始日期。</p><p>有关支持的日期格式的列表，请参阅 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">键入强制 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[！UICONTROL结束日期]</td>
      <td><p>输入或映射个性化优惠的结束日期。</p><p>有关支持的日期格式的列表，请参阅 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">键入强制 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[！UICONTROL决策规则]</td>
      <td>选择要添加到此个性化优惠的决策规则。
      </td>
    </tr>
   <tr>
      <td role="rowheader">[！UICONTROL优先级]</td>
      <td>选择此优惠的优先级。 优先级会影响是否会呈现此选件而不是其他选件。
      </td>
    </tr>
   <tr>
      <td role="rowheader">[！UICONTROL上限约束]</td>
      <td>输入或映射此选件将显示的次数。
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 删除记录]

此操作模块删除中的单个记录 [!DNL Adobe Journey Optimizer].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
     <td>有关创建与的连接 [!DNL Adobe Journey Optimizer]，请参见 <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >创建与的连接 [!DNL Adobe Journey Optimizer]</a> 本文章中。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [！UICONTROL记录类型]
      </td>
      <td>
        选择要删除的记录类型
        <ul>
        <li>[！UICONTROL位置]</li>
        <li>[！UICONTROL决策规则]</li>
        <li>[！UICONTROL决策]</li>
        <li>[！UICONTROL标记]</li>
        <li>[！UICONTROL收藏集]</li>
        <li>[！UICONTROL后备优惠]</li>
        <li>[！UICONTROL个性化优惠]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Placement]/[！UICONTROL Decision rule]/[！UICONTROL Decision]/[！UICONTROL Tag]/[！UICONTROL Collection]/[！UICONTROL后备优惠]/[！UICONTROL个性化优惠]
      </td>
      <td>
        选择要删除的记录。
      </td>
    </tr>

</tbody>
</table>

#### [!UICONTROL 进行自定义API调用]

此模块对进行自定义API调用 [!DNL Adobe Journey Optimizer] API

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[！UICONTROL Connection]</td>
     <td>有关创建与的连接 [!DNL Adobe Journey Optimizer]，请参见 <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >创建与的连接 [!DNL Adobe Journey Optimizer]</a> 本文章中。</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL路径]</p>
      </td>
      <td>
        <p>输入相对路径 {baseURL} 开始于<code>/</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL方法]</p>
      </td>
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Headers]</td>
      <td>
        <p>以标准JSON对象的形式添加请求的标头。</p>
        <p>例如， <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion会自动添加授权标头和x-api-key标头。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL查询字符串]  </td>
      <td>
        <p>输入请求查询字符串。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Body]</td>
   <td> <p>以标准JSON对象的形式添加API调用的正文内容。</p> <p>注意：  <p>使用条件语句(例如 <code>if</code> 在JSON中，将引号放在条件语句之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
     <tr>
      <td role="rowheader">[！UICONTROL限制]  </td>
      <td>
        <p>输入您希望模块在一个执行周期内返回的结果的最大数目。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 删除记录]

此操作模块删除中的单个记录 [!DNL Adobe Journey Optimizer].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[！UICONTROL Connection]</td>
     <td>有关创建与的连接 [!DNL Adobe Journey Optimizer]，请参见 <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >创建与的连接 [!DNL Adobe Journey Optimizer]</a> 本文章中。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [！UICONTROL记录类型]
      </td>
      <td>
        选择要删除的记录类型
        <ul>
        <li>[！UICONTROL位置]</li>
        <li>[！UICONTROL决策规则]</li>
        <li>[！UICONTROL决策]</li>
        <li>[！UICONTROL标记]</li>
        <li>[！UICONTROL收藏集]</li>
        <li>[！UICONTROL后备优惠]</li>
        <li>[！UICONTROL个性化优惠]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Placement]/[！UICONTROL Decision rule]/[！UICONTROL Decision]/[！UICONTROL Tag]/[！UICONTROL Collection]/[！UICONTROL后备优惠]/[！UICONTROL个性化优惠]
      </td>
      <td>
        选择要删除的记录。
      </td>
    </tr>

</tbody>
</table>

#### [!UICONTROL 更新记录]

此操作模块可创建投放位置、决策、决策规则、标记、个性化优惠、收藏集或备用优惠。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[！UICONTROL Connection]</td>
     <td>有关创建与的连接 [!DNL Adobe Journey Optimizer]，请参见 <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >创建与的连接 [!DNL Adobe Journey Optimizer]</a> 本文章中。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [！UICONTROL记录类型]
      </td>
      <td>
        选择要更新的记录类型
        <ul>
        <li>[！UICONTROL位置]</li>
        <li>[！UICONTROL决策规则]</li>
        <li>[！UICONTROL决策]</li>
        <li>[！UICONTROL标记]</li>
        <li>[！UICONTROL收藏集]</li>
        <li>[！UICONTROL后备优惠]</li>
        <li>[！UICONTROL个性化优惠]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Placement]/[！UICONTROL Decision rule]/[！UICONTROL Decision]/[！UICONTROL Tag]/[！UICONTROL Collection]/[！UICONTROL后备优惠]/[！UICONTROL个性化优惠]
      </td>
      <td>
        选择要更新的记录。
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [！UICONTROL字段]
      </td>
      <td>对于要更新的每个字段：
      <ol>
      <li>单击 <b>[！UICONTROL添加]</b>.</li>
      <li>选择要添加、替换还是删除值。</li>
      <li>输入要更新的字段。</li>
      <li>为该字段输入新值。</li>
      </td>
    </tr>

</tbody>
</table>


### 搜索

#### [!UICONTROL 列出记录]

此搜索模块列出所选类型的记录，并根据您指定的条件返回结果。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[！UICONTROL Connection]</td>
     <td>有关创建与的连接 [!DNL Adobe Journey Optimizer]，请参见 <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >创建与的连接 [!DNL Adobe Journey Optimizer]</a> 本文章中。</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL记录类型]</p>
      </td>
      <td>
        <p>选择要列出的记录类型。</p>
        <ul>
        <li>[！UICONTROL位置]</li>
        <li>[！UICONTROL决策规则]</li>
        <li>[！UICONTROL决策]</li>
        <li>[！UICONTROL标记]</li>
        <li>[！UICONTROL收藏集]</li>
        <li>[！UICONTROL后备优惠]</li>
        <li>[！UICONTROL个性化优惠]</li>
       </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL查询运算符]</p>
      </td>
      <td>
        <p>选择要应用于查询中的参数的运算符</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL字段]</td>
      <td><p>如果要将搜索限制在特定字段中，请输入相应的字段。 对于要将搜索限制到的每个字段，单击[！UICONTROL添加项]并输入该字段的名称。</p><p>路径表达式采用点分隔路径的形式，例如 <code>_instance.xdm:name</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Order by] </td>
      <td>输入或映射要对结果排序的属性。
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL顺序方向]</td>
   <td>选择要按升序或降序方向对结果排序。
    </td>
     </tr>
  </tbody>
</table>
