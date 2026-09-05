# 大数据与人工智能 · 课程作业仓库

> Big Data & Artificial Intelligence — Coursework Repository

本仓库用于管理《大数据与人工智能》课程的所有作业、实验代码与学习笔记。当前主要包含**作业 1：用 AI 构建个人概念学习资料生成 Skill**。

## 📁 仓库结构

```
bigdata-ai-coursework/
├── .workbuddy/
│   └── skills/
│       └── concept-study-generator/     # 项目级 Skill
│           └── SKILL.md                 # 概念学习资料生成 Skill 定义
├── learning-materials/                  # 由 Skill 生成的概念学习资料
│   ├── agent.html                       # Agent（智能体）
│   ├── llm-context.html                 # 大模型的上下文
│   ├── skill.html                       # Skill（技能/可复用能力）
│   ├── concept-relationship.html        # 概念关系说明（可视化）
│   └── concept-relationship.md          # 概念关系说明（Markdown 版）
├── assignments/                         # 平时作业
│   └── hw00-example/                    # 示例作业目录
├── labs/                                # 课程实验
├── notes/                               # 课程笔记
├── datasets/                            # 小型数据集（大文件已忽略）
├── README.md                            # 本文件
└── .gitignore                           # Git 忽略规则
```

## 🧩 项目级 Skill

- **Skill 名称**：`concept-study-generator`
- **存放路径**：`.workbuddy/skills/concept-study-generator/SKILL.md`
- **功能**：为任意新概念生成结构化、可核查的个人学习资料（HTML 格式）。
- **输入**：概念名称（如 `Agent`）、解释深度（可选）、侧重方向（可选）。
- **输出**：固定包含“一句话定义、个人理解、核心机制、应用场景、易混淆边界、可核查来源”六个部分的 HTML 文件。
- **自检清单**：Skill 中附带 7 项自检要求，确保资料完整、准确、可复用。

## ▶️ 如何在 WorkBuddy 中调用本 Skill

1. 在 WorkBuddy 中打开本仓库（`C:\Users\20665\Documents\bigdata-ai-coursework`）。
2. 对助手说：
   > “调用 `.workbuddy/skills/concept-study-generator` Skill，为 `Transformer` 生成学习资料。”
3. 助手会按照 `SKILL.md` 中的流程，生成 `learning-materials/transformer.html`。
4. 对照 SKILL.md 中的自检清单检查生成结果，人工修改后提交。

## 📚 已生成的学习资料

| 概念 | 文件 | 说明 |
|------|------|------|
| Agent | `learning-materials/agent.html` | 智能体的定义、机制、应用场景与边界 |
| 大模型的上下文 | `learning-materials/llm-context.html` | 上下文组成、作用、与记忆和训练数据的区别 |
| Skill | `learning-materials/skill.html` | Skill 的组成、与提示词/Agent 的区别、应用场景 |
| 概念关系说明 | `learning-materials/concept-relationship.html` | 三者的关系、流程图（含 Mermaid）、个人判断 |

## 🤖 AI 使用与人工核查说明

本作业允许并鼓励使用 AI 协助设计 Skill、编写 Git 命令和整理资料，但已按要求完成以下人工核查与修改：

1. **Skill 设计**：人工确定了 Skill 的六大输出模块和自检清单，确保其可复用、不局限于本次三个概念。
2. **概念理解**：每份资料的“个人理解”部分均基于课堂所学和资料阅读重新组织，未整段照搬 AI 输出。
3. **资料来源**：所有来源均为官方文档、经典教材或权威论文，并附带了可核查的链接或引用信息。
4. **事实核查**：核对了 Agent 与 LLM 的区别、上下文与长期记忆的区别、Skill 与一次性提示词的区别。
5. **HTML 格式**：每份资料均可直接在浏览器中打开，结构清晰、样式统一。
6. **关系说明**：使用表格和 Mermaid 流程图呈现三者关系，并加入个人判断。

## 🔄 Git 工作流速查

```bash
# 1. 拉取最新代码（开始写作业前）
git pull

# 2. 完成编辑后，查看改动
git status
git diff

# 3. 暂存并提交
git add .
git commit -m "描述本次修改"

# 4. 推送到 GitHub
git push
```

## ⚠️ 注意事项

- 本仓库为 **Public**，便于教师直接查看。
- 大数据集（> 50MB）不要提交到仓库，已配置 `.gitignore` 排除。
- Python 虚拟环境（`venv/`）、缓存（`__pycache__/`）已自动忽略。
- 不要上传 API Key、密码或个人隐私信息。
