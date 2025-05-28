---
title: 使用Adobe App Builder为Workfront创建自定义应用程序
description: 由Adobe App Builder提供支持的Workfront UI扩展允许客户和合作伙伴创建自定义的用户体验。
author: Courtney
feature: Digital Content and Documents
exl-id: 2ed75053-8199-474c-afb4-fa9bbd3750f8
source-git-commit: a4e715d5212c3c166ce6ed995b327eb2b7198123
workflow-type: tm+mt
source-wordcount: '1693'
ht-degree: 0%

---

# 使用Adobe App Builder为Workfront创建自定义应用程序

由Adobe App Builder提供支持的Workfront UI扩展允许客户和合作伙伴创建自定义的用户体验。 这些工具提高了效率，提供了无缝的、互联的体验，并显着提高了用户满意度，并帮助企业实现他们独特的愿景。

例如，如果没有Workfront UI扩展，项目经理可能需要在Workfront和单独的时间跟踪系统之间切换以记录小时数。 通过UI扩展，可以将时间跟踪直接集成到Workfront体验中，从而简化工作流并节省时间。 此外，您还可以添加自定义组件以提高可用性，自动执行重复任务，并通过元数据标记和内容预览等功能增强内容管理。 Adobe App Builder还提供了可扩展性和强大的身份管理(IMS)，确保在任何规模下均能安全高效地自定义。

Workfront UI扩展提供了几项主要优势：

* 精确定制：标准软件界面往往无法满足所有业务需求。 UI扩展允许开发人员修改和扩展默认用户界面，以满足特定业务需求。
* 系统集成： UI扩展有助于集成其他系统，确保无缝的工作流和数据一致性。
* 可扩展性：随着业务的增长，可以开发UI扩展来添加新功能，而无需全面的系统大修。
* 缩短开发时间：预建的扩展点和工具可显着减少实施自定义功能所需的时间和精力。
* 增强的用户采用率：优化的用户体验可以显着提升软件采用率。 根据用户偏好设计的自定义UI元素可以提高采用率和整体满意度。
* 利用Workfront UI扩展，企业可以创建量身定制的用户体验，从而提高效率、集成和用户满意度。

在Adobe App Builder中创建应用程序后，Workfront管理员可以使用布局模板将其添加到Workfront主菜单和左侧导航面板。 具有布局模板的用户点击应用程序后，将看到应用程序嵌入到Workfront中，而不必单独打开它。

本文介绍了如何访问App Builder并使用模板创建应用程序。

有关将自定义应用程序添加到布局模板的信息，请参阅[使用布局模板自定义主菜单](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)和[使用布局模板自定义左面板](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)。

## 先决条件

您必须具备以下条件：

* 启用了IMS的Workfront帐户
* 具有节点v18和npm的开发计算机
* App Builder许可证

## 访问Adobe App Builder

要创建UI扩展，您必须有权访问Adobe Developer Console中的Adobe App Builder 。

