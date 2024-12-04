---
title: 关于默认Adobe Workfront布局
user-type: administrator
content-type: reference;overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: 默认布局是主菜单、左侧面板以及视图、分组和筛选器的排列，Adobe Workfront管理员随后使用布局模板进行任何更改。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: a68bca5e-1cec-432d-bb38-14b426a9c051
source-git-commit: 52877ab16210699019c82e709f288b5f98e7d811
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 9%

---

# 关于默认Adobe Workfront布局

默认布局是主菜单![](assets/main-menu-icon.png)或主菜单![](assets/lines-main-menu.png)（如果可用）、左侧面板、视图、分组和筛选器的布局，Adobe Workfront管理员使用布局模板进行任何更改。

有关Workfront管理员如何通过为用户分配布局模板来修改用户默认布局的信息，请参阅[将用户分配给布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)。

>[!NOTE]
>
>用户可以通过编辑用户配置文件首选项来更改自己的布局。 有关详细信息，请参阅[配置我的设置](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md)中的[首选项](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md#preferences)部分。

## 每种许可证类型的默认主菜单项

每个用户的默认布局取决于其许可证类型。 某些用户可能无法看到主菜单中的某些区域或某些左侧面板项目，具体取决于分配给他们的许可证类型。

您的组织可能分配两种类型的许可证：

* 新许可证
* 当前许可证

<!--rename the above if we change Current to Legacy-->

有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

### 当前许可证类型的默认主菜单

下表显示了默认的主菜单项以及每个当前许可证类型所显示的左面板项：

<table class="tg"><thead>
  <tr>
    <th class="tg-0lax"><span style="font-weight:bold">面积</span></th>
    <th class="tg-0lax"><span style="font-weight:bold">左侧面板项目</span></th>
    <th class="tg-0lax"><span style="font-weight:bold">系统管理员</span></th>
    <th class="tg-0lax"><span style="font-weight:bold">规划器</span></th>
    <th class="tg-0lax"><span style="font-weight:bold">员工</span></th>
    <th class="tg-1wig">审阅者</th>
    <th class="tg-1wig">请求人</th>
    <th class="tg-1wig">外部用户</th>
  </tr></thead>
<tbody>
  <tr>
    <td class="tg-0lax">主页</td>
    <td class="tg-0lax">主页<br>优先级</td>
    <td class="tg-0lax">✔（默认登陆页面）</td>
    <td class="tg-0lax">✔（默认登陆页面）</td>
    <td class="tg-0lax">✔（默认登陆页面）</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">项目</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔ </td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">项目组合</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">项目群</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">报告</td>
    <td class="tg-0lax">我的报告<br>与我共享<br>所有报告</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔（与我共享以及左侧面板中的所有报表）</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔（与我共享以及左侧面板中的所有报表）</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">仪表板</td>
    <td class="tg-0lax">我的仪表板<br>共享仪表板<br>所有仪表板<br>画布仪表板*</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">日程表</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">资源</td>
    <td class="tg-0lax">规划者<br>工作负载均衡器<br>利用率<br>资源池</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔（左侧面板中的“规划者和资源池”）</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">团队</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">用户</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">请求</td>
    <td class="tg-0lax">已提交<br>草稿</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">时间表</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">文档</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">模板</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">分析</td>
    <td class="tg-0lax">工作<br>人员</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">方案</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">展示板</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">Blueprint</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔（安装功能）</td>
    <td class="tg-0lax">✔（仅限请求功能）</td>
    <td class="tg-0lax">✔（仅限请求功能）</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">优先次序</td>
    <td class="tg-0lax">主页<br>优先级</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔<br></td>
  </tr>
  <tr>
    <td class="tg-0lax">设置</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔（功能有限）</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">我的更新</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔（默认登陆页面）</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
  </tr>

</tbody></table>

*您必须注册画布功能板测试版才能查看此区域。 有关详细信息，请参阅[画布功能板测试版信息](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md)。

### 新许可证类型的默认主菜单

下表显示了默认的主菜单项以及针对每种新许可证类型显示的左面板项：

<table class="tg"><thead>
  <tr>
    <th class="tg-fymr">面积</th>
    <th class="tg-fymr">左侧面板项目</th>
    <th class="tg-fymr">系统管理员</th>
    <th class="tg-fymr">标准</th>
    <th class="tg-fymr">轻量</th>
    <th class="tg-fymr">投稿人</th>
    <th class="tg-fymr">外部用户</th>
  </tr></thead>
<tbody>
  <tr>
    <td class="tg-0pky">主页</td>
    <td class="tg-0pky">主页<br>优先级</td>
    <td class="tg-0pky">✔（默认登陆页面）</td>
    <td class="tg-0pky">✔（默认登陆页面）</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔（默认登陆页面）</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">项目</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔ </td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">项目组合</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">项目群</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">报告</td>
    <td class="tg-0pky">我的报告<br>与我共享<br>所有报告</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔（与我共享以及左侧面板中的所有报表）</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">仪表板</td>
    <td class="tg-0pky">我的仪表板<br>共享仪表板<br>所有仪表板<br>画布仪表板*</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">日程表</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">资源</td>
    <td class="tg-0pky">规划者<br>工作负载均衡器<br>利用率<br>资源池</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">团队</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">用户</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">请求</td>
    <td class="tg-0pky">已提交<br>草稿</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">时间表</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">文档</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">模板</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">分析</td>
    <td class="tg-0pky">工作<br>人员</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">方案</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">展示板</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">Blueprint</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔（安装功能）</td>
    <td class="tg-0pky">✔（仅限请求功能）</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">优先次序</td>
    <td class="tg-0pky">主页<br>优先级</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔<br></td>
  </tr>
  <tr>
    <td class="tg-0pky">设置</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔（功能有限）</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">我的更新</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔（默认登陆页面）</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
  </tr>
</tbody></table>

*您必须注册画布功能板测试版才能查看此区域。 有关详细信息，请参阅[画布功能板测试版信息](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md)。

<!--

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
   <th>Area</th> 
   <th> Left panel items </th> 
   <th> System Administrator</th> 
   <th> Planner </th> 
   <th>Worker</th> 
   <th>Reviewer</th> 
   <th>Requestor</th> 
   <th>External User</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td rowspan="2"><strong>Projects</strong> </td> 
   <td><strong>Projects</strong> </td> 
   <td>✔ <br>(Default landing area)</td> 
   <td><span style="font-weight: 400;"> ✔</span> <br>(Default landing area)</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>Portfolios</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td rowspan="3"><strong>Reporting</strong> </td> 
   <td><strong>Reports</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p><strong>Dashboards</strong> </p> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>Calendars</strong> </td> 
   <td>✔ </td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td rowspan="5"><strong>People</strong> (renamed to <strong>Teams</strong> for users with a Work license)</td> 
   <td><strong>Teams</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>People</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>Planning</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>Scheduling</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td rowspan="3"><strong>Requests</strong> </td> 
   <td>New Request </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td><strong>Requests I've Submitted</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ <br>(Default landing area)</td> 
   <td>✔ <br>(Default landing area)</td> 
  </tr> 
  <tr> 
   <td><strong>All Requests</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td rowspan="3"><strong>Timesheet</strong> </td> 
   <td><strong>My Timesheets</strong> </td> 
   <td>✔ </td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>Timesheets I Approve</strong> </td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>All Timesheets</strong> </td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>Documents</strong> </td> 
   <td>&nbsp;</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>Setup</strong> </td> 
   <td>&nbsp;</td> 
   <td>✔ </td> 
   <td>Limited Functionality</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
 </tbody> 
</table>
-->