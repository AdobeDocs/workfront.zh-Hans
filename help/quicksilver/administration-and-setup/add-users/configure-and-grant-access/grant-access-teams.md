---
title: 授予团队访问权限
description: 作为Adobe Workfront管理员，您可以使用访问级别定义用户对Workfront中团队的访问权限
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 915d1520-f5c4-4e33-b645-cb219289383c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 4%

---

# 授予团队访问权限

作为Adobe Workfront管理员，您可以使用访问级别定义用户对Workfront中团队的访问权限，如 [访问级别概述](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 配置用户的访问权限以使用自定义访问级别编辑用户

1. 开始创建或编辑访问级别，如 [创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. 单击齿轮图标 ![](assets/gear-icon-settings.png) 在 **查看** 或 **编辑** 按钮，然后选择要在 **优化设置**.

   * **查看**:如果您正在配置具有任何许可证的用户如何查看团队，请更改以下任意选项：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">查看与我的组关联的团队</td>
         <td>
          <p><b>已启用</b>:当用户在“团队提前类型”(Team-aed)字段中查找团队时，无论用户是否为团队成员，都可以查看与其组关联的团队。 </p>
          <p><b>已禁用</b>:当用户在“团队先行”(Team-aed)字段中查找团队时，用户只能在他们是团队成员的位置查看与其组关联的团队</p><p>默认情况下，此选项处于启用状态。</p>
          </td>
        </tr>
        <tr>
         <td role="rowheader">查看所有团队</td>
         <td><p>启用此选项后，当用户在“团队提前类型”(Team type-ahead)字段中查找团队时，用户可以查看和选择任何团队。</p><p>默认情况下，此选项处于启用状态。 </p></td>
        </tr>
       </tbody>
      </table>

   * **编辑**:如果要配置具有计划许可证和工作许可证的用户如何管理团队，请更改以下任意选项：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">创建</td>
         <td><p>允许具有计划许可证或工作许可证的用户创建团队。</p><p>默认情况下，此选项处于启用状态。</p></td>
        </tr>
        <tr>
         <td role="rowheader">删除</td>
         <td><p> 允许具有计划许可证的用户删除他们有权编辑的团队（对于具有工作许可证的用户不可用）。</p><p>默认情况下，此选项处于启用状态。</p></td>
        </tr>
        <tr>
         <td role="rowheader">编辑我管理的组中的团队（仅组管理员）</td>
         <td><p>允许被指定为群组管理员的计划许可证用户编辑与其管理的群组关联的团队。</p><p>默认情况下，此选项处于启用状态。</p></td>
        </tr>
        <tr>
         <td role="rowheader">编辑我所在的团队</td>
         <td><p>允许用户在计划许可证或工作许可证中编辑他们所属的团队。</p><p>默认情况下，此选项处于禁用状态。</p></td>
        </tr>
        <tr>
         <td role="rowheader">查看与我的组关联的团队</td>
         <td>
         <p><b>已启用</b> 当用户在“团队提前类型”(Team-aed)字段中查找团队时，无论用户是否为团队成员，都可以查看与其组关联的团队。 </p>
         <p><b>已禁用</b>:当用户在“团队先行”(Team-aed)字段中查找团队时，用户只能在他们是团队成员的位置查看与其组关联的团队</p><p>默认情况下，此选项处于启用状态。</p>
         </td>
        </tr>
        <tr>
         <td role="rowheader">查看所有团队</td>
         <td><p>启用此选项后，当用户在“团队提前类型”(Team type-ahead)字段中查找团队时，用户可以查看和选择任何团队。</p><p>默认情况下，此选项处于启用状态。 </p></td>
        </tr>
       </tbody>
      </table>

1. 单击X以关闭 **优化设置** 框中。
1. （可选）要在您正在处理的访问级别中为其他对象和区域配置访问设置，请继续阅读 [配置对Adobe Workfront的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)，例如 [授予对任务的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) 和 [授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. 完成后，单击 **保存**.

>[!NOTE]
>
>* 无论访问级别设置如何，下面是true:
   >
   >   * 团队所有者可以随时查看和编辑其团队
   >   * 用户始终有权查看其所在的团队
>
* 如果您决定在访问级别选择“查看”，而不是“编辑”或“编辑”，则“查看”和“编辑”选项（例如“查看与我的组关联的团队”）的配置将保留。
>


## 按许可证类型访问团队

有关每个访问级别中的用户可以处理问题的信息，请参阅部分 [团队](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#teams) 在文章中 [可用于每种对象类型的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
