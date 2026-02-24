---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: 创建项目摄取Forms
description: 您可以使用项目引入表单来简化在Workfront中创建项目的过程
author: Becky
feature: Work Management, Requests
role: User, Admin
hide: true
hidefromtoc: true
source-git-commit: 5ff71313c550d949079e7426b657a0a4e19a656c
workflow-type: tm+mt
source-wordcount: '1329'
ht-degree: 2%

---

# 创建项目接收表单

<span class="preview">此页面上的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

项目接收表单是一种允许用户请求项目的请求表单。 项目是从表单创建的，无需从已提交的问题创建项目。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>“任一” </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>新许可证： Standard </p>
   或
   <p>当前许可证：计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员才能创建项目接收表单。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">其他产品</td> 
   <td> <p>贵组织必须已购买Workfront Planning才能使用Planning功能，例如自动化。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 项目摄取Forms的功能和限制

### 功能

项目接收表单包括以下功能：

#### Workfront规划自动化

Workfront项目接收表单支持Workfront规划自动化，以配置所创建的特定于项目的属性。

有关Planning自动化的详细信息，请参阅[配置Adobe Workfront Planning自动化](/help/quicksilver/planning/records/configure-automations-to-create-records.md)。

### 审批配置

项目接收表单包括配置已提交请求的批准者的功能。

### 限制

#### 支持的字段类型

项目录取Forms可以包含具有项目对象类型的任何自定义表单中的字段。

项目录取Forms中当前不支持以下字段类型：

* 部分
* 公式
* 汇总
* 单行汇总
* 规划连接
* 引用了只读项目本机字段的本机字段引用（例如，`workRequiredExpression`）

#### 请求体验

项目接收表单只能用于新的请求体验。

有关新请求体验的信息，请参阅[创建并提交请求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)。

#### 共享

项目接收表单不支持公开共享。 共享选项包括：

* **任何人**：系统中的任何人都可以使用表单提交项目请求。
* **指定的用户**：您可以选择哪些特定用户有权访问项目请求表单。

## 创建项目接收表单

{{step1-to-requests}}

1. 启用屏幕右上角的&#x200B;**切换到新体验**&#x200B;设置。
1. 单击屏幕右上角的&#x200B;**请求表单**。

   >[!NOTE]
   >
   >由于只有Workfront管理员可以创建接收表单，因此“请求表单”按钮仅对管理员可见。

   此时将显示当前可用的请求表单列表。 这包括Workfront Planning的申请表。

1. 单击屏幕右上角的&#x200B;**新建请求表单**。
1. 输入申请表单的名称。 默认情况下，表单的名称为&#x200B;**无标题表单**。
1. 选择下拉列表顶部附近的对象类型&#x200B;**项目**。 目前，这是唯一可用的Workfront项目类型。 列表中的其他项目属于Workfront Planning。
1. （可选）为请求表单添加&#x200B;**描述**。
1. 单击&#x200B;**创建**。此时将在“表单”选项卡中打开选定记录类型的请求表单。

   此时将打开项目接收表单生成器，以显示表单选项卡。

   默认情况下，引入表单包含以下信息：

   * **默认的分区**：这是Workfront应用于请求表单的默认分区界限。 所有记录字段都显示在&#x200B;**默认部分**&#x200B;区域。
   * **主题**&#x200B;字段：将在Workfront中标识该请求的字段。 “主题”字段的配置和值不可编辑。
   * 与项目关联的所有字段。

     提交项目请求的每个人均可看到请求表单中包含的字段。

1. 要将字段添加到表单，请单击左侧导航中的字段类型，然后选择该字段。
1. （可选）要删除字段，请将鼠标悬停在要删除的表单上的字段上，然后单击&#x200B;**x**&#x200B;图标以将其删除。
1. （可选）要从表单中删除&#x200B;**默认节**，请执行以下操作：

   1. 从“默认部分”中删除所有字段。
   1. 单击&#x200B;**内容元素**&#x200B;选项卡并添加新分区，然后添加该分区的名称。
   1. 向新部分添加字段。
   1. 单击&#x200B;**x**&#x200B;图标可删除&#x200B;**默认部分**。
