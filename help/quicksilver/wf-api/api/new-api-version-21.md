---
content-type: api
navigation-topic: api-navigation-topic
title: API版本21中的新增功能
description: Adobe Workfront于2025年10月23日发布了API版本21。 API版本21具有对版本20的以下更改。
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 50edbfa342ed7f51d1fe2b9654b55b579bb3f5af
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 4%

---

# API版本21中的新增功能

Adobe Workfront于2025年10月23日发布了API版本21。 API版本21具有对版本20的以下更改。

## 已添加资源

### 人员配备计划模板(SPTMPL)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">核心字段</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
          <li>对象代码</li>
        </ul>
      </td>
   <tr>
      <td role="rowheader">运营</td>
      <td>
        <ul>
          <li>添加</li>
          <li>计数</li>
          <li>删除</li>
          <li>编辑</li>
          <li>GET</li>
          <li>报告</li>
          <li>SEARCH</li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

## 已删除资源

### AssignmentBillingRole (ASBLRL)

AssignmentBillingRole对象及其所有字段已被删除。

## 已修改的资源

### AccessLevelPermissions (ALVPER)

AccessLevelPermissions对象表示访问、创建或修改Workfront对象的特定权限。 然后，可将这些权限与访问级别关联。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b>
            </p>
            <p>添加了以下可能值：</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> （编辑联系人信息）</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>添加了以下可能值：</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> （编辑联系人信息）</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>添加了以下可能值：</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> （编辑联系人信息）</p>
              </li>
            </ul>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRequest (ACSREQ)

如果用户无权访问Workfront中他们需要的对象，则可以请求对该对象的访问权限。 AccessRequest对象表示此请求。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>操作</b>
            </p>
            <p>添加了以下可能值：</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> （编辑联系人信息）</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### AccessRule (ACSURL)

AccessRule对象表示自定义访问级别中的规则集，该规则集确定用户如何共享他们创建的项目。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b>
            </p>
            <p>添加了以下可能值：</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> （编辑联系人信息）</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>添加了以下可能值：</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> （编辑联系人信息）</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>添加了以下可能值：</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> （编辑联系人信息）</p>
              </li>
            </ul>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 公告附件(ANMATT)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>文件扩展名</b>
            </p>
            <p>添加了以下可能值：</p>
             <ul>
              <li><p><code>AI</code></p></li>
              <li><p><code>PSD</code></p></li>
              <li><p><code>ASE</code></p></li>
              <li><p><code>INDD</code></p></li>
              <li><p><code>PUB</code></p></li>
              <li><p><code>BMP</code></p></li>
              <li><p><code>DNG</code></p></li>
              <li><p><code>HEIC</code></p></li>
              <li><p><code>HEIF</code></p></li>
              <li><p><code>JP2</code></p></li>
              <li><p><code>PJPEG</code></p></li>
              <li><p><code>RAW</code></p></li>
              <li><p><code>SVG</code></p></li>
              <li><p><code>WEBP</code></p></li>
              <li><p><code>EPS</code></p></li>
              <li><p><code>MP4</code></p></li>
              <li><p><code>MPEG</code></p></li>
              <li><p><code>WMV</code></p></li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### 批准(APPROVAL)

给定工作项，如任务、文档或时间表，可能要求主管或其他用户签发该工作项。 审批对象表示在工作项上注销的操作。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>已添加</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">收藏集字段</td>
      <td>
        <ul>
          <li>
            <p><b>团队分配</b>
            </p>
            <p>已添加</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>

### 分配(ASSGN)

Assignment对象表示工作项与分派处理该工作项的用户、团队或组之间的连接。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">收藏集字段</td>
      <td>
        <ul>
          <li>
            <p><b>assignmentBillingRoles</b>
            </p>
            <p>已移除</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### 类别(CTGY)

Category对象是自定义表单。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>catObjCode</b>
            </p>
            <p>添加了以下可能值：</p>
             <ul>
              <li>
                <p><code>SPTMPL</code> (enum.categorytypeenum.staffingplantemplate)</p>
              </li>
              <li>
                <p><code>TEAMOB</code> （团队）</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>objTypes</b>
            </p>
            <p>添加了以下可能值：</p>
             <ul>
              <li>
                <p><code>SPTMPL</code> (enum.categorytypeenum.staffingplantemplate)</p>
              </li>
              <li>
                <p><code>TEAMOB</code> （团队）</p>
              </li>
            </ul>
          </li>
           </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 客户（客户）

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><code>APDISAB</code> （禁用用于时间表计算的Java applet）
            </p>
            <p>已添加</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### 文档(DOCU)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">操作</td>
      <td>
        <ul>
          <li>
            <p><b>getTemporaryCloudURL</b>
            </p>
            <p>已添加</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### 文档文件夹

DocumentFolder对象添加了标志`RESTORABLE`。

### Hour (HOUR)

Hour对象表示用户在时间表上记录的小时。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>getTeresircementCommentmporaryCloudURL</b>
            </p>
            <p>已添加验证器 <code>MAX_LENGTH</code></p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### Op任务(OPTASK)

OpTask对象通常称为“问题”。 问题是一个工作项，它通常表示存在阻止任务或项目完成的问题。 问题也可以是技术支持请求。 变更单、请求和错误也是问题。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>已添加</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### 参数（参数）

