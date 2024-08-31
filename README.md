# Lenovo-XiaoXin-310-15IKB-Hackintosh
本项目修改自 [lee-namc / Lenovo-V310-15IKB-Hackintosh](https://github.com/lee-namc/Lenovo-V310-15IKB-Hackintosh) 。
目前提供 Monterey 和 Ventura 两个版本。
## Monterey-EFI
| 规格     | 详细信息                 |
| -------- | ------------------------ |
| CPU      | i5-7500U                 |
| GPU      | HD 620                   |
| Memory   | 8 GB                    |
| Wireless | Realtek AC201             |
| 操作系统 | Monterey |  

大致可用情况与原项目相同。本项目主要做了以下修改：
- 由于两机型网卡不同，移除了INTEL网卡驱动，目前机载网卡无解
- 注入了声卡 ID，可以使用内置扬声器及话筒
## Ventura-EFI
| 规格     | 详细信息                 |
| -------- | ------------------------ |
| CPU      | i5-7500U                 |
| GPU      | HD 620                   |
| Memory   | 8 GB                    |
| Wireless | DW1560             |
| 操作系统 | Ventura |  

本 EFI 文件由 Monterey 版本修改而来，主要改动有：
- 更新 OpenCore 版本至 v1.0.1，并改用 MOD 版本以解决 Windows 启动问题
- 拆机更换原网卡为 DW1560，并注入相关驱动解决 Wi-Fi 和蓝牙问题
- 恢复到 Monterey 版本 EFI 的可用性（主要是驱动显卡）
- 使用 USBToolBox 定制 USB 接口

---

**请注意：本仓库的两份 EFI 文件都在 `config.plist` 文件中写入了三码，并且尚在使用，请在使用本 EFI 时自行更改，谢谢！**