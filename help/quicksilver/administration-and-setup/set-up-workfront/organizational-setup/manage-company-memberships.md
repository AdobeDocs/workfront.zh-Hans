---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: 管理公司成员资格
description: 在“设置”的[!UICONTROL 公司]区域中，您可以添加和删除公司成员。 您还可以编辑其用户配置文件，提醒他们在 [!DNL Workfront], deactivate them in [!DNL Workfront], and remove them from the [!DNL Workfront] 系统中注册。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f0efd985-76e3-435e-bf19-87008f6a5e9d
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '872'
ht-degree: 1%

---

# 管理公司成员资格

在[!UICONTROL 设置]的[!UICONTROL 公司]区域，您可以添加和删除公司成员。 您还可以编辑其用户配置文件，提醒他们在[!DNL Workfront]中注册，在[!DNL Workfront]中停用它们，并从[!DNL Workfront]系统中删除它们。

有关创建新公司的信息，请参阅[创建和编辑公司](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto">
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] 计划</p> </td> 
   <td><p>当前： [!UICONTROL 团队]或更高版本</p>
   <p>或</p>
   <p>新建：任何</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] 许可证</p> </td> 
   <td><p>当前： [!UICONTROL 计划]</p>
   <p>或</p>
   <p>新文档： [!UICONTROL Standard]</p>
   </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>访问级别配置</strong> </td> 
   <td> <p>下列选项之一：</p> 
    <ul> 
     <li> <p>[!UICONTROL 系统管理员]访问级别，允许您编辑系统中的任何公司。</p> </li> 
     <li> <p>管理公司的管理权限，允许您编辑系统中的任何公司。</p> </li> 
    </ul> <p><b>注释</b>：  
     <ul> 
      <li> <p>您还可以管理与您被分配为组管理员的任何组关联的公司。</p> </li> 
      <li> <p>若要在[!DNL Workfront]系统中添加和删除用户，您必须具备以下任一项：</p> 
       <ul> 
        <li> <p>[!UICONTROL 系统管理员]访问级别。</p> </li> 
        <li> <p>在访问级别中，必须为[!UICONTROL 用户]设置选择[!UICONTROL 编辑] 。 此外，对于[!UICONTROL 用户]设置，在[!UICONTROL 微调设置] <img src="assets/gear-icon-in-access-levels.png">下，必须启用[!UICONTROL 创建]选项以及两个[!UICONTROL 用户管理]选项中的至少一个。 </p> <p> <img src="assets/access-req-users.png"> </p> <p>如果您使用[!UICONTROL 用户管理员（组用户）]选项，您必须是用户所属组的组管理员。</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 管理公司成员资格

{{step-1-to-setup}}

