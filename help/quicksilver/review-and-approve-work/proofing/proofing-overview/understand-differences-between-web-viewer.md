---
content-type: reference
product-area: documents
navigation-topic: proofing-overview
title: Web校对查看器与桌面校对查看器概述之间的差异
description: Adobe Workfront提供两种不同的校样查看器 — “编辑我”。
author: Courtney
feature: Digital Content and Documents
exl-id: 72ce147b-29c9-4c3b-a03c-2da0758bc178
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 2%

---

# Web校对查看器与桌面校对查看器概述之间的差异

Adobe Workfront提供两种不同的校样查看器：

* **Web校对查看器：** 主要用于校对静态和视频文件。 在Google Chrome、Firefox或Safari中运行。
* **桌面校对查看器：** 专为校对交互式文件以及视频和静态文件而设计。 在您的工作站上作为独立应用程序运行。 有关更多信息，请参阅 [了解桌面校对查看器](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md)

* 如果您的组织出于安全原因无法使用桌面校对查看器应用程序，则Workfront管理员可以配置您的系统，以便您能够在Web校对查看器中查看捆绑在ZIP存档文件中的交互式内容。 有关更多信息，请参阅  [在Web校对查看器中设置交互式内容校对](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/interactive-content-in-web-viewer.md).

以下列表可帮助您了解哪些校对查看器可用于对特定类型的内容进行校样：

* **交互式Web内容 — URL**:如果您使用URL为Web内容创建校样，并且希望以交互方式校样内容，则必须使用桌面校样查看器。
* **交互式Web内容 — ZIP文件**:如果您使用ZIP文件为Web内容创建校样，则可以使用Web校样查看器（存在一些限制）或桌面校样查看器。 有关在交互式内容中使用Web校样查看器时涉及的限制的信息，请参阅 [在Web校对查看器中设置交互式内容校对](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/interactive-content-in-web-viewer.md).

* **静态和视频内容**:如果创建包含静态内容的校样，则可以使用Web校样查看器或桌面校样查看器。

## 静态校样

| **功能** | **Web校对查看器** | **桌面校对查看器** |
|---|---|---|
| 打开静态校样 | ✓ | ✓&#42; |
| 单页、杂志和连续视图 | ✓ | ✓&#42; |
| 平移 | ✓ | ✓&#42; |
| 缩放 | ✓ | ✓&#42; |
| 旋转 | ✓ | ✓&#42; |
| 测量工具 | ✓（设置自定义大小的区域） | ✓&#42; |
| 缩略图视图 | ✓ | ✓&#42; |
| 静态校样导航器 | ✓ | ✓&#42; |
| 文档搜索 | ✓ | ✓&#42; |
| 在多个页面上发布评论 | ✓（适用于所有视图） | ✓&#42; （可在所有视图中使用） |
| 高级静态校样快捷键 | ✓(有关更多信息，请参阅 [校对查看器中的键盘快捷键](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/keyboard-shortcuts-proof.md)) | ✓&#42;(有关详细信息，请参阅 [校对查看器中的键盘快捷键](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/keyboard-shortcuts-proof.md)) |

{style=&quot;table-layout:auto&quot;}

&#42; 仅当Workfront管理员将桌面校样查看器配置为所有校样的默认查看器时，此功能才起作用。

## 视频校样

| **功能**  | **Web校对查看器** | **桌面校对查看器** |
|---|---|---|
| 打开视频校样 | ✓ | ✓&#42; |
| 缓冲 | ✓ | ✓&#42; |
| 使用时间进行审阅 | ✓ | ✓&#42; |
| 使用帧或时间码查看 | ✓ | ✓&#42; |
| 更快或更慢地查看 | ✓ | ✓&#42; |
| 音量调节 | ✓ | ✓&#42;  |
| 全屏模式 | ✓ | ✓&#42;  |
| 范围注释 | ✓ | ✓&#42;  |
| 循环视频校样（视频完成并自动开始） | ✓ | ✓&#42;  |
| 高级视频快捷键 | ✓(有关更多信息，请参阅 [校对查看器中的键盘快捷键](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/keyboard-shortcuts-proof.md)) | ✓&#42;  |

{style=&quot;table-layout:auto&quot;}

&#42; 仅当桌面校样查看器配置为所有校样的默认查看器时，此功能才起作用。

## 交互式校样

| **功能**  | **Web校对查看器** | **桌面校对查看器** |
|---|---|---|
| 打开根据ZIP文件中捆绑的内容创建的交互式校样 | ✓ | ✓（推荐） |
| 打开从URL创建的交互式校样 | 不支持 | ✓ |
| 以各种屏幕大小查看交互式校样（根据ZIP文件中捆绑的内容创建） | ✓ | ✓ |
| 查看各种设备的交互式校样（根据ZIP文件中捆绑的内容创建） | 不支持 | ✓ |
| 查看不安全的(HTTP)站点 | 不支持 | ✓ |
| 查看受iFrame保护的站点（iFrame中不能查看的站点） | 不支持 | ✓ |

