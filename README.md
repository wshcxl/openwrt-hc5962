# openwrt-hc5962

极路由4增强版 (HiWiFi HC5962) 的 ImmortalWrt 云编译仓库。

## 固件内容

- 基底：ImmortalWrt 24.10（ramips/mt7621）
- 插件：
  - **QModem**（网络拨号，`luci-app-qmodem-next` 纯JS前端）— 来自 fork: [wshcxl/QModem](https://github.com/wshcxl/QModem)（上游 [FUjr/QModem](https://github.com/FUjr/QModem)）
  - **OpenAppFilter**（手机APP管理/应用过滤）— 来自 fork: [wshcxl/Open-App](https://github.com/wshcxl/Open-App)（上游 [destan19/OpenAppFilter](https://github.com/destan19/OpenAppFilter)）

## 编译方式

推送到 `main` 分支或手动触发 Actions（workflow_dispatch）即自动编译，
固件在 Actions 的 Artifact 和 Releases 里下载。

## 刷机

- 已在 OpenWrt/ImmortalWrt 系统：用 `*-sysupgrade.bin`，LuCI 或 `sysupgrade` 均可
- 从原厂固件/不死鸟 breed：用 `*-factory.bin`