1. 单击&#x200B;**[!UICONTROL 公司]**。
1. 单击公司名称。
1. 在左侧面板中选择了&#x200B;**[!UICONTROL 公司成员]**&#x200B;部分，执行以下任一操作：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">添加成员</td> 
      <td> <p>单击<b>[!UICONTROL 添加成员]</b>，然后在显示的下拉菜单中选择以下选项之一：</p> 
       <ul> 
        <li> <p><b>[!UICONTROL 新用户]</b>：添加尚未添加到[!DNL Workfront]的用户。</p> <p>有关将用户添加到[!DNL Workfront]的信息，请参阅<a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">添加用户</a>和<a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">编辑用户的配置文件</a>。</p> </li> 
        <li> <p><b>[!DNL Existing user]</b>：添加系统中已存在但您有权编辑的用户。</p> <p><b>重要信息</b>：如果用户已经是其他公司的成员，则新分配将覆盖旧分配。 用户将失去对与前公司共享项目的访问权限，并将获得对与此公司共享项目的访问权限。</p> </li> 
        <li> <p><b>[!UICONTROL 导入用户]</b>：通过上传电子表格导入文件来导入用户。 有关详细信息，请参阅<a href="../../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">导入用户</a>。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">编辑成员</td> 
      <td> 
       <ol> 
        <li value="1"> <p>至少选择一个用户，然后单击工具栏中的[!UICONTROL 编辑]图标<img src="assets/edit-icon.png">。</p> </li> 
        <li value="2"> <p>在显示的<b>[!UICONTROL Edit User]</b>框中配置选项。</p> <p>有关这些选项的信息，请参阅<a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">编辑用户的配置文件</a>。</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">复制成员</td> 
      <td> <p>您可以通过复制现有公司成员来创建公司成员。 </p> <p><b>注释</b>：  <p>以这种方式创建用户时，除以下内容外，所有信息都将从原始用户复制到新创建的用户：</p> 
        <ul> 
         <li>[!UICONTROL 个人信息]部分中的信息。</li> 
         <li>[!UICONTROL 登录时，显示]：此框中选择了访问级别的默认登录选项卡。</li> 
         <li>[!UICONTROL 直接报告]</li> 
        </ul> </p> 
       <ol> 
        <li value="1"> <p>选择用户，然后单击[!UICONTROL 复制]图标<img src="assets/copy-icon.png">。 </p> </li> 
        <li value="2"> <p>在显示的<b>[!UICONTROL 新用户]</b>框中，编辑新用户可用的字段。</p> <p>有关与用户关联的所有字段的信息，请参阅<a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">编辑用户配置文件</a>。</p> </li> 
        <li value="3"> <p>单击<strong>[!UICONTROL 添加此用户]</strong>。</p> <p>或</p> <p>单击<strong>[!UICONTROL Add Person User &amp; Start Another]</strong>保存新用户并添加另一个用户。</p> </li> 
       </ol> <p>这会在[!DNL Workfront]中为用户创建一个新帐户。</p> <p>如果选择向用户发送邀请的选项，用户应会收到一封电子邮件，并在其中单击链接以创建其[!DNL Workfront]密码。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">删除用户</td> 
      <td> 
       <div> 
        <p>至少选择一个用户，单击<b>[!UICONTROL 删除用户]</b>，然后在显示的下拉菜单中选择以下选项之一：</p> 
        <ul> 
         <li> <p><b>[!UICONTROL 从公司中删除]</b>：从公司中删除一个或多个用户。</p> </li> 
         <li> <p><b>[!UICONTROL Delete]</b>：从[!DNL Workfront]系统中删除一个或多个用户。</p> <p><b>重要信息</b>：从系统中删除用户也会删除与您可能希望保留的用户相关联的信息。 我们建议停用而不是删除用户。 有关详细信息，请参阅<a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">停用或重新激活用户</a>。</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">向用户及其[!UICONTROL 更新]区域发送评论</td> 
      <td> 
       <ol> 
        <li value="1"> <p>至少选择一个用户，然后单击工具栏中的[!UICONTROL 注释]图标<img src="assets/comment-icon.png">。</p> </li> 
        <li value="2"> <p>键入要发送给用户及其用户配置文件的[!UICONTROL 更新]区域的注释。</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">导出公司成员列表</td> 
      <td> <p>单击工具栏中的[!UICONTROL 导出]图标<img src="assets/export.png">，然后为导出的文件选择所需的格式。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">停用系统中的成员</td> 
      <td> <p>至少选择一个用户，单击工具栏中的[!UICONTROL 更多]图标<img src="assets/more-icon.png">，然后选择<b>[!UICONTROL 停用]</b>。</p> <p>有关详细信息，请参阅<a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">停用或重新激活用户</a>。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">提醒用户在系统中注册</td> 
      <td> <p> 在<b>[!UICONTROL Name]</b>列中，<b>[!UICONTROL 已取消注册]</b>显示在每个已取消注册用户的名称旁边。 要提醒这些用户在系统中注册，请选择这些用户，单击工具栏中的[!UICONTROL 更多]图标<img src="assets/more-icon.png">，然后选择<b>[!UICONTROL 提醒用户注册]</b>。</p> </td> 
     </tr> 
    </tbody> 
   </table>
