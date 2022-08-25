# Hackintosh-ASUS-GL552VW-FXPRO6300HQ-OpenCore Bootloader Configuration

好久不见，这个仓库在2020年创建，由于本人比较忙一直没有时间制作。

2022年，我也有了新的笔记本电脑，最近突然想起了这个旧电脑，打算把它改装成台式机。所以研究了一下，并取得了一定的成功。

这个仓库中的引导文件使用 `OpenCore 0.8.3` 制作，经过本人测试可以正常运行 `macOS Big Sur 11.6.8`。

> 支持`macOS Monterey`的测试版本已在测试分支中推送，它未经测试且不稳定，如果您想体验macOS Monterey，可以尝试。

## 配置BIOS

1. 把你的UEFI固件版本升级为`304`版本
2. 在UEFI设置中关闭`Fast Boot`, `CSM Mode`, `Secure Boot`, `VT-d`
3. 在UEFI中的`Graphic Configuration`菜单中把`dvmt`设置为`256mb`
4. 你需要使用`modGrubShell`关闭主板的的`cfg lock`

## 电脑配置

| 种类 | 硬件名 |
| - | - |
| CPU | i5-6300hq |
| GPU | Intel HD Graphics 530 |
| RAM | 16gb (经测试该机型最高支持32gb内存)|
| Touchpad | ELAN 1000 |
| Sound | Conexant 20751/2 |
| WLAN | Boradcom 94350(DW1820A) |

## 注意

硬件兼容性：
| 正常运行 | 硬件 |
| - | - |
| no | Touchpad |
| yes | Sound |
| yes | GPU |
| yes | WLAN |
| yes | Camera |
| yes | Bluetooth |