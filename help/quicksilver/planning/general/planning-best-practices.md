---
title: Adobe Workfront规划最佳实践
description: 作为营销运营负责人，您可以使用Adobe Workfront Planning为所有团队在营销生命周期中组织工作。 我们建议在开始Workfront规划时采用下面一些最佳实践。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 6e039b80-e3bf-412c-8c86-8f801f5861e3
source-git-commit: 0e37a5a519770d3d48192f1799491aa53a871508
workflow-type: tm+mt
source-wordcount: '3344'
ht-degree: 0%

---

<!--drafted because Kari Woolf will write something for Field Readiness instead, nothing for ExL, public-facing documentation-->

# Adobe Workfront规划最佳实践

<!-- add to TOC and mini TOC-->

{{planning-important-intro}}

作为营销运营负责人，您可以使用Adobe Workfront Planning为所有团队在营销生命周期中组织工作。

本文记录了在开始使用Workfront规划时我们建议的一些常见问题和最佳实践。

## 配置最佳实践

### 工作区

工作区是团队计划工作的集中位置。 工作区是团队使用的记录类型的集合，表示团队的工作生命周期。

以下是有关配置Workfront Planning的一些常见问题。

#### 我应该如何开始？

* ✅当您首次登录Planning时，请遵循我们的应用程序内载入流程，该流程清楚地传达了Planning的价值并指导您如何有效地导航和利用产品。 这可确保您了解其功能以及如何轻松开始工作。
* ✅首先，浏览我们预定义的工作区模板，以了解现有类似用例的想法。 您可以使用模板中的预定义记录类型和字段，也可以添加自己的类型和字段。
* ✅确定要通过Workfront Planning解决的主要用例。 例如，大多数组织都希望提高战略活动的可见性，其中可能包括构建更好的“营销活动日历”。 因此，对于此用例，您可能希望首先回答几个问题：

   * 谁在要求它？
   * 他们要放进日历里的东西叫什么？
营销活动？ 战术？ 计划？ 活动？ 活动？
   * 他们想用这个日程表回答什么样的问题？
   * 他们是否为同一受众开展了重叠的营销活动？
   * 该活动、策略、活动或事件的预算是多少？

  这些问题的答案将决定您需要在Workfront Planning中构建什么。

  此外，请考虑可能有其他规划人员当前不是Workfront用户。 这些规划者可以利用Excel电子表格、Word文档、PowerPoint演示文稿等进行操作。 考虑他们可以如何在Workfront Planning中访问您的信息。

* ✅要充分利用Workfront Planning，请考虑将Workfront中的项目组合和程序用作Workfront Planning中的其他上层结构。

  如今，Workfront客户通过项目组合和项目组合来代表他们的战略工作，在某些情况下，他们作为不同类型的项目进行展现。 随着Planning的推出，所有此类战略性工作都应通过Workfront Planning中的自定义记录类型来处理，而Workfront将围绕以项目和任务形式呈现的工作的执行阶段来处理。

#### 何时应创建新工作区而不是修改现有工作区？

* ✅为组织级别的工作区中的最低容量进行设计。 您可以为特定的运营组织单位创建工作区，以匹配每个单位独特的工作方式。

  将信息放在单个Workspace中，以确保可以轻松管理所有数据之间的关系。

  例如，尝试为所有营销创建单个工作区。

  可以为具有完全不同运营结构的团队创建新工作区：

  例如，**产品开发**&#x200B;工作区应不同于&#x200B;**营销**&#x200B;工作区。

* ⛔不要为组织内的每个团队或进程创建唯一的工作区。

  营销组织应努力维护一个工作区，以保持可见性，并允许数据在全球计划级别汇总。

  避免为遵循类似流程（例如，EMEA营销与APAC营销）的团队创建类似或重复的工作区，尤其是当这些团队的工作可提升到通用战略活动时。

#### 我应该如何使用Workspace分区？

* ✅创建并标记部分，以帮助用户了解您如何组织运营生命周期。

  例如，您可以创建一个名为&#x200B;**Core records**&#x200B;的部分，将您的营销活动、战术和交付项放置到工作区中。
