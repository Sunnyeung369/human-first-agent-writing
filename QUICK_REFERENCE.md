# Human-First Agent Writing - 快速参考

旧称 `ai-agent-team` 仍可作为兼容口令；新安装和文档使用 `human-first-agent-writing`。

## 🎯 三种使用方式

### 1. 让主编协调（推荐用于复杂任务）
```
[Chief] 我需要写一篇深度分析文章
```

### 2. 指定 Agent（推荐用于单一任务）
```
[@researcher] 研究 AI 趋势
[@writer] 撰写文章
[@editor] 优化内容
[@fact-checker] 验证数据
[@archivist] 查找文档
```

### 3. 任务分类（快速模式）
```
[task:research] 调研主题
[task:writing] 撰写内容
[task:editing] 优化结构
[task:fact-check] 验证事实
```

---

## 👥 Agent 速查表

| Agent | 角色 | 一句话描述 |
|-------|------|-----------|
| **Chief** | 主编 | 协调团队，分解任务，整合输出 |
| **Researcher** | 研究员 | 收集信息，调研趋势，提供资料 |
| **Writer** | 作者 | 创作内容，撰写文章，生成文案 |
| **Editor** | 编辑 | 优化结构，精炼语言，提升质量 |
| **Fact-Checker** | 核查员 | 验证事实，检查数据，确保准确 |
| **Archivist** | 档案员 | 检索知识，查找文档，建立关联 |

---

## 🔄 标准工作流程

### 内容创作
```
Chief 规划 → Researcher 研究 → Writer 创作 → Editor 优化 → Fact-Checker 验证 → Chief 审核
```

### 研究分析
```
Chief 定义 → Researcher 调研 → Archivist 补充 → Fact-Checker 验证 → Writer 撰写 → Editor 整理
```

### 快速模式
```
Chief → Researcher (15分钟) → Writer (30分钟) → Editor (15分钟) → Chief 输出
```

---

## 💬 常用命令示例

### 内容创作类
```
[Chief] 写一篇关于 AI 的技术博客
[@writer] 基于研究结果写文章
[@editor] 审查并优化这篇文章
```

### 研究分析类
```
[@researcher] 调研区块链应用场景
[Chief] 分析市场前景并给出建议
[@fact-checker] 验证这些数据的准确性
```

### 知识管理类
```
[@archivist] 查找相关历史文档
[Chief] 建立知识库并整理分类
```

### 质量控制类
```
[@fact-checker] 检查所有引用和数据
[Chief] 启动三轮质量审查
```

---

## 🚀 高级功能

### 可拆分任务
```
[Chief] 标记可拆分任务：
      - Researcher 研究市场
      - Archivist 分析历史数据
      - Fact-Checker 验证来源
```

### 迭代优化
```
[Chief] 三轮迭代：
      Round 1: Writer 起草
      Round 2: Editor 深度优化
      Round 3: Fact-Checker 全面验证
```

### 质量检查点
```
[Chief] 设置检查点：
      ✓ 研究阶段
      ✓ 创作阶段
      ✓ 编辑阶段
      ✓ 最终阶段
```

---

## ⚡ 快速决策树

```
你的任务是什么？
│
├─ 简单单一任务？
│  └─ 直接指定对应 Agent [@agent-name]
│
├─ 复杂多步骤任务？
│  └─ 使用 [Chief] 协调团队
│
└─ 不确定？
   └─ 使用 [task:category] 自动分类
```

---

## 🎨 场景速查

| 场景 | 使用方式 |
|------|---------|
| 写技术博客 | `[Chief] 写一篇关于 X 的技术博客` |
| 市场分析 | `[Chief] 分析 X 市场的发展前景` |
| 产品文案 | `[@writer] 为产品 X 撰写营销文案` |
| 文档优化 | `[@editor] 优化这份技术文档` |
| 信息验证 | `[@fact-checker] 验证这些事实` |
| 知识检索 | `[@archivist] 查找关于 X 的文档` |

---

## 🔗 SKILL 组合

### 完整内容生产
```
/brainstorming (构思)
→ /human-first-agent-writing (创作)
→ /docx (Word)
→ /pdf (导出)
```

### 研究项目
```
/human-first-agent-writing (团队研究)
→ /obsidian-markdown (笔记)
→ /xlsx (数据表)
→ /pptx (演示)
```

### 知识管理
```
/human-first-agent-writing (整理)
→ /obsidian-bases (数据库)
→ /obsidian-canvas-creator (可视化)
```

---

## ✅ 最佳实践

### DO ✅
- 明确任务目标
- 提供充分上下文
- 遵循工作流程
- 给出具体反馈

### DON'T ❌
- 简单任务不用全部 Agent
- 不要跳过验证环节
- 不要忽略编辑步骤
- 避免重复信息

---

## 📊 效率对比

| 方式 | 适用场景 | 时间 | 质量 |
|------|---------|------|------|
| 单 Agent | 简单任务 | 快 | 中 |
| 指定 Agent | 单一明确任务 | 中 | 高 |
| Chief 协调 | 复杂项目 | 长 | 最高 |

---

## 🆘 故障排除

### 问题：Agent 响应不符合预期
**解决**：
1. 提供更具体的任务描述
2. 增加上下文信息
3. 使用迭代优化

### 问题：流程太慢
**解决**：
1. 使用快速模式
2. 减少不必要的 Agent
3. 标记可拆分的独立任务（是否并发由宿主决定）

### 问题：质量不够高
**解决**：
1. 启用多轮迭代
2. 设置质量检查点
3. 明确质量标准

---

**记住**：当不确定如何开始时，直接使用 `[Chief]` 让主编协调团队！

---

灵感来源：[newtype-profile](https://github.com/newtype-01/newtype-profile)
