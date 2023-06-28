---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: SOAP模块
description: 您可以使用SOAP模块连接到Adobe Workfront Fusion中的SOAP API。
author: Becky
feature: Workfront Fusion
exl-id: 752e0766-25f2-4d22-bed5-7c931284258d
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 1%

---

# [!UICONTROL SOAP] 模块

您可以使用 [!UICONTROL SOAP] 要连接的模块 [!UICONTROL SOAP] 中的API [!UICONTROL Adobe Workfront Fusion].

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
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] 用于工作自动化和集成] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 计划，您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 计划。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关以下项的信息 [!DNL Adobe Workfront Fusion] 许可证，请参见 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 使用 [!UICONTROL SOAP] 模块

此 [!UICONTROL SOAP] 模块当前为测试版，不支持：

* 重新定义元素
* 分数数字限制
* 总数字限制
* 空格限制
* 输入和输出消息中的多个部分。 仅支持单部分消息
* 帮助定义的自定义XML架构元素 [[!UICONTROL SOAP] 编码](http://schemas.xmlsoap.org) 架构和元素。

>[!INFO]
>
>**示例:**
>  
>以下内容无法正确识别 [!UICONTROL Workfront Fusion]：
>
>```
><complexType name="ArrayOfFloat">
>
>   
>  <complexContent>
>
>      
>     <restriction base="soapenc:Array">
>
>         
>        <attribute ref="soapenc:arrayType"
>
>            
>           wsdl:arrayType="xsd:integer[]"/>
>
>      
>     </restriction>
>
>   
>  </complexContent>
>
>
></complexType>
>```

它包括 `soapenc:Array`， `soapenc:arrayType` 和 `wsdl:arrayType` 尚未支持的引用 [!UICONTROL Workfront Fusion].

## 解决方法

如果 [!UICONTROL SOAP] 模块拒绝处理WSDL文件，或在模块配置中引发各种错误，您可以尝试使用通用的 **[!UICONTROL HTTP] > [!UICONTROL 提出请求]** 模块代替：

1. In [!DNL Workfront Fusion]，创建新方案。
1. 插入 **[!UICONTROL HTTP] > [!UICONTROL 提出请求]** 场景中的模块。
1. 打开模块的配置并填写以下字段：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL方法]</td> 
      <td> <p>[！UICONTROLPOST]</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[！UICONTROL正文类型]</td> 
      <td> <p>[！UICONTROL Raw]</p> </td> [！UICONTROL ]
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL内容类型]</td> 
      <td> <p>[！UICONTROL XML (application/xml)]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL解析响应]</td> 
      <td>[！UICONTROL已启用]</td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/workaround-350x443.png)

1. 打开新的Web浏览器窗口或选项卡。
1. 将WSDL URL粘贴到Web浏览器的地址栏中，并获取XML文件。

   WSDL URL通常以 `?wsdl`，但不一定，例如 `http://voip.ms/api/v1/server.wsdl`.

1. 如果WSDL文件未直接显示在Web浏览器中，请在文本编辑器中打开下载的文件。
1. 搜索 `<service>` 或 `<wsdl:service>` 标记：

   ![](assets/service-350x65.png)

1. 找到后，从 `location` 属性。
1. In [!DNL Workfront Fusion]，将URL粘贴到HTTP模块的URL字段中。
1. 打开 [在线 [!UICONTROL SOAP] 客户端](https://wsdlbrowser.com/) 在新的Web浏览器窗口/选项卡中。
1. 将WSDL URL粘贴到“WSDL URL”字段中。
1. 单击 **[!UICONTROL 浏览]**.
1. 从左侧的函数列表中选取，例如 `getLanguages`.
1. 复制的内容 [!UICONTROL 请求XML] 文本区域。
1. In [!UICONTROL Workfront Fusion]，将复制的内容粘贴到模块的URL字段。
1. 通过将问号替换为实际值来提供所选参数的值：

   ![](assets/request-xml-350x172.png)

1. 通过单击关闭模块的配置 **[!UICONTROL 确定]**.
1. 执行方案或模块。
