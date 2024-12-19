---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 使用cURL添加HTTP模块
description: 您可以将cURL请求粘贴到场景中，然后Fusion会创建根据cURL请求配置的HTTP模块。
author: Becky
feature: Workfront Fusion
exl-id: 5eac3e87-0dd3-4bad-ae3e-77264329b717
source-git-commit: 785f39fabcb19233fd1bc79c14222225a3ea72a2
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 1%

---

# 使用cURL添加HTTP模块

您可以将cURL请求粘贴到场景中，然后Fusion会创建根据cURL请求配置的HTTP模块。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能使用本文中的功能：

<table style="table-layout:auto"> 
  <tbody>  
    <tr>  
      <td>Adobe Workfront计划</td>  
      <td>任何</td>  
    </tr>  
    <tr>  
      <td>Adobe Workfront许可证</td>  
      <td>
        新建： Standard<br>
        或<br>
        当前：工作或更高
      </td>  
    </tr>  
    <tr>  
      <td>Adobe Workfront Fusion许可证</td>  
      <td> 
        当前：无Workfront Fusion许可证要求。<br>
        或<br>
        旧版：任意
      </td>  
    </tr>  
    <tr>  
      <td>产品</td>  
      <td> 
        新文档：选择或Prime Workfront计划：您的组织必须购买Adobe Workfront Fusion。<br>
        Ultimate Workfront计划：包含Workfront Fusion。<br>
        或<br>
        当前：您的组织必须购买Adobe Workfront Fusion。
      </td>  
    </tr> 
  </tbody>  
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

+++

## 从cURL请求创建HTTP模块


要使用cURL创建HTTP模块，请执行以下操作：

1. 在Fusion之外创建cURL请求的文本，例如在文本编辑器中。
1. 将cURL请求复制到剪贴板。
1. 单击左侧面板中的&#x200B;**[!UICONTROL 方案]**&#x200B;选项卡。
1. 选择要创建模块的方案。
1. 单击方案上的任意位置以进入方案编辑器。
1. 右键单击方案编辑器中的任何空白区域，然后选择&#x200B;**粘贴**。

   或

   按Ctrl + V (Windows)或Cmd + V (Mac)。


   创建HTML模块。
1. 拖动模块以将其连接到场景。

## 故障排除

如果cURL未粘贴到场景中，请检查浏览器设置以确保启用从剪贴板粘贴。