* ✅组将“赞”记录类型组合在一起。

  例如，您可以创建一个名为&#x200B;**地理位置**&#x200B;的部分，其中包含记录类型，如：地区、国家/地区和城市。

### 记录类型

记录类型是Workfront Planning Workspace的构建块。 您可以定义记录类型的互连方式。

#### 如何在我的工作区中定义记录类型？

* ✅请花一些时间确定您需要跟踪哪些信息（我需要哪些记录类型）以及需要如何连接这些信息。 与将使用该工作区考虑其所有需求的利益相关者交谈。 您还可以创建具有不同记录类型的自定义分区，以便以非常方便使用的方式呈现信息。

* ⛔不要在不同的时间段重复记录类型（例如，不要为&#x200B;**营销活动2024**&#x200B;和&#x200B;**营销活动2025**）创建单独的记录类型。

  每当您想要比较多个年份的数据时，创建不同的记录类型都会中断数据流。 今天的视图是按记录类型划分的，因此一旦一年结束，该记录类型的视图将不再显示未来的项目。 最佳实践是为工作类型创建一个记录类型，并使用基于不同字段的过滤器对数据进行分段，或根据需要进行存档。

#### 与链接记录类型相比，何时应使用单选或多选字段？

* ✅如果对象将用于多个其他记录类型，请添加新记录类型

  例如，营销活动可以关联到多个目标受众，而战术可以关联到单个目标受众。 因此，“营销活动”、“策略”和“受众”应该是记录类型，而不是多选字段。

* ✅如果对象需要存储可能在查找中有用的其他元数据值，请添加新记录类型

  例如，渠道记录类型（如&#x200B;**电子邮件**）可能会存储支持交付项的列表，这些交付项既可以存储为本机元数据，也可以存储为与独立&#x200B;**交付项**&#x200B;记录类型的连接。
* ⛔如果您存储的数据只与单个记录类型相关，请不要添加新记录类型。

  例如，**促销活动**&#x200B;记录类型可能具有名为&#x200B;**促销活动大小**&#x200B;的单选字段，该字段仅在与特定促销活动直接关联时才相关。 请创建一个字段来捕获此信息。

#### 如何标记我的记录类型？

* ✅创建并标记表示单个构造或名词的记录类型，如&#x200B;**营销活动**。
* ⛔不要创建更好地表示为视图的记录类型。

  例如，**日历**&#x200B;对于记录类型来说是一个糟糕的选择，因为它不是记录类型本身，而是记录视图。

### 字段管理

字段是记录类型的属性，在表格视图中显示为列。 您可以为记录类型创建自定义字段，然后将这些字段与Workfront Planning记录关联以增强记录信息。

#### 建议将哪个字段定义为“主”字段？

* ✅确实使用唯一的主字段值，以便在建立连接时更容易查找和“挑选”这些记录。 

  建立连接时，用户将按“主要”字段中的值进行搜索，如果它们不是唯一的，用户将无法知道应该选择哪一个。 
* ⛔避免将非唯一值用作主字段，因为这样可能会给使用连接选取器菜单时必须搜索主字段的用户造成混淆。 

#### 应如何使用公式？

* ✅确实使用公式字段类型以减少手动输入。 当您根据表格视图中已有的数据输入信息时，可以使用公式自动计算该信息，从而节省一些精力。

#### 如何开始连接工作区中的数据？

