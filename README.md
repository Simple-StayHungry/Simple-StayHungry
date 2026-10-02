# SYY

**金融业务流程 · 软件工程 · 自动化工具**

围绕债券承销、合规核查和文档处理，开发本地化自动化工具。重点是将重复且可规则化的业务流程转化为可验证、可追溯的软件工作流，并在规则不足的场景保留人工复核。

> Local automation for bond underwriting and compliance workflows, with explicit rules, traceable outputs and human review where required.

## 项目

<table>
<tr>
<td width="72"><img src="assets/document-review-workbench.png" width="56" alt="Document Review Workbench"></td>
<td><a href="https://github.com/Simple-StayHungry/document-review-workbench"><b>Document Review Workbench</b></a><br>债券业务核查分析文件自动化工作台<br><sub>结构化文档比对、Word 修订生成、人工复核与导出校验</sub></td>
</tr>

<tr>
<td width="72"><img src="assets/document-update-workbench.png" width="56" alt="Document Update Workbench"></td>
<td><a href="https://github.com/Simple-StayHungry/document-update-workbench"><b>Document Update Workbench</b></a><br>债券发行说明性文件批量更新工作台<br><sub>批量内容映射、受保护区域隔离、格式保留与人工复核</sub></td>
</tr>

<tr>
<td width="72"><img src="assets/bond-weekly-automation.png" width="56" alt="Bond Weekly Automation"></td>
<td><a href="https://github.com/Simple-StayHungry/bond-weekly-automation"><b>Bond Weekly Automation</b></a><br>债券市场周报自动化生成<br><sub>多来源公开数据采集、完整性核验、模板继承写入与历史区域校验</sub></td>
</tr>

<tr>
<td width="72"><img src="assets/duecheck.png" width="56" alt="DueCheck"></td>
<td><a href="https://github.com/Simple-StayHungry/duecheck"><b>DueCheck</b></a><br>网页核查截图「主体 · 时间 · 结果」自动化质检<br><sub>站点映射、证据提取、五态判断与人工确认</sub></td>
</tr>

<tr>
<td width="72"><img src="assets/electronic-date-stamp.png" width="56" alt="Electronic Date Stamp"></td>
<td><a href="https://github.com/Simple-StayHungry/electronic-date-stamp"><b>Electronic Date Stamp</b></a><br>PDF 落款日期自动化写入与审计<br><sub>候选定位、数字级写入、追加式处理与独立像素审计</sub></td>
</tr>
</table>

## 共同设计原则

```mermaid
flowchart LR
    A["明确业务规则"] --> B["拆分定位 / 判断 / 写入 / 审计"]
    B --> C["规则不足时转人工"]
    C --> D["保留证据与修改记录"]
    D --> E["本地运行"]
```

这些项目的共同目标不是追求尽可能高的自动化覆盖率，而是在可规则化的部分提高处理效率，同时保留人工确认、审计和回溯能力。

## 技术

`Python` · `OOXML / DOCX / XLSX` · `PDF` · `FastAPI` · `OpenCV` · `SQLite` · `pytest`  
`原生 JavaScript` · `macOS / Windows / Linux`
