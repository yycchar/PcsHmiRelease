# PcsHmi 发布下载

本仓库提供 PCS 调试、维护、部署软件及 08B 边端服务安装包；工程源码位于 [PcsHmi](https://github.com/yycchar/PcsHmi)。

## 当前发布：2026-10-30

[打开本次完整发布页](https://github.com/yycchar/PcsHmiRelease/releases/tag/release-20261030-01)

| 产品 | 版本 | 平台与运行要求 |
|---|---|---|
| 调试上位机 PcsHmi.App | 1.1.5 | Windows x64，需安装 .NET 10 x64 Runtime |
| 维护上位机 PcsHmi.StationApp | 1.1.5 | Windows x64，已包含 .NET 运行时 |
| 部署上位机 PcsHmi.DeployApp | 1.1.4 | Windows x64，已包含 .NET 运行时 |
| 边端服务 PcsHmi.EdgeService | 1.1.5 | Linux ARM64 / 08B，包含 .NET 运行时，需兼容的系统库及系统 SQLite |

本次调试包的 3.5MW 机型与边端包均使用：PCS01 `192.168.111.200:502`、PCS02 `192.168.111.201:502`，Modbus Unit ID 均为 1。使用前核对现场网络，设备地址可在对应 `devices.csv` 中调整。

Windows ZIP 请完整解压后运行对应 EXE。调试上位机包含 3.5MW、2.5MW 两套独立配置，启动时选择机型。维护上位机参数群发选择调试包中的 `config/profiles/PCS_3.5MW` 目录，不使用 2.5MW 点表。

边端 `.tar.gz` 供部署上位机选择后部署；下载或更新电脑程序不会自动升级板卡。部署时根据实际需要选择使用包内点表、本地点表或保留板卡点表。

各附件的完整文件名、大小与 SHA-256 见发布页和 `SHA256SUMS.txt`。GitHub 自动生成的 Source code ZIP/TAR 仅含本发布仓库的说明，不是软件安装包。

## 历史发布

- [调试上位机 1.0.10](https://github.com/yycchar/PcsHmiRelease/releases/tag/pcshmi-app-v1.0.10)
- [2026-10-15 产物快照](https://github.com/yycchar/PcsHmiRelease/releases/tag/release-20261015-01)
