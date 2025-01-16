---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: ' [!DNL Adobe Workfront Fusion]中的数学变量'
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
feature: Workfront Fusion
exl-id: 2fb561d2-0780-4fd6-87b3-5360a02df177
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 2%

---

# [!DNL Adobe Workfront Fusion]中的数学变量

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* [数学变量](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/mapping-panel/functions/math-variables.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

<!--Audited: 4/2024-->

## 访问要求

您必须具有以下权限才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td>  
   <td> <p>任何</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td>  
   <td> <p>新文档： [！UICONTROL Standard]</p><p>或</p><p>当前： [！UICONTROL Work]或更高版本</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td>  
   <td> 
   <p>当前：无[!DNL Workfront Fusion]许可证要求。</p> 
   <p>或</p> 
   <p>旧版：任意 </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">产品</td>  
   <td> 
   <p>新增：</p> <ul><li>[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Workfront]计划：您的组织必须购买[!DNL Adobe Workfront Fusion]。</li><li>已包括[！UICONTROL Ultimate] [!DNL Workfront]计划： [!DNL Workfront Fusion]。</li></ul> 
   <p>或</p> 
   <p>当前：您的组织必须购买[!DNL Adobe Workfront Fusion]。</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## pi

表示数学符号$\pi$。

## [!UICONTROL random]

返回范围[`0`，`1`]中的浮点伪随机数（包括`0`但不包括`1`）。

使用以下公式生成范围[`min`，`max`]中的整数伪随机数（包括`min`和`max`）：

![](assets/math-variable-random-350x61.png)

```
floor(random * (1.max - 1.min + 1)) + 1.min
```
