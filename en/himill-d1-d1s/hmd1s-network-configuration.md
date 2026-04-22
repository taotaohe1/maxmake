# 📡 MaxmakeLab HiMill D1/D1S Network Configuration

## 🌟 Feature Introduction

The HiMill device is equipped with a built-in WiFi module that supports wireless control functionality. After configuring the network and connecting to the device, you can achieve the same operation experience as using a data cable connection when the network is stable. Below are detailed instructions for the two WiFi connection methods:

---

## 🏠 Local Network Connection

Local network connection allows the HiMill device to connect directly to your home or office router, enabling computers on the same local network to access the device (the computer must also be connected to the same router).
    
### Step 1: Connect Device via USB and Complete Reset

1. Launch the MaxmakeLab software
2. Connect the device to your computer using a USB cable
3. Wait for the device to complete automatic reset, and ensure the device status is normal before proceeding to the next step

<img src="/eng/himill-d1-d1s/media/network-configuration/usb连接.webp" alt="Connect Device via USB" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

### Step 2: Select STA Mode and Configure WiFi Parameters

1. Click the "Device Settings" button in the software interface
2. Select "STA Mode" in the settings interface
3. Enter your router's WiFi name (SSID) and password

> ⚠️ **Important Notice**：
> - Please ensure the WiFi name (SSID) and password are entered correctly, as this process will directly write the configuration information to the device's WiFi module. Incorrect input will result in connection failure
> - WiFi name (SSID) and password should not contain spaces or special characters, as this may cause configuration failure
> 
> {.is-warning}

<img src="/eng/himill-d1-d1s/media/network-configuration/切换sta.webp" alt="Select STA Mode and Configure WiFi" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

### Step 3: Click Config Button to Configure

1. Click the "Config" button to start the configuration process
2. The software will transfer the configuration information to the device item by item, please wait patiently for the configuration to complete
3. After successful configuration, the software will display a "Restarting network module" prompt
4. Click "Confirm" and wait 15-30 seconds for the device to complete the network module restart

<img src="/eng/himill-d1-d1s/media/network-configuration/点击config.webp" alt="Click Config to Configure" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

### Step 4: View Device IP Address

1. After waiting 15-30 seconds, reopen the "Device Settings" interface
2. If the device successfully connected to the router, the interface will display the IP address obtained by the device
3. Record this IP address, as it will be needed for subsequent connections
4. Close the software and power off the device to complete the network configuration process

> ⚠️ **Important Notice**：
> - Please unplug the USB cable before restarting the device
> - Keep the USB cable disconnected during wireless control
> 
> {.is-warning}

<img src="/eng/himill-d1-d1s/media/network-configuration/查看sta_ip地址.webp" alt="View IP Address" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

### Step 5: Connect to Device via IP Address

1. Restart the MaxmakeLab software
2. Click the "Connect" button and select "IP Connection" mode
3. Select your computer's IP address from the "Local IP Address" dropdown menu (usually only one option; if there are multiple, check the wireless network adapter IP address in your computer's network settings)
4. Enter the device IP address you recorded earlier in the "Device IP" input box
5. Click the "Connect" button, and a connection success prompt will appear after successful connection

> ⚠️ **Connection Tips**：
> - If the first connection attempt fails, disconnect and try again
> - After successful connection, it is recommended to enter the "workflow" interface and perform a "homing" operation to confirm the device responds normally
> 
> {.is-warning}

<img src="/eng/himill-d1-d1s/media/network-configuration/通过sta连接设备.webp" alt="Connect via IP Address" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

---

## 📱 Hotspot Connection

If you don't have a network at home or the local network connection has high latency, you can try using the hotspot connection method.

### Default Hotspot Information

- **Hotspot Name**: HiMill-AP
- **Hotspot Password**: 12345678
- **Default IP Address**: 192.168.0.1

### Steps to Switch to Hotspot Mode

If the device has been configured for network connection and you want to switch to hotspot mode, follow these steps:

### Step 1: Connect Device via USB and Complete Reset

1. Launch the MaxmakeLab software
2. Connect the device to your computer using a USB cable
3. Wait for the device to complete automatic reset, and ensure the device status is normal

<img src="/eng/himill-d1-d1s/media/network-configuration/usb连接.webp" alt="Connect Device via USB" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

### Step 2: Select AP Mode and Prepare Configuration

1. Click the "Device Settings" button in the software interface
2. Select "AP Mode" in the settings interface

> ℹ️ **Feature Description**：
> - Currently, AP mode conflicts with STA mode, and you must enter a name and password to click the configuration button (you can enter any values, this issue will be fixed in future versions)
> 
> {.is-info}

<img src="/eng/himill-d1-d1s/media/network-configuration/切换ap.webp" alt="Select AP Mode and Prepare Configuration" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

### Step 3: Click Config Button to Configure

1. Click the "Config" button to start the configuration process
2. Wait for the software to complete the configuration transfer
3. After successful configuration, the software will display a "Restarting network module" prompt
4. Click "Confirm" and wait 15-30 seconds for the device to complete the network module restart

<img src="/eng/himill-d1-d1s/media/network-configuration/点击config2.webp" alt="Click Config to Configure" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

### Step 4: Restart Device and Confirm Hotspot Mode

1. Close the software and power off the device
2. After restarting, the device will automatically enter hotspot mode with the hotspot name "HiMill-AP"

> ⚠️ **Important Notice**：
> - Please unplug the USB cable before restarting the device
> - Keep the USB cable disconnected during wireless control
> 
> {.is-warning}

<img src="/eng/himill-d1-d1s/media/network-configuration/通过ap连接设备.webp" alt="View IP Address" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

### Step 5: Connect Computer to Device Hotspot

1. Find and connect to the "HiMill-AP" hotspot in your computer's WiFi settings
2. Enter the hotspot password: 12345678

> ⚠️ **Connection Tips**：
> - After connecting to the device hotspot, your computer will temporarily disconnect from the internet
> 
> {.is-warning}

### Step 6: Connect to Device via IP Address

1. Launch the MaxmakeLab software
2. Click the "Connect" button and select "IP Connection" mode
3. Select your computer's IP address from the "Local IP Address" dropdown menu
4. Enter the default IP address: 192.168.0.1 in the "Device IP" input box
5. Click the "Connect" button, and a connection success prompt will appear after successful connection

> ⚠️ **Connection Tips**：
> - If the first connection attempt fails, disconnect and try again
> - After successful connection, it is recommended to enter the "workflow" interface and perform a "homing" operation to confirm the device responds normally
> 
> {.is-warning}

<img src="/eng/himill-d1-d1s/media/network-configuration/通过ap连接设备.webp" alt="Connect via IP Address" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

---

## 📋 Feature Description

> ℹ️ **Current Feature Status**：
> - Currently only IP network connection is supported
> - Other network-related features are under development
> - Please stay tuned to this page for future updates
> 
> {.is-info}

---

