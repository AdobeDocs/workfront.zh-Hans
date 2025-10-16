---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 使用Workfront Fusion创建具有Adobe Experience Manager工作流的Workfront项目
description: 如果您通过Workfront Fusion创建项目并希望在项目上包含Adobe Experience Manager工作流，则必须使用特定的Fusion模块配置，如本文所述。
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps, Workfront Fusion
exl-id: b8132d5e-234d-47f6-a09c-ca46018a2d77
source-git-commit: 6a21465ab8c92888c83344f33574302c5cc446e8
workflow-type: tm+mt
source-wordcount: '877'
ht-degree: 0%

---

# 使用Workfront Fusion将Workfront问题转换为包含Adobe Experience Manager工作流的项目

如果您通过Workfront Fusion创建项目并希望在项目上包含Adobe Experience Manager工作流，则必须使用特定的Fusion模块配置，如本文所述。

>[!NOTE]
>
>工作流仅在Adobe Experience Manager as a Cloud Service集成中可用。 它们不可用于与Adobe Experience Manager Assets Essentials的集成。


## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table>
  <tr>
    <td><strong>Adobe Workfront包</strong></td>
   <td> <p>任何Adobe Workfront Workflow包和任何Adobe Workfront自动化和集成包</p><p>Workfront Ultimate</p><p>Workfront Prime和Select包，以及额外购买的Workfront Fusion。</p> </td> 
  </tr>
  <tr>
   <td><strong>Adobe Workfront许可证</strong></td>
   <td><p>参与者或更高版本</p><p>请求或更高版本</p></td>
  </tr>
  <tr>
   <td><strong>产品</strong></td>
   <td>
     <p><b>Adobe Experience Manager：</b></p>
     <ul>
       <li>
         <p>您必须安装了Experience Manager Assets as a Cloud Service或Assets Essentials，并且您必须作为用户添加到Admin Console的产品中。</p>
       </li>
       <li>
        <p>您必须对Adobe Experience Manager中的存储库具有写入权限。</p>
       </li>
     </ul>
     <p><b>Workfront Fusion：</b></p>
     <ul>
       <li>
        <p>如果贵组织具有不包含Workfront Automation and Integration的Select或Prime Workfront包，则贵组织必须购买Adobe Workfront Fusion。</li></ul>
       </li>
     </ul>
   </td>
  </tr>
  <tr>
   <td><strong>访问级别配置</strong>
   </td>
   <td><p>编辑对文档的访问权限</p>
   </td>
  </tr>
</table>

+++

## 先决条件

开始之前，

