---
product-previous: workfront-proof
product-area: documents
navigation-topic: create-proofs-and-files
title: 在中生成校样 [!DNL Workfront Proof]
description: Workfront校样允许您从文档或网站创建校样，并与他人共享这些校样。 以下步骤描述了各种可用的配置选项 — 编辑我。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 49657851-2948-4d3b-b2ce-c8359eeb315b
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '2267'
ht-degree: 0%

---

# 在中生成校样 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文介绍独立产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参阅 [校对](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] 使您能够从文档或网站创建校样，并与他人共享这些校样。 以下步骤描述了可用的各种配置选项：

## 为文档生成校样

1. 执行以下任一操作，以开始创建新校样并显示 [!UICONTROL 新校样] 页面：

   * 单击绿色 **[!UICONTROL 新校样]** 按钮。
   * 在 **[!UICONTROL 功能板]** 区域，在 **[!UICONTROL 概述]** ，单击 **[!UICONTROL 新校样]** 链接。

   * 通过Dropzone提交（企业功能）。
   * 的 **[!UICONTROL 新校样]** 页面。

1. 要校样一个或多个文档，请按以下任一方式添加要校样的文档（重复此过程以添加多个要校样的文档）：

   * 将文档从文件系统拖到 **[!UICONTROL 添加文件]** 的上界。
   * 在 **[!UICONTROL 添加文件]** 区域，然后浏览以查找并选择要从工作站的文件系统上传的文档。

      ![proof_document_upload.png](assets/proof-document-upload-350x64.png)

1. 要校样一个或多个网站，请在 **[!UICONTROL 添加文件]** 区域，然后按 **[!UICONTROL 输入]**.

