---
title: 配置记录类型业务规则
description: 您可以配置记录类型业务规则，以根据字段值对记录强制执行某些操作。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: a0ba955b089480c01b187e39ed5a8a8226b23ea7
workflow-type: tm+mt
source-wordcount: '1164'
ht-degree: 1%

---


# 配置记录类型业务规则

{{planning-important-intro}}

<span class="preview">此页面上的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在发布到“预览”版之后，启用了“快速发布”的客户的生产环境中每月还会提供相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

您可以为Adobe Workfront Planning记录类型配置业务规则，以指示在允许或阻止对该类型的记录执行操作之前需要某些字段。

根据规则的制定方式，如果满足定义的业务规则，您可以允许对记录执行以下操作：

* 编辑或不编辑记录
* 删除或不删除记录

## 访问权限要求

+++ 展开以查看访问要求以执行本文中的步骤：  

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront 包</p></td> 
   <td> 
<ul> 
<li><p>带规划包的任何Workfront或工作流</p></li>
或
<li><p>作为独立产品购买时的任何Planning包</p></li></ul>
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p>工作流参与者或更高版本</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe计划许可证</p></td> 
   <td><p>规划标准</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td> <p>当您同时具有Workflow和Planning包时，必须将工作流和Planning许可证类型添加到访问级别</p>   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>   <p>管理对工作区和记录类型的权限</p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>  </td> 
  </tr>  
</tbody> 
</table>

有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 配置业务规则时的注意事项

* 业务规则将条件附加到字段更改或记录删除。 规则只有在经过审慎考虑的特定时刻才会生效：即字段即将更改为您在规则中配置的字段值时。

* 以纯语言显示的规则如下所示：“在编辑此记录之前，Campaign摘要字段必须具有值”。

  如果字段为空，将阻止记录编辑，并且用户将收到一条明确消息，说明在继续操作之前需要解决哪些问题。 更新必填字段并重试后，允许更改。

* 规则不会阻止记录创建。 用户仍可以创建记录，但必须确保必填字段不为空或包含指定值。
* 规则不会自动编辑或删除记录。 更改必须由用户自行决定并触发。
* 规则不会追溯应用：旧记录不会受到影响。 该规则检查仅在下次有人尝试编辑或删除记录时运行。
* 不能将业务规则添加到其主工作区或辅助工作区中的全局记录类型。
* 您可以为业务规则创建一个条件，该条件引用除以下字段类型之外的所有字段类型：
  * 公式字段
  * 查找字段
  * 引用字段
* 规则适用于可以编辑或删除记录的每个人。
* 记录类型可以有多个业务规则。 <!--Syuzanna is checking this because it should be just ONE rule per action: one per edit and one per delete - see this: https://workfront.slack.com/archives/C0BHWEUSJCU/p1788281638322049?thread_ts=1787924876.280359&cid=C0BHWEUSJCU; I also logged a bug for this because it released with more than one per action - https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/6a99add600001e9aa90435ec181dec3e/overview-->

  所有规则将同时检查在一起。<!-- I have asked Syuzanna and Norayr multiple times HOW are the rules run/ prioritized and I got no answers; when I know, I will update here-->

## 配置业务规则

1. 转到记录类型页面。
1. 从任何视图中，单击记录类型名称右侧的&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，然后单击&#x200B;**业务规则**。

   此时将打开“业务规则”表页。
1. 单击&#x200B;**新建业务规则**。
1. 在&#x200B;**新业务**&#x200B;规则框中，在第一个可用字段中添加该业务规则的名称。 这是必填字段
1. （可选）添加描述以定义业务规则，然后单击&#x200B;**保存**。

   随即会打开业务规则设置表单。

   ![业务规则设置表单](assets/business-rule-setup-form.png)

1. 在业务规则设置窗体的&#x200B;**If**&#x200B;部分中，根据特定规则选择要限制或允许的操作。 从以下内容中选择： <!--check UI text-->
   * **记录编辑**：如果满足此规则中定义的条件，将允许用户编辑或不编辑记录。
   * **记录删除**：如果满足此规则中定义的条件，将允许用户删除或不删除记录。
     <!--add screen shot when UI text is final-->
