# 本地Word文档框架使用指南

## 概述

本Skill支持使用本地Markdown文档(.md)作为文档框架源。相比飞书在线文档框架，本地文档框架更稳定、访问更快速。

## 支持的22个Markdown文档框架

以下文档框架文件位于 `references/templates/` 目录下：

### PRD类文档框架（11个）

| 序号 | 文档框架文件名 | 文档框架类型 | PRD阶段 | 适用场景 |
|-----|-----------|---------|---------|---------|
| 1 | `Discovery PRD.md` | 产品需求文档 | 探索 | 问题验证、假设验证、用户研究 |
| 2 | `Business PRD-BRD.md` | 产品需求文档 | 探索 | 商业价值分析、ROI评估 |
| 3 | `Systemic Solution PRD template.md` | 产品需求文档 | 方案 | 系统解决方案、端到端设计 ⭐推荐 |
| 4 | `Experiment PRD.md` | 产品需求文档 | 方案 | A/B测试、MVP验证、实验设计 |
| 5 | `Feature PRD.md` | 产品需求文档 | 实现 | 功能级设计、功能细节 |
| 6 | `Technical PRD.md` | 产品需求文档 | 实现 | 技术实现方案、系统架构 |
| 7 | `System Evolution PRD.md` | 产品需求文档 | 演进 | 长期演进规划、架构路线图 |
| 8 | `Default Product Requirements Document.md` | 产品需求文档 | 探索/演进 | 通用PRD文档框架 |
| 9 | `OKRs.md` | 管理文档 | 方案/演进 | 目标与关键结果管理 |
| 10 | `PRD 文档目录结构.md` | 产品需求文档 | - | PRD文档结构指南 |
| 11 | `PRD_一级功能名称_二级功能名称.md` | 产品需求文档 | 实现 | PRD功能模块文档框架 |

### 技术设计类文档框架（2个）

| 序号 | 文档框架文件名 | 文档框架类型 | 适用场景 |
|-----|-----------|---------|---------|
| 12 | `Technical Design Document.md` | 技术文档 | 技术设计文档、系统架构 |
| 13 | `API Documentation.md` | 技术文档 | API接口文档 |

### 用户研究类文档框架（4个）

| 序号 | 文档框架文件名 | 文档框架类型 | 适用场景 |
|-----|-----------|---------|---------|
| 14 | `User Personas.md` | 产品设计 | 用户画像分析 |
| 15 | `Customer Journey Map.md` | 产品设计 | 用户旅程地图 |
| 16 | `User Testing Plan.md` | 测试文档 | 用户测试计划 |
| 17 | `Usability Test Plan.md` | 测试文档 | 可用性测试计划 |

### 市场分析类文档框架（4个）

| 序号 | 文档框架文件名 | 文档框架类型 | 适用场景 |
|-----|-----------|---------|---------|
| 18 | `Competitive Analysis Report.md` | 业务分析 | 竞品分析报告 |
| 19 | `Go-to-Market Plan.md` | 运营方案 | 市场推广计划 |
| 20 | `Release Plan.md` | 项目管理 | 发布计划 |
| 21 | `PR FAQ.md` | 产品文档 | 产品常见问题 |

### 其他类文档框架（1个）

| 序号 | 文档框架文件名 | 文档框架类型 | 适用场景 |
|-----|-----------|---------|---------|
| 22 | `Accessibility Compliance Checklist.md` | 合规检查 | 无障碍合规检查清单 |

## 使用步骤

**使用文档框架**:

智能体会直接读取 `references/templates/` 下的Markdown文档框架，无需额外操作。

### 使用流程

1. 智能体读取 `references/templates/` 目录下的22个Markdown文档框架
2. 根据输入内容类型选择合适的文档框架
3. 将内容填充到文档框架结构中
4. 输出标准化文档

智能体会：
1. 读取 `references/templates/` 目录下的Markdown文档框架
2. 根据内容类型选择合适的文档框架
3. 将用户输入的内容填充到文档框架结构中
4. 输出标准化的文档

## 文档框架选择逻辑

智能体会根据输入内容自动选择文档框架：

### PRD阶段选择逻辑

