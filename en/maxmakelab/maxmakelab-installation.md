# MaxmakeLab Software Installation Guide: Download & Setup Tutorial

Learn how to install MaxmakeLab software for HiMill CNC machines. This guide covers system requirements, download links for Windows and macOS, installation steps, and troubleshooting tips.

## 📖 Software Introduction
MaxmakeLab is an intelligent control software designed specifically for HiMill series CNC equipment, providing an intuitive operation interface and rich processing functions to help users easily complete various creative processing tasks.

## 🖥️ System Requirements

### Windows System
- **Operating System**: Windows 10/11 (64-bit) or higher
- **Processor**: Intel i3 or equivalent performance CPU (non-ARM architecture)
- **Memory**: 4GB or more
- **Storage Space**: 1GB or more available space
- **Display**: Resolution 1920x1080 or higher
- **USB Port**: USB 2.0 or higher version

### macOS System
- **Operating System**: macOS 14 (Sonoma) or higher
- **Processor**: Apple Silicon
- **Memory**: 4GB or more
- **Storage Space**: 1GB or more available space
- **Display**: Resolution 1920x1080 or higher
- **USB Port**: USB 2.0 or higher version

> ⚠️ **Processor Compatibility Note**:
> Only supports Apple Silicon M-series chips, not Intel series chips.
> {.is-warning}

## 📥 Software Download
You can download MaxmakeLab software through the following links. Choose the appropriate version according to your operating system and needs:

