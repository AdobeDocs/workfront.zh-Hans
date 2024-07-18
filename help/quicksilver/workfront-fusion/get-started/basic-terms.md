---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion中的基本术语
description: 除了Adobe Workfront许可证之外，Adobe Workfront Fusion还需要Adobe Workfront Fusion许可证。
author: Becky
feature: Workfront Fusion
exl-id: 2169dc2e-2135-47e0-a615-3de12cd120a9
source-git-commit: f11af8d9d1e5fa65c2efb4d882d25f9e13784611
workflow-type: tm+mt
source-wordcount: '828'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]中的基本术语

>[!NOTE]
>
>除[!UICONTROL Adobe Workfront]许可证外，[!DNL Adobe Workfront Fusion]还需要[!DNL Adobe Workfront Fusion]许可证。


<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>操作</p> </td> 
   <td>一个模块，允许您从选定的应用程序或服务读取捆绑包，或将捆绑包写入其中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL汇总]</p> </td> 
   <td> <p>一种模块类型，可将多个捆绑包（多个数据阵列）合并到一个捆绑包中。 有关详细信息，请参阅[！UICONTROL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/aggregator-module.md" class="MCXref xref">[！UICONTROL Aggregator]模块。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API 密钥</td> 
   <td>唯一代码，用于标识调用用于身份验证的软件API的用户、开发人员或程序。 由于[!DNL Adobe Workfront Fusion]模块通过连接API工作，因此API密钥有时是必需的。 API密钥由需要它们的应用程序分发。 例如，如果您需要[!DNL ActiveCampaign]的API密钥，可以通过您的[!DNL ActiveCampaign]帐户请求它。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">应用程序或服务</td> 
   <td> <p>最常见的软件应用程序。</p> <p>应用程序也可以是处理数据的特殊功能，如迭代器或聚合器。 </p> <p>服务是捆绑包的来源，这些捆绑包可能包括Web API、网页、不同类型的服务器(FTP、SMTP、IMAP)等。 </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">应用程序连接器</td> 
   <td>连接到其他系统的应用程序。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>捆绑</p> </td> 
   <td> <p>捆绑是模块返回或接收的基本单元。 捆绑包由项目组成。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>将应用或服务添加到方案时，很可能是您必须首先在[!DNL Workfront Fusion]与应用或服务之间创建连接，以检索或发送所选数据。 有关详细信息，请参阅<a href="../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md" class="MCXref xref">连接概述</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>周期</p> </td> 
   <td> <p>循环是指方案运行的两个阶段：操作和提交。 此方案可能包含一个或多个周期。 有关更多详细信息，请参阅[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">方案执行、周期和阶段。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>数据存储</p> </td> 
   <td> <p>一种工具，用于存储方案中的数据，或允许您在单个方案或方案运行之间传输数据。 有关详细信息，请参阅[！UICONTROL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/data-stores.md" class="MCXref xref">数据存储。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>数据传输</p> </td> 
   <td> <p>通过您的方案传输的数据量。 有关详细信息，请参阅[！UICONTROL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">方案详细信息。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>筛选</p> </td> 
   <td> <p>可在两个模块之间应用的附加功能。 过滤器允许您然后仅使用符合特定条件的包。 您可以应用许多不同的过滤器。 有关详细信息，请参阅<a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">在[！UICONTROL Adobe Workfront Fusion]</a>中将筛选器添加到方案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>ID</p> </td> 
   <td> <p>用于唯一标识捆绑包的名称。 ID通常用于区分要从给定服务中更新或删除的捆绑包。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>项</p> </td> 
   <td> <p>捆绑的一部分。 捆绑包可以包含多个项目。 有多种不同类型的项目：文本、数字、布尔值（是/否）、日期、时间、缓冲区（二进制数据）、集合、选择菜单、数组和验证。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL迭代器]</p> </td> 
   <td> <p>一种模块类型，允许您接收一捆数据（一组数据）并将其划分为单独的捆绑包。 有关详细信息，请参阅[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">[！UICONTROL迭代器]模块。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>模块</p> </td> 
   <td> <p>方案中的单一步骤，在关联的应用程序或服务中执行功能，例如创建记录。</p> <p>每个应用程序或服务都有各种模块定义其响应请求的方式。</p> <p>模块有4种类型：操作、触发器、迭代器和聚合。</p> <p> <img src="assets/module.jpg"> </p> <p>有关详细信息，请参阅<a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">模块类型</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>操作</p> </td> 
   <td> <p>模块执行的任务。</p><p>有关详细信息，请参阅[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/get-started/operations-in-workfront-fusion.md" class="MCXref xref">操作。</p>
  </tr> 
  <tr> 
   <td role="rowheader">公钥/私钥</td> 
   <td>公钥和私钥用于加密和解密数据。 公钥可以分发，任何拥有公钥的人都可以加密数据，但只有私钥可以解密。 同样，拥有私钥的用户可以加密任何拥有公钥的用户都可以解密的数据。 私钥加密可确保数据来自私钥的所有者，并用作数据来源的验证。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Router]</p> </td> 
   <td>允许您复制数据或向场景添加新路由，以便重新路由数据并单独处理不同的数据组。 有关详细信息，请参阅[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/router-module.md" class="MCXref xref">[！UICONTROL Router]模块。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>方案</p> </td> 
   <td> <p>用户创建的一系列自动化步骤，每个步骤均由模块表示和执行。 场景的目的是移动和处理数据。</p> <p> <img src="assets/scenario-350x178.jpg" style="width: 350;height: 178;"> </p> <p> 有关详细信息，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[！UICONTROL Adobe Workfront Fusion]</a>中创建方案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>交易</p> </td> 
   <td> <p>[!DNL Workfront Fusion] 使用事务处理捕获方案生命周期。 事务由若干阶段组成，在这些阶段中，数据从一个一致状态转换为另一个一致状态。 有4个阶段：初始化、操作（读取或写入）、提交/回滚和最终化。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>触发器</p> </td> 
   <td> <p>一个模块，允许您获取自上次运行方案以来添加或更新过的包。 有两种类型的触发器：轮询和即时(webhook)。 有关详细信息，请参阅[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">即时触发器(webhook)。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Webhook</p> </td> 
   <td> <p>一种特殊类型的触发器，允许您在新捆绑包可用后立即运行场景。 有关详细信息，请参阅[！UICONTROL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">即时触发器(webhook)。</p> </td> 
  </tr> 
 </tbody> 
</table>
