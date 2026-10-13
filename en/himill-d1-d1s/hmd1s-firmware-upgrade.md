# MaxmakeLab HiMill D1/D1S Firmware Upgrade

## ⚠️ Important Notes

> 1. **Software Version Requirement**: It is recommended to use the latest version of the software. If you have used the beta version before the product release, please uninstall and delete it first, then download the latest version.
> 2. **Connection Method**: Firmware upgrade must use a USB data cable. Please exit WiFi mode and plug in the USB data cable.
> 3. **Upgrade Process**: Do not unplug the connection cable or turn off the power during the upgrade process.
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
>   2. After selecting the correct serial port, click Open. The message <Boot|Ver:1.4> will appear below indicating a successful connection
>   3. Click Select to manually choose the firmware file
>   4. Click Flash and wait for the flashing progress to complete
>   5. Restart the device

---

## 📝 Auto Upgrade Process

### Step 1: Software Version Check

After the software connects to the device, it automatically queries the current firmware version. If an update is needed, a prompt box will appear.

<img src="/eng/himill-d1-d1s/media/hmd1s-firmware-upgrade/自动步骤一.png" alt="Firmware Update Prompt" style="max-width: 800px;">

### Step 2: Enter Bootloader Mode

After clicking confirm, the device settings will open automatically, and a prompt box will appear asking whether to enter bootloader mode and start the firmware upgrade.

<img src="/eng/himill-d1-d1s/media/hmd1s-firmware-upgrade/自动步骤二.png" alt="Enter Bootloader Mode Prompt" style="max-width: 800px;"> 

### Step 3: Open Firmware Flashing Window

After clicking confirm, the firmware flashing window will appear.

<img src="/eng/himill-d1-d1s/media/hmd1s-firmware-upgrade/自动步骤三.png" alt="Firmware Flashing Window" style="max-width: 800px;">

### Step 4: Execute Firmware Flashing

In the flashing window, select the corresponding device serial port, click Open to establish a connection, then click Flash to start flashing directly — no need to manually select a firmware file. Wait for the progress to complete.

<img src="/eng/himill-d1-d1s/media/hmd1s-firmware-upgrade/自动步骤四.png" alt="Execute Firmware Flashing" style="max-width: 800px;">

---

## 📝 Manual Upgrade Process

### Step 1: Open Device Settings

After connecting the device, click the device settings button to open the device settings interface, then click the Firmware Flash button.

<img src="/eng/himill-d1-d1s/media/hmd1s-firmware-upgrade/手动步骤一.png" alt="Open Device Settings" style="max-width: 800px;">

### Step 2: Confirm Entering Flashing Mode

Click confirm to enter the firmware flashing mode.

<img src="/eng/himill-d1-d1s/media/hmd1s-firmware-upgrade/手动步骤二.png" alt="Confirm Entering Flashing Mode" style="max-width: 800px;">

### Step 3: Configure Flashing Parameters and Flash

After entering the flashing window, follow these steps:
1. **Select the device serial port**: On Windows, typically select a COM port; on Mac, typically select cu.usbmodem or tty.usbmodem
2. **Establish a connection**: After selecting the correct serial port, click Open. The message `<Boot|Ver:1.4>` displayed below the window indicates a successful connection
3. **Select the firmware file**: Click Select to manually choose the firmware file to flash

> Note: The latest firmware can be downloaded on this page ([Go to Firmware Release Page](/en/himill-d1-d1s/hmd1s-firmware-release-record.md))
> {.is-info}

4. **Start flashing**: Click Flash and wait for the flashing progress to complete

Windows:
<img src="/eng/himill-d1-d1s/media/hmd1s-firmware-upgrade/手动步骤三.png" alt="Select Device Serial Port (Windows)" style="max-width: 800px;">

Mac:
<img src="/eng/himill-d1-d1s/media/hmd1s-firmware-upgrade/手动步骤三mac.png" alt="Select Device Serial Port (Mac)" style="max-width: 800px;">

### Step 4: Complete the Upgrade

After flashing is complete, click OK in the flashing window, then restart the device to use the new firmware.

<img src="/eng/himill-d1-d1s/media/hmd1s-firmware-upgrade/手动步骤四.png" alt="Upgrade Complete" style="max-width: 800px;">
