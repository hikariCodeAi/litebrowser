LiteBrowser 公开发布仓库

本仓库用于发布 LiteBrowser 可下载二进制包、版本说明与 SHA256 校验和，不存放产品源码。

下载入口：https://github.com/hikariCodeAi/litebrowser/releases

当前平台状态（2026-10-21）：
Linux x86_64：提供 LiteBrowser 1.0.0（build 1）Preview 1，基于 Chromium 155.0.8059.39。
下载与说明：https://github.com/hikariCodeAi/litebrowser/releases/tag/linux-x86_64-1.0.0-preview.1
下载 litebrowser-1.0.0-linux-x86_64.tar.gz 与同名 .sha256；先用 sha256sum -c 校验，解包后以普通用户执行 LiteBrowser-linux-x86_64/chrome。
包大小：563831731 字节。
SHA256：61dba307f14b7cb67f1413c97ed549e25a3fff4f00a1f52436c9083038ca4a20
完整构建/运行依赖/第三方许可覆盖通过；普通用户 Xvfb 图形显示下默认桌面、Qt6 失败回退和最终包全新解压三套会话均通过基础导航/JS/图片/音视频、版本/试用状态、重启持久性、原生沙箱和正常退出检查。完整文件/权限/相对链接在测试与解包前后核同。真实30天/48小时等待及生产激活未测试。
运行需要相应桌面系统库与可用的 Chromium 原生沙箱。Qt 桌面集成为可选功能；随包 Qt6 插件要求 Qt 6.4 或更新版本，本轮 Ubuntu 22.04 宿主 Qt 6.2.4 不支持该插件，Qt6 兼容性尚未验证。其他发行版与旧系统兼容性未验证。
Linux 更新通过发布仓库手动下载，不支持直接自动安装。新版性能对比、长期稳定性、真实 Create 业务和 B1/B2 均未测试；历史八层候选数据不作为本版性能结论。

macOS arm64：提供 LiteBrowser L 155.0.8059.39 Preview 1，适用于 Apple Silicon。
下载与说明：https://github.com/hikariCodeAi/litebrowser/releases/tag/macos-arm64-155.0.8059.39-preview.1
下载 ZIP 与同名 .sha256，在 Mac 内置 APFS 磁盘解压后运行 Chromium.app。
应用声明最低 macOS 13.0；旧版系统兼容性未验证。Intel Mac 不适用。
ZIP 大小：241,781,825 字节。
SHA256：15152dacedbca0477d585f440769684a7e611221323928b112c9ec62b13b0b7e

本版为试用预发布版：B3/L 完整构建、可见窗口、基础功能和 APFS 重新解包验证在构建机 macOS 26.6.2 上通过。
macOS 26.0.1 首次自动验证在初始 CDP 控制阶段超时，首次启动的系统安全提示需用户本人处理；处理后新标签页和内部版本页可显示，外网导航及五项自动检查尚未复验通过，不作系统不兼容或跨机器完整验收结论。
完整应用签名验证未通过，未完成 Developer ID 签名及 Apple 公证。
Mac 性能、长期稳定性及 Create 业务验收尚未运行，不作正式产品验收或性能收益声明。
随包原始许可与版权声明保持；旧 INTERNAL-NOTICE 记录构建时范围，本次按后续授权公开供试用，不新增项目源码开源许可。

Windows x64：尚未提供可下载的 Windows Release。
仅下载 Releases 中已实际上传的平台资产。各平台构建和测试结论不互相替代。

公开主页导航：
index.html：学术风静态发布页，包含策略说明、明确标注的非实测示意图与真实平台下载入口。
assets/：本层公开品牌图片与独立主视觉，见 assets/readme.txt。
DESIGN_GUIDE.md、design-theme.json、design-variables.css、motion-variables.css：主页设计规范与集中主题变量。
AGENTS.md：公开仓库的内容和样式协作约定。
