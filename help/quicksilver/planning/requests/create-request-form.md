---
title: 在Adobe Workfront Planning中创建和管理申请表单
description: 在Adobe Workfront Planning区域中选择记录类型后，您可以创建请求表单并将其与该记录类型关联。 然后，您可以与其他内部或外部用户共享指向该页面的链接。 具有表单链接的用户可以填写表单上的字段值，通过提交表单，他们可以为与表单关联的记录类型添加新记录。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 49f25b03-90bb-4317-9e48-289fd61df791
source-git-commit: 9629558bfc2c4fa7fb040bcc45534164e0d8b3b4
workflow-type: tm+mt
source-wordcount: '1367'
ht-degree: 2%

---

# 在Adobe Workfront Planning中创建和管理申请表单

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

您可以创建请求表单，并将其与Adobe Workfront Planning中的记录类型相关联。 然后，您可以与其他内部或外部用户共享指向该页面的链接。

具有表单链接的用户可以更新表单上的字段值，并通过提交来添加新记录。

本文介绍了工作区管理员如何创建与记录类型关联的请求表单。

有关向记录类型提交请求以创建记录的信息，请参阅[提交Adobe Workfront Planning请求以创建记录](/help/quicksilver/planning/requests/submit-requests.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 产品</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront规划<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront计划*</p></td>
   <td>
<p>以下任意Workfront计划：</p>
<ul><li>选择</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning不适用于旧版Workfront计划</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront规划包*</p></td>
   <td>
<p>任何 </p>  
<p>有关每个Workfront计划中包括的内容的更多信息，请联系您的Workfront客户经理。 </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront平台</p></td>
   <td>
<p>贵组织的Workfront实例必须载入AdobeUnified Experience，才能访问Workfront Planning的所有功能。</p>
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">AdobeWorkfront的Unified Experience</a>。 </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td>
   <td>
   <p>标准</p>
   <p>Workfront计划不适用于旧版Workfront许可证</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>访问级别配置</p></td>
   <td> <p>Adobe Workfront Planning没有访问级别控制</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>对象权限</p></td>
   <td>
   <ul>
   <li><p>管理工作区的权限</p></li>
    <li><p>系统管理员可以管理他们未创建的工作区。 </p></li>
    </ul>
   <p>有关共享Workfront Planning对象权限的信息，请参阅  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">在Adobe Workfront Planning中共享权限概述</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>必须为所有用户(包括Workfront管理员)分配一个布局模板，该模板应包括主菜单中的Planning区域。 </p>  
</td>
  </tr>
 </tbody>
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 为记录类型创建请求表单

{{step1-to-planning}}

1. 单击要在其中添加记录的工作区。

   工作区将打开，记录类型显示为卡片。

1. 单击记录类型卡片。 有关创建记录类型的信息，请参阅[创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)。

   记录类型页面将在您上次访问的视图中打开。 默认情况下，将在表格视图中打开记录类型页面。

1. 单击页眉中记录类型名称右侧的&#x200B;**更多**&#x200B;菜单![](assets/more-menu.png)，然后单击&#x200B;**创建请求表单**。
1. 更新请求表单的名称。 默认情况下，表单的名称为&#x200B;**无标题的请求表单**。<!--check this; you logged a bug to rename it to this but was it fixed?-->
1. （可选）为请求表单添加&#x200B;**描述**。

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. 单击&#x200B;**创建**。此时将打开所选记录类型的请求表单。

   ![](assets/campaigns-request-form-edit-mode.png)

   默认情况下，请求表单包含以下信息：

   * 所选记录类型的表视图中可用的记录字段。<!--they are working on removing the limitation below-->

   >[!IMPORTANT]
   >
   > 根据创建请求表单时所用的环境，存在以下情况：
   >
   >* 以下类型的字段未显示在预览</span>或生产环境的请求表单<span class="preview">中：
   >
   >    * 人员（包括“创建者”和“上次修改者”）
   >    * 公式
   >    * 创建日期
   >    * 上次修改日期
   >    * Workfront对象的已连接字段或查找字段
   >    * Workfront Planning记录的已连接查找字段
   >* 以下类型的字段不会显示在生产环境的请求表单中。 <span class="preview">它们显示在预览环境中：</span>
   >    * <span class="preview"> Workfront Planning记录&#39;连接的字段</span>


   * **默认的分区**：这是Workfront应用于请求表单的默认分区界限。 无法重命名或删除默认部分。
   * **主题**&#x200B;字段：将在Workfront中标识该请求的字段。 此功能尚不可用。 “主题”字段的配置和值不可编辑。
   * 与记录类型关联的所有字段。

     向此记录类型提交请求的每个人均可看到请求表单中包含的字段。

1. （可选）将鼠标悬停在要删除的表单上的任何字段上，然后单击&#x200B;**x**&#x200B;图标以删除它们。 它们已添加到表单左侧的&#x200B;**字段**&#x200B;选项卡中。

   例如，删除&#x200B;**主题**&#x200B;字段，因为此字段在Workfront Planning中不可见。<!--remove this step when we connect intake with the Requests area in Workfront-->
1. 单击任意字段，然后使用表单右侧面板中的控件定义其大小或以下任何信息：

   * **标签**：这是显示在请求表单中的字段名称。 这不会更改记录字段的名称。
   * **说明**：添加有关该字段的更多信息。
   * **生成必填字段**：选定后，该字段必须具有值。 否则，无法提交表单。
   * **添加逻辑**：定义必须满足哪些条件才能显示或隐藏字段。

   >[!NOTE]
   >
   >   选择表单上的字段后，每个字段的字段类型都会显示在右侧面板的顶部。
   >   
   >
   >   “货币”、“数字”和“百分比”字段显示为“单行”文本字段类型。 但是，字段格式将保留，并且这些字段中的值将显示为货币、数字和百分比值。

1. （可选）单击表单左侧的&#x200B;**内容元素**&#x200B;选项卡，然后添加以下任意元素：

   * **描述性文本**
   * **分节符**

   有关生成自定义表单的详细信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

1. （可选）单击&#x200B;**预览**&#x200B;以查看当其他用户使用表单提交新记录时，该表单将如何显示给其他用户。
1. （可选）单击标题中表单名称右侧的&#x200B;**更多**&#x200B;菜单![](assets/more-menu.png)，然后单击&#x200B;**编辑**&#x200B;以更新表单名称。
1. 单击&#x200B;**Publish**&#x200B;发布表单并获取其唯一链接。

   出现以下情况：

   * 已删除&#x200B;**Publish**&#x200B;按钮。
   * **取消发布**&#x200B;按钮已添加到表单中。 单击此按钮将阻止访问表单。
   * **共享**&#x200B;按钮已添加到表单。

1. 单击&#x200B;**共享**&#x200B;以与他人共享表单。

   ![](assets/share-box-for-request-form.png)

1. 从以下选项中进行选择，以指示哪些类型的用户可以访问此表单：

   * 任何对工作区具有查看或更高访问权限的人员
   * 任何对工作区具有贡献或更高访问权限的人员
   * 任何知道链接的人

   >[!WARNING]
   >
   >
   >当您选择&#x200B;**具有链接**&#x200B;的任何人时，任何人都可以访问表单并提交新记录，甚至包括您组织外没有Workfront帐户的人员。

1. （视情况而定）如果您在上一步中选择了&#x200B;**具有链接**&#x200B;的任何人，请从可用日历中选择&#x200B;**链接到期日期**。 链接过期后，用户会收到错误消息，您必须更新链接日期，然后才能再次访问表单。

   您可以选择自当前日期起180天内的将来日期。

1. 单击&#x200B;**保存并复制链接**&#x200B;以保存表单的共享详细信息。

   表单共享选项已保存，并且链接已复制到您的剪贴板。 您现在可以与其他人共享。

   有关使用请求表单链接创建记录的信息，请参阅[提交Adobe Workfront Planning请求](/help/quicksilver/planning/requests/submit-requests.md)。

1. 单击屏幕右下角的&#x200B;**保存**&#x200B;以保存表单。
1. 单击标题中表单名称左侧的向左箭头以关闭表单。

   此时将打开记录类型页面。
1. （可选）单击标题中记录类型名称右侧的&#x200B;**更多**&#x200B;菜单![](assets/more-menu.png)，然后执行以下操作之一：
   * 单击&#x200B;**更新请求表单**&#x200B;以更改请求表单。
   * 单击&#x200B;**复制请求表单的链接**&#x200B;以与其他人共享该表单的链接。

   >[!TIP]
   >
   >在这种情况下，会显示链接已公开共享。
   >![](assets/publicly-shared-link-to-form-on-record-type-menu-highlighted.png)
