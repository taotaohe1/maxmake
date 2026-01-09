# MaxmakeLab Software Getting Started

## 📖 Software Overview

MaxmakeLab is an intelligent control software designed specifically for HiMill series CNC equipment, providing an intuitive operation interface and rich processing functions to help users easily complete various creative processing tasks. Whether you are a CNC beginner or an experienced user, you can quickly get started with using it.

The software supports both CNC processing and laser processing modes, with complete design, toolpath generation, and processing control functions, providing users with a one-stop processing solution.


## 🎨 Main Interface Function Introduction

MaxmakeLab adopts a modular interface design, mainly divided into the following functional areas:

<div style="display: flex; gap: 16px; flex-wrap: wrap;">
  <img src="/eng/maxmakelab/media/software-manual/main-interface1.png" alt="Main Interface Layout 1" style="width: calc(50% - 8px); height: auto; border-radius: 8px;" />
  <img src="/eng/maxmakelab/media/software-manual/main-interface2.png" alt="Main Interface Layout 2" style="width: calc(50% - 8px); height: auto; border-radius: 8px;" />
</div>

### Interface Function Partition

| Area | Name | Function Description |
|------|------|---------------------|
| 1 | Menu Bar | Import and export files, adjust view size, software settings, help guide, language switching, mode switching |
| 2 | Design Bar | Add various types of primitives (lines, rectangles, circles, text, images, etc.) |
| 3 | Canvas | Generally the size of the device's working area, used for designing and editing processing graphics |
| 4 | Color Bar | Assign different colors to primitives for easy distinction and processing parameter setting |
| 5 | Device Bar | Select, connect, and quickly control devices |
| 6 | Parameter Setting | Set blank parameters and tool library parameters in CNC mode, set processing parameters in laser mode |
| 7 | Generate Toolpath | Choose the way to generate toolpath (contour milling, plane milling, V-type milling, drilling, relief, etc.) |
| 8 | Toolpath List | Display already generated toolpaths |
| 9 | Quick Control | Quick control functions in laser mode, such as fast movement, reset, etc. |
| 10 | Layer Bar | Assign different processing parameters to primitives of different colors |
| 11 | Simulation Preview | Simulate and preview processing paths |

## 🚀 Core Function Features

### 1. Design Functions
- **Basic Primitive Drawing**: Lines, rectangles, circles, text, etc.
- **Image Import**: Support PNG, JPG, JPEG format image import
- **Pen Tool**: Create complex Bezier curves
- **Graphic Editing**: Node editing, offset, array (rectangular/circular), Boolean operations, etc.
- **Graphic Library**: Provide rich preset graphics
- **Plugin Extension**: Support advanced functions like box generation, gear generation, etc.

### 2. Device Control
- **Auto Connect**: One-click search and connect HiMill series devices
- **Manual Connect**: Manually select serial port for connection
- **Device Settings**: Quick access to device-related settings and help
- **Status Monitoring**: Real-time display of device connection status and operation information

### 3. Processing Functions

#### CNC Processing
- **Blank Setting**: Custom blank size
- **Tool Library Management**: Add and manage tool parameters
- **Multiple Toolpath Generation**: Contour milling, plane milling, V-type milling, drilling, relief, etc.
- **Toolpath Simulation**: 2D/3D preview of processing paths
- **Precise Control**: Single-step control, spindle switch, tool change, etc.
- **Coordinate Setting**: Flexible setting of XY0 and Z0 coordinates

#### Laser Processing
- **Color Mapping**: Different colors correspond to different processing parameters
- **Layer Management**: Move up/move down/delete layers
- **Processing Modes**: Support absolute coordinate mode and current position mode
- **Laser Control**: Activate laser function and motor high-speed mode

## 🛠️ Typical Processing Workflow

### CNC Processing Workflow

1. **Design or Import Graphics**: Draw graphics on the canvas or import external files
2. **Set Blank Parameters**: Set the size of processing material in the parameter bar
3. **Select Tools**: Select appropriate tools from the tool library
4. **Generate Toolpath**: Choose toolpath generation method and set processing parameters
5. **Preview Toolpath**: Check processing paths in the simulation preview area
6. **Connect Device**: Click "Auto Connect" or manually connect the device
7. **Zero Return Operation**: Must execute zero return operation after turning on the device
8. **Start Processing**: Click the "Run" button to start processing, can pause or stop at any time

### Laser Processing Workflow

1. **Design or Import Graphics**: Draw graphics on the canvas or import external files
2. **Set Colors**: Assign different colors to different primitives
3. **Set Processing Parameters**: Set processing parameters for different colors in the layer bar
4. **Preview Effect**: Check graphics and processing parameter settings
5. **Connect Device**: Click "Auto Connect" or manually connect the device
6. **Activate Laser**: Click the "Activate Laser" button
7. **Set Start Position**: Select the start position for processing
8. **Start Processing**: Click the "Run" button to start processing

## ⌨️ Common Shortcuts

| Shortcut | Function |
|----------|----------|
| Ctrl + S | Save file |
| Ctrl + Z | Undo operation |
| Delete | Delete selected primitives |
| Esc | Cancel selection |

## ❓ Frequently Asked Questions and Solutions

### Device Connection Issues
- **Cannot find device**: Try restarting the software, reconnecting the USB data cable, checking if the device is properly powered
- **Connected but cannot control**: Check if the USB data cable is intact, try replacing the data cable or USB port

### Software Usage Issues
- **Abnormal interface display**: Check if the computer has the latest graphics card driver installed, adjust monitor resolution

### Processing Issues
- **Adjust processing speed**: Adjust the "Feed Rate" parameter in the processing parameters area. The larger the value, the faster the processing speed
- **Incorrect processing path preview**: Check if the imported file is correct, or reset the processing origin

## 📚 Learning Resources

If you want to learn more about MaxmakeLab's features in depth, you can refer to:
- [MaxmakeLab Software Installation Guide](/en/maxmakelab/maxmakelab-installation.md)
- [MaxmakeLab Software Manual](/en/maxmakelab/maxmakelab-software-manual.md)
- [HiMill D1S Processing Control](/en/himill-d1-d1s/hmd1s-processing-control.md)
- [HiMill D1S Laser Processing](/en/himill-d1-d1s/hmd1s-laser-processing.md)

---
