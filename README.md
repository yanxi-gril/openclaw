# Hi,I'm Regulus
These are some of my learning notes on AI.
#

---

## 📚 文档摘要

### 1. Agent 区别与联系 (`agent_comparison.html`)

本文档详细解释了 OpenCode 系统中三大 Agent 角色的定位、能力和协作关系：

| Agent | 定位 | 核心能力 |
|-------|------|----------|
| **主 agent** | 全能型 | 直接响应用户请求，拥有完整工具权限 |
| **@explore** | 代码探索专家 | 快速文件搜索、关键词代码搜索、回答代码库问题 |
| **@general** | 复杂任务专家 | 多步骤任务处理、综合分析、自主规划执行 |

**协作模式**：主 agent 接收用户请求 → 根据任务类型委派给合适的子 agent → 子 agent 独立运行 → 返回结果给主 agent → 主 agent 整合回复用户

---

### 2. Git 使用详解 (`git_tutorial.html`)

完整的 Git 命令参考指南，涵盖七大主题：

1. **初始化与配置** - `git init`、`git clone`、`git config`
2. **基本工作流** - `git status`、`git add`、`git commit`、`git reset`、`git restore`、`git checkout`
3. **分支操作** - `git branch`、`git merge`、`git rebase`、`git cherry-pick`
4. **远程操作** - `git remote`、`git fetch`、`git pull`、`git push`
5. **查看与对比** - `git log`、`git diff`、`git show`、`git blame`
6. **高级功能** - `git stash`、`git tag`、`git reflog`、`git bisect`、`git submodule`、`git revert`
7. **实用技巧** - 常用别名配置、功能开发工作流

包含每个命令的详细说明、使用示例和最佳实践。

---

### 3. OpenClaw 配置说明 (`openclaw_config_base_url_or_api_key.txt`)

关于模型提供商和 API key 更换的简要说明：

- **情况一**：仅更换 API Key（Base URL 不变）
  - 只需更新配置中的 `apiKey` 字段
  - 例如：阿里云百炼 API Key 切换

- **情况二**：更换模型提供商（Base URL 需更新）
  - 需同时更新 Base URL 和 API Key
  - 例如：从阿里云百炼切换到硅基流动（SiliconFlow）