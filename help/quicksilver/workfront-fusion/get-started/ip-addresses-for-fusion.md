---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 用于访问Adobe Workfront Fusion的IP地址
description: Adobe Workfront Fusion除了需要Adobe Workfront许可证之外，还需要Adobe Workfront Fusion许可证。
author: Becky
feature: Workfront Fusion
exl-id: f6295cc7-367f-4c8b-891b-cc11ff42a225
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 3%

---

# 用于访问的IP地址 [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] 需要 [!DNL Adobe Workfront Fusion] 除 [!DNL Adobe Workfront license].

如果您的防火墙或邮件服务器配置为仅允许访问某些供应商，则必须向其添加某些IP地址，以便允许在您的环允许列表境和 [!DNL Adobe Workfront Fusion].

将以下IP地址添加到您的允许列表以启用 [!DNL Workfront Fusion] 来访问您的系统。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 欧盟数据中心</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] 美国数据中心</p> </td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

此外，如果贵组织使用出站网络过滤，请将以下域添加到允许列表您的中，以启用系统访问Workfront Fusion。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 欧盟数据中心</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] 美国数据中心</p> </td> 
   <td> <p>hook.app.workfrontfusion.com </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>出站网络过滤不常见。 请咨询网络管理员，以了解您是否需要更新允许列表以适应此情况。

有关设置贵组织的更多信允许列表息，请参阅 [配置防火墙的允许列表](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
