# Maa Verge Automation

面向 [MaaFramework（MaaFW）](https://github.com/MaaXYZ/MaaFramework) 的共享自动化模块，集中维护原语、组合和 Pipeline 相关的 JSON/JSONC 与 TypeScript，供 [Maa Verge](https://github.com/maa-verge/maa-verge)、[Maa Verge Debugger](https://github.com/maa-verge/maa-verge-debugger) 及后续插件内容包复用。

当前处于规划与仓库初始化阶段，尚未交付独立可用包或完成双端集成。现有实现参考 Maa Verge 的迁移分支，实际拆分与接入按计划逐步推进。

## 设计方向

- 以原语、组合、Pipeline/业务流程组织资产，通用能力与明日方舟领域模块分别导出。
- 优先复用 MaaFW 原生 Pipeline、资源布局和执行语义；复杂算法与业务验证通过受控 TS Custom 扩展。
- 两端计划通过 Git submodule 固定共享提交，避免复制另一份 JSON/TS；具体包 API、挂载路径和兼容范围在实施时确定。
- 共享库提供流程、必要契约与有限端口；设备租约、原生进程、权限预算、业务数据库和应用界面由各宿主管理。
- 为插件内容包保留入口、依赖和兼容信息，市场分发与第三方代码隔离另行建设。

## 开发计划

- [整体重构计划 #1](https://github.com/maa-verge/maa-verge-automation/issues/1)：仓库边界、三层映射、原生化、双端消费与分阶段验收。
- [原生化试点 #2](https://github.com/maa-verge/maa-verge-automation/issues/2)：冻结基线，以唤醒与公招验证 MaaFW 原生流程及 TS Custom。
- [Debugger 计划](https://github.com/maa-verge/maa-verge-debugger/issues/1)：独立通用编辑与调试工具，共享模块作为可选项目适配接入。

建议与问题请提交到 [Issues](https://github.com/maa-verge/maa-verge-automation/issues)。

## 许可与致谢

本项目采用 **AGPL-3.0-only**，详见 [LICENSE](LICENSE)。MaaFramework 及其他第三方代码、模型、图片和游戏资料遵循各自许可与权利声明；本项目为独立社区项目。
