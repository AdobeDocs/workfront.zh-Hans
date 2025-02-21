---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 视图：在列中显示图像而不是字符串
description: 您可以使用文本模式将视图中对象的名称替换为图像。 您还可以添加指向图像的链接，该链接可以打开它替换的对象。
author: Nolan
feature: Reports and Dashboards
exl-id: e1e4a993-f05c-4b6e-b00a-e96c9ab4c94f
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# 视图：在列中显示图像而不是字符串

<!--Audited: 11/2024-->

您可以使用文本模式将视图中对象的名称替换为图像。 您还可以添加指向图像的链接，该链接可以打开它替换的对象。

>[!NOTE]
>
>图像以实际分辨率显示，因此请尝试使用小图像。

![将项目名称替换为图像和链接](assets/replace-project-name-with-image-and-link-350x125.png)

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> 
    <p>新增：</p>
   <ul><li><p>修改过滤器的参与者 </p></li>
   <li><p>用于修改报告的标准</p></li> </ul>

<p>当前：</p>
   <ul><li><p>请求修改筛选器 </p></li>
   <li><p>计划修改报告</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限以修改报告</p> <p>编辑对筛选器、视图和分组的访问权限以修改筛选器</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p>  </td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 示例：将项目视图中项目的名称替换为图像：

1. 将图像上传到Adobe Workfront外部的网站或服务器。 您必须能够使用Web浏览器访问图像。

   >[!TIP]
   >
   >* 每种浏览器类型各不相同，但都能够显示URL。
   >* 避免使用上载到Workfront的图像。 由于存储在Workfront中的图像不是公开可用的，并且其访问密钥会在一段时间后过期，因此这些图像会随着时间的推移停止显示在视图中。
   >* 保存在计算机上的图像没有固有URL。 查找提供图像托管的网站，并在该网站上托管您的图像。 您的组织可能已经拥有此类站点。

1. 使用Web浏览器，转到您保存的图像。
1. 通过执行以下操作获取图像的URL：

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: I used this blog post to document what kind of image we need for this: https://www.canto.com/blog/image-url/ (consulting uses this)) </p>
   -->

   1. 右键单击并选择&#x200B;**复制图像位置**&#x200B;或&#x200B;**获取链接**，具体取决于您的浏览器。 现在，您拥有该特定图像的URL，并且可以从剪贴板中粘贴该URL。
   1. 确保具有该链接的所有人都有权查看图像，只需转到该链接即可，无需登录即可访问。

1. 转到项目，单击项目名称旁边的&#x200B;**更多**&#x200B;菜单![更多图标](assets/more-icon-45x33.png)，然后单击&#x200B;**编辑**。

1. 在&#x200B;**URL**&#x200B;字段中，添加指向该图像的链接。
1. 转到项目列表中的项目视图。
1. 单击&#x200B;**视图**&#x200B;下拉菜单，然后单击&#x200B;**新建视图**。
1. 单击&#x200B;**项目名称**&#x200B;的列标题，然后单击&#x200B;**切换到文本模式**。

1. 将以下代码添加到现有代码的列中：

   ```
   displayname=Link Project
   image.name=Link Project
   image.valuefield=URL
   link.linkproperty.0.name=projectID
   link.linkproperty.0.value=ID
   link.lookup=link.edit
   link.page=/view
   link.valuefield=objCode
   link.valueformat=val
   textmode=true
   type=image
   valueformat=
   ```

1. 单击&#x200B;**完成** > **保存视图**。
您选择的图像将替换项目视图中的项目名称，并且该图像是项目的链接。