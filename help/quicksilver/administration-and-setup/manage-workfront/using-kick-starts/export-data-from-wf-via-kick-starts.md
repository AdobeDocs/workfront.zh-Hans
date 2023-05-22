---
user-type: administrator
product-area: system-administration
keywords: kickstart，kick-start，kickstarts，kick-starts
navigation-topic: use-kick-starts
title: 透過Kick-Starts從Adobe Workfront匯出資料
description: 身為Adobe Workfront管理員，您可以使用Kick-Starts資料匯出工具從Workfront匯出資料。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7f56b63e-a674-43e4-bef6-d276898e2074
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '1101'
ht-degree: 9%

---

# 透過Kick-Starts從Adobe Workfront匯出資料

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

身為Adobe Workfront管理員，您可以使用Kick-Starts資料匯出工具從Workfront匯出資料。 匯出後即可在其他應用程式中使用。

透過Kick-Starts匯出資料也有助於瞭解哪些欄位與每個物件相關聯、這些欄位的編碼方式，以及這些欄位的值在資料庫中的格式化。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>：如果您還是沒有存取權，請洽詢Workfront管理員，瞭解他們是否對您的存取層級設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 使用kick-start匯出資料的優缺點

在Workfront中匯出資料有兩種方式：

* 從報表或清單匯出資料

   如需從報表或清單匯出資料的詳細資訊，請參閱 [匯出資料](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

* 透過Kick-Start匯出資料

下表顯示每種方法的優缺點：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>  </th> 
   <th> <p>匯出的資料包含物件和欄位值</p> </th> 
   <th> <p>可同時匯出多個物件型別周圍的資料</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>從清單檢視匯出資料</strong> </p> <p>如需從清單匯出資料的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">匯出資料</a></p> </td> 
   <td> <p>是</p> <p>會匯出與物件相關聯的Workfront原生欄位和自訂欄位。</p> </td> 
   <td> <p>否</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>透過Kick-Start匯出資料</strong> </p> </td> 
   <td> <p>是（受限）</p> <p>大部分與物件相關聯的Workfront原生欄位都會匯出，但有些則不會。 例如，您無法透過專案快速啟動匯出來匯出排程、專案所有者或專案贊助者欄位。</p> <p>在附加了自訂表單的專案中，在表單上的欄位中輸入的任何資料都不會匯出。</p> <p>但您可以匯出自訂表單。 產生的檔案會列出表單中設定的欄位，例如文字方塊和選項按鈕。</p> </td> 
   <td> <p>是</p> <p>使用Kick-Starts匯出Workfront資料可讓您在單一匯出中匯出與多個物件型別相關的資料。 例如，您可以在單一匯出中包含任務、問題和專案。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 匯出限制

透過Kick-starts匯出資料時，有下列限制（資料會以Excel檔案格式匯出）：

* **50,000列：** 檔案中允許的列數。
* **65,530個超連結：** 這是Excel對包含超過65,530個超連結的檔案所施加的限制。 這些檔案匯出後即無法開啟。 請注意，一個Excel檔案可能只有200列資料，但如果檔案中有超過65,530個連結，則檔案不會開啟。

## 透過Kick-Start匯出資料

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) Adobe Workfront右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **系統** > **Kick-Starts，** 然後按一下 **匯出資料。**

