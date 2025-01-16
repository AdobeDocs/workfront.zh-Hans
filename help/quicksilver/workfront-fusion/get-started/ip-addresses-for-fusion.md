---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 用于访问Adobe Workfront Fusion的IP地址
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
feature: Workfront Fusion
exl-id: f6295cc7-367f-4c8b-891b-cc11ff42a225
source-git-commit: 3983d811a849c01b3c34b1cd6ee895e5552225a6
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# 用于访问[!DNL Adobe Workfront Fusion]的IP地址

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* [在组织的允许列表中配置Fusion的IP地址](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/set-up-and-manage-orgs-and-teams/set-up-orgs-teams-and-users/set-up-ip-addresses-for-fusion.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

>[!NOTE]
>
>除[!DNL Adobe Workfront license]外，[!DNL Adobe Workfront Fusion]还需要[!DNL Adobe Workfront Fusion]许可证。

列入允许列表如果您的防火墙或邮件服务器配置为仅允许访问某些供应商，则必须将某些IP地址添加到其，以允许您的环境与[!DNL Adobe Workfront Fusion]之间的开放通信。

您可以将所有Fusion IP地址和域添加到允许列表，也可以查找Fusion群集并仅添加该群集的IP地址和域。

## 添加所有Fusion IP地址和域

将以下IP地址添加到您的允许列表：

* 52.30.133.50
* 54.220.93.204
* 34.254.76.122
* 54.244.142.219
* 52.39.217.230
* 44.241.82.96
* 100.20.126.137
* 34.223.32.4
* 52.39.176.220
* 20.36.133.48/28
* 20.81.156.240/28
* 172.172.84.48/28

此外，如果贵组织使用出站网络过滤，请将以下域添加到您的以使您的允许列表能够访问Workfront Fusion。 这些用于Webhook。

* hook.app.workfrontfusion.com
* hook.app-eu.workfrontfusion.com
* hook.app-az.workfrontfusion.com

## 仅为群集添加Fusion IP地址和域

### 识别您的数据中心

IP地址因存储数据的位置而异。

如果通过URL访问Fusion，则可以检查该URL以查找数据中心。

| URL | 数据中心 |
| --- | --- |
| `https://app.workfrontfusion.com/` | 美国数据中心 |
| `https://app-eu.workfrontfusion.com/` | 欧盟数据中心 |
| `https://app-az.workfrontfusion.com/` | Azure数据中心 |

如果您通过experience.adobe.com访问Fusion，则可以检查浏览器中的“网络”选项卡以识别数据中心。

| URL | 数据中心 |
| --- | --- |
| 对`https://fusion.adobe.com`的调用 | 美国数据中心 |
| 对`https://eu.fusion.adobe.com`的调用 | 欧盟数据中心 |
| 对`https://az.fusion.adobe.com`的调用 | Azure数据中心 |

### 为数据中心添加IP地址和域

将以下IP地址添加到您的允许列表以使[!DNL Workfront Fusion]能够访问您的系统。

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
     <li>100.20.126.137</li>
     <li>34.223.32.4</li>
     <li>52.39.176.220</li>
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 在Microsoft Azure群集上</td> 
   <td> 
    <ul> 
     <li>20.36.133.48/28</li> 
     <li>20.81.156.240/28</li> 
     <li>172.172.84.48/28</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

此外，如果贵组织使用出站网络过滤，请将以下域添加到您的以使您的允许列表能够访问Workfront Fusion。

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
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront Fusion] 在Microsoft Azure群集上</p> </td> 
   <td> <p>hook.app-az.workfrontfusion.com </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>出站网络过滤不常见。 请咨询网络管理员，了解是否需要更新允许列表以适应环境。

列入允许列表 列入允许列表有关设置组织的详细信息，请参阅[配置防火墙的](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)。
