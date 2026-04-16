---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: 将费率更改推送到项目
description: 费率卡表示与客户签订的合同协议，合同中为完成工作的工作角色定义了每小时的费率。 在费率卡中，您可以根据属性为每个工作角色定义多个记帐费率。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c38e60dd-7fb2-4afc-976a-b0966398c162
source-git-commit: c27dd9d972b89af09c0865a0e878f1665416c80e
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 6%

---

# 将费率更改推送到项目

将费率卡附加到项目<!--or a staffing plan-->时，费率卡上的费率仍可调整。 然后，您可以选择将这些费率推送到费率卡附加到的项目<!--and staffing plans -->。 如果不推送新费率，则原始费率将保留在项目<!-- or staffing plan-->上。

有关将费率卡附加到项目的信息，请参阅[将费率卡附加到项目](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 包</td> 
   <td>工作流 Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 许可证</td> 
   <td>[!UICONTROL 标准版]</td>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>编辑对[!UICONTROL 费率卡]的访问权限</td> 
  </tr> 
  <tr> 
   <td>对象权限</td> 
   <td>要编辑与您共享的费率卡，您必须拥有费率卡的管理权限。</td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 将费率更改推送到项目

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;[!UICONTROL **费率卡**]。
1. 在“费率卡”列表中单击费率卡的名称。
1. 在费率卡>工作角色和费率屏幕上，验证费率是否正确，并根据需要编辑任何费率。
1. 单击&#x200B;[!UICONTROL **推送更改**]。
1. 在&#x200B;[!UICONTROL **应用于所有项目**]<!--/staffing plans-->&#x200B;对话框中，默认情况下选择使用此费率卡的所有项目<!--and staffing plans -->。 如果不希望项目<!--or staffing plan -->应用费率更改，则必须取消选择该项目。
1. 单击&#x200B;[!UICONTROL **保存**]。

   新费率现在反映在使用费率卡的项目<!--and staffing plans -->上。
