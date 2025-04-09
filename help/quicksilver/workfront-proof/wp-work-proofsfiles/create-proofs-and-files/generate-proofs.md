---
product-previous: workfront-proof
product-area: documents
navigation-topic: create-proofs-and-files
title: 在 [!DNL Workfront Proof]中生成验证
description: Workfront Proof允许您从文档或网站创建验证，并与他人共享这些验证。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 49657851-2948-4d3b-b2ce-c8359eeb315b
source-git-commit: 1443551b605dac6e53531c5d445b89517384fe11
workflow-type: tm+mt
source-wordcount: '1889'
ht-degree: 2%

---

# 在[!DNL Workfront Proof]中生成验证

<!-- Audited: 4/2025 -->

>[!IMPORTANT]
>
>本文提及独立产品[!DNL Workfront Proof]中的功能。 有关[!DNL Adobe Workfront]内部校对的信息，请参阅[校对](../../../review-and-approve-work/proofing/proofing.md)。

[!DNL Workfront Proof]允许您从文档或网站创建校样，并与他人共享这些校样。 以下步骤描述了可用的各种配置选项：

## 从文档生成验证

1. 执行以下操作之一以打开&#x200B;**[!UICONTROL 新验证]**&#x200B;页面：

   * 单击任何页面左上角的&#x200B;**[!UICONTROL 新验证]**&#x200B;按钮。
   * 通过Dropzone（企业功能）提交。

1. 要校对一个或多个文档，请通过以下任一方式添加要校对的文档（重复此过程以添加多个文档）：

   * 将文档从文件系统拖放到&#x200B;**[!UICONTROL 添加文件]**&#x200B;区域的拖放区域。
   * 在&#x200B;**[!UICONTROL 添加文件]**&#x200B;区域中，单击&#x200B;**浏览**&#x200B;链接以查找并选择要从工作站上的文件系统上传的文档。

     ![proof_document_upload.png](assets/proof-document-upload-350x64.png)