1. 選取要匯出的物件。
1. 按一下 **更多選項** 以檢視物件的完整清單。

   此處列出的所有物件也可用來將資料匯入Workfront。

   唯一的例外是 **存取層級** 物件。 匯出中包含的「存取層級」資料表僅供參考之用。 它可讓您依ID將存取層級指派給新的使用者帳戶。

   如需透過Kick-starts將資料匯入Workfront的詳細資訊，請參閱 [使用Kick-Start範本將資料匯入Adobe Workfront](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md). 以下是可透過kick-start匯出的所有物件清單：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p>对象</p> </th> 
      <th> <p>Excel檔案的匯出工作表</p> </th> 
      <th> <p>匯出格式</p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top">访问级别</td> 
      <td scope="col" valign="top">存取層級<br>偏好設定</td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">分配</td> 
      <td scope="col" valign="top">指定任務<br>偏好設定</td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">公司</td> 
      <td scope="col" valign="top"> 公司<br>偏好設定 </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">电子邮件模板</td> 
      <td scope="col" valign="top"> 電子郵件範本<br>偏好設定 </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">费用</td> 
      <td valign="top"> 費用<br>偏好設定 </td> 
      <td scope="col" valign="top"> Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">外部页面</td> 
      <td valign="top"> 外部頁面<br>偏好設定 </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">筛选</td> 
      <td valign="top"> 篩選<br>偏好設定 </td> 
      <td valign="top">ZIP </td> 
     </tr> 
     <tr> 
      <td valign="top">组</td> 
      <td valign="top"> 群組<br>偏好設定  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">分组</td> 
      <td valign="top"> 分組<br>偏好設定 </td> 
      <td valign="top">ZIP</td> 
     </tr> 
     <tr> 
      <td valign="top">小时</td> 
      <td valign="top"> 小時<br>偏好設定 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">问题</td> 
      <td valign="top"> 問題<br>偏好設定 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">工作角色</td> 
      <td valign="top"> 工作角色<br>偏好設定 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">里程碑路径</td> 
      <td valign="top"> 里程碑<br>里程碑路徑<br>偏好設定 </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">注释</td> 
      <td valign="top"> 注意<br>偏好設定 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">项目组合</td> 
      <td valign="top"> Portfolio<br>偏好設定  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">项目</td> 
      <td valign="top"> 佇列<br>專案<br>路由規則<br>佇列主題<br>偏好設定 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">资源评估</td> 
      <td valign="top"> 資源估計<br>偏好設定 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">资源池</td> 
      <td valign="top"> 資源集區<br>偏好設定 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">风险</td> 
      <td valign="top"> 風險<br>偏好設定  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">风险类型</td> 
      <td valign="top"> 風險型別<br>偏好設定  </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">记分卡</td> 
      <td valign="top">計分卡問題<br>計分卡選項<br>計分卡<br>偏好設定 </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">任务</td> 
      <td valign="top"> 任務<br>偏好設定 </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">模板</td> 
      <td valign="top"> 佇列<br>範本<br>路由規則<br>佇列主題<br>偏好設定 </td> 
      <td valign="top">Excel  </td> 
     </tr> 
     <tr> 
      <td valign="top">模板分派</td> 
      <td valign="top"> 範本指派<br>偏好設定 </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">模板任务</td> 
      <td valign="top"> 範本任務<br>偏好設定 </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">时间表</td> 
      <td valign="top"> 週期性時程表<br>時間表<br>偏好設定 </td> 
      <td valign="top">Excel  </td> 
     </tr> 
     <tr> 
      <td valign="top"> 查看 </td> 
      <td valign="top"> 檢視<br>偏好設定  </td> 
      <td valign="top">ZIP</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **下載。**

   匯出的kick-start檔案會以Excel檔案或下載至您的電腦。 包含多個Excel和屬性檔案的zip檔案。 每個Excel檔案都是工作表的集合，其中每個工作表代表與所選物件相關聯的欄位。 有一個 **屬性** 與每次匯出相關聯的頁面。

   此 **儀表板** 和 **報告** 選項可讓您選取要包含在下載中的特定儀表板和報表。 您只能匯出在整個系統內共用的儀表板。

   您無法匯出矩陣報表。 如需矩陣報表的詳細資訊，請參閱 [建立矩陣報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

   在單一匯出中，您最多可以選取100個儀表板和100個報表。

   ![](assets/kickstart-export-350x381.png)

   您可以一次匯出多個物件。

   依預設，下列物件會顯示在 **要包含的內容** 標籤（按一下之前） **更多選項**)：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong>对象</strong> </p> </th> 
      <th> <p><strong>Excel檔案的匯出工作表</strong> </p> </th> 
      <th> <p> <strong>匯出格式</strong></p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top"> <p>仪表板</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top"> <p>引數<br>引數選項<br>引數群組<br>類別引數<br>類別<br>報告<br>入口網站頁簽區段<br>儀表板<br>偏好設定</p> </td> 
      <td scope="col" valign="top"> ZIP</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>报告</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top">引數<br>引數選項<br>引數群組<br>類別引數<br>類別<br>報告<br>偏好設定</td> 
      <td scope="col" valign="top"> ZIP </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>审批</p> </td> 
      <td scope="col" valign="top"> <p>步驟核准者<br>核准步驟<br>核准<br>核准流程<br>偏好設定</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>自定义数据</p> </td> 
      <td scope="col" valign="top"> <p>引數<br>引數選項<br>引數群組<br>類別引數<br>類別<br>偏好設定</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>费用类型</p> </td> 
      <td valign="top"> <p>費用型別<br>偏好設定</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>小时数类型</p> </td> 
      <td valign="top"> <p>小時型別<br>偏好設定</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>团队</p> </td> 
      <td valign="top"> 團隊成員<br>團隊<br>偏好設定 </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>用户</p> </td> 
      <td valign="top"> <p>使用者<br>偏好設定</p> </td> 
      <td valign="top"> <p> Excel</p> </td> 
     </tr> 
    </tbody> 
   </table>

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong></strong> </p> </th> 
      <th> <p><strong>Excel檔案的匯出工作表</strong> </p> </th> 
      <th> <p> <strong>匯出格式</strong></p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top"> <p>仪表板</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top"> <p>引數<br>引數選項<br>引數群組<br>類別引數<br>類別<br>報告<br>入口網站頁簽區段<br>儀表板<br>偏好設定</p> </td> 
      <td scope="col" valign="top"> ZIP</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>报告</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top">引數<br>引數選項<br>引數群組<br>類別引數<br>類別<br>報告<br>偏好設定</td> 
      <td scope="col" valign="top"> ZIP </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>审批</p> </td> 
      <td scope="col" valign="top"> <p>步驟核准者<br>核准步驟<br>核准<br>核准流程<br>偏好設定</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>自定义数据</p> </td> 
      <td scope="col" valign="top"> <p>引數<br>引數選項<br>引數群組<br>類別引數<br>類別<br>偏好設定</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>费用类型</p> </td> 
      <td valign="top"> <p>費用型別<br>偏好設定</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>小时数类型</p> </td> 
      <td valign="top"> <p>小時型別<br>偏好設定</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>团队</p> </td> 
      <td valign="top"> 團隊成員<br>團隊<br>偏好設定 </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>用户</p> </td> 
      <td valign="top"> <p>使用者<br>偏好設定</p> </td> 
      <td valign="top"> <p>Excel</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （建議）分析匯出的資料，以確保已匯出您預期看到的所有資訊。

   對於大型匯出，Workfront會在背景工作以產生Excel檔案，並會向您提供有關延遲的警告訊息。 下載完成後，系統會將kick-start檔案透過電子郵件傳送給您。

   ![](assets/large-kick-start-file-warning-350x65.png)