1. 单击任意字段，然后使用表单右侧面板中的控件定义其大小或以下任何信息：

   * **标签**：这是显示在请求表单中的字段名称。 这不会更改记录字段的名称。
   * **说明**：添加有关该字段的更多信息。
   * **生成必填字段**：选定后，该字段必须具有值。 否则，无法提交表单。
   * **添加逻辑**：定义必须满足哪些条件才能显示或隐藏字段。

   >[!TIP]
   >
   >   选择表单上的字段后，每个字段的字段类型都会显示在右侧面板的顶部。
   >     

1. （可选）单击表单左侧的&#x200B;**内容元素**&#x200B;选项卡，然后添加以下任意元素：

   * **描述性文本**
   * **分区界限**

   有关生成自定义表单的详细信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

1. 单击表单左侧的&#x200B;**自动化**&#x200B;选项卡，然后执行以下任一操作：

   * 选择项目模板
   * 附加任何自定义表单
   * 设置项目所有者
   * 将项目添加到项目组合或项目群

   您在此处所做的任何选择都将应用于从此引入表单创建的项目。

1. （可选）单击&#x200B;**预览**&#x200B;以查看当其他用户使用表单提交新记录时，该表单将如何显示给其他用户。

1. （可选）单击&#x200B;**配置**&#x200B;选项卡，然后向&#x200B;**审批者**&#x200B;字段添加至少一个用户或团队&lt;，以审批此接收表单的新请求。

   * 将摄取表单与批准者关联时，任何新请求都必须首先由所有批准者批准，然后才能生成项目。
   * 您可以将一个或多个批准者添加到引入表单。
   * 如果至少有一位审批者拒绝了请求，则该请求会被拒绝，并且不会创建项目。
   * 在批准或拒绝项目之前，所有批准者都必须做出决定。
   * 如果将团队设置为批准者，则只需从团队中做出一个决策。

     有关将审批添加到请求表单的详细信息，请参阅[将审批添加到请求表单](/help/quicksilver/planning/requests/add-approval-to-request-form.md)。

1. （可选）单击标题中表单名称右侧的&#x200B;**更多**&#x200B;菜单![更多菜单](assets/more-menu.png)，然后单击&#x200B;**编辑**&#x200B;以更新表单名称。

1. 单击&#x200B;**发布**&#x200B;发布表单并获取其唯一链接。

   出现以下情况：

   * **发布**&#x200B;按钮已删除。
   * **取消发布**&#x200B;按钮已添加到表单中。 单击此按钮将阻止访问表单。
   * **共享**&#x200B;按钮已添加到表单。
   * 该表单将在Workfront主菜单的请求区域中可用。

1. 单击&#x200B;**共享**&#x200B;以与他人共享表单。
1. 单击标题中表单名称左侧的向左箭头以关闭表单。

   将打开&#x200B;**请求表单**&#x200B;表格视图，并将表单添加到其中。

1. （可选）将鼠标悬停在表视图中请求表单的名称上，然后单击表单名称右侧的&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，然后单击以下任一项：

   * **编辑表单**：单击此项可进一步编辑表单上的信息。
   * **取消发布**：单击此项可取消发布将表单从Workfront的“请求”区域删除的表单。
   * **共享**：单击此项可修改谁有权访问该表单。
   * **复制链接**：单击此项可快速复制请求表单的链接，而无需打开表单。
   * **删除**：单击此项可删除表单。 使用该表单添加的所有请求和记录都不会被删除。 无法恢复表单。

   >[!NOTE]
   >
   >您可以在表格视图中标识项目引入表单，因为它们在“对象类型”列中显示“项目”。

1. 单击标题中&#x200B;**请求表单**&#x200B;左侧的左箭头以关闭请求表单表。