1. （可选）重复此过程以添加多个网站进行校样。

   有关校样网站的更多详细信息，请参阅 [为URL生成校样](#generate-a-proof-for-a-url).

   ![](assets/proof-website-350x65.png)

1. （可选）修改任何已上传文件的文件名：

   1. 将鼠标悬停在 **[!UICONTROL 添加文件]** ，然后单击 **[!UICONTROL 编辑]** 图标。

      ![proof_edit.png](assets/proof-edit-350x53.png)

   1. 在 **[!UICONTROL 校样名称]** 字段，指定新名称，然后单击 **[!UICONTROL 完成]**.

   1. （可选）要删除要上载的任何文件，请将鼠标悬停在 **[!UICONTROL 添加文件]** ，然后单击 **[!UICONTROL 删除]** 图标。

      ![proof_delete.png](assets/proof-delete-350x53.png)

   1. （可选）启用选项， **[!UICONTROL 将所有兼容的文件合并到单个校样中]**.

      **启用此选项后：** 所有静态文件和网站都可通过单个校样获取，并且您在给定时间最多可上传50个文件。

      >[!NOTE]
      >
      >交互式文件（包括视频和交互式网站）不能合并为单个校样。

      **禁用此选项时：** 所有文档和网站都作为单个校样生成，并且您在给定时间最多可上传20个文件。

      要将所有上传的文件和网站合并到一个校样中，请执行以下操作：

      1. 启用选项， **[!UICONTROL 将所有兼容的文件合并到单个校样中]**.
      1. 在 **[!UICONTROL 校样名称]** 字段，为组合校样指定新名称。
      1. 在 **[!UICONTROL 添加文件]** 区域，通过将文件拖动到所需的顺序来重新排序包含的文件。 文件的顺序是组合校样的页面顺序。 有关创建组合校样的更多信息，请参阅 [创建多页校样](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

1. （可选）如果您要在 **[!UICONTROL 工作流]** 选项：

   * **基本：** 选择此选项可指定在创建校样后立即有权访问校样的用户。 您可以与多个用户共享校样。

      有关共享校样的更多信息，请参阅 [在中共享校样 [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

   * **自动：** 选择此选项可在您拥有复杂的审阅流程时管理内容审阅和批准，或者如果您定期将内容发送给同一组人员进行审阅。 使用自动化工作流，校样会从舞台移动到舞台直至最终批准。 相关用户在需要批准时随时会收到通知。

      有关创建自动化工作流的更多信息，请参阅 [在中使用自动工作流设置校样 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md#create2).

1. 选择是否向您在上一步中选择的用户发送电子邮件通知和自定义消息：

   * **通知收件人此校样：** 选择此选项可向用户发送电子邮件通知。 When **[!UICONTROL 基本共享]** 的 **[!UICONTROL 工作流]** 部分，在创建校样时发送电子邮件通知。 When **[!UICONTROL 自动化工作流]** 的 **[!UICONTROL 工作流]** 部分，当校样进入用户关联的自动工作流阶段时，会发送电子邮件通知。

   * **添加自定义消息：** 选择此选项可在通知中包含自定义消息。 您可以指定主题和消息正文。 消息正文可以包含富文本格式，如粗体、项目符号和超链接。

1. 选择以下任何校样设置：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">需要登录 — 校样只能与其他用户共享</td> 
      <td> <p><strong>需要登录 — 校样只能与其他用户共享：</strong> 选择此选项时，仅 [!DNL Workfront Proof] 用户可以查看校样。</p> <p>此选项默认处于禁用状态；任何具有URL的人员都可以查看校样。</p> <p>选择此选项时：</p> 
       <ul> 
        <li>用户无法登录到校样，除非已将他们添加到校样中。</li> 
        <li>无法启用订阅。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">只需要一个决定即可进行此证明</td> 
      <td> <p>当选择此选项时，在其中一名决策者作出决定后完成审查。</p> <p>默认情况下，此选项处于禁用状态。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">要求对决策进行电子签名</td> 
      <td>用户在决定校样时需要指定其用户名和密码。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">在做出所有必需的决策时锁定验证</td> 
      <td> <p><strong></strong> 启用此设置后，在做出所有决策后，校样状态将被锁定。 当最终审批者做出决策时，状态会自动从已解锁更改为已锁定。</p> <p>默认情况下，此选项处于禁用状态。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">下载原始文件</td> 
      <td> <p><strong></strong> 选择此选项后，审阅人可以下载创建校样的原始文件。</p> <p>取消选择此选项后，“下载”图标将不再可见。<br>默认情况下，此选项处于启用状态。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">通过公共URL或嵌入代码共享校样</td> 
      <td>选择此选项后，可通过公共URL或嵌入代码共享校样。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">通过公共URL或嵌入代码订阅校样</td> 
      <td> <p>选择此选项后，尚未明确添加到校样的人员可订阅校样。 在以下设置中，校样订阅者将获得您定义的角色和电子邮件：</p> 
       <ul> 
        <li><strong>订阅者角色</strong>:分配给所有订阅校样的审阅人的默认校样角色。</li> 
        <li><strong>订阅者的电子邮件警报设置</strong>:分配给所有订阅校样的审阅人的默认电子邮件警报。</li> 
        <li> <p><strong>通过电子邮件链接进行验证访问是</strong>:配置订阅者是否收到包含校样链接的电子邮件。 您可以选择 <strong>无电子邮件</strong> （访问校样不需要电子邮件链接）、 <strong>仅校样通知电子邮件</strong> （订阅者通过电子邮件接收指向校样的链接，且无需任何验证）或 <strong>验证和校样通知电子邮件</strong> (订阅者会通过电子邮件收到指向校样的链接，并且必须单击该链接才能访问校样；此选项旨在确保人员输入了他们有权访问的正确电子邮件地址)。</p> <p>注意：如果校样附加了自动工作流，则所有订阅都会向校样所有者生成确认电子邮件，以便他们决定应将人员添加到哪个阶段。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **[!UICONTROL 创建校样]**.

   Workfront开始生成所选文档或网站的校样。 根据文件大小和类型，文档上传的滞后时间会有所不同。 请耐心等待，因为生成较大的文件需要更长的时间。 您可以从页面导航到其他位置，Workfront将继续生成您的文件。 最大文件上传大小为4 GB。

   生成校样后，单击 **[!UICONTROL 转到校样]** 以启动校样工具。

   ![Screenshot_2018-05-16_08-59-34.png](assets/screenshot-2018-05-16-08-59-34-350x134.png)

   文档将显示在校样工具中。

   帐户中未启用校样的用户仍可以查看文档并对校样进行评论。

## 为URL生成校样 {#generate-a-proof-for-a-url}

您可以首次为URL生成校样。 或者，您也可以生成之前已生成校样的URL校样的新版本。

>[!NOTE]
>
>仅当您的 [!DNL Workfront] 环境与 [!DNL Workfront Proof] 高级帐户。 如果无法按此部分所述使用校样，请与系统管理员联系。

要为URL生成校样，请执行以下操作：

1. 执行以下任一操作，以开始创建新校样并显示 [!UICONTROL 新校样] 页面：

   * 单击绿色 **[!UICONTROL 新校样]** 按钮。
   * 在 **[!UICONTROL 功能板]** 区域，在 **[!UICONTROL 概述]** ，单击 **[!UICONTROL 新校样]** 链接。

   * 通过Dropzone提交（企业功能）。

1. （视情况而定）在 **[!UICONTROL 新校样]** ，以创建现有校样的新版本：

   1. 选择要添加新版本的URL校样。
   1. 单击 **[!UICONTROL 新版本]** 按钮。

      ![Screenshot_2018-05-15_10-59-56.png](assets/screenshot-2018-05-15-10-59-56-350x80.png)

1. 在显示的New校样版本页面中，指定要在 **[!UICONTROL 添加文件]** 区域，然后按 **[!UICONTROL 输入]**.

1. （可选）重复此过程以添加多个网站进行校样。

   ![proof_website.png](assets/proof-website-350x65.png)

1. 单击 **[!UICONTROL 添加文件]** 的上界。

   ![proof_upload_website_modify.png](assets/proof-upload-website-modify-350x185.png)

1. 指定 **[!UICONTROL 校样名称]** 来证明。

   默认情况下，校样名称与网站URL相同。

1. 选择 **[!UICONTROL 处理网站内容]** 选项：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">捕获屏幕截图</td> 
      <td>创建URL首页的静态图像校样。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">交互型</td> 
      <td> <p>创建校样，以允许审阅人导航网站、查看HTML5图像、Flash元素等。</p> <p>要创建交互式校样，网站必须使用安全协议(https)托管。 此外，无法将无法嵌入iFrame的网站作为交互式校样生成（iFrame嵌入限制由您尝试嵌入的网站控制）。</p> <p>创建初始校样后，在创建后续版本时无法更改此设置。</p> <p>有关交互式校对的更多信息，请参阅 <a href="#generate-a-proof-for-interactive-content" class="MCXref xref">为交互式内容生成校样</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">屏幕截图分辨率</td> 
      <td> <p>（此选项不适用于交互式校样。） 您可以调整内容所显示的分辨率，也可以选择多个分辨率。</p> <p>这样，用户便可以查看校样以查看内容在不同设备（如各种大小的手机、平板电脑和显示器）上的显示方式。</p> <p>如果选择多个分辨率，则会为您选择的每个分辨率创建单独的校样。</p> <p>当用户对校样进行注释时，当前屏幕分辨率会自动显示在注释中，以确保其他用户了解该注释关联的分辨率。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">查找子页面</td> 
      <td>（此选项不适用于交互式校样。） 选择此选项可在网站的各个页面之间导航。 您可以将网站从主页的深度扩展到2个级别。 将鼠标悬停在页面上可查看页面的URL。 仅选择要校样的页面。 默认情况下，您选择的每个页面都将作为单个校样创建；或，启用 <strong>合并到单个校样中</strong> 选项，将所有选定页面合并到一个校样中。</td> 
     </tr> 
    </tbody> 
   </table>

1. （可选）配置任何高级校对选项，例如共享校样、添加自动工作流，或设置访问和订阅设置。 有关这些选项的更多详细信息，请参阅以下文章：

   * [在中共享校样 [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [在中使用自动工作流设置校样 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md)
   * [配置校样的访问和订阅设置](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. 单击 **[!UICONTROL 完成]**.

   如果向现有URL校样添加新版本，则在原始校样或以前版本上配置的任何选项都将保留在此版本中。如果向现有URL校样添加新版本，则在原始校样或以前版本上配置的任何选项都将在此版本中保留。

1. 单击 **[!UICONTROL 创建校样]**.

## 为交互式内容生成校样 {#generate-a-proof-for-interactive-content}

使用此功能需要专业Workfront计划或更高版本。 有关各种可用计划的更多信息，请参阅 [Workfront计划](https://www.workfront.com/plans).

有关交互式内容的更多信息，请参阅 [交互式内容校样概述](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

* [将交互式内容添加为URL](#add-interactive-content-as-a-url)
* [将交互式内容添加为ZIP文件](#add-interactive-content-as-a-zip-file)

### 将交互式内容添加为URL {#add-interactive-content-as-a-url}

有关如何添加交互式URL校样的信息，请参阅  [为URL生成校样](#generate-a-proof-for-a-url).

### 将交互式内容添加为ZIP文件 {#add-interactive-content-as-a-zip-file}

1. 通过创建捆绑的.zip文件来准备内容。

   有关.zip捆绑文件规范的信息，请参阅 [关于在ZIP文件中准备交互式内容以进行校对](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md#howtoprepareaninteractiveziparchive) 在文章中 [交互式内容校样概述](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. 执行以下任一操作，以开始创建新校样并显示 [!UICONTROL 新校样] 页面：

   * 单击绿色 **[!UICONTROL 新校样]** 按钮。
   * 在 **[!UICONTROL 功能板]** 区域，在 **[!UICONTROL 概述]** ，单击 **[!UICONTROL 新校样]** 链接。

   * 通过Dropzone提交（企业功能）。

1. 在 **[!UICONTROL 新校样]** 页面，将您的交互式.zip包拖放到 **[!UICONTROL 添加文件]** 的上界。

1. （可选）配置任何高级校对选项，例如共享校样、添加自动工作流，或设置访问和订阅设置。 有关这些选项的更多详细信息，请参阅以下文章：

   * [在中共享校样 [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * 在文章中
   * [配置校样的访问和订阅设置](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. 单击 **[!UICONTROL 创建校样]**.

   Workfront开始生成.zip包的校样。 根据包大小，文档上传的滞后时间会有所不同。 生成较大的文件需要更长的时间。 您可以从页面导航到其他位置，Workfront将继续生成您的文件。 最大文件上传大小为4 GB。

   在生成校样后，您可以单击 **[!UICONTROL 转到校样]** 按钮来打开校样。