{style=&quot;table-layout:auto&quot;}

## 注释

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>功能</th> 
   <th>Web校对查看器 </th> 
   <th>桌面校对查看器 </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>添加、删除和编辑注释</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>添加和删除回复</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>矩形、箭头、折线图、手绘和高亮标记工具</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>折线工具</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>裁剪蒙版标记工具</p> </td> 
   <td>不支持</td> 
   <td>不支持</td> 
  </tr> 
  <tr> 
   <td> <p>文本选择标记工具</p> </td> 
   <td>✓仅静态校样</td> 
   <td>✓仅静态校样</td> 
  </tr> 
  <tr> 
   <td> <p>更改标记颜色</p> </td> 
   <td>✓（32种可用颜色） </td> 
   <td>✓（32种可用颜色） </td> 
  </tr> 
  <tr> 
   <td> <p>更改标记不透明度</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>更改标记厚度</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>剪切、复制和粘贴标记</p> </td> 
   <td> 不支持</td> 
   <td> 不支持</td> 
  </tr> 
  <tr> 
   <td> <p>撤消和重做上次操作</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>复制标记</p> </td> 
   <td> 不支持</td> 
   <td> 不支持</td> 
  </tr> 
  <tr> 
   <td>将操作设置为注释</td> 
   <td>✓（在设置操作后，注释中会立即显示操作）</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>将标记颜色设置为默认颜色</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>解决注释</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>锁定注释</p> </td> 
   <td>不支持</td> 
   <td> 不支持</td> 
  </tr> 
  <tr> 
   <td> <p>标记用户</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>恢复注释</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>在紧凑视图中查看注释列表</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>在标准、完整或单个视图中查看评论列表</p> </td> 
   <td>计划在将来</td> 
   <td>计划在将来</td> 
  </tr> 
  <tr> 
   <td> <p>搜索评论</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>按用户筛选评论</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>按用户筛选评论和回复</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>对评论排序</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>注释自动更新</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## 决策

| 功能 | Web校对查看器 | 桌面校对查看器 |
|---|---|---|
| 做出决策 | ✓ | ✓ |
| 自定义决策 | ✓ | ✓ |

{style=&quot;table-layout:auto&quot;}

## 比较证据

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>功能</th> 
   <th>Web校对查看器 </th> 
   <th>桌面校对查看器 </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>比较不同版本的校样</td> 
   <td>✓</td> 
   <td>✓<br></td> 
  </tr> 
  <tr> 
   <td>比较单独的校样</td> 
   <td> ✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
 </tbody> 
</table>

## 校样操作

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>功能</th> 
   <th>Web校对查看器 </th> 
   <th>桌面校对查看器 </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>更改校样版本 </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td>创建新版本</td> 
   <td> <p>仅在Workfront Proof中可用(计划在将来在Workfront中进行校样)<br></p> </td> 
   <td>仅在Workfront Proof中可用(计划在将来在Workfront中进行校样)</td> 
  </tr> 
  <tr> 
   <td>查看校样详细信息 </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>审阅校样工作流</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>编辑工作流阶段</td> 
   <td>不支持</td> 
   <td>不支持</td> 
  </tr> 
  <tr> 
   <td>共享校样</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>获取团队URL</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>更改电子邮件通知</td> 
   <td>✓ </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>下载原始文件</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>锁定和解锁校样和阶段</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>打印校样摘要</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>删除校样</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>从同一文件夹管理校样</td> 
   <td><strong>仅在Workfront校样中可用</strong> </td> 
   <td><strong>仅在Workfront校样中可用</strong> </td> 
  </tr> 
  <tr> 
   <td>品牌（自定义徽标）</td> 
   <td>✓</td> 
   <td> ✓<br>(Workfront Logo on launch页面) </td> 
  </tr> 
  <tr> 
   <td>自定义链接(仅限Workfront校样)</td> 
   <td>不支持</td> 
   <td> 不支持 </td> 
  </tr> 
  <tr> 
   <td>Basecamp集成(仅限Workfront Proof) </td> 
   <td>计划将来</td> 
   <td>计划将来</td> 
  </tr> 
  <tr> 
   <td>存在指示器 </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>校样自动更新（权限更改和新版本）</td> 
   <td>✓</td> 
   <td>✓ </td> 
  </tr> 
 </tbody> 
</table>

## 微型查看器

| **功能**  | **Web校对查看器**  | **桌面校对查看器** |
|---|---|---|
| 嵌入代码 | 计划将来进行静态和本机视频校样 | 不支持  |

{style=&quot;table-layout:auto&quot;}

## 翻译

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>功能</strong> </th> 
   <th><strong>Web校对查看器</strong> </th> 
   <th><strong>桌面校对查看器</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>英语以外的支持语言</td> 
   <td>✓</td> 
   <td>✓<br></td> 
  </tr> 
 </tbody> 
</table>
