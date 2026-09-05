# 大数据与人工智能 · 课程作业仓库

> Big Data & Artificial Intelligence — Coursework Repository

本仓库用于管理《大数据与人工智能》课程的所有作业、实验代码与学习笔记。

## 📁 目录结构

```
bigdata-ai-coursework/
├── assignments/     # 平时作业（每次作业一个子目录，如 hw01-linear-regression）
├── labs/            # 课程实验（如 lab01-hadoop、lab02-spark）
├── notes/           # 课程笔记（Markdown 格式）
├── datasets/        # 小型数据集（大于 50MB 的数据不入库，见 .gitignore）
├── README.md        # 本文件
└── .gitignore       # Git 忽略规则
```

## 📝 作业提交规范

1. 每次作业在 `assignments/` 下新建子目录，命名格式：`hw<序号>-<主题>`，例如 `hw03-decision-tree`
2. 每个子目录内包含：
   - 源代码（`.py` / `.ipynb`）
   - `README.md`：作业要求、思路说明、运行方法、结果截图
3. 提交信息格式：`hw03: 完成决策树作业` 或 `hw03: finish decision tree`

## 🔄 Git 工作流速查

```bash
# 1. 拉取最新代码（开始写作业前）
git pull

# 2. 完成编辑后，查看改动
git status
git diff

# 3. 暂存并提交
git add assignments/hw03-decision-tree
git commit -m "hw03: 完成决策树作业"

# 4. 推送到 GitHub
git push
```

## ⚠️ 注意事项

- 大数据集（> 50MB）不要提交到仓库，放在本地并用 `.gitignore` 排除
- Python 虚拟环境（`venv/`）、缓存（`__pycache__/`）已自动忽略
- 仓库为 **Private**，仅自己可见；如需助教查看可临时开放或添加协作者
