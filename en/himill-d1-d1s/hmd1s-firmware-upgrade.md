# HiMill D1/D1S Firmware Upgrade Guide: Auto & Manual Flashing Tutorial

Learn how to upgrade firmware on HiMill D1/D1S CNC machine. This guide covers automatic update process, manual flashing steps, bootloader mode, and important precautions during firmware installation.

## ⚠️ Important Notes

> 1. **Software Version Requirement**: It is recommended to use the latest version of the software. If you have used the beta version before the product release, please uninstall and delete it first, then download the latest version.
> 2. **Connection Method**: Firmware upgrade must use USB data cable. Please exit WiFi mode and plug in the USB data cable.
> 3. **Upgrade Process**:
>    - Do not unplug the connection cable during the upgrade process
>    - Do not turn off the power during the upgrade process
>
> {.is-warning}
>
> **Starting from Software Version 0.9.17**:
>
> Firmware updates open in a new pop-up window.
>
> - **Auto Update**: Follow the prompts to proceed.
> - **Manual Update**: Please follow these steps:
>   1. Select the device serial port: On Windows, typically select COM**, on Mac, typically select cu.usbmodem*** or tty.usbmodem***
>   2. After selecting the correct serial port, click Open. The message <Boot|Ver:1.4> will appear below indicating successful connection
>   3. Click Select to manually choose the firmware file
>   4. Click Flash and wait for the flashing progress to complete
>   5. Restart the device

---

## 📝 Auto Upgrade Process

### Step 1: Software Version Check

After the software connects to the device, it will automatically check the current firmware version. If an update is needed, a prompt box will pop up.

<img src="/eng/himill-d1-d1s/media/hmd1s-firmware-upgrade/firmware_update_prompt.png" alt="Firmware Update Prompt" style="max-width: 800px;">

### Step 2: Enter Bootloader Mode

After clicking confirm, the device settings will open automatically, and a prompt box will pop up asking whether to enter bootloader mode and start firmware upgrade.

<img src="/eng/himill-d1-d1s/media/hmd1s-firmware-upgrade/bootloader_mode_prompt.png" alt="Enter Bootloader Mode Prompt" style="max-width: 800px;">

### Step 3: Firmware Flashing

After clicking confirm, the firmware flashing will start automatically. Wait for the progress bar to complete loading.

<img src="/eng/himill-d1-d1s/media/hmd1s-firmware-upgrade/firmware_flashing.png" alt="Firmware Flashing Progress" style="max-width: 800px;">

### Step 4: Upgrade Complete

After the flashing is complete, a success prompt box will pop up. At this point, you need to reconnect the device to use the upgraded firmware.

---

## 📝 Manual Upgrade Process

### Step 1: Open Device Settings

After connecting the device, click the device settings button to open the device settings interface.

<img src="/eng/himill-d1-d1s/media/hmd1s-firmware-upgrade/1.png" alt="Open Device Settings" style="max-width: 800px;">

### Step 2: Select Firmware File

Click "Open" and select the downloaded firmware file.

>Note: The latest firmware can be downloaded on this page ([Jump to Firmware Release Page](/en/himill-d1-d1s/hmd1s-firmware-release-record.md))
> {.is-info}

<img src="/eng/himill-d1-d1s/media/hmd1s-firmware-upgrade/2.png" alt="Select Firmware File" style="max-width: 800px;">

### Step 3: Start Flashing

After selecting the firmware, click "Flash" and confirm in the pop-up prompt.

<img src="/eng/himill-d1-d1s/media/hmd1s-firmware-upgrade/3.png" alt="Start Flashing" style="max-width: 800px;">

### Step 4: Upgrade Complete

Wait for the progress bar to complete. After the flashing is complete, you can reconnect to use the device.

<img src="/eng/himill-d1-d1s/media/hmd1s-firmware-upgrade/4.png" alt="Upgrade Complete" style="max-width: 800px;">
