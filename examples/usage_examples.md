# AI Agent Team - 使用示例

本文档提供了 AI Agent Team SKILL 的详细使用示例。

## 目录

- [基础示例](#基础示例)
- [进阶示例](#进阶示例)
- [专业场景](#专业场景)
- [故障排除](#故障排除)

---

## 基础示例

### 示例 1: 快速测试

```bash
claude
> [Chief] 测试一下 AI Agent Team 是否正常工作
```

**预期输出**: Chief 应该协调所有 Agent 进行简单测试。

---

### 示例 2: 单个 Agent 调用

```bash
# 研究任务
> [@researcher] 研究 Claude Code 的核心特性

# 写作任务
> [@writer] 写一段关于 AI Agent 的介绍

# 编辑任务
> [@editor] 审查并优化这段文字

# 核查任务
> [@fact-checker] 验证这个技术细节
```

---

### 示例 3: 任务分类

```bash
# 研究任务
> [task:research] 调研 AI 在医疗领域的应用

# 写作任务
> [task:writing] 撰写技术博客草稿

# 编辑任务
> [task:editing] 优化文档结构

# 核查任务
> [task:fact-check] 验证所有数据
```

---

## 进阶示例

### 示例 4: 完整文章创作

```bash
> [Chief] 我需要创作一篇关于 RAG 技术的深度技术文章，2000字，面向开发者

# Chief 会自动协调：
# 1. Researcher 研究 RAG 技术原理、应用场景、最新进展
# 2. Archivist 查找相关技术文档和案例
# 3. Writer 基于研究结果撰写 2000 字技术文章
# 4. Editor 审查并优化技术内容和表达
# 5. Fact-Checker 验证所有技术细节和数据
# 6. Chief 最终审核并整合输出
```

**预期产出**: 2000-3000 字高质量技术文章

---

### 示例 5: 市场分析报告

```bash
> [Chief] 分析 AI Agent 市场的发展前景并给出投资建议

# 工作流程：
# Phase 1: 研究准备
#   ├─ Researcher 调研市场规模、增长趋势、主要玩家
#   └─ Archivist 收集历史数据和过往案例
#
# Phase 2: 数据验证
#   └─ Fact-Checker 验证市场数据和预测
#
# Phase 3: 报告撰写
#   └─ Writer 撰写分析报告
#
# Phase 4: 质量优化
#   └─ Editor 优化报告结构和逻辑
#
# Phase 5: 最终输出
#   └─ Chief 整合并提供投资建议
```

**预期产出**: 完整的市场分析报告 + 关键发现 + 投资建议

---

### 示例 6: 并行任务处理

```bash
> [Chief] 我需要同时完成以下任务：
      - 研究 AI Agent 最新技术进展
      - 分析竞品产品功能
      - 收集用户反馈和需求
      请协调团队并行完成这些任务

# Chief 会设计并行执行方案：
# Task 1: Researcher + Archivist → 技术调研
# Task 2: Researcher + Fact-Checker → 竞品分析
# Task 3: Writer + Archivist → 用户反馈整理
#
# 然后整合所有结果
```

---

## 专业场景

### 场景 1: 技术博客创作

```bash
# 1. 头脑风暴（可选）
> /brainstorming
我想写一篇关于 AI Agent 协作模式的技术博客

# 2. Agent 团队创作
> [Chief] 基于上面的头脑风暴，创作完整的技术博客

# 3. 格式化为文档
> /obsidian-markdown
将文章转换为 Obsidian 格式

# 4. 发布（可选）
> /pdf
生成 PDF 版本
```

---

### 场景 2: 产品发布准备

```bash
# 1. 市场研究
> [task:research] 调研目标市场和用户群体

# 2. 竞品分析
> [task:research] 分析主要竞品的优劣势

# 3. 产品文案
> [task:writing] 撰写产品发布新闻稿

# 4. 技术文档
> [task:writing] 编写用户手册和技术文档

# 5. 演示文稿
> /pptx
基于研究结果创建产品演示 PPT
```

---

### 场景 3: 知识库构建

```bash
# 1. 主题规划
> [Chief] 帮我规划一个云原生技术知识库

# 2. 内容收集
> [@researcher] 收集各个技术领域的核心知识
> [@archivist] 建立知识点之间的关联

# 3. 内容整理
> [@writer] 撰写知识条目
> [@editor] 优化知识结构

# 4. 质量保证
> [@fact-checker] 验证技术概念准确性

# 5. 组织到 Obsidian
> /obsidian-markdown
> /obsidian-bases
创建笔记和数据库视图
> /obsidian-canvas-creator
创建知识图谱可视化
```

---

### 场景 4: 研究论文辅助

```bash
# 1. 文献调研
> [@researcher] 调研 RAG 技术的最新研究论文
> [@archivist] 查找我们之前的相关资料

# 2. 内容分析
> [task:fact-check] 验证所有引用和数据

# 3. 论文撰写
> [task:writing] 撰写论文草稿
> [task:editing] 优化论文结构和语言

# 4. 格式化
> /docx
生成符合格式的 Word 文档
```

---

### 场景 5: 企业级内容生产

```bash
# 1. 需求分析
> [Chief] 分析企业内部文档需求并制定内容生产计划

# 2. 批量生产
> [task:writing] 批量撰写技术文档
> [task:editing] 统一文档风格
> [task:fact-check] 验证技术准确性

# 3. 质量控制
> [Chief] 设置质量检查点并执行三轮审查

# 4. 输出
> /docx
> /pdf
批量生成多种格式
```

---

## 高级技巧

### 技巧 1: 迭代优化

```bash
> [Chief] 启动三轮优化流程：
      Round 1: Writer 起草初稿
      Round 2: Editor 深度优化
      Round 3: Fact-Checker 全面验证

# 每轮迭代质量会明显提升
```

---

### 技巧 2: 质量检查点

```bash
> [Chief] 在每个阶段设置质量检查点：
      ✓ 研究阶段：确保信息全面性
      ✓ 创作阶段：确保内容完整性
      ✓ 编辑阶段：确保结构清晰性
      ✓ 最终阶段：确保事实准确性
```

---

### 技巧 3: Agent 投票机制

```bash
> [Chief] 这个技术方案有争议，
      请 Researcher, Archivist, Fact-Checker
      分别评估并提供意见
      综合分析后做出决策

# 多 Agent 投票提高决策质量
```

---

## 与其他 SKILL 配合

### 组合 1: 完整内容生产管道

```bash
/brainstorming          # 1. 构思
> /human-first-agent-writing        # 2. 团队创作
> /docx                 # 3. Word 文档
> /pdf                  # 4. PDF 导出
```

---

### 组合 2: 研究到演示

```bash
/human-first-agent-writing          # 1. 团队研究
> /xlsx                 # 2. 数据表格
> /pptx                 # 3. 演示文稿
> /theme-factory        # 4. 应用主题
```

---

### 组合 3: Obsidian 知识管理

```bash
/human-first-agent-writing          # 1. 内容创作
> /obsidian-markdown    # 2. 格式化
> /obsidian-bases       # 3. 数据库
> /obsidian-canvas-creator  # 4. 可视化
```

---

## 故障排除

### 问题 1: Agent 响应不符合预期

**解决方案**:
1. 提供更具体的任务描述
2. 增加上下文信息
3. 使用迭代优化

```bash
# ❌ 不好的示例
> [Chief] 写篇文章

# ✅ 好的示例
> [Chief] 写一篇关于 AI Agent 的技术文章，
  2000字，面向开发者，
  包含技术原理、应用场景、代码示例
```

---

### 问题 2: 流程太慢

**解决方案**:
1. 使用快速模式
2. 减少不必要的 Agent
3. 并行处理独立任务

```bash
# 标准模式（2-3小时）
> [Chief] 完整流程创作

# 快速模式（1小时）
> [task:writing] 快速撰写
> [task:editing] 简要优化
```

---

### 问题 3: 质量不够高

**解决方案**:
1. 启用多轮迭代
2. 设置质量检查点
3. 明确质量标准

```bash
> [Chief] 启动质量保证模式：
      - 三轮迭代优化
      - 每个阶段质量检查
      - 最终全面审查
```

---

## 最佳实践总结

### ✅ DO

1. **明确目标**
   - 清楚描述你想要什么
   - 提供充分的上下文

2. **合理选择**
   - 简单任务用单 Agent
   - 复杂任务用 Chief
   - 快速任务用任务分类

3. **遵循流程**
   - 研究先行
   - 验证在后
   - 迭代优化

4. **提供反馈**
   - 给出具体建议
   - 明确改进方向

### ❌ DON'T

1. 不要对简单任务用全部 Agent
2. 不要跳过验证环节
3. 不要忽略编辑步骤
4. 不要重复相同信息

---

## 更多资源

- [快速参考](../QUICK_REFERENCE.md)
- [完整文档](../README.md)
- [贡献指南](../CONTRIBUTING.md)
- [更新日志](../CHANGELOG.md)

---

**需要帮助？** 查看 [Issues](https://github.com/Sunnyeung369/human-first-agent-writing/issues) 或 [Discussions](https://github.com/Sunnyeung369/human-first-agent-writing/discussions)

---

*最后更新: 2026-01-15*
