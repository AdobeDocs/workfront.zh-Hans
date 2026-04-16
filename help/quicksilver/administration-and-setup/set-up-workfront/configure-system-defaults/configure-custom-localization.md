---
user-type: administrator
product-area: system-administration;setup
title: 配置自定义本地化
description: 通过自定义本地化，您可以使用不同的语言定义自定义术语和短语。 然后，Workfront会以浏览器设置中设置的语言显示这些术语。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: bdc6d5ee-2037-4d0b-bf18-3e6cc9cb078e
source-git-commit: 28178c3794832e14552d988259c1792a6fed1da1
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 7%

---

# 配置自定义本地化

通过自定义本地化，您可以使用不同的语言定义自定义术语和短语。 然后，Workfront会以用户的Adobe Identity Management (IMS)设置中设置的语言显示这些术语。 如果用户不在Adobe IMS上，则术语将以用户的浏览器设置中设置的语言显示。

例如，您可以设置标签“Target Audience”以翻译为德语单词“Zielgruppe”。 任何选择德语作为浏览器主要语言的用户都会看到“Zielgruppe”一词作为任何英语中标记为“目标受众”的字段的标签。

您可以配置多种语言的翻译。 当前可用的语言包括：

* 中文（繁体）
* 中文（简体）
* 法语
* 德语
* 意大利语
* 日语
* 韩语
* 葡萄牙语（巴西）
* 西班牙语

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>工作流Prime或更高版本 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>标准</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员才能配置翻译。</p>  </td> 
  </tr>
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 设置本地化时的注意事项

配置本地化时，请考虑以下事项：

* 您可以将术语配置为翻译成多种语言。
* 本地化适用于自定义字段标签（包括用作列标题时）和工具提示。
* 自定义本地化可应用于从Business Rules生成的消息，但必须在Business Rule中启用。

  有关说明，请参阅创建和编辑业务规则一文中的[在业务规则中启用本地化](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md#using-custom-localization-with-business-rules)。

## 配置翻译

在“设置”区域中配置转换。

1. 单击Adobe Workfront右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon.png)，或（如果可用）单击左上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png)，然后单击&#x200B;**[!UICONTROL 设置]** ![设置图标](/help/_includes/assets/gear-icon-setup.png)。
1. 在设置区域中，单击左侧导航面板中的&#x200B;**本地化**。
1. 若要添加新翻译，请单击&#x200B;**新建行**。
1. 在&#x200B;**英语**&#x200B;列中，输入应翻译的英语术语。
1. 在要翻译术语的语言列中，输入目标语言中的术语。
1. 要将单词翻译成其他语言，请将翻译添加到相应的语言列。
1. 要重新排序语言列，请单击要移动的列的标题，然后将其拖动到所需位置。
