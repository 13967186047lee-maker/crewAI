# CrewAI 简体中文说明

> 本页是 `README.md` 的简体中文辅助说明，用来快速了解项目。功能细节、安装命令、版本变化和企业产品信息请以英文 [README.md](README.md) 与官方文档为准。

[English README](README.md) · [官方文档](https://docs.crewai.com) · [官网](https://crewai.com) · [PyPI](https://pypi.org/project/crewai/)

## 项目概览

CrewAI 是一个用于编排多 AI Agent 协作的 Python 框架。它强调轻量、快速、可控，既可以用高层抽象快速组织多个 Agent 协作，也可以在低层定制任务流程、提示词、工具调用和执行逻辑。

核心能力包括：

- **Crews**：让多个 Agent 按角色分工协作，适合研究、写作、分析、运营和自动化任务。
- **Flows**：用事件驱动方式编排更精确的生产级流程，可以与 Crews 一起使用。
- **工具生态**：可通过 `crewai[tools]` 安装常用工具扩展，让 Agent 访问搜索、文件、网页、数据库等能力。
- **企业控制面**：CrewAI AMP Suite 和 Crew Control Plane 提供观测、管理、部署和企业支持能力。

## 快速开始

确保本机安装 Python `>=3.10 <3.14`。项目推荐使用 [UV](https://docs.astral.sh/uv/) 管理依赖。

安装基础包：

```shell
uv pip install crewai
```

如果需要同时安装 Agent 工具扩展：

```shell
uv pip install 'crewai[tools]'
```

创建新的 CrewAI 项目：

```shell
crewai create crew <project_name>
```

更多项目结构、YAML 配置、Flow 与 Crew 混合使用示例，请阅读英文 [README.md](README.md#getting-started) 和 [docs.crewai.com](https://docs.crewai.com)。

## 适合场景

- 多 Agent 研究、分析和报告生成。
- 营销、销售、客服和内容生产自动化。
- 数据处理、监控、告警和运营流程编排。
- 需要可观测、可部署、可扩展的企业级 Agent 工作流。

## 开发与贡献

本仓库使用 `uv` 管理开发环境。常用命令包括：

```shell
uv sync
uv run pytest .
uvx mypy src
```

提交贡献前，请先查看英文 README 中的贡献说明和项目现有规范。

## 许可证

本项目使用 MIT License。详见 [LICENSE](LICENSE)。
