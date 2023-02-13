---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Adobe Workfront聚变中的类型强制
description: 本文档介绍如何 [!DNL Adobe Workfront Fusion] 在收到预期和意外数据格式值时的行为。
author: Becky
feature: Workfront Fusion
exl-id: 847a17c9-bd67-4132-81a8-2a5fe8d516cb
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 1%

---

# 在中键入强制 [!DNL Adobe Workfront Fusion]

## 访问要求

您必须具有以下访问权限才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]许可证**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

### 类型强制

本文档介绍如何 [!DNL Adobe Workfront Fusion] 在收到预期和意外数据格式值时的行为。

<table style="table-layout:auto">
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>预期</th> 
   <th>已收到</th> 
   <th> <p>描述</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>阵列 </td> 
   <td>阵列 </td> 
   <td> <p>该值保持不变。</p> </td> 
  </tr> 
  <tr> 
   <td>阵列 </td> 
   <td>其他 </td> 
   <td> <p>如果接收的值不是数组类型， [!DNL Workfront Fusion] 将创建一个数组，第一个（且唯一的）元素将是接收的值。</p> </td> 
  </tr> 
  <tr> 
   <td>布尔 </td> 
   <td>布尔 </td> 
   <td> <p>该值保持不变。</p> </td> 
  </tr> 
  <tr> 
   <td>布尔 </td> 
   <td>数字 </td> 
   <td> <p>即使值为0，该值也会转换为逻辑是。</p> </td> 
  </tr> 
  <tr> 
   <td>布尔 </td> 
   <td>文本 </td> 
   <td> <p>如果值等于false或值为空，则会将其转换为逻辑编号。 如果没有，则转换为逻辑是。</p> </td> 
  </tr> 
  <tr> 
   <td>布尔 </td> 
   <td>其他 </td> 
   <td> <p>只要接收的值存在（不为空），该值就会转换为逻辑“是”。</p> </td> 
  </tr> 
  <tr> 
   <td>缓冲 </td> 
   <td>缓冲 </td> 
   <td> <p>只有在代码页按预期情况下，才会将值保持不变。 如果代码页不同， [!DNL Workfront Fusion] 将尝试将收到的值转换为请求的代码页。 如果此转换不受支持， [!DNL Workfront Fusion] 将返回验证错误。</p> </td> 
  </tr> 
  <tr> 
   <td>缓冲 </td> 
   <td>布尔 </td> 
   <td> <p>该值将转换为文本(true/false)，然后按照上述步骤转换为文本，再转换为二进制数据。</p> </td> 
  </tr> 
  <tr> 
   <td>缓冲 </td> 
   <td>日期 </td> 
   <td> <p>该值将转换为ISO 8601文本，然后按照上述转换为文本的步骤转换为二进制数据。</p> </td> 
  </tr> 
  <tr> 
   <td>缓冲 </td> 
   <td>数字 </td> 
   <td> <p>该值将转换为文本，然后按照上述步骤转换为文本，从而转换为二进制数据。</p> </td> 
  </tr> 
  <tr> 
   <td>缓冲 </td> 
   <td>文本 </td> 
   <td> <p>该值将转换为二进制数据并按预期进行编码。 如果未指定预期的编码，将使用utf8编码。</p> </td> 
  </tr> 
  <tr> 
   <td>缓冲 </td> 
   <td>其他 </td> 
   <td> <p>[!DNL Workfront Fusion] 返回验证错误。</p> </td> 
  </tr> 
  <tr> 
   <td>收藏集 </td> 
   <td>收藏集 </td> 
   <td> <p>该值保持不变。</p> </td> 
  </tr> 
  <tr> 
   <td>收藏集 </td> 
   <td>其他 </td> 
   <td> <p>[!DNL Workfront Fusion] 返回验证错误。</p> </td> 
  </tr> 
  <tr> 
   <td>日期 </td> 
   <td>日期 </td> 
   <td> <p>该值保持不变。</p> </td> 
  </tr> 
  <tr> 
   <td>日期 </td> 
   <td>文本 </td> 
   <td> <p>[!DNL Workfront Fusion] 会尝试将文本转换为日期。 如果转换失败，则会返回验证错误。 日期必须包含日、月和年。 日期可能包含时区。 默认时区基于您的设置。 示例:</p> <p><code>2016-06-20T17:26:44.356Z</code> </p> <p><code>2016-06-20 19:26:44 GMT+02:00</code> </p> <p><code>2016-06-20 19:26+0200</code> </p> <p><code>2016-06-20 17:26:44</code> </p> <p><code>2016-06-20</code> </p> <p><code>2016/06/20 17:26:44</code> </p> <p><code>2016/06/20 19:26:44+02:00</code> </p> <p><code>2016/06/20 17:26</code> </p> <p><code>2016/06/20 5:26 PM</code> </p> <p><code>2016/06/20</code> </p> <p><code>06/20/2016 17:26:44</code> </p> <p><code>06/20/2016 19:26:44+02:00</code> </p> <p><code>06/20/2016 17:26</code> </p> <p><code>06/20/2016 5:26 PM</code> </p> <p><code>06/20/2016</code> </p> <p><code>20.6.2016 17:26:44</code> </p> <p><code>20.6.2016 19:26:44+02:00</code> </p> <p><code>20.6.2016 17:26</code> </p> <p><code>20.6.2016</code> </p> </td> 
  </tr> 
  <tr> 
   <td>日期 </td> 
   <td>其他 </td> 
   <td> <p>[!DNL Workfront Fusion] 返回验证错误。</p> </td> 
  </tr> 
  <tr> 
   <td>数字 </td> 
   <td>数字 </td> 
   <td> <p>该值保持不变。</p> </td> 
  </tr> 
  <tr> 
   <td>数字 </td> 
   <td>文本 </td> 
   <td> <p>[!DNL Workfront Fusion] 会尝试将文本转换为数字。 如果转换失败，则会返回验证错误。</p> </td> 
  </tr> 
  <tr> 
   <td>数字 </td> 
   <td>其他 </td> 
   <td> <p>[!DNL Workfront Fusion] 返回验证错误。</p> </td> 
  </tr> 
  <tr> 
   <td>文本 </td> 
   <td>文本 </td> 
   <td> <p>该值保持不变。</p> </td> 
  </tr> 
  <tr> 
   <td>文本 </td> 
   <td>阵列 </td> 
   <td> <p>如果给定的数组支持转换为文本，则值将被转换。 如果没有， [!DNL Workfront Fusion] 将返回验证错误。</p> </td> 
  </tr> 
  <tr> 
   <td>文本 </td> 
   <td>布尔 </td> 
   <td> <p>此值将转换为文本(true/false)。</p> </td> 
  </tr> 
  <tr> 
   <td>文本 </td> 
   <td>缓冲 </td> 
   <td> <p>如果为二进制数据指定了文本编码，则值将转换为文本。 如果没有， [!DNL Workfront Fusion] 将返回验证错误。</p> </td> 
  </tr> 
  <tr> 
   <td>文本 </td> 
   <td>日期 </td> 
   <td> <p>值将转换为ISO 8601文本。</p> </td> 
  </tr> 
  <tr> 
   <td>文本 </td> 
   <td>数字 </td> 
   <td> <p>值将转换为文本。</p> </td> 
  </tr> 
  <tr> 
   <td>文本 </td> 
   <td>其他 </td> 
   <td> <p>[!DNL Workfront Fusion] 返回验证错误。</p> </td> 
  </tr> 
  <tr> 
   <td>时间 </td> 
   <td>时间 </td> 
   <td> <p>该值保持不变。</p> </td> 
  </tr> 
  <tr> 
   <td>时间 </td> 
   <td>文本 </td> 
   <td> <p>[!DNL Workfront Fusion] 会尝试将时间转换为小时:minutes:秒格式。 如果转换失败，则会返回验证错误。</p> </td> 
  </tr> 
  <tr> 
   <td>时间 </td> 
   <td>其他 </td> 
   <td> <p>[!DNL Workfront Fusion] 返回验证错误。</p> </td> 
  </tr> 
 </tbody> 
</table>