Parameter对象是一个自定义字段。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>数据类型</b>
            </p>
            <p>添加了以下可能值：</p>
             <ul>
              <li>
                <p><code>RICHLX</code> （词法富文本）</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>显示类型</b>
            </p>
            <p>添加了以下可能值：</p>
             <ul>
              <li>
                <p><code>SNGLROLLUP</code> （单行汇总）</p>
              </li></ul>
         <li>
            <p><b>isActive</b>
            </p>
            <p>已添加</p>
           </li>
           </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">默认字段</td>
      <td>
        <ul>
         <li>
            <p><b>isActive</b>
            </p>
            <p>已添加</p>
           </li>
           </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Portfolio（端口）

Portfolio对象是争夺相同资源（通常是资金或人员来完成这些资源）的项目集合。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>overrideCurrency</b>
            </p>
            <p>已添加</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### 计划(PRGM)

项目群对象是项目组合中项目的子集，其中类似的项目可以分组在一起。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>货币</b>
            </p>
            <p>已添加</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### 项目（项目）

项目是Workfront中的工作项，是Workfront帮助人们完成工作方式中的主要构建基块。 Project对象表示一组具有通用、特定目标的任务。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>已添加</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef (QUED)

QueueDef对象表示队列，这是一个已发布到技术支持区域以允许用户向其提交问题的项目。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>requestorCoreAction</b>
            </p>
            <p>添加了以下可能值：</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> （编辑联系人信息）</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>添加了以下可能值：</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> （编辑联系人信息）</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">操作</td>
      <td>
        <ul>
          <li>
            <p><b>技术支持项目</b>
            </p>
            <p>已添加</p>
            </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 比率（比率）

Rate对象表示Workfront中的记帐费率。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>localBillingPerHour</b>
            </p>
            <p>已移除</p>
              </li>
          <li>
            <p><b>localCostPerHour</b>
            </p>
            <p>已移除</p>
              </li>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### 计划报告(SCHREP)

ScheduledReport对象表示已配置为计划提交的报表。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>格式</b>
            </p>
            <p>添加了以下可能值：</p>
             <ul>
              <li><p><code>AI</code></p></li>
              <li><p><code>PSD</code></p></li>
              <li><p><code>ASE</code></p></li>
              <li><p><code>INDD</code></p></li>
              <li><p><code>PUB</code></p></li>
              <li><p><code>BMP</code></p></li>
              <li><p><code>DNG</code></p></li>
              <li><p><code>HEIC</code></p></li>
              <li><p><code>HEIF</code></p></li>
              <li><p><code>JP2</code></p></li>
              <li><p><code>PJPEG</code></p></li>
              <li><p><code>RAW</code></p></li>
              <li><p><code>SVG</code></p></li>
              <li><p><code>WEBP</code></p></li>
              <li><p><code>EPS</code></p></li>
              <li><p><code>MP4</code></p></li>
              <li><p><code>FLV</code></p></li>
              <li><p><code>M4V</code></p></li>
              <li><p><code>MPEG</code></p></li>
              <li><p><code>WMV</code></p></li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### 记分卡问题(SCOREQ)

ScoreCardQuestion对象表示已添加到记分卡的问题。 这些问题通常由Portfolio经理决定，这些问题的答案让经理能够了解项目与项目组合目标的对齐情况。<table>
<col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>显示类型</b>
            </p>
            <p>添加了以下可能值：</p>
             <ul>
              <li>
                <p><code>SNGLROLLUP</code> （单行汇总）</p>
              </li></ul>
         </ul>
      </td>
    </tr>
 </tbody>
</table>

### 人员配备计划

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>totalEstimatedCost</b>
            </p>
            <p>已添加</p>
              </li>
         <li>
            <p><b>totalEstimatedHours</b>
            </p>
            <p>已添加</p>
              </li>
         <li>
            <p><b>totalEstimatedRevenue</b>
            </p>
            <p>已添加</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### 人员配备计划资源

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>totalEstimatedCost</b>
            </p>
            <p>已添加</p>
              </li>
         <li>
            <p><b>totalEstimatedHours</b>
            </p>
            <p>已添加</p>
              </li>
         <li>
            <p><b>totalEstimatedRevenue</b>
            </p>
            <p>已添加</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### 任务（任务）

Task对象表示作为实现最终目标（完成项目）的步骤而必须执行的工作项。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>已添加</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">收藏集字段</td>
      <td>
        <ul>
          <li>
            <p><b>团队分配</b>
            </p>
            <p>已添加</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>

### 团队

Team对象添加了标志`DATA_EXTENDIBLE`和`SHARABLE`。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>类别ID</b>
            </p>
            <p>已添加</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">引用字段</td>
      <td>
        <ul>
          <li>
            <p><b>类别</b>
            </p>
            <p>已添加</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">收藏集字段</td>
      <td>
        <ul>
          <li>
            <p><b>对象类别</b>
            </p>
            <p>已添加</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>


### 模板分派

TemplateAssignment对象添加了标志`ATTRIBUTE_ATTACHABLE`。

### 时间表(TSHET)

工时表对象表示一个虚拟工时表，允许用户输入任务、项目和管理费用小时类型的实际工作小时数。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">核心字段</td>
      <td>
        <ul>
          <li>
            <p><b>objCode</b>
            </p>
            <p>已移除</p>
              </li>
         </ul>
      </td>
    </tr>
  </tbody>
</table>

### 工作（工作）

Work对象是Task和OpTask都继承的公用接口，它们共享公用代码。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>已添加</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">收藏集字段</td>
      <td>
        <ul>
          <li>
            <p><b>团队分配</b>
            </p>
            <p>已添加</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>


