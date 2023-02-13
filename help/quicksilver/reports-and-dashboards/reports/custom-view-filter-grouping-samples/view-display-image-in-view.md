---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: “查看：在列中显示图像而不是字符串'
description: 您可以使用文本模式将视图中对象的名称替换为图像。 您还可以添加指向图像的链接，以打开该链接所替换的对象。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e1e4a993-f05c-4b6e-b00a-e96c9ab4c94f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 0%

---

# 查看：在列中显示图像而不是字符串

您可以使用文本模式将视图中对象的名称替换为图像。 您还可以添加指向图像的链接，以打开该链接所替换的对象。

>[!NOTE]
>
>图像以实际分辨率显示，因此请尝试使用小图像。

![](assets/replace-project-name-with-image-and-link-350x125.png)

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报表、功能板、日历的访问</p> <p>编辑对过滤器、视图、分组的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 示例：将项目视图中项目的名称替换为图像：

1. 将图像上传到Adobe Workfront外部的网站或服务器。 您必须能够使用Web浏览器访问图像。

   >[!TIP]
   >
   >* 每种浏览器类型都不同，但都能显示URL。
   >* 避免使用上传到Workfront的图像。 由于存储在Workfront中的图像不可公开使用，并且具有在一段时间后过期的访问键，因此这些图像会随着时间的推移而停止在视图中显示。
   >* 保存在计算机上的图像没有固有URL。 查找提供图像托管的网站，并将您的图像托管到该网站。 贵组织可能已经拥有此类网站。


1. 使用Web浏览器，转到您保存的图像。
1. 通过执行以下操作获取图像的URL:

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: I used this blog post to document what kind of image we need for this: https://www.canto.com/blog/image-url/ (consulting uses this)) </p>
   -->

   1. 右键单击并选择 **复制图像位置**&#x200B;或 **获取链接**，具体取决于您的浏览器。 您现在拥有该特定图像的URL，并可以从剪贴板中粘贴该URL。
   1. 确保具有该链接的每个人都有权通过转到链接来查看图像，并且他们无需登录即可访问该图像。

1. 转到项目，单击 **更多** 菜单 ![](assets/more-icon-45x33.png) 在项目名称旁边，单击 **编辑**.

1. 在 **URL** 字段中，添加指向图像的链接。
1. 在列表或报表中导航到项目视图，并自定义该视图。
1. 单击 **项目名称**，然后单击 **切换到文本模式**.

1. 将以下代码添加到列中的现有代码：

   ```
   displayname=Link Project
   ```

   ```
   image.name=Link Project
   ```

   ```
   image.valuefield=URL
   ```

   ```
   link.linkproperty.0.name=projectID
   ```

   ```
   link.linkproperty.0.value=ID
   ```

   ```
   link.lookup=link.edit
   ```

   ```
   link.page=/view
   ```

   ```
   link.valuefield=objCode
   ```

   ```
   link.valueformat=val
   ```

   ```
   textmode=true
   ```

   ```
   type=image
   ```

   ```
   valueformat=
   ```

   您选择的图像将替换项目视图中的项目名称，并且该图像是指向项目的链接。

1. 单击 **保存视图**.
