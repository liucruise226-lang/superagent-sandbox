# superagent-sandbox

dsh-superagent sandbox

## 项目简介

`superagent-sandbox` 是 dsh-superagent 的沙盒仓库，用于在真实 GitHub 仓库中验证 superagent 的端到端工作链路。仓库本身不包含业务代码或可部署的服务，只保留用于验证和演示的最小内容。

### 用途

- 验证从 GitHub Issue 触发任务、由 Agent 接手并提交 Pull Request 的完整流程。
- 作为 dsh-superagent 在权限、触发规则、审阅与合并等配置调整后的回归环境。
- 为文档、示例和流程演示提供一个不会影响生产代码的试验场所。

### 工作方式

在仓库中创建 Issue 并 @ 提及 Agent 账号后，dsh-superagent 会接收任务，在独立分支上完成改动并提交 Pull Request，等待评审与合并。
