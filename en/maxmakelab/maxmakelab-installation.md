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

> ℹ️ **Version 0.9.20 Update**:
> 
> **1. Probe Function**
> 1. Added probe status indicator on the tool setting interface
> 2. Added F value after M3/M4 commands in GCode for probe height map application
> 
> **2. Tool Parameters & Toolpath**
> 1. Fixed incorrect toolpath issue in offset contour milling with complex tools
> 2. Tool parameter database adjustment: software updates will no longer overwrite user-modified tool parameters. Defaults to loading toolbase_user.db3 (automatically copied from toolbase.db3 if not present), user parameters are saved in this file
> 3. Added popup prompt for resetting tool parameter library
> 
> **3. Layer Management**
> 1. Fixed the issue where layers appeared in laser mode after adding graphics in CNC mode
> 2. Fixed the issue where layer info was still displayed when no elements existed in the layer in laser mode
> 
> **4. Element Operations & Rendering**
> 1. Added element width/height rendering, ruler width/height highlight rendering
> 2. Alignment operations now support using Shift-selected single element as reference element
> 3. Added snap-to-alignment function when moving elements on 2D canvas
> 4. Fixed the issue where elements disappeared after multiple ungroup operations
> 5. Added crop function
> 
> **5. Text Editing**
> 1. Fixed UI issue when pressing ESC during text addition interaction
> 2. Fixed rendering issue when pressing ESC during double-click text re-editing
> 3. When the selected font doesn't support certain characters, fallback fonts (from project) are used to load glyphs
> 4. Changed ESC behavior from cancel to submit during text interaction; pressing ESC after re-editing text now triggers submit
> 5. Redesigned node editing: currently only supports moving control points; adding/removing nodes will be added in future
> 
> **6. Error Handling & Stability**
> 1. Fixed the issue where homing and detection buttons in alarm errors 3, 4, 5, 8, 9 caused software crashes
> 2. Alarm popup display now consistent with About window display, no longer shown as a separate window
> 
> **7. UI/UX Optimization**
> 1. User prompt on software startup is now closed by default
> 2. Tool change popup now auto-closes after 3 seconds
> 3. Fixed cursor issue when switching from crop action to node editing action
> 
> If you encounter any software issues, please contact us in the Discord software feedback channel. We will actively consider your suggestions and fix issues promptly: [Discord](https://discord.com/channels/1436232802227064903/1436232803061600351)
> {.is-info}

### Latest Version (v0.9.20)
**[MaxmakeLab Software Download Link(Windows)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.20.exe)**
**[MaxmakeLab Software Download Link(macOS)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.20.dmg)**

### Previous Version (v0.9.19)
**[MaxmakeLab Software Download Link(Windows)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.19.exe)**
**[MaxmakeLab Software Download Link(macOS)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.19.dmg)**

### Previous Version (v0.9.18)
**[MaxmakeLab Software Download Link(Windows)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.18.exe)**
**[MaxmakeLab Software Download Link(macOS)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.18.dmg)**

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