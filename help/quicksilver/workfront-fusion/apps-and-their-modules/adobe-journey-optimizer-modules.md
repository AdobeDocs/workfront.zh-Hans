---
filename: adobe-journey-optimizer-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Journey Optimizer模块
description: 在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!DNL Adobe Journey Optimizer]，并将其连接到多个第三方应用程序和服务。
author: Becky
exl-id: 2c1aea46-edbf-42a3-a6e9-f8aea042a48d
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1554'
ht-degree: 0%

---

# [!DNL Adobe Journey Optimizer] 模块

<!--
Becky: pull from main, add to TOCs, then push to merge.
-->

在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!DNL Adobe Journey Optimizer]，并将其连接到多个第三方应用程序和服务。 [!DNL Adobe Journey Optimizer] 模块允许您创建、读取、更新或删除记录，或对自定义API调用 [!DNL Adobe Journey Optimizer] API。


如果您需要有关创建方案的说明，请参阅 [创建方案](../../workfront-fusion/scenarios/create-a-scenario.md).

有关模块的信息，请参阅 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## 访问要求

您必须具有以下访问权限才能使用本文中的功能：

<table>
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
  </tbody>
</table>


要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 先决条件

在使用 [!DNL Adobe Journey Optimizer] 连接器中，必须确保满足以下先决条件：

* 您必须具有活动 [!DNL Adobe Journey Optimizer] 帐户。

## 创建连接 [!DNL Adobe Journey Optimizer]

为 [!DNL Adobe Journey Optimizer] 模块：

1. 在任意 [!DNL Adobe Journey Optimizer] 模块，单击 **[!UICONTROL 添加]** 中。

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
          <td>输入 [!DNL Adobe] [!UICONTROL客户端ID]。 此信息可在的[!UICONTROL凭据详细信息]部分中找到 [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL客户端密钥]</td>
          <td>输入 [!DNL Adobe] [!UICONTROL客户端密钥]。 此信息可在的[!UICONTROL凭据详细信息]部分中找到 [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL技术帐户ID]</td>
          <td>输入 [!DNL Adobe] [!UICONTROL技术帐户ID]。 此信息可在的[!UICONTROL凭据详细信息]部分中找到 [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL组织ID]</td>
          <td>输入 [!DNL Adobe] [!UICONTROL组织ID]。 此信息可在的[!UICONTROL凭据详细信息]部分中找到 [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL元作用域]</td>
          <td>
            输入连接所需的任何元作用域。
          </td>
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

## [!DNL Adobe Journey Optimizer] 模块及其字段

