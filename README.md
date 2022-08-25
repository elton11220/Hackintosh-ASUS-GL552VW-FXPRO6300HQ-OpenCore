# Hackintosh-ASUS-GL552VW-FXPRO6300HQ-OpenCore Bootloader Configuration

It's been a long time. This repo was created in 2020. I haven't had time to archive it because I'm busy.

In 2022, I have a new notebook computer. Recently, I suddenly thought of this old computer and planned to convert it into a desktop computer. So I studied it and got some success.

The boot file in this repo is made with `OpenCore 0.8.3`. After my test, it can run `macOS Big Sur 11.6.8` normally.

> The test version with the support for `macOS Monterey` is pushed in the test branch, it is untested and unstable, you can try it if you want to experience macOS Monterey.

## Configure BIOS

1. Update your bios to `v304`
2. Turn off `Fast Boot`, `CSM Mode`, `Secure Boot`, `VT-d` in the UEFI
3. Set `dmvt` to `256mb` in `Graphic Configuration` menu
4. You need to use `modGrubShell` to disable `cfg lock`

## Configuration of the laptop

| Type | Name |
| - | - |
| CPU | i5-6300hq |
| GPU | Intel HD Graphics 530 |
| RAM | 16gb (32gb is also supported in this laptop)|
| Touchpad | ELAN 1000 |
| Sound | Conexant 20751/2 |
| WLAN | Boradcom 94350(DW1820A) |

## Attention

Hardware compatibility:
| Work well | Hardware |
| - | - |
| no | Touchpad |
| yes | Sound |
| yes | GPU |
| yes | WLAN |
| yes | Camera |
| yes | Bluetooth |