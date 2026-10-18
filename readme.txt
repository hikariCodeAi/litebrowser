LiteBrowser 公开发布仓库

本仓库用于发布 LiteBrowser 可下载二进制包、版本说明与 SHA256 校验和，不存放产品源码。

下载入口：https://github.com/hikariCodeAi/litebrowser/releases

当前平台状态（2026-10-18）：
macOS arm64：提供 LiteBrowser L 155.0.8059.39 Preview 1，适用于 Apple Silicon。
下载与说明：https://github.com/hikariCodeAi/litebrowser/releases/tag/macos-arm64-155.0.8059.39-preview.1
下载 ZIP 与同名 .sha256，在 Mac 内置 APFS 磁盘解压后运行 Chromium.app。
应用声明最低 macOS 13.0；旧版系统兼容性未验证。Intel Mac 不适用。
ZIP 大小：241,781,825 字节。
SHA256：15152dacedbca0477d585f440769684a7e611221323928b112c9ec62b13b0b7e

本版为试用预发布版：B3/L 完整构建、可见窗口、基础功能和 APFS 重新解包验证在构建机 macOS 26.6.2 上通过。
macOS 26.0.1 已知问题：本机自动验证在初始 CDP 控制阶段超时，内部版本页可显示，外网导航尚未验证通过；请仅作排查试用，不作跨机器验收通过。
完整应用签名验证未通过，未完成 Developer ID 签名及 Apple 公证。
Mac 性能、长期稳定性及 Create 业务验收尚未运行，不作正式产品验收或性能收益声明。
随包原始许可与版权声明保持；旧 INTERNAL-NOTICE 记录构建时范围，本次按后续授权公开供试用，不新增项目源码开源许可。

Windows x64：尚未提供可下载的 Windows Release。
Linux x86_64：已有候选构建，本仓库尚未上传。
仅下载 Releases 中已实际上传的平台资产。各平台构建和测试结论不互相替代。