> ℹ️ **Version 0.9.18 Update**:
> 1. Text function upgrade: Text creation function optimization
> 2. New tool library function: Add tools in the tool library, and edit tool parameters when generating toolpaths
> 3. Stock setup optimization: After setting stock, 2D area displays stock size within machine working area, supports adding graphics within the area
> 4. New Profile Milling, Pocket Milling, and Grayscale Relief strategies
> 5. New Simulation Preview: Supports machining simulation after generating toolpaths
> {.is-info}
>
> > ⚠️ **Notes**:
> > 1. The tool parameter library currently only supports one material type. Multi-material switching will be added in future updates. The software currently includes a set of parameters for soft wood machining.
> > 2. Currently supported tools: Flat end mill, Ball nose end mill, Flat tip V-bit, V-bit. Other tool types will be added in the future.
> > 3. Toolpaths are currently generated starting from the material surface. Start height setting will be added in future updates.
> > 4. Bridge function will be added in future updates.
> > 5. Ramp function will be added in future updates, so currently only soft wood and similar materials are supported. Hard wood and metal are not recommended.
> > 6. The relief function currently reserves a large roughing allowance. It is not recommended for hard woods like sandalwood. This feature will be optimized in future updates.
> > 7. G-code Generation: The generated code includes the first tool change command. Therefore, before machining, please click tool change in the software, measure tool height, set Z0, then start machining. (Must be executed, otherwise machining errors or height errors may occur)
> > 8. Mac version is expected to be updated next week.
> > 9. If you encounter any software issues, please contact us in the Discord software feedback channel. We will actively consider your suggestions and fix issues promptly: [Discord](https://discord.com/channels/1436232802227064903/1436232803061600351)
> > {.is-warning}

### Latest Version (v0.9.18)
**[MaxmakeLab Software Download Link(Windows)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.18.exe)**
**[MaxmakeLab Software Download Link(macOS)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.18.dmg)**

### Previous Version (v0.9.17)
**[MaxmakeLab Software Download Link(Windows)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.17.exe)**
**[MaxmakeLab Software Download Link(macOS)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.17.dmg)**

### Previous Version (v0.9.16)
**[MaxmakeLab Software Download Link(Windows)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.16.exe)**
**[MaxmakeLab Software Download Link(macOS)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.16.dmg)**

### Previous Version (v0.9.15)
**[MaxmakeLab Software Download Link(Windows)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.15.exe)**
**[MaxmakeLab Software Download Link(macOS)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.15.dmg)**

### Previous Version (v0.9.14)
**[MaxmakeLab Software Download Link(Windows)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.14.exe)**
**[MaxmakeLab Software Download Link(macOS)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.14.dmg)**

> Recommendation: Please always download the latest version of the software for the best functional experience and stability.
{.is-info}

## 🎬 Installation and Usage Process

### Windows System Installation and Usage Steps

#### 1. Double-click the installer to install the software

<img src="/eng/maxmakelab/media/maxmakelab-installation/1-双击安装软件.webp" alt="MAXMAKE MaxmakeLab Double-click Installer to Install Software" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

#### 2. Open the software

<img src="/eng/maxmakelab/media/maxmakelab-installation/2-打开软件.webp" alt="MAXMAKE MaxmakeLab Open Software" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

#### 3. Click auto-connect to find device, and click return to zero after connection

<img src="/eng/maxmakelab/media/maxmakelab-installation/3-自动连接，点击回零.webp" alt="MAXMAKE MaxmakeLab Auto-connect to Find Device" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

#### 4. You can also select device and manually select serial port to connect

<img src="/eng/maxmakelab/media/maxmakelab-installation/4-手动连接.webp" alt="MAXMAKE MaxmakeLab Manual Device Connection" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<!-- ### macOS System Installation and Usage Steps

#### 1. Download and install the software

> 📥 **Download and Install**:
> 
> - Download the Mac version installer from the official website
> - Double-click the .dmg file to open the image
> - Drag MaxmakeLab to the Applications folder
> - Authorization required in system preferences during first run

#### 2. Open the software

> 🚀 **Start Software**:
> 
> - Open MaxmakeLab from Launchpad or Applications folder
> - If security prompt appears, hold Control key and click to select "Open"
> - Wait for software to fully load

#### 3. Click auto-connect to find device, and click return to zero after connection

> 🔌 **Device Connection**:
> 
> - Click the "Auto Connect" button
> - Wait for software to search for devices
> - After successful connection, click "Return to Zero" operation
> - Confirm device status is normal

#### 4. You can also select device and manually select serial port to connect

> ⚙️ **Manual Connection**:
> 
> - Select your device from the device list
> - Manually enter or select the serial port number
> - Click the connect button to establish connection
> - Verify connection status -->

## ⚠️ Important Notes

> 🔍 **Device Connection Issues**:
> 
> When device cannot be found:
> 1. Try restarting the software
> 2. Try unplugging and re-plugging the USB data cable
> 3. Check if the device is properly powered on
> 4. Ensure the correct driver is installed
> 
> {.is-warning}

> ⚡ **Electrical Safety**:
> 
> - Ensure USB data cable connection is firm
> - Avoid disconnecting during data transmission
> - Check if USB port is working normally
> 
> 🛡️ **System Compatibility**:
> - Confirm operating system version meets requirements
> - Run software as administrator (if required)
> - Close potentially conflicting software of the same type
> 
> 🔧 **Troubleshooting**:
> - Restart software and equipment, then retry
> - Check driver status in Device Manager
> - Try different USB ports
> {.is-info}


## ❓ Frequently Asked Questions

### Windows System Issues

### Q: What should I do if an error occurs during installation?
A: Please ensure your computer meets system requirements, close other potentially conflicting software, re-download the installer and try installation again.

### Q: The software doesn't respond after startup?
A: Check if your computer has the latest graphics driver installed, try running the software as administrator.

### macOS System Issues

### Q: macOS system shows "Cannot be opened because it is from an unidentified developer"?
A: Hold the Control key and click the application icon, select "Open", then click "Open" again in the popup dialog.

### Q: Device cannot be recognized under macOS system?
A:
1. Ensure the latest version of macOS is installed
2. Check if USB data cable connection is stable, try changing USB port
3. Open "System Preferences" → "Security & Privacy" → "General", confirm MaxmakeLab's USB access permission is authorized
4. Try restarting software and equipment

### Common Issues

### Q: Device connects successfully but cannot be controlled?
A: Check if USB data cable is intact, try replacing the data cable or USB port, ensure device is properly powered on.

### Q: Software interface displays abnormally?
A: Check if your computer has the latest graphics driver installed, or adjust display resolution to recommended value.

---