配置 [!DNL Adobe Journey Optimizer] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!DNL Adobe Journey Optimizer] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [操作](#actions)
* [搜索](#searches)

### 操作

* [[!UICONTROL 创建记录]](#create-a-record)
* [[!UICONTROL 进行自定义API调用]](#make-a-custom-api-call)
* [[!UICONTROL 删除记录]](#delete-a-record)
* [[!UICONTROL 更新记录]](#update-a-record)

#### [!UICONTROL 创建记录]

此操作模块可创建版面、决策规则、标记、个性化选件、收藏集或备用选件。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL连接]</td>
     <td>有关创建与 [!DNL Adobe Journey Optimizer]，请参阅 <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >创建连接 [!DNL Adobe Journey Optimizer]</a> 在本文中。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL记录类型]
      </td>
      <td>
        选择要创建的记录类型
        <ul>
        <li><b>[!UICONTROL Placement]</b>:继续 <a href="#placement-fields" >[!UICONTROL Placement]字段</a>.</li>
        <li><b>[!UICONTROL决策规则]</b>:继续 <a href="#decision-rule-fields" >[!UICONTROL决策规则]字段</a>.</li>
        <li><b>[!UICONTROL Decision]</b>:继续 <a href="#decision-fields" >[!UICONTROL Decision]字段</a>.</li>
        <li><b>[!UICONTROL标记]</b>:继续 <a href="#tag-fields" >[!UICONTROL标记]字段</a>.</li>
        <li><b>[!UICONTROL集合]</b>:继续 <a href="#collection-fields" >[!UICONTROL集合]字段</a>.</li>
        <li><b>[!UICONTROL后备优惠]</b>:继续 <a href="#fallback-offer-fields" >[!UICONTROL后备优惠]字段</a>.</li>
        <li><b>[!UICONTROL Personalized offer]</b>:继续 <a href="#personalized-offer-fields" >[!UICONTROL Personalized offer]字段</a>.</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL 版面] 字段

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL名称]</td>
     <td>输入或映射版面的名称。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL描述]
      </td>
      <td>输入或映射版面的描述。
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
      <td role="rowheader">[!UICONTROL名称]</td>
     <td>输入或映射描述规则的名称。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL描述]
      </td>
      <td>输入或映射决策规则的说明。
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL条件]
      </td>
      <td>在决策规则中输入或映射条件。
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
      <td role="rowheader">[!UICONTROL名称]</td>
     <td>输入或映射描述规则的名称。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL状态]</td>
      <td>选择决策的状态。
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL开始日期]</td>
      <td><p>输入或映射决策的开始日期。</p><p>有关支持的日期格式列表，请参阅 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在中键入强制 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL结束日期]</td>
      <td><p>输入或映射决策的结束日期。</p><p>有关支持的日期格式列表，请参阅 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在中键入强制 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL版面]</td>
      <td>选择要添加到此决策的版面
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL集合]</td>
      <td>选择包含此决策将考虑的选件的选件集合。
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL后备优惠]</td>
      <td>选择将呈现给与此决策规则不匹配的客户的备用选件。
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
      <td role="rowheader">[!UICONTROL名称]</td>
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
      <td role="rowheader">[!UICONTROL名称]</td>
     <td>输入或映射集合的名称。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL过滤器类型]
      </td>
      <td>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Elements]
      </td>
      <td>选择要包含在选区中的标记。
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
      <td role="rowheader">[!UICONTROL名称]</td>
     <td>输入或映射备用选件的名称。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL状态]
      </td>
      <td> 选择备用选件的状态。
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Placement]
      </td>
      <td>输入或映射备用选件的版面。
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
      <td role="rowheader">[!UICONTROL名称]</td>
     <td>输入或映射描述规则的名称。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL状态]</td>
      <td>选择决策的状态。
      </td>
    </tr>
    <tr>
      <td role="rowheader">版面</td>
      <td>选择个性化选件的版面。
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL开始日期]</td>
      <td><p>输入或映射个性化选件的开始日期。</p><p>有关支持的日期格式列表，请参阅 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在中键入强制 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL结束日期]</td>
      <td><p>输入或映射个性化选件的结束日期。</p><p>有关支持的日期格式列表，请参阅 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在中键入强制 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL决策规则]</td>
      <td>选择要添加到此个性化选件中的决策规则。
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL优先级]</td>
      <td>选择此选件的优先级。 优先级会影响是否将显示此选件，而不是其他选件。
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL上限约束]</td>
      <td>输入或映射此选件的显示次数。
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 删除记录]

此操作模块将删除 [!DNL Adobe Journey Optimizer].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL连接]</td>
     <td>有关创建与 [!DNL Adobe Journey Optimizer]，请参阅 <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >创建连接 [!DNL Adobe Journey Optimizer]</a> 在本文中。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL记录类型]
      </td>
      <td>
        选择要删除的记录类型
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL决策规则]</li>
        <li>[!UICONTROL Decision]</li>
        <li>[!UICONTROL标记]</li>
        <li>[!UICONTROL集合]</li>
        <li>[!UICONTROL后备优惠]</li>
        <li>[!UICONTROL Personalized offer]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Decision rule]/[!UICONTROL Decision]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback offer]/[!UICONTROL Personalized offer]
      </td>
      <td>
        选择要删除的记录。
      </td>
    </tr>

</tbody>
</table>

#### [!UICONTROL 进行自定义API调用]