[Adobe Developer网站](https://developer.adobe.com/uix/docs/guides/get-access/)上提供了其他说明。

### 将开发人员添加到Adobe Admin Console

>[!IMPORTANT]
>
>请确保为以下所有步骤选择了正确的IMS组织。 如果您属于多个组织，则可能会选择错误的组织。 确保您在正确的组织下操作，该组织通常位于右上角。

1. 导航到生产： https://adminconsole.adobe.com/

1. 在&#x200B;**用户**&#x200B;部分中，单击&#x200B;**开发人员** > **添加开发人员**。

   ![在管理控制台中添加用户](assets/manage-users-admin-console.png)

   >[!NOTE]
   >
   >如果您看不到用于管理开发人员的选项，则表示您没有允许开发人员访问权限的产品。

1. 添加用户的电子邮件。 它应该搜索已从Admin Console中添加的现有用户。

1. 将必要的产品添加到开发人员配置文件中，然后单击&#x200B;**保存**。\
   ![添加开发人员](assets/add-developer.png)

### 访问App Builder

组织必须与其客户经理合作才能购买App Builder。

如果AppBuilder配置正确，则在创建新项目时，您应该会看到从模板创建项目。

## 在Adobe Developer Console中创建新项目

您必须使用Adobe Developer Console来构建UI扩展。

[Adobe Developer网站](https://developer.adobe.com/uix/docs/guides/creating-project-in-dev-console/)上提供了其他说明。

1. 使用您的Adobe ID登录到Adobe Developer Console 。

1. 选择您的帐户，以及您的个人资料或组织。

1. 在“快速入门”区域单击&#x200B;**从模板创建项目**，或单击&#x200B;**从模板创建新项目>项目**。

   >[!IMPORTANT]
   >
   >如果您看不到从模板创建项目的选项，则表明您在Admin Console中的配置有误，并且无权访问App Builder目录。 仅当您有权访问AppBuilder时，才会显示此选项。

   ![从模板创建](assets/create-from-template.png)

1. 选择&#x200B;**App Builder**。

1. 输入&#x200B;**项目标题**&#x200B;和&#x200B;**应用程序名称**。 两者都有默认值，但如果您自定义值，则以后可以更轻松地识别所需的项目。

1. 保留&#x200B;**包含运行时**&#x200B;处于选中状态。

1. 单击&#x200B;**保存**。

## 使用Adobe IO (aio) CLI

Adobe提供了一个开源CLI，您可以使用它创建App Builder应用程序。

GitHub和Adobe Developer网站上提供了其他说明：

* https://github.com/adobe/aio-cli
* https://developer.adobe.com/app-builder/docs/getting_started/first_app/

1. 要安装该工具，（确保您首先在节点v18上）运行： `npm install -g @adobe/aio-cli`。
1. 启动终端并使用以下命令登录AIO： `aio login`。 如果您在登录到正确的IMS组织时遇到问题，请尝试`aio login -f`以强制显示登录提示。 使用`aio where`查看您登录到正确IMS组织的组织。 有关详细信息，请使用`aio config`。
1. 通过运行`aio app init example-app`开始设置应用程序，请确保将“example-app”替换为应用程序名称。 如果您不确定应用程序名称，则可以使用命令`aio console project list`查看应用程序名称列表。
1. 从提供的选项中选择您的组织和项目。
   ![命令结果](assets/1-command-result.png)
   ![选择项目](assets/2-select-a-project.png)

1. 浏览所有可用的模板，并为您的项目选择&#x200B;**@adobe/workfront-ui-ext-tpl**。
   ![选择模板](assets/3-choose-template.png)
1. 选择并输入您在Adobe Developer Console中创建的项目名称。
   ![选择并输入项目名称](assets/4-select-and-enter-project-name.png)

1. 回答应用程序的提示：

   * 命名扩展。
   * 提供扩展功能的描述性摘要。
   * 选择要开始的初始版本号。
   * 如果在系统提示“下一步要做什么？”时选择“将自定义按钮添加到主菜单项”，则模板将为主导航按钮创建代码。

   ![选择完成](assets/5-select-done.png)

1. 选择“我已完成”以确认完成。 正在从模板生成代码。
   正在生成![](assets/6-generation-in-process.png)
1. 等待您看到应用程序初始化已完成的消息。 然后，您可以在IDE中打开该项目（建议使用Visual Studio代码）并访问src文件夹。

   有关项目中文件夹和文件的详细信息，请参阅[Adobe开发人员网站](https://developer.adobe.com/app-builder/docs/getting_started/first_app/#5-anatomy-of-an-appbuilder-application)。

## 在VSCode中构建扩展

要通过Workfront主菜单或辅助导航（左侧面板）启用导航，需要App.js文件配置。

在Workfront布局模板中显示扩展名需要ExtensionRegistration.js文件配置。

以下示例说明了如何使用UI扩展将自定义应用程序添加到Workfront主菜单和对象的左侧面板。

### 配置ExtensionRegistration.js

要在Workfront主菜单中允许自定义应用程序，请执行以下操作：

1. 转到ExtensionRegistration.js。

在ExtensionRegistration函数中，您应该会看到以下代码。 此代码由模板为您创建。 可以添加此代码以创建其他菜单项。 请务必替换ID和URL。

    “
    mainMenu： {
    
    getItems() {
    
    return [
    
    {
    
    id： &#39;main-menu-label&#39;，
    
    url： &#39;/index.html#/main-menu-label&#39;，
    
    label： &#39;Main menu label&#39;，
    
    icon： icon1，
    
    }，
    
    ]；
    
    ，
    
    }
    “
”
1. 添加以下代码片段：
   ![代码段](assets/7-extension-registration-step1-from-sam.png)
此示例显示了一个主菜单项。 您必须将ID、标签、图标和URL更新为应用程序的正确名称。 添加多个项目时，请确保ID是唯一的。

1. 保存您所做的工作。

### 允许在Workfront左侧面板导航中使用自定义应用程序

要在Workfront左侧面板导航中允许自定义应用程序，请执行以下操作：

1. 转到ExtensionRegistration.js。
1. 在ExtensionRegistration函数中，添加以下代码片段：

   ```
   secondaryNav: {  
   
   TASK: {  
   
       getItems() {       return [         {           id: "TASK", 
   
   label: "My TASK",           icon: metricsIcon,           url: "/myTask",  
   
           },  
   
       ];  
   
       },  
   
   },  
   
   },  
   ```

   ![扩展注册](assets/8-extension-registration-file-step2.png)

   * 此示例显示了一个名为“我的任务”的左侧面板导航项。 您必须将ID、标签、图标和URL更新为应用程序的正确名称。

   * 此示例显示了Project对象类型的左侧面板导航项。 您必须为Workfront中支持的每个对象单独创建这些项目。 以下对象可用：项目、任务、问题、项目组合和项目群。

1. 保存您所做的工作。

### 配置应用程序.js

1. 转到App.js。

1. 该模板将为主菜单选项提供一个路由。 路由定义URL路径与针对这些路径呈现的组件之间的映射。 要添加路由，请使用以下代码片段，并确保将确切的路径和元素替换为您的路径和元素。

   ```
       <Route 
   
               exact path="custom-application" 
   
               element={<Customapplication />} 
   
           /> 
   ```

   ![代码示例](assets/9-app-file-step-1-from-sam.png)
1. 保存您所做的工作。

有关开发和运行该应用程序的详细信息，请参阅[Adobe开发人员网站](https://developer.adobe.com/app-builder/docs/getting_started/first_app/#6developing-the-application)。

## 共享上下文

共享上下文用于将数据从Workfront共享到UI扩展。 通过共享上下文可用的数据包括用户数据和应用程序上下文。


### 用户

Workfront的UI扩展共享用户数据。 通过共享上下文提供的用户对象包括Workfront用户ID和用户的电子邮件地址。

`user = (conn?.sharedContext?.get("user")); // {ID: '1', email: 'test@aaa.com'} userID = user.ID userEmail = user.email `

### 应用程序上下文

在使用辅助导航扩展点添加自定义应用程序时，自定义应用程序通常使用上下文数据，如项目ID或文档ID。 对于这些数据，共享上下文包括对象代码和对象ID。

下面是获取文档应用程序上下文的示例：

`context = conn?.sharedContext; // Using the connection created above, grab the document details from the host tunnel. // conn?.host?.document?.getDocumentDetails().then(setDocDetails); `

## 在Workfront中测试应用程序

在为Workfront开发App Builder应用程序时，您可能需要在Workfront中测试您的应用程序而不发布它。

在App Builder应用程序中，您可以启动`aio app run`以进行本地开发。 这将为您提供一个URL，通常类似于`https://localhost:9080`。 或者，您可以执行`aio app deploy`以获取静态Adobe域。 请务必记下这些URL以供将来使用。

接下来，导航到要在浏览器中开发的特定页面。 打开开发人员工具并访问workfront.com或workfront.adobe.com的本地存储。 您必须在此添加一个条目。 使用`extensionOverride`作为键，使用以前提到的应用程序生成器URL作为值。

如果配置正确完成，则在Workfront中重新加载布局模板页面时，您将看到App Builder应用程序中的按钮。 将应用程序按钮添加到对象的主菜单和左侧面板，并验证它们是否正确显示在这些区域中。

Adobe开发人员网站上提供了其他说明，并以AEM为例：https://developer.adobe.com/uix/docs/guides/preview-extension-locally/

## 发布应用程序并批准提交

要发布并批准应用程序，请按照[Adobe开发人员网站](https://developer.adobe.com/uix/docs/guides/publication/)上的说明操作。
