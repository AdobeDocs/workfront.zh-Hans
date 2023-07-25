---
title: 隐藏的测试文件
author: Bob
description: 在搜索和左侧导航中隐藏
hidefromtoc: true
hide: true
exl-id: b6b0f429-b619-4b8e-ab81-ad190dae5a0b
source-git-commit: 5c47b09550c54b7ea4f8319bb42e93572e06324b
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 1%

---


# 隐藏测试文件 — 功能分支测试

此文件在搜索中隐藏(`hide: yes`)和左侧导航栏(`hidefromtoc: yes`)。

<span class="preview">此文件为 **隐藏** 从搜索(`hide: yes`)和左侧导航栏(`hidefromtoc: yes`)。</span>

<p class="preview">此文件在搜索中**隐藏**（“隐藏：是”）并在左侧导航中（“hidefromtoc：是”）隐藏。</p>

## 图像测试

![图像测试](assets/get-started.png){width="50" align="center"}

## 预览突出显示测试

**对组件块使用DIV。**

DIV从下面开始。

<div class="preview">

DIV的开头。

>[!NOTE]
>
>这是张便笺。
>
>我请求突出显示注释的背景。

![图像](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/assets/add-admin-1.png)

最后一个高亮显示的项目。

</div>

DIV在上方结束。

**对段落或短语使用SPAN**

这是段落。 <span class="preview">我是黄色文字。</span> 请记住正确关闭您的语法，否则页面可能会呈现“怪异”。

DIV和SPAN在HTML表中也很有用。

**其他支持的HTML元素**

您还可以指定 `class="preview"` 中的语法 `<p>`， `<td>`， `<tr>`，等等。 确保在预览时测试。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr class="preview"> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront计划</a>*</td> 
   <td> <p>专业或专业以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"></td> 
   <td> <p class="preview">计划</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jira访问</td> 
   <td> <p><span class="preview">系统管理员访问权限</p> <p>重要信息：我们建议您在Jira和Workfront中创建单独的系统管理员帐户以专门用于此集成，而不是使用可能附加到用户的现有帐户。 </span></p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>您必须是Workfront管理员。 有关Workfront管理员的信息，请参阅。</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

视频品质= 12

>[!VIDEO](https://video.tv.adobe.com/v/3413544/?quality=12)

视频品质= 6

>[!VIDEO](https://video.tv.adobe.com/v/3413544/?quality=6)

HTML表中的视频

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  </tr> 
  <tr> 
   <td role="rowheader">此视频是否有效？</td> 
   <td>不，它没有 </td> 
  </tr> 
 </tbody> 
</table>

Markdown表格中的视频

| 列 1 | 列 2 |
|---|---|
| 这行得通吗？ | 也不是 |