此模块对 [!DNL Adobe Journey Optimizer] API

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL连接]</td>
     <td>有关创建与 [!DNL Adobe Journey Optimizer]，请参阅 <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >创建连接 [!DNL Adobe Journey Optimizer]</a> 在本文中。</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL路径]</p>
      </td>
      <td>
        <p>输入相对于{baseURL}的路径（以开头）<code>/</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL方法]</p>
      </td>
      <td>
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL标头]</td>
      <td>
        <p>以标准JSON对象的形式添加请求的标头。</p>
        <p>例如， <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion会自动添加授权标头和x-api-key标头。</p>
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
     <tr>
      <td role="rowheader">[!UICONTROL限制]  </td>
      <td>
        <p>输入希望模块在一个执行周期中返回的最大结果数。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 删除记录]

此操作模块将删除 [!DNL Adobe Journey Optimizer].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL连接]</td>
     <td>有关创建与 [!DNL Adobe Journey Optimizer]，请参阅 <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >创建连接 [!DNL Adobe Journey Optimizer]</a> 在本文中。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL记录类型]
      </td>
      <td>
        选择要删除的记录类型
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL决策规则]</li>
        <li>[!UICONTROL Decision]</li>
        <li>[!UICONTROL标记]</li>
        <li>[!UICONTROL集合]</li>
        <li>[!UICONTROL后备优惠]</li>
        <li>[!UICONTROL Personalized offer]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Decision rule]/[!UICONTROL Decision]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback offer]/[!UICONTROL Personalized offer]
      </td>
      <td>
        选择要删除的记录。
      </td>
    </tr>

</tbody>
</table>

#### [!UICONTROL 更新记录]

此操作模块可创建版面、决策、决策规则、标记、个性化选件、收藏集或备用选件。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL连接]</td>
     <td>有关创建与 [!DNL Adobe Journey Optimizer]，请参阅 <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >创建连接 [!DNL Adobe Journey Optimizer]</a> 在本文中。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL记录类型]
      </td>
      <td>
        选择要更新的记录类型
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL决策规则]</li>
        <li>[!UICONTROL Decision]</li>
        <li>[!UICONTROL标记]</li>
        <li>[!UICONTROL集合]</li>
        <li>[!UICONTROL后备优惠]</li>
        <li>[!UICONTROL Personalized offer]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Decision rule]/[!UICONTROL Decision]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback offer]/[!UICONTROL Personalized offer]
      </td>
      <td>
        选择要更新的记录。
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL字段]
      </td>
      <td>对于要更新的每个字段：
      <ol>
      <li>单击 <b>[!UICONTROL Add]</b>.</li>
      <li>选择是要添加、替换还是删除值。</li>
      <li>输入要更新的字段。</li>
      <li>为字段输入新值。</li>
      </td>
    </tr>

</tbody>
</table>


### 搜索

#### [!UICONTROL 列出记录]

此搜索模块会列出选定类型的记录，并根据您指定的条件返回结果。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL连接]</td>
     <td>有关创建与 [!DNL Adobe Journey Optimizer]，请参阅 <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >创建连接 [!DNL Adobe Journey Optimizer]</a> 在本文中。</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL记录类型]</p>
      </td>
      <td>
        <p>选择要列出的记录类型。</p>
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL决策规则]</li>
        <li>[!UICONTROL Decision]</li>
        <li>[!UICONTROL标记]</li>
        <li>[!UICONTROL集合]</li>
        <li>[!UICONTROL后备优惠]</li>
        <li>[!UICONTROL Personalized offer]</li>
       </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL查询运算符]</p>
      </td>
      <td>
        <p>选择要应用于查询中参数的运算符</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL字段]</td>
      <td><p>如果要将搜索限制为特定字段，请输入字段。 对于要将搜索限制为的每个字段，单击[!UICONTROL添加项目]并输入字段名称。</p><p>路径表达式采用点分隔路径的形式，如 <code>_instance.xdm:name</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Order by] </td>
      <td>输入或映射要按其对结果排序的属性。
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL顺序方向]</td>
   <td>选择要按升序还是降序方向对结果进行排序。
    </td>
     </tr>
  </tbody>
</table>