* ✅创建连接是Workfront Planning最强大的功能之一。 您可以将记录类型相互连接或记录类型与其他应用程序(如Adobe Workfront（与项目、项目组合、程序、公司和组的连接）、Adobe Experience Manager Assets（与资源和文件夹的连接）和Adobe GenStudio for Performance Marketing的对象类型连接。

  连接对象和记录类型为您提供了公司中所有内容的连接方式的完整概述。

  例如，您有&#x200B;**促销活动**&#x200B;记录类型和&#x200B;**战术**&#x200B;记录类型，您可以创建这两种记录类型之间的连接，以查看哪些&#x200B;**战术**&#x200B;与特定的&#x200B;**促销活动**&#x200B;相关联。

  定义连接后，工作区中的所有人员可以通过双击连接字段，开始添加&#x200B;**促销活动**&#x200B;的值，他们将在连接字段中看到所有可用&#x200B;**战术**&#x200B;的列表。 这使您能够快速找到需要与营销活动关联的战术。

#### 如何使用查找字段？

* ✅在记录或对象类型之间建立连接后，可以将各个记录相互连接，并在Workfront Planning记录中显示链接记录或对象类型中的字段。 您将减少必须更新同一段信息的位置数量，并确保它们完全匹配。

  例如，一旦您在&#x200B;**促销活动**&#x200B;记录类型与&#x200B;**战术**&#x200B;记录类型之间建立连接，您将会看到主要字段信息，但是当您添加查找字段时，您将能够从相应记录类型中获取其他信息，例如&#x200B;**战术**&#x200B;的&#x200B;**启动日期**。 添加记录后，将自动填充这些查找字段的数据。

#### 对于URL，建议使用什么字段类型？ 

* ✅使用单行文本字段将URL数据添加到记录。

### 视图

#### 如何确定视图与记录类型是什么？

* ✅对于表示单个构造或名词的项目（如&#x200B;**促销活动**），请创建记录类型。 

* ⛔不要创建更好地表示为视图的记录类型。

  例如，**日历**&#x200B;对于记录类型来说是一个糟糕的选择，因为它不是记录类型本身，而是记录视图。 

#### 我应该隐藏还是删除与我无关的字段？

* ✅隐藏列，而不是删除此列，因为此信息可能与使用相同记录类型的不同人员相关。 如果删除特定表视图中的字段，则还将删除此记录的其余视图中的该字段，以及此记录类型链接的任何其他位置。

#### 如何在表格视图和时间线视图中使用筛选器和分组？

* ✅使用带有筛选器和分组的视图来显示您需要查看内容的快照。 您可以过滤和分组数据，以便采用更易于使用的方式了解计划内容。 您可以按元数据字段对记录进行分组。

  例如，您可以拥有&#x200B;**Campaign**&#x200B;记录类型的时间线视图，您可以按&#x200B;**Target受众**&#x200B;进行分组，并按&#x200B;**日期**&#x200B;进行筛选以仅显示当前年份。

#### 为什么我在时间线视图中看不到所有记录？

* ✅请记住为记录定义2个日期字段。 仅当至少有两个日期字段与记录类型关联时，才能创建时间线视图。 当开始日期或结束日期或两者均没有值或者开始日期在结束日期之后时，某些记录可能不会显示在时间轴视图中。

#### 应如何使用时间线视图设置？

* ✅定义时间轴视图的设置，如&#x200B;**条形样式**&#x200B;和&#x200B;**颜色**，以获得更直观的视图。 通过定义您是否希望看到带有有意义图像的缩略图以及添加更多字段以在栏上显示（例如，**所有者**&#x200B;或&#x200B;**状态**），您可以自定义&#x200B;**栏样式**。

  默认情况下，您只看到主字段。 您还可以按字段值定义条形图的颜色（例如，可以通过将条形图与“状态”字段匹配来自定义条形图的颜色），也可以按已应用的分组定义条形图的颜色。 默认情况下，颜色与记录类型的颜色匹配。

  只有记录类型颜色或带有与颜色关联的选项的字段才能影响时间轴中记录栏的颜色。

### 权限和共享

使用共享功能向他人授予查看和工作区的相应权限。

#### 我该如何管理对工作区的权限？

* ✅当您创建&#x200B;**工作区**&#x200B;时，它仅供您使用。 不是系统管理员的任何其他人将无法找到它。 定义工作区并准备好将您的团队引入开始协作后，您需要与他们共享该工作区并定义其权限级别。

  您可以从以下权限级别中进行选择：

   * **管理**：用户可以编辑、删除和共享工作区、记录类型，以及编辑、删除和创建记录。
   * **Contribute**：人员可以创建、编辑和删除记录。
   * **查看**：人员可以查看记录。

* ✅尽管许多客户感觉他们会向大多数人授予对工作区的&#x200B;**管理**&#x200B;权限，但确实会将&#x200B;**管理**&#x200B;权限限制为仅允许一组选定的受信任人员，这样就不会意外删除记录类型或创建不必要的记录类型和字段。 他们可以编辑、共享甚至删除工作区。 此级别的权限授予他们对Workspace的完全管理访问权限。

  需要有标准用户许可证，用户才能拥有工作区的管理权限。

* ✅如果您希望用户只能创建、编辑和删除记录，但不希望他们更改工作区的结构，请授予用户&#x200B;**Contribute**&#x200B;权限。 他们具有&#x200B;**Contribute**&#x200B;权限，无法创建记录类型或更改现有记录类型上的字段。

  对于具有工作区的&#x200B;**Contribute**&#x200B;权限的用户，需要标准用户许可证。

* 如果您希望用户仅查看记录，请✅授予用户&#x200B;**查看**&#x200B;权限。

#### 如何管理记录类型的权限？

* ✅请记住，具有工作区管理权限的用户无法降低其记录类型的权限。 他们还将继承记录类型的管理权限。 您不能向用户授予对工作区的“管理”权限，而是授予对记录类型的“贡献”或“查看”权限。
* ✅如果您希望用户对于记录类型的权限级别（例如“查看”权限）低于他们对工作区的权限级别，我们建议为他们授予对工作区的“贡献”权限。 然后，您可以授予他们查看记录类型的权限。
* 从记录类型的权限中移除用户，仍然会为他们至少赋予工作区的“查看”权限。

#### 我应如何管理视图的权限？

* ✅确实为想要编辑、删除和共享视图的人员保留&#x200B;**管理**&#x200B;权限。 这意味着他们可以更改筛选器、分组字段或视图的某些配置。 这些更改将影响同时使用该视图的其他所有用户的视图的主配置。

  需要有标准用户许可证，用户才能拥有视图的管理权限。

* ✅授予用户&#x200B;**视图**&#x200B;权限以便应用该视图。 他们将能够更改某些过滤器或分组和排序，但这些更改将是临时的；更改不会为访问视图的所有其他用户保存。 这些更改不会影响同时使用该视图的其他所有用户的视图的主配置。  他们的更改仅对应用修改后的设置的用户可见。 刷新屏幕后，更改将重置为默认设置。

* ✅授予&#x200B;**当您希望可以查看工作区的每个人都可以查看该特定视图中的记录及其字段时，工作区中的每个人都可以查看**&#x200B;权限。 这样，您就不需要手动将任何人添加到视图的共享权限框中。

  >[!NOTE]
  >
  >如果尚未共享某个视图，而您与其他人共享指向该视图的链接，则他们将能够在&#x200B;**默认表视图**&#x200B;中查看记录。 如果他们拥有标准Workfront许可证，则可以构建自己的视图。

#### **Workspace共享**&#x200B;与&#x200B;**视图共享**&#x200B;有何不同？

* **Workspace共享**&#x200B;定义用户对工作区、其记录类型、记录及其字段的访问权限。

* **视图共享**&#x200B;定义用户是否可以看到您创建的视图，以及他们是否可以更改该视图的筛选器、分组字段或其他配置。 视图中显示记录的可见性由Workspace共享控制，而不是由视图共享控制。

#### Workfront许可证类型如何影响Workfront Planning权限？

* 对于&#x200B;**Workspace共享**： Light和Contribute许可证用户只能获得对工作区的查看访问权限。 要向某人授予对工作区的“贡献”或“管理”权限，此人需要具有Standard许可证。

* **视图共享**：具有工作区管理权限的标准许可证用户可以创建视图。 Light和Contribute许可证用户只能使用Standard用户已创建并与他们共享的视图。 否则，如果未共享任何内容，则用户将能够看到&#x200B;**默认表视图**。

#### 当Workspace所有者更改时，我该怎么做？

* Workfront将工作区创建者设置为所有者，但从功能上讲，该所有者与具有管理权限的任何用户具有相同的权限。
* 如果所有者被停用，则其他成员可以在工作区中继续工作，而不会出现任何中断。
* 系统管理员有权访问任何工作区，因此，如果所有者是唯一具有管理权限的人员，则管理员可以添加其他人员并授予他们管理权限以处理工作区的管理。

### 在Workfront规划中提交请求

当希望用户在记录类型的页面外添加记录时，可以为每种记录类型创建请求表单。 提交表单会将新记录添加到记录类型。

#### 何时应开始创建记录类型的请求表单？

* ✅您应确保先通过向表中添加必要的字段来设置记录类型结构。 这些字段描述了您的记录，可在表单生成器中访问。

  理想情况下，在记录类型结构最终确定后构建请求或引入表单，以避免缺少任何关键字段。

#### 谁可以创建请求表单？

* ✅任何对工作区具有“管理”访问权限的用户都可以创建或编辑记录类型的请求表单。 确保正确分配用户的权限以允许此功能。

#### 如何创建或编辑记录类型的请求表单？

* ✅任何对工作区具有“管理”访问权限的用户都可以按照文章[在Adobe Workfront计划中创建和管理申请表](/help/quicksilver/planning/requests/create-request-form.md)中所述的步骤进行操作。


#### 谁能够使用申请表提交新记录？

* ✅提交权限取决于您为每个表单配置的设置。

  在表单生成器中，发布表单后，您可以管理权限以控制谁可以提交请求。

  您可以从以下共享选项中进行选择：

   * 要与Workfront中的人员内部共享，请执行以下操作：

      * **具有工作区查看权限或更高权限的任何人：**&#x200B;允许具有工作区查看权限或更高权限的所有用户提交创建记录的请求。
      * **对工作区具有Contribute或更高访问权限的任何人**：限制向对工作区具有Contribute或更高权限的用户提交。
      * **只有受邀人员才能访问**：添加可向表单提交请求的人员、团队、角色、组或公司。
   * 对于与没有Workfront帐户的用户进行外部共享：
      * **创建公共链接**，然后复制该链接并与任何人共享，甚至与没有Workfront帐户的人共享：允许拥有该表单链接的任何人提交请求。
      * **链接到期日期：**&#x200B;请确保为公共链接设置到期日期以增强安全性。

### 管理请求表单的最佳实践

以下是管理请求表单的建议：

* 提前计划：在创建表单之前明确定义请求者需要或需要哪些信息，以避免以后过度修改。
* 使用清晰的标签：确保字段标签和描述清晰易懂，可供所有用户使用。
* 测试表单：在将新表单推广到更广泛的受众之前，请使用表单链接和表单预览选项测试表单，以确保所有字段和逻辑都按预期运行。
* 保持表单更新：定期审查表单并更新表单，以匹配记录类型结构或操作流程中的任何更改。

<!--do we need to add anything for the Configuration tab of a request form?? -->

<!-- this is hidden, per Andrea:  

2.2 Migration  

Migrating your data from external <span style="text-decoration:underline;">s~~S~~</span>ystems to Workfront Planning unlocks new ways to create important connections in your workflow and uncover insights that you might not have been able to identify with your previous tools. 

By having all your data in one central location, you can more easily form connections between your Workfront data than if they all existed in separate tools. 

We have some options that will help you to accelerate the migration process:  

* **Fusion** – You can create a Scenario in Fusion that runs after certain criteria and connects objects. 
* **Bulk Data Operations** _through the new functionality -[ [E] Make connected Planning data consumable through WF forms](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6641b040000b880ccd74aab6365c3361/overview?source-id=unifiedShareMFE)  (Q3 2024)_ -  
* **Copy and paste – **You can copy and paste directly from a spreadsheet. This is best suited to a simple table of data from tools like Excel or Google Sheets.  
* **Upload a C<span style="text-decoration:underline;">SV~~VS~~</span> or Excel **- The CSV (comma-separated values) format or Excel is one of the most common ways to move data between applications, and tools. This functionality is not available yet, but we are planning to work on it in Q4 2024.  

-->

<!--
     

1. Data Flow  

Currently the metadata modelling in Workfront Planning is done by Ops Admins through adding various data points to the record type from the table view, including: 



* Fields added directly on the current record type 
* Connections with custom defined operational and taxonomical record types 
* Connections with execution work captured in Workfront 
* Connections with deliverables stored as assets in AEM 
* Any lookup fields captured in any of the above connections. 

Here is a summary of how you can define the data flow within Workfront Planning and other applications.  


     



* **Connections and Lookup fields. **Creating **connections** is one of the most powerful features of Workfront Planning. You can connect record types to one another or record types with object types from other applications like Adobe Workfront (connection to Project, Portfolios, Programs, Companies, and Groups) or Adobe Experience Manager Assets (connection to assets and folders).  Connections give you a full overview of how everything in your company is connected.  

    - e.g.: You have a Campaign record type, and a Tactics record type, then you can create a connection between these two record types to see to see which Tactics are associated to a specific Campaign. After defining the connection, all the people in the workspace can start adding values by double-clicking into the connection field that displays the tactic where they will see a list of all the Tactics available and you can quickly select the tactics to be associated with each campaign. 


    After you establish the connection between records or object types, you can connect individual records to one another, and display fields from the linked record or object types on a Workfront Planning record. The connected fields are called **Lookup fields**. You will reduce the number of places you have to update the same piece of information and ensure that they match perfectly.  


    - e.g.: Once you have a connection between a Campaign record type and a Tactics record type, you will see the primary field information when you add the tactic, but when you add lookup fields, you will be able to bring additional information from the tactic, like the Launch date for that Tactic. The data for these lookup fields is auto populated. Find more information in the Adobe Experience League documentation in the article about Connecting records.  


     

* **Planning (or Connections) tab** **in Workfront _-[ [E] Global Connect capability in Planning connections area](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6617d7760001e250f5ffb9ebf04baacc/overview?source-id=unifiedShareMFE)_** 

    When you go to the Planning section of Adobe Workfront objects, you can display both connections with linked records or any available connections with Planning record types. With that, you can view and edit any connection field without having to navigate away from the current section in Workfront to other areas. The Planning section is available for the following Workfront objects: Project, Portfolio and Program. For more information, see [Manage records in the Planning section of Adobe Workfront objects](https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-records/manage-records-in-planning-section).   


* Create new records within the connection fields - In-context creation of connected records https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6656c1a30026b903c6edf0210b8cbb23/overview?source-id=unifiedShareMFE  When you need to link records through a connection field but cannot find the required records in the connected record type, you can also create new records in the connected record type directly within the connection fields, with that you can efficiently establish necessary links without having to leave the current record type context. For more information, see Create records https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-records/create-records.   

     

* **Field on Customer Form** (CF)[ - [E] Make connected Planning data consumable through WF forms](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6641b040000b880ccd74aab6365c3361/overview?source-id=unifiedShareMFE) _(Planned completion date Sep 15, 2024 10:00 PM)._ Considering that the Workfront Project metadata modeling is done through forms, you are also able to add Planning connections to your custom forms. You can embed any lookup field value from the connected Planning record types within the custom form of your Workfront object. With that capability, when you are managing objects in Workfront, you can present any taxonomies or operational records connected to the Workfront object in custom forms, alongside other details, so that your teams can easily consume and update all the relevant information through a unified interface.  They should not need to navigate to different areas to view and update the information relevant for their work.  

     

* **Connection between Workspaces with Record types accessible from multiple workspaces** – ~~Epic – "[Connect to record types across workspaces](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/64dfad3100027190324dcc35b2176e76/overview?source-id=unifiedShareMFE)"~~ When you are creating a workspace in Planning, you can define certain record types once and then configure them to be accessible from multiple workspaces so you can create connections with them from anywhere. This way, you can streamline the data management process, eliminate duplicative work, and ensure data consistency across teams. As a result, your teams can tag their records with common taxonomies and unlock better visualization, filtering, grouping, and reporting of cross-team work.  For more information, see [Edit record types](https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-architecture/edit-record-types). 

     

* **Fusion connector – You can create a connection to your Workfront Planning account from inside a Workfront Fusion module. **With this connector, you can trigger a scenario when events occur in Workfront Planning. You can also create, read, update, and delete records, or perform a custom API call to your Adobe Workfront Planning account. More information in Experience League in[ Adobe Workfront Planning modules](https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-fusion/fusion-apps-and-modules/workfront-planning-moduleshttps:/experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-fusion/fusion-apps-and-modules/workfront-planning-modules) article.  

-->
