---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: JWT模块
description: 此 [!DNL Adobe Workfront Fusion] [!UICONTROL JWT] 应用程序提供了一个模块，用于根据提供的算法创建JWT令牌。
author: Becky
feature: Workfront Fusion
source-git-commit: d4f6f5d4919120e37fb94a23ac834a3896019584
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 0%

---

# [!UICONTROL JWT] 模块

此 [!DNL Adobe Workfront Fusion] [!UICONTROL JWT] 应用程序提供了一个模块，用于根据提供的算法创建JWT令牌。

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

## JWT模块及其字段

### 生成JWT

此模块基于所选算法生成JWT。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL算法]</td> 
   <td> <p>选择要生成JWT的算法。</p> <ul>
   <li><b>HS256</b>：使用SHA-256哈希算法的HMAC</li>
   <li><b>HS384</b>：使用SHA-384哈希算法的HMAC</li>
   <li><b>HS512</b>：使用SHA-512哈希算法的HMAC</li>
   <li><b>RS256</b>：使用SHA-256哈希算法的RSASSA-PKCS1-v1_5</li>
   <li><b>RS384</b>：使用SHA-384哈希算法的RSASSA-PKCS1-v1_5</li>
   <li><b>RS512</b>：使用SHA-512哈希算法的RSASSA-PKCS1-v1_5</li>
   <li><b>PS256</b>：使用SHA-256哈希算法的RSASSA-PSS（仅限节点^6.12.0或&gt;=8.0.0）</li>
   <li><b>PS384</b>：使用SHA-384哈希算法的RSASSA-PSS（仅限节点^6.12.0或&gt;=8.0.0）</li>
   <li><b>PS512</b>：使用SHA-512哈希算法的RSASSA-PSS（仅限节点^6.12.0或&gt;=8.0.0）</li>
   <li><b>ES256</b>：ECDSA采用P-256曲线和SHA-256哈希算法</li>
   <li><b>ES384</b>：ECDSA采用P-384曲线和SHA-384哈希算法</li>
   <li><b>ES512</b>：ECDSA采用P-521曲线和SHA-512哈希算法</li>
   </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL有效负载] </td> 
   <td> <p>对于要添加的每个有效负荷项目，单击 <b>添加项目</b> 并输入项目的键和值。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Options] </td> 
   <td> <p>对于要添加的每个选项项，单击 <b>添加项目</b> 并输入项目的键和值。</p> <p>可以使用以下键：
   <ul>
   <li><b>算法</b>：（默认：RS256）</li>
   <li><b>expiresIn</b>：以秒或描述时间范围的字符串表示（例如2天、10小时、7天）。 数值将解释为秒计数。 如果使用字符串，请确保提供时间单位（天、小时等），否则默认使用毫秒单位（120等于120毫秒）。</li>
   <li><b>notBefore</b>：以秒或描述时间范围的字符串表示（例如2天、10小时、7天）。 数值将解释为秒计数。 如果使用字符串，请确保提供时间单位（天、小时等），否则默认使用毫秒单位（120等于120毫秒）。
</li>
   <li><b>受众</b></li>
   <li><b>发行者</b></li>
   <li><b>jwtid</b></li>
   <li><b>主题</b></li>
   <li><b>noTimestamp</b></li>
   <li><b>标题</b></li>
   <li><b>keyid</b></li>
   <li><b>mutatePayload</b>：如果 <code>true</code>，sign函数将直接修改有效负载对象。 如果在应用声明后但在将其编码为令牌之前需要原始引用有效负载，则可以使用此功能。</li>
   <li><b>allowInsecureKeySizes</b>：如果 <code>true</code>，允许将模数低于2048的私钥用于RSA。</li>
   <li><b>allowInvalidAsymmetricKeyTypes</b>：如果 <code>true</code>，允许与指定算法不匹配的非对称密钥。 此选项仅用于向后兼容，应当避免。</li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>