1. 要校对网站，请在&#x200B;**[!UICONTROL 添加文件]**&#x200B;区域输入网站的URL，然后按&#x200B;**[!UICONTROL Enter]**。 重复此步骤以添加多个要验证的网站。

   有关校对网站的更多详细信息，请参阅[为URL生成校对](#generate-a-proof-for-a-url)。

   ![校对网站](assets/proof-website-350x65.png)

1. （可选）修改任何已上载文件的文件名：

   1. 在文档列表中，将鼠标悬停在要修改的文档名称上，然后单击&#x200B;**[!UICONTROL 编辑]**&#x200B;图标。

      ![proof_edit.png](assets/proof-edit-350x53.png)

   1. 在&#x200B;**[!UICONTROL 校对名称]**&#x200B;字段中，指定新名称，然后单击&#x200B;**[!UICONTROL 完成]**。

   1. （可选）若要删除上传的任何文件，请将鼠标悬停在文档列表中要删除的文档上，然后单击&#x200B;**[!UICONTROL 删除]**&#x200B;图标。

      ![proof_delete.png](assets/proof-delete-350x53.png)

   1. （可选）启用&#x200B;**[!UICONTROL 将所有兼容的文件合并为单个校对]**&#x200B;选项。

      **启用此选项时：**&#x200B;所有静态文件和网站都在一个验证中可用，您最多可以在给定时间上传50个文件。

      >[!NOTE]
      >
      >交互式文件（包括视频和交互式网站）无法合并为单个验证。

      **禁用此选项时：**&#x200B;所有文档和网站都作为单个校样生成，您最多可以在给定时间上传20个文件。

      要将所有上传的文件和网站合并到一个验证中，请执行以下操作：

      1. 启用&#x200B;**[!UICONTROL 将所有兼容的文件合并为单个校对]**&#x200B;选项。
      1. 在&#x200B;**[!UICONTROL 验证名称]**&#x200B;字段中，为组合验证输入新名称。
      1. 在&#x200B;**[!UICONTROL 添加文件]**&#x200B;区域，通过将文件拖到所需顺序来重新排序包含的文件。 文件的顺序是组合验证的页面顺序。 有关创建组合验证的更多信息，请参阅[创建多页验证](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md)。

1. （可选）如果要使用包括多个阶段的自动工作流，请从&#x200B;**[!UICONTROL 工作流]**&#x200B;部分中选择以下选项：

   * **基本：**&#x200B;选择此选项可指定希望在校对创建后立即访问校对的用户。 您可以与多个用户共享验证。

     有关共享校样的更多信息，请参阅[在 [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)内共享校样。

   * **自动：**&#x200B;选择此选项可在您拥有复杂的审阅流程，或定期将内容发送给同一组人员审阅时，管理内容审阅和批准。 借助自动化工作流，验证会从一个阶段移动到另一个阶段，直至最终批准。 相关用户可随时收到需要批准的通知。

     有关创建自动工作流的详细信息，请参阅[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md#create2)中设置具有自动工作流的验证。

1. 选择是否向在上一步中选择的用户发送电子邮件通知和自定义消息：

   * **将此验证通知收件人：**&#x200B;选择此选项可向用户发送电子邮件通知。 在&#x200B;**[!UICONTROL 工作流]**&#x200B;部分中选择&#x200B;**[!UICONTROL 基本共享]**&#x200B;时，会在创建验证时发送电子邮件通知。 在&#x200B;**[!UICONTROL 工作流]**&#x200B;部分中选择&#x200B;**[!UICONTROL 自动化工作流]**&#x200B;时，当验证进入用户关联的自动化工作流的阶段时，将发送电子邮件通知。

   * **添加自定义消息：**&#x200B;选择此选项可在通知中包含自定义消息。 您可以指定主题和消息正文。 消息正文可以包括富文本格式，例如粗体、项目符号和超链接。

1. 选择以下任何验证设置：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">需要登录。 此校对无法与其他用户共享</td> 
      <td> <p>选中此选项时：</p> 
       <ul> 
        <li>用户无法登录验证进行查看，除非已将他们添加到验证中。</li> 
        <li>无法启用订阅。</li> 
       </ul> 
       <p>默认禁用此选项。</p> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">要求对决策进行电子签名</td> 
      <td><p>如果选择该选项，用户必须在做出验证决策时指定用户名和密码。</p>
      <p>默认禁用此选项。</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">作出所有必需的决策时锁定验证</td> 
      <td> <p>启用此设置后，将在做出所有决策后锁定验证状态。 当最终批准者做出决定时，状态会自动从已解锁更改为已锁定。</p> 
      <p>默认禁用此选项。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允许下载原文件</td> 
      <td> <p><strong></strong> 选择此选项后，审阅人将能够下载从中创建验证的原始文件。</p> <p>取消选择此选项时，“下载”图标不再可见。</p>
      <p>此选项默认处于启用状态。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允许通过公共 URL 或嵌入代码共享证明</td> 
      <td><p>选择此选项后，可以通过公共URL或嵌入代码共享验证。</p>
       <p>此选项默认处于启用状态。</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允许通过公共URL或嵌入代码订阅验证</td> 
      <td> <p>选择此选项后，尚未添加到验证的用户可以订阅验证。 订阅验证的用户将获得您在以下设置中定义的角色和电子邮件：</p> 
       <ul> 
        <li><strong>订阅者角色</strong>：分配给订阅了验证的所有审阅人的默认验证角色。</li> 
        <li><strong>订阅者的电子邮件警报设置</strong>：分配给订阅验证的所有审阅者的默认电子邮件警报。</li> 
        <li> <p><strong>通过电子邮件链接访问</strong>所需的校对：配置订阅者是否收到包含校对链接的电子邮件。 您可以选择<strong>无电子邮件</strong> （访问验证不需要电子邮件链接）、<strong>仅验证通知电子邮件</strong> （订阅者通过电子邮件接收验证链接，无需任何验证）或<strong>验证和验证通知电子邮件</strong> (订阅者通过电子邮件接收验证链接，必须单击该链接才能访问验证。 此选项的目的是确保人员输入了他们有权访问的正确电子邮件地址)。</p> <p>注意：如果验证附加了自动工作流，则所有订阅都将向验证所有者生成确认电子邮件，以便他们决定应将人员添加到哪个阶段。</p> </li> 
       </ul> 
        <p>默认禁用此选项。</p>
       </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**[!UICONTROL 创建校对]**。 Workfront生成选定文档或网站的验证。

   文档上传的滞后时间因文件大小和类型而异。 生成较大的文件需要较长时间。 在Workfront继续生成文件时，您可以导航离开页面。 最大文件上传大小为4GB。

## 使用URL生成静态校对 {#generate-a-proof-for-a-url}

您可以使用网站URL生成静态校对。

>[!NOTE]
>
>仅当您的[!DNL Workfront]环境与[!DNL Workfront Proof] Premium帐户集成时，才能为URL生成交互式验证。 如果您无法使用本节中讨论的验证，请与Workfront管理员联系。

1. 执行以下操作之一以打开&#x200B;**[!UICONTROL 新验证]**&#x200B;页面：

   * 单击任何页面左上角的&#x200B;**[!UICONTROL 新验证]**&#x200B;按钮。
   * 通过Dropzone（企业功能）提交。

1. 在&#x200B;**新建校对**&#x200B;页面中，在&#x200B;**[!UICONTROL 添加文件]**&#x200B;区域输入您要创建校对的网站的URL，然后按键盘上的&#x200B;**[!UICONTROL Enter]**&#x200B;或&#x200B;**[!UICONTROL Return]**。

1. （可选）重复此过程以将多个网站添加到验证中。

   ![proof_website.png](assets/proof-website-350x65.png)

1. 在&#x200B;**[!UICONTROL 添加文件]**&#x200B;区域中，单击URL右侧的&#x200B;**编辑**&#x200B;图标以打开网站校对详细信息。

   ![proof_upload_website_modify.png](assets/proof-upload-website-modify-350x185.png)

1. 输入&#x200B;**[!UICONTROL 校对名称]**。 默认情况下，验证名称与网站URL相同。

1. 选择以下&#x200B;**[!UICONTROL 处理网站内容]**&#x200B;选项中的任意一个：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">捕获屏幕快照</td> 
      <td>创建URL头页的静态图像的校对。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">交互型</td> 
      <td> <p>创建一个校样，允许审阅人导航站点、查看HTML5图像、Flash元素等。</p> <p>要创建交互式验证，必须使用安全协议(https)托管网站。 此外，无法嵌入到iframe中的网站无法生成为交互式验证（iframe嵌入限制由您尝试嵌入的网站控制）。</p> <p>创建初始验证后，创建后续版本时无法更改此设置。</p> <p>有关交互式校对的更多信息，请参阅<a href="#generate-a-proof-for-interactive-content" class="MCXref xref">为交互式内容生成校对</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">屏幕快照分辨率</td> 
      <td> <p>（此选项不适用于交互式验证。） 您可以调整内容显示所用的分辨率，也可以选择多个分辨率。</p> <p>这使用户能够查看验证以查看内容在不同设备上的显示方式，例如各种尺寸的电话、平板电脑和显示器。</p> <p>如果选择多个分辨率，则会为您选择的每个分辨率创建单独的校样。</p> <p>当用户对验证进行评论时，当前屏幕分辨率自动显示在评论中，以确保其他用户知道评论关联的分辨率。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">查找子页面</td> 
      <td>（此选项不适用于交互式验证。） 选择此选项可导航浏览网站的页面。 您可以将网站从主页扩展到深2层。 将鼠标悬停在页面上可查看该页面的URL，并仅选择您要验证的页面。 默认情况下，您选择的每个页面都将作为单独的验证创建。 或者，您可以启用<strong>将所有兼容的文件合并为单个校对</strong>选项。</td> 
     </tr> 
    </tbody> 
   </table>

1. （可选）配置任何高级验证选项，例如共享验证、添加自动工作流或设置访问和订阅设置。 有关这些选项的更多详细信息，请参阅以下文章：

   * [在 [!DNL Adobe Workfront]内共享验证](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [在 [!DNL Workfront Proof]中设置具有自动工作流的验证](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md)
   * [配置验证的访问和订阅设置](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. 单击&#x200B;**[!UICONTROL 完成]**。

1. 单击&#x200B;**[!UICONTROL 创建校对]**。

## 为交互式内容生成验证 {#generate-a-proof-for-interactive-content}

<!--A Pro Workfront Plan or higher is required to use this feature. For more information about the various plans available, see [Workfront Plans](https://www.workfront.com/plans).-->

有关交互式内容的详细信息，请参阅[交互式内容校对概述](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md)。

* [将交互式内容添加为URL](#add-interactive-content-as-a-url)
* [将交互式内容添加为ZIP文件](#add-interactive-content-as-a-zip-file)

### 将交互式内容添加为URL {#add-interactive-content-as-a-url}

有关如何添加交互式URL校对的信息，请参阅[生成URL的校对](#generate-a-proof-for-a-url)。

### 将交互式内容添加为ZIP文件 {#add-interactive-content-as-a-zip-file}

1. 通过创建.zip捆绑文件来准备内容。

   有关.zip捆绑文件规范的信息，请参阅[交互式内容校对概述](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md)。

1. 执行以下操作之一以打开&#x200B;**[!UICONTROL 新验证]**&#x200B;页面：

   * 单击任何页面左上角的&#x200B;**[!UICONTROL 新验证]**&#x200B;按钮。
   * 通过Dropzone（企业功能）提交。

1. 在&#x200B;**[!UICONTROL 新验证]**&#x200B;页面中，将交互式.zip包拖放到&#x200B;**[!UICONTROL 添加文件]**&#x200B;区域。

1. （可选）配置任何高级验证选项，例如共享验证、添加自动工作流或设置访问和订阅设置。 有关这些选项的更多详细信息，请参阅以下文章：

   * [在 [!DNL Adobe Workfront]内共享验证](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [配置验证的访问和订阅设置](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. 单击&#x200B;**[!UICONTROL 创建校对]**。 Workfront会生成一个zip文件验证。

   文档上传的滞后时间因zip文件大小而异。 在Workfront继续生成文件时，您可以导航离开页面。 最大文件上传大小为4GB。
