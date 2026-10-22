---
title: "MaxmakeLab HiMill D1/D1S 固件升级"
---

# MaxmakeLab HiMill D1/D1S 固件升级

## ⚠️ 注意事项

> 1. **软件版本要求**：建议使用最新版本软件。如果在产品发布前使用过测试版软件，请先卸载删除后下载最新版本。
> 2. **连接方式**：升级固件必须使用USB数据线，请退出WiFi模式并插上USB数据线。
> 3. **升级过程**：升级过程中，请勿拔掉连接线，请勿关闭电源
>
> {.is-warning}
>
> **从软件版本0.9.17开始**：
>
> 固件更新在新弹窗进程中打开。
>
> - **自动更新**：可按照提示进行操作。
> - **手动更新**：请遵循以下步骤：
>   1. 选择设备串口：Windows端通常选择COM**，Mac端通常选择cu.usbmodem***或tty.usbmodem***
>   2. 选择正确的串口后点击Open，下方会显示<Boot|Ver:1.4>表示连接成功
>   3. 点击Select，手动选择固件文件
>   4. 点击Flash，等待烧写进度完成
>   5. 重启设备

---

## 📝 自动升级流程

### 步骤 1：软件版本检查

软件连接到设备后，会自动查询当前设备的固件版本。如需更新，会弹出提示框。

<img src="/chi/himill-d1-d1s/media/hmd1s-firmware-upgrade/自动步骤一.png" alt="固件更新提示" style="max-width: 1100px;">

### 步骤 2：进入引导模式

点击确认后，自动打开设备设置，并弹出提示框，询问是否进入引导模式并开始固件升级。

<img src="/chi/himill-d1-d1s/media/hmd1s-firmware-upgrade/自动步骤二.png" alt="进入引导模式提示" style="max-width: 1100px;"> 

### 步骤 3：打开固件烧录窗口

点击确认后，系统会弹出固件烧录窗口。

<img src="/chi/himill-d1-d1s/media/hmd1s-firmware-upgrade/自动步骤三.png" alt="固件烧录窗口" style="max-width: 1100px;">

### 步骤 4：执行固件烧录

在烧录窗口中选择对应的设备串口，点击 Open 建立连接，然后直接点击 Flash 开始烧录，无需手动选择固件文件，等待进度完成即可。

<img src="/chi/himill-d1-d1s/media/hmd1s-firmware-upgrade/自动步骤四.png" alt="执行固件烧录" style="max-width: 1100px;">

---

## 📝 手动升级流程

### 步骤 1：打开设备设置界面

连接设备后，点击设备设置按钮，打开设备设置界面，然后点击 Firmware Flash 按钮。

<img src="/chi/himill-d1-d1s/media/hmd1s-firmware-upgrade/手动步骤一.png" alt="打开设备设置界面" style="max-width: 1100px;">

### 步骤 2：确认进入烧录模式

点击确认，进入固件烧录模式。

<img src="/chi/himill-d1-d1s/media/hmd1s-firmware-upgrade/手动步骤二.png" alt="确认进入烧录模式" style="max-width: 1100px;">

### 步骤 3：配置烧录参数并烧录

进入烧录窗口后，按以下步骤操作：
1. **选择设备串口**：Windows 端通常选择 COM 接口，Mac 端通常选择 cu.usbmodem 或 tty.usbmodem
2. **建立连接**：选择正确的串口后点击 Open，窗口下方显示 `<Boot|Ver:1.4>` 表示连接成功
3. **选择固件文件**：点击 Select，手动选择要烧录的固件文件

> 提示：最新固件可在此页面下载（[跳转到固件发布界面](/zh/himill-d1-d1s/hmd1s-firmware-release-record.md)）
> {.is-info}

4. **开始烧录**：点击 Flash，等待烧写进度完成

Windows 端：
<img src="/chi/himill-d1-d1s/media/hmd1s-firmware-upgrade/手动步骤三.png" alt="选择设备串口（Windows）" style="max-width: 1100px;">

Mac 端：
<img src="/chi/himill-d1-d1s/media/hmd1s-firmware-upgrade/手动步骤三mac.png" alt="选择设备串口（Mac）" style="max-width: 1100px;">

### 步骤 4：完成升级

烧录完成后，在烧录窗口中点击 OK，然后重启设备即可使用新固件。

<img src="/chi/himill-d1-d1s/media/hmd1s-firmware-upgrade/手动步骤四.png" alt="升级完成" style="max-width: 1100px;">
