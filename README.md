# Superseal

我用 Python 开发客服 Agent 和知识库检索工具，也维护 DeepSeek Harness 的模型接入插件。目前在找深圳的 AI 应用开发或 Python 后端岗位。

### DeepSeek Harness 模型接入插件

这个插件让用户在网页端和 Windows 桌面端配置第三方模型。有人反馈重启后插件报错，我复现了问题，调整了读取模型配置的方式，在 v0.10.0 发布了修复。

[项目与安装说明](https://github.com/supersealwqas/dsh-custom-provider-settings) · [用户反馈和我的回复](https://github.com/supersealwqas/dsh-custom-provider-settings/issues/1) · [修复提交](https://github.com/supersealwqas/dsh-custom-provider-settings/commit/f42354f) · [版本验证记录](https://github.com/supersealwqas/dsh-custom-provider-settings/releases/tag/v0.10.0)

### Python 知识库检索服务

我把本地文档检索接成了 AI 助手可以调用的工具，返回相关片段和引用来源。我也为搜索结果重新排序的步骤加了回退逻辑和测试。如果这一步超时，调用方仍能拿到第一轮检索的结果。

[项目与运行方法](https://github.com/supersealwqas/MODULAR-RAG-MCP-SERVER) · [查询工具的实现](https://github.com/supersealwqas/MODULAR-RAG-MCP-SERVER/commit/249fe95) · [异常处理和测试](https://github.com/supersealwqas/MODULAR-RAG-MCP-SERVER/commit/48bd51f)

### MewHelp 电商客服

我用 Python 和 LangGraph 搭建客服流程，用 Claude Code 辅助编码和调试。我负责的两处逻辑是长对话压缩和工单确认。压缩旧对话时，工具调用和结果要成对保留。客服提出建单建议后，要等用户单独确认才执行。

[项目与运行方法](https://github.com/supersealwqas/MEWHELP) · [长对话压缩的实现和测试](https://github.com/supersealwqas/MEWHELP/commit/8260eca0857b2e9703956427b53030dbd6f89bd5) · [工单确认的实现和测试](https://github.com/supersealwqas/MEWHELP/commit/90cc17aa349c1f07e216f6fe70b7831266f53489)
