> ⚠️ **本仓库已废弃**：内容已并入 [agent-deploy](https://github.com/hpsks416/agent-deploy) 的 skills/skill-optimizer/ 子目录，请以 agent-deploy 为准。本仓库保留仅供历史归档。

# skill-optimizer

轻量版 SkillOpt：把「skill 文档当可训练参数」，用 rollout→reflect→edit→gate 四步循环自动改进一个 skill 的正文。核心是**用验证门控防过拟合**——只有能通过留出验证集的改进才被接受。产出永远是 `_draft`，人类终审。

## 环境依赖

- 操作系统：Windows
- 运行时：Python 3（标准库）
- 第三方软件：无（仅依赖系统自带的 PowerShell / 标准库）

## 目录结构

    skill-optimizer/
    ├── SKILL.md    技能入口与工作流
    ├── evals.yaml

## 安装

    # GitHub
    git clone https://github.com/hpsks416/skill-optimizer.git "$env:USERPROFILE\.dsh\skills\skill-optimizer"
    # 或 Gitee（国内直连）
    git clone https://gitee.com/hpsks416/skill-optimizer.git "$env:USERPROFILE\.dsh\skills\skill-optimizer"

克隆后 DSH 自动重新发现，无需构建。

## License

MIT License. See [LICENSE](LICENSE).