1. 在&#x200B;**公式字段**&#x200B;中添加业务规则。 从右侧面板的&#x200B;**公式表达式**&#x200B;部分中为规则选择一个运算符。

   例如，您可以从&#x200B;**Other**&#x200B;字段部分选择&#x200B;**IF**，或开始输入“IF”，然后在建议列表中显示时单击它。

   >[!TIP]
   >
   >为了保持规则的语法正确，建议从建议列表中选择字段和运算符。
1. 选择您要使其成为必填项的字段，以允许编辑或删除此记录类型的记录。

   例如，您可以键入以下语句，以使&#x200B;**促销活动摘要**&#x200B;字段为必填字段：

   ```
      IF(ISBLANK({Campaign summary}),"Campaign summary is a required field. You cannot edit this record without a value for the Campaign summary field.")
   ```

   >[!IMPORTANT]
   >
   >我们强烈建议您在规则公式中包含以下信息，以便用户轻松了解何时不允许他们尝试对记录执行的操作：
   >
   >* 为规则设置的确切字段。
   >* 不符合规则时的确切后果。

   当字段或表达式错误时，**公式**&#x200B;字段中有指示符。 <!--add screen shot?-->

   在业务规则的&#x200B;**Then**&#x200B;部分中，您可以查看规则的用途的说明。

1. 单击“激活”****&#x200B;以激活此记录类型的规则，然后单击“保存”****。

   规则在激活后立即应用，所有有权编辑或删除选定记录类型中记录的用户都必须遵循这些规则。
1. （可选）单击页眉中业务规则名称的&#x200B;**更多**&#x200B;菜单![](assets/more-menu.png)以打开&#x200B;**规则详细信息**&#x200B;框并更新有关该业务规则的信息。
1. （可选，推荐）单击页眉中&#x200B;**业务规则**&#x200B;左侧的返回箭头以显示记录类型页面，转到表视图或打开记录页面，然后尝试编辑或删除记录，以测试您刚刚创建的规则。

## 管理业务规则

您可以编辑、删除或停用现有业务规则。

编辑现有规则不会更改现有记录。 编辑后的规则仅适用于有人尝试编辑或删除现有记录时。

1. 返回记录类型的&#x200B;**业务规则**&#x200B;表页。
1. 在表格视图中查找要更改的规则。
1. 将鼠标悬停在活动规则的名称上，然后单击&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，然后单击以下选项之一：

   * **编辑**：这将打开业务规则设置页面，您可以编辑有关业务规则的信息。
   * **停用**：这将阻止触发规则，但会保留以备将来使用。
   * **删除**：已删除有关该规则的所有信息。 无法恢复已删除的规则。

   ![业务规则更多菜单已展开](assets/business-rule-more-menu-in-table-expanded.png)

   已编辑的规则或规则的停用仅适用于将来记录，不会追溯应用。
1. （可选且有条件）将鼠标悬停在表中已停用业务规则的名称上，然后单击&#x200B;**更多** > **激活**&#x200B;以激活该规则。

   规则已激活。




<!--

***********FROM CLAUDE - BELOW - MUST EDIT*******************


### What business rules actually do

Business rules attach a condition to a **status change**. Instead of enforcing complete data the moment someone creates a record (which would slow everyone down), the rule only kicks in at one specific, deliberate moment: when a status is about to change to a status you've configured.

A rule looks like this in plain language:

> "Before a record can move to **Ready for Execution**, the field **Brand** must have a value."

If the field is empty, the status change is blocked and the person gets a clear message telling them what to fix. Once they fill it in and try again, the change goes through.

A few important things this is *not*:

* **It doesn't block record creation.** People can still create a new record instantly and fill it in over time, exactly like today. 
* **It doesn't auto-fill anything or auto-change statuses.** A person always has to make the status change themselves.
* **It doesn't retroactively flag old records.** Records that are already sitting in the target status aren't affected — the check only runs the next time someone tries to move a record *into* that status.

### Step 1: Open the business rules configuration area

Business rules live alongside your other admin setup — you won't need to hunt for a separate "Planning" panel. From your workflow setup area:

1. Go to the main **workflow setup / admin configuration** area for your workspace.
2. Look for the **business rules** section for the record type you want to configure (for example, "Materials" or "Campaigns").


