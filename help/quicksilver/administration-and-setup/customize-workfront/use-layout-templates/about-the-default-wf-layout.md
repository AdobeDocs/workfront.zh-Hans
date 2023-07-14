---
title: 关于默认Adobe Workfront布局
user-type: administrator
content-type: reference;overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: 默认布局是Adobe Workfront管理员使用布局模板进行任何更改之前的主菜单、左侧面板以及视图、分组和筛选器的排列。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: a68bca5e-1cec-432d-bb38-14b426a9c051
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 14%

---

# 关于默认Adobe Workfront布局

默认布局是主菜单的排列 ![](assets/main-menu-icon.png)，以及Adobe Workfront管理员使用布局模板进行任何更改之前的视图、分组和筛选器。

有关Workfront管理员如何通过为用户分配布局模板来修改用户默认布局的信息，请参阅 [将用户分配给布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

>[!NOTE]
>
>用户可以通过编辑其用户配置文件首选项来更改自己的布局。 欲了解更多信息，请参见 [首选项](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md#preferences) 中的部分 [配置我的设置](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

## 每个访问级别的默认布局

每个用户的默认布局取决于其访问级别。 某些用户可能无法看到主菜单中的某些区域或某些左侧面板项目，具体取决于分配给他们的访问级别。

下表显示了默认情况下，每个访问级别显示的左侧面板项目。 还指示了每个访问级别的默认登陆区域：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>区域</th> 
   <th> 左侧面板项目 </th> 
   <th> <p>系统管理员</p> </th> 
   <th> <p>计划人</p> </th> 
   <th>员工</th> 
   <th>查看者</th> 
   <th>请求人</th> 
   <th>外部用户</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td rowspan="2"><strong>项目</strong> </td> 
   <td><strong>项目</strong> </td> 
   <td>✔ <br>（默认登陆区域）</td> 
   <td><span style="font-weight: 400;"> ✔</span> <br>（默认登陆区域）</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>项目组合</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="3"><strong>报告</strong> </td> 
   <td><strong>报告</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>仪表板</strong> </p> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>日历</strong> </td> 
   <td>✔ </td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="5"><strong>人员</strong> (已重命名为 <strong>团队</strong> （适用于拥有工作许可证的用户）</td> 
   <td><strong>团队</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>人员</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> <!--
   <tr> 
    <td><strong>Legacy Resource Planning</strong> </td> 
    <td>✔ </td> 
    <td>✔ </td> 
    <td>&nbsp;</td> 
    <td>&nbsp;</td> 
    <td>&nbsp;</td> 
    <td>&nbsp;</td> 
   </tr>
  --> 
  <tr> 
   <td><strong>计划</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>正在调度</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="3"><strong>请求</strong> </td> 
   <td><strong>新建请求</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td><strong>我已提交的请求</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ <br>（默认登陆区域）</td> 
   <td>✔ <br>（默认登陆区域）</td> 
  </tr> 
  <tr> 
   <td><strong>所有请求</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td rowspan="3"><strong>时间表</strong> </td> 
   <td><strong>我的工时表</strong> </td> 
   <td>✔ </td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>我审批的工时表</strong> </td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>所有时间表</strong> </td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>文档</strong> </td> 
   <td> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>设置</strong> </td> 
   <td> </td> 
   <td>✔ </td> 
   <td>功能有限</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
