---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「群組：Portfolio擁有者、方案擁有者、專案擁有者和專案狀態的4層級任務群組」
description: 此作業「群組」提供4個層次的「群組」。 在此情況下，任務會依Portfolio擁有者、方案擁有者、專案擁有者和專案狀態分組。 使用標準介面，您最多只能有3個層次的「群組」。 若要新增第四個層級，您必須使用「文字模式」。 您無法同時依4個以上的條件將報表分組。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a1780a57-b94c-4d3a-b526-9bf45dba21f1
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# 群組：Portfolio擁有者、方案擁有者、專案擁有者和專案狀態的4層級作業群組

此作業「群組」提供4個層次的「群組」。 在此情況下，任務會依Portfolio擁有者、方案擁有者、專案擁有者和專案狀態分組。 使用標準介面，您最多只能有3個層次的「群組」。 若要新增第四個層級，您必須使用「文字模式」。 您無法同時依4個以上的條件將報表分組。

![four_tier_grouping_for_tasks.png](assets/four-tier-grouping-for-tasks-350x239.png)

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>請求修改群組 </p>
   <p>計畫修改報告</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯對篩選器、檢視、群組的存取權以修改群組</p> <p><b>注释</b>

如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 為Portfolio擁有者、方案擁有者、專案擁有者和專案狀態建立4層級任務群組

若要套用此群組：

1. 前往工作清單。
1. 從 **分組** 下拉式功能表，選取 **新群組**.

1. 按一下&#x200B;**切換至文字模式**.
1. 移除 **將報表分組** 區域。
1. 將文字取代為下列程式碼：

   <pre>group.0.linkedname=project<br>group.0.name=Portfolio擁有者<br>group.0.notime=false<br>group.0.valuefield=project:portfolio:owner：name<br>group.0.valueformat=string<br>group.1.linkedname=project<br>group.1.name=程式所有者<br>group.1.notime=false<br>group.1.valuefield=project:program:owner：name<br>group.1.valueformat=string<br>group.2.linkedname=projectOwnerMM<br>group.2.listgrouingparsedmethod=nested(project)。nested(owner)。string(name)<br>group.2.namekey=projectownermm<br>group.2.notime=false<br>group.2.valuefield=projectOwnerMM：name<br>group.2.valueformat=string<br>group.3.enumclass=com.attask.common.constants.ProjectStatusEnum<br>group.3.linkedname=project<br>group.3.namekey=view.relatedcolumn<br>group.3.namekeyargkey.0=專案<br>group.3.namekeyargkey.1=status<br>group.3.notime=false<br>group.3.valuefield=project：status<br>group.3.valueformat=val</pre>

1. 按一下 **儲存群組**.
