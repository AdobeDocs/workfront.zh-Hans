---
content-type: api
navigation-topic: api-navigation-topic
title: API响应中的转义字符
description: API响应中的转义字符
author: Becky
feature: Workfront API
exl-id: 1477b98e-1cdc-4661-b3ee-0b6ab1e8c3ee
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 8%

---

# API响应中的转义字符

某些API响应的语法可能包含转义字符、 `\` （反斜线）。 转义字符表示紧靠转义字符后面的字符或字符串具有特殊值。 例如， `\t` 告诉阅读设备 `t` 应解释为 `tab` 而不是字母&quot;t&quot; 反斜线后面包含一个或多个字符的字符串称为转义序列。

十六进制转义序列需要使用有效的十六进制数字。 下表列出了在Adobe Workfront API响应中编码的转义序列：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>转义序列</strong> </th> 
   <th><strong>Unicode字符</strong> </th> 
   <th><strong>表示</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>\u000<em>x</em></p> <p>其中， <em>x</em> 是十六进制代码，表示数字0到7</p> </td> 
   <td>0-7</td> 
   <td>由代码点0到7表示的Unicode字符</td> 
  </tr> 
  <tr> 
   <td>\b</td> 
   <td>8</td> 
   <td>使用退格符</td> 
  </tr> 
  <tr> 
   <td>\t</td> 
   <td>9</td> 
   <td>选项卡</td> 
  </tr> 
  <tr> 
   <td>\n</td> 
   <td>10</td> 
   <td>新行</td> 
  </tr> 
  <tr> 
   <td>\u000b</td> 
   <td>11</td> 
   <td>垂直选项卡</td> 
  </tr> 
  <tr> 
   <td>\f</td> 
   <td>12</td> 
   <td>表单馈送</td> 
  </tr> 
  <tr> 
   <td>\r</td> 
   <td>13</td> 
   <td>回车符</td> 
  </tr> 
  <tr> 
   <td> <p>\u00<em>xx</em></p> <p><em>其中，xx是以14到31为单位的十六进制代码</em> </p> </td> 
   <td>14 - 31</td> 
   <td>由代码点14到31表示的Unicode字符</td> 
  </tr> 
  <tr> 
   <td> <p>\/</p> </td> 
   <td>47</td> 
   <td>/（正斜杠）</td> 
  </tr> 
  <tr> 
   <td> <p>\u003c</p> </td> 
   <td>60</td> 
   <td>&lt;（小于）</td> 
  </tr> 
  <tr> 
   <td> <p>\\</p> </td> 
   <td>92</td> 
   <td>\（反斜杠）</td> 
  </tr> 
  <tr> 
   <td> <p>\u<em>xxxx</em></p> <p>其中， <em>xxxx</em> 是任何大于127的十六进制代码</p> </td> 
   <td>128+</td> 
   <td>超过127的任何代码的Unicode字符</td> 
  </tr> 
 </tbody> 
</table>
