# Shopcity 广告控制器 · 桌面版

这个仓库用于发布 Windows 桌面版安装包、更新文件和版本说明。开发项目在独立私有仓库维护。

## v1.0.0 正式版

- 独立桌面运行，支持单店铺、多广告账户管理。
- 观察／操作模式，持续执行广告保护、暂停复核和可选的账户当地时间定时开启。
- 广告明细、账户汇总、操作日志采用本地表格，支持独立视图、筛选、排序、分组、冻结、汇总和完整 CSV 导出。
- 支持托盘常驻、断网恢复、可选本地加密自动登录，以及手动／每日自动备份。
- 重启软件、安装更新或恢复备份后，需要手动启动任务。

## 首次安装

从 [最新正式版本](https://github.com/harmony-s/sc-fb-desktop/releases/latest) 下载 `ShopcityControllerSetup.exe`，关闭旧版后安装。

安装包链接：[下载 Windows 安装包](https://github.com/harmony-s/sc-fb-desktop/releases/latest/download/ShopcityControllerSetup.exe)。

## 后续更新

在软件左侧打开“软件更新”，检查并下载新版本，然后点击“重启安装更新”。软件也会在后台定期检查新版本。

重启安装前会停止广告任务，完成已发送请求的核验。本地数据库、规则、视图和登录会话会保留。更新后需要手动点击运行来继续广告任务。

v0.10.0 及更早版本没有内置更新入口，需要先手动安装一次带更新功能的版本。

## 发布文件

- `ShopcityControllerSetup.exe`：首次安装或手动更新。
- `RELEASES` 和 `XHShopcityController-<版本>-full.nupkg`：软件内置更新使用。
- `SHA256SUMS.txt`：发布文件校验值。

这些文件随 GitHub Release 提供，不存入 Git 文件历史。此仓库不存放使用者的本地广告数据库、登录信息或个人配置。