| PRD阶段 | 内容特征 | 推荐文档框架 | 文档框架文件名 |
|---------|---------|---------|--------|
| **探索阶段** | 探索、发现、假设、验证、机会 | `Discovery PRD` | `Discovery PRD.md` |
| **探索阶段** | 商业价值、ROI、市场机会 | `Business PRD-BRD` | `Business PRD-BRD.md` |
| **方案阶段** | 方案、设计、架构、系统、端到端 | `Systemic Solution PRD template` | `Systemic Solution PRD template.md` ⭐推荐 |
| **方案阶段** | 实验、A/B测试、MVP、验证 | `Experiment PRD` | `Experiment PRD.md` |
| **实现阶段** | 功能、特性、功能模块、功能细节 | `Feature PRD` | `Feature PRD.md` |
| **实现阶段** | 技术实现、技术细节、技术PRD | `Technical PRD` | `Technical PRD.md` |
| **演进阶段** | 演进、规划、长期、路线图 | `System Evolution PRD` | `System Evolution PRD.md` |

### 非PRD文档选择逻辑

| 内容特征 | 推荐文档框架 | 文档框架文件名 |
|---------|---------|--------|
| 产品功能需求、PRD（通用） | 产品需求文档文档框架 | `Default Product Requirements Document.md` |
| PRD目录、结构 | PRD文档结构指南 | `PRD 文档目录结构.md` |
| 一级功能、二级功能 | PRD功能模块文档框架 | `PRD_一级功能名称_二级功能名称.md` |
| 目标管理、OKR | 目标与关键结果 | `OKRs.md` |
| API接口说明 | API接口文档 | `API Documentation.md` |
| 技术设计、架构 | 技术设计文档 | `Technical Design Document.md` |
| 用户画像 | 用户画像文档框架 | `User Personas.md` |
| 用户旅程、体验、触点 | 用户旅程地图 | `Customer Journey Map.md` |
| 用户测试计划 | 用户测试计划 | `User Testing Plan.md` |
| 可用性测试 | 可用性测试计划 | `Usability Test Plan.md` |
| 竞品对比分析 | 竞品分析文档框架 | `Competitive Analysis Report.md` |
| 市场推广策略、GTM | 市场推广计划 | `Go-to-Market Plan.md` |
| 产品发布计划、版本迭代 | 发布计划 | `Release Plan.md` |
| 产品FAQ、问答 | 产品常见问题 | `PR FAQ.md` |
| 无障碍、合规、可访问性 | 无障碍合规检查 | `Accessibility Compliance Checklist.md` |

## 注意事项

### 关于文档框架维护

**文档框架格式调整**:
- 可以手动编辑 `references/templates/` 下的.md文件调整格式
- 建议保持文档框架结构的稳定性

**文档框架选择**:
- 如果智能体没有选择合适的文档框架，可以在输入内容中明确说明"使用XX文档框架"或"参考XX文档框架"

**关于图片**:
- 当前版本的MD文档不包含图片
- 如果文档框架包含图片，建议手动添加到Markdown文件中

### 关于文档框架更新

如果需要更新文档框架内容：
1. 直接编辑 `references/templates/` 下的.md文件
2. 或者重新从Word源文件转换（如有需要）

### PRD阶段选择建议

对于PRD类文档，智能体会根据以下因素选择文档框架：
1. **问题成熟度**: 
   - 早期探索 → Discovery PRD / Business PRD-BRD
   - 方案成型 → Systemic Solution PRD / Experiment PRD
   - 功能明确 → Feature PRD / Technical PRD
   - 长期规划 → System Evolution PRD

2. **颗粒度需求**:
   - 粗略、开放 → Discovery PRD
   - 中等、结构化 → Systemic Solution PRD
   - 详细、精确 → Feature PRD / Technical PRD
   - 宏观、战略 → System Evolution PRD

3. **用户明确指定**:
   - 如果用户明确提到PRD阶段，优先使用对应文档框架
   - 如果用户提到具体文档类型（如"功能PRD"），直接使用该文档框架

## 常见问题

**Q: 智能体没有选择合适的文档框架？**
A: 可以在输入内容中明确说明"使用XX文档框架"或"参考XX文档框架"

**Q: 能否添加新的文档框架？**
A: 可以，直接将新的.md文件放到 `references/templates/` 目录

**Q: 如何修改文档框架结构？**
A: 直接编辑 `references/templates/` 下的.md文件即可

**Q: PRD有这么多文档框架，我该用哪个？**
A: 
- 如果不确定，智能体会根据您的输入内容自动判断并推荐
- 您也可以明确说明PRD阶段（探索/方案/实现/演进）
- 或直接指定文档框架名称（如"使用Feature PRD"）