### Step 2: Choose the record type

Rules are configured per record type, so pick the one you want to add a rule to. For example, if you want to make sure every Materials record has key fields filled in before execution, select **Materials**.

### Step 3: Create a new rule

For each rule, you'll specify three things:

| What you set | Example |
|---|---|
| **Record type** | Materials |
| **Target status** | Ready for Execution |
| **Required field** | Brand |

In other words: "When a Materials record's status is changed to **Ready for Execution**, the field **Brand** must have a value."

You can add more than one rule for the same status. For example, you might require Brand, Therapeutic Area, Indication, and Estimated Launch Date all to be filled in before a record can move to "Ready for Execution" — each is its own rule, and all of them are checked together.

**What fields can you require?**

* Connected record fields (e.g., a linked Brand or Indication record) — the rule passes as soon as at least one record is linked.
* Standard text fields (single-line or paragraph) — the rule passes once there's any value.
* Date fields — the rule passes once a date is set.

**What you can't use yet:** formula fields and lookup fields aren't supported as rule targets in this release, since they're calculated in the background rather than filled in directly by a person.

### Step 4: Write the message people will see

When you create a rule, you'll also provide the message that shows up if someone tries to make the change without the field filled in. Keep it specific and actionable — something like:

> "Brand is required."

You don't need to worry about formatting a whole error banner — the system handles combining messages if multiple rules are violated at once (see below).

### Step 5: Save the rule

Once saved, the rule takes effect **immediately** for everyone in the workspace — no need to log out, refresh, or wait for a deployment. The very next time anyone tries to move a record into that status, the rule is checked.

### What your team will actually experience

Here's what changes for the people using Planning day to day, once a rule is live.

#### If a required field is empty

1. A planner opens a record and changes the status to the gated status (say, "Ready for Execution").
2. The system checks all rules tied to that status.
3. If a required field is empty, the change is **rejected** — the status reverts back to what it was.
4. A toast message appears, naming exactly which field(s) are missing:
   > *"Status change blocked: 'Brand' and 'Estimated Launch Date' must be populated before moving to 'Ready for Execution.'"*
5. The planner fills in the missing field(s) and tries the status change again.
6. This time, the rule passes, and the status updates normally.

#### If everything is already filled in

Nothing changes. The status updates instantly, with no extra steps or popups. Business rules are invisible until they're actually needed.

#### If several fields are missing at once

All the violated rules are checked together, and the message lists every missing field in one go — planners don't have to fix one field, try again, get told about the next one, and repeat.

### Step 6: Edit or remove a rule later

Rules aren't set in stone. To make changes:

1. Go back to the business rules configuration area for the record type.
2. Find the rule you want to change.
3. Edit the required field, target status, or message — or delete the rule entirely.
4. Save. The change applies immediately to future status changes.

Keep in mind: editing or deleting a rule **only affects transitions going forward.** Records that already made it into the target status before the change aren't reevaluated.
3## A few things worth knowing

* **This is separate from locking records after a status change.** Business rules (as described here) only check field completeness *before* a status change goes through. A different, related feature governs whether a record becomes fully locked from edits/deletion once it reaches a certain status — that's not what's covered here.
* **Bulk status changes** (changing status on many records at once) aren't fully defined yet for how they interact with business rules — if your team relies heavily on bulk actions, check with your Adobe contact on current behavior.
* **If a rule can't be evaluated** due to a system error, the transition is blocked rather than silently allowed through — you'll never end up with an incomplete record slipping past a rule because of a backend hiccup.
* **Turning the feature off** doesn't delete your configured rules — they're just paused. Turning it back on restores them exactly as they were, no reconfiguration needed.

### Quick reference: setting up your first rule

1. Confirm the feature is enabled for your tenant.
2. Go to workflow setup → business rules for your record type.
3. Choose the record type (e.g., Materials).
4. Create a rule: target status + required field.
5. Write a clear, specific error message.
6. Save — it's live immediately.
7. Repeat for each field you want to require.
8. Test it yourself: try changing a record's status with the field empty, confirm you see the expected message, fill in the field, and confirm the status change now goes through.

That's it — from here on, anyone converting a record forward will get a clear nudge if something's missing, instead of a downstream project quietly showing up incomplete.

-->