* 您的Workfront管理员必须在Adobe Experience Manager集成中配置工作流。 有关详细信息，请参阅[配置Experience Manager Assets as a Cloud Service集成](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional)。
* 您必须使用Adobe Experience Manager集成链接文件夹工作流配置项目模板。
* 您必须在Workfront中创建OAuth应用程序才能配置此模块的连接。

  有关说明，请参阅本文中的[创建OAuth应用程序](#create-an-oauth-application)。

## 模块配置

在Workfront Fusion中，如果要创建包含Adobe Experience Manager工作流的项目，则必须使用Workfront >杂项操作模块。

1. 将&#x200B;**Workfront** > **杂项操作**&#x200B;模块添加到您的方案。
1. 在&#x200B;**连接**&#x200B;字段中，选择连接到此模块将使用的帐户的Workfront连接。

   有关创建连接的说明，请参阅Workfront模块一文中的[连接 [!DNL Workfront] 到 [!DNL Workfront Fusion]](https://experienceleague.adobe.com/zh-hans/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-modules#connect-workfront-to-workfront-fusion)。

   有关创建客户端ID和客户端密钥的说明，您将需要创建连接，请参阅本文中的[创建OAuth应用程序](#create-an-oauth-application)。

1. 在&#x200B;**记录类型**&#x200B;字段中，选择`Issue`。
1. 在&#x200B;**操作**&#x200B;字段中，选择`convertToProject`。
1. 在&#x200B;**ID**&#x200B;字段中，输入或映射要转换为项目的问题的ID。
1. 启用&#x200B;**显示高级设置**。
1. 滚动到模块的底部，并找到&#x200B;**项目（高级集合）**&#x200B;字段。
1. 将以下文本粘贴到&#x200B;**项目（高级收藏集）**&#x200B;字段中。

   ```
   {
       "aemNativeFolderTreeIDs": ["Folder Tree ID here"],
       "aemNativeFolderWorkflowEnabled": "true",
       "name": "New project name here",
       "templateID": "Template ID here"
   }
   ```

1. 将`Folder tree ID here`替换为文件夹ID。

   要查找文件夹树ID，请参阅本文中的[查找文件夹树ID](#locate-folder-tree-ids)。

   要使用多个文件夹树，请使用逗号分隔ID：

   `"aemNativeFolderTreeIDs": ["Folder tree ID here","Second folder tree ID here"],`
1. 将`New project name here`替换为新项目将具有的名称。
1. 将`Template ID here`替换为您用于新项目的模板的ID。

   您可以映射上一个模块(如Workfront >搜索模块)中的模板ID，或在Workfront中模板页面的URL中找到它。

1. 单击&#x200B;**确定**&#x200B;以保存模块配置。

## 查找文件夹树ID

要查找文件夹树ID，请执行以下操作：

>[!NOTE]
>
>这些说明使用Chrome浏览器。

1. 在Workfront中，打开要用于此项目的模板。 此模板必须包含要用于项目的Adobe Experience Manager配置。
1. 打开浏览器的开发人员工具。
1. 在开发人员工具中打开&#x200B;**网络**&#x200B;选项卡。
1. 在&#x200B;**筛选器**&#x200B;框中，输入`object-workflow`。
1. 在“名称”列中，单击显示的字母数字ID。

   ![查找文件夹ID 1](assets/finding-folder-id-1.png)

1. 单击字母数字ID右侧的&#x200B;**预览**&#x200B;选项卡。
1. 打开以下折叠的部分：
   1. `data`
   1. `objectWorkflow`
   1. `workflows`
   1. `enhancedLinkedFolderCreationWorkflow`
   1. `enhancedLinkedFolderCreationWorkflowConfigurations`

   每个文件夹树都由一个数字表示。 0（零）表示列表中的第一个文件夹，1表示第二个文件夹，依此类推。 如果模板只包含一个文件夹树，则其值为0。

1. 打开要用于新项目的文件夹树。 记下`_id`字段值。 如果要使用多个文件夹树，请记下要使用的文件夹树的所有`_id`字段值。

   ![查找文件夹ID 2](assets/finding-folder-id-2.png)

   在`aemNativeFolderTreeIDs`Workfront **>**&#x200B;其他操作&#x200B;**Fusion模块的**&#x200B;项目（高级收藏集）**字段中，您将输入这些**&#x200B;值。

## 创建OAuth应用程序

您必须在Workfront中为此模块的连接设置OAuth应用程序。 您只需对Fusion中的给定Workfront连接执行一次此操作。

1. 在Workfront中，开始创建OAuth应用程序，如文章为[集成创建OAuth2应用程序中的](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-application-using-user-credentials-authorization-code-flow)使用用户凭据（授权代码流）[!DNL Workfront]创建OAuth2应用程序中所述。
1. 将客户端ID和客户端密钥复制到安全位置。
1. 在&#x200B;**重定向URI**&#x200B;字段中，输入以下内容：

   ```
   http://app.workfrontfusion.com/oauth/cb/workfront-workfront
   ```

1. 单击&#x200B;**保存**。

在Fusion中配置模块的连接时，您将使用此客户端ID和客户端密钥。

有关创建连接的说明，请参阅Workfront模块一文中的[连接 [!DNL Workfront] 到 [!DNL Workfront Fusion]](https://experienceleague.adobe.com/zh-hans/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-modules#connect-workfront-to-workfront-fusion)。
