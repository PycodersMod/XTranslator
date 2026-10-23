# XTranslator

**状态：研究暂停；尚未实现。**

XTranslator 是一个计划中的离线独立转换工具：分析已知 Loader 生态的 Mod JAR，在来源和行为可验证的范围内进行转换，并尝试生成新的 XLoader 原生 Mod JAR。XTranslator 与 XLoader Runtime 分离；XLoader 不内嵌通用转换器。

本仓库用于保存设计边界和研究断点，不包含可运行的转换器、翻译模型或成功转换的证明。不能据此宣称任意 JAR 可转换。

## 研究范围

- 纯 JAR 分析与可选、经用户授权的可信源码来源匹配。
- 元数据、Mixin/Transformer、注册、映射、依赖和生命周期证据。
- 可追溯的来源置信阶段、可解释的转换结果和明确的 `PARTIAL` / `UNSUPPORTED` 输出。
- 确定性构建与真实行为验证；模型能力仅可作为以后可选的辅助层。
- 不自动执行未审查的第三方构建脚本。

详见 [`docs/RESEARCH_CHECKPOINT.md`](docs/RESEARCH_CHECKPOINT.md)。

## 许可

本仓库文档按 MIT License 发布。未来输入 Mod、源码和依赖仍须遵守各自许可与用户授权。
