# MaxmakeLab Software Getting Started

## 📖 Software Overview

MaxmakeLab is an intelligent control software designed specifically for HiMill series CNC equipment, providing an intuitive operation interface and rich processing functions to help users easily complete various creative processing tasks. Whether you are a CNC beginner or an experienced user, you can quickly get started with using it.

## 🎨 Interface Introduction

### Main Interface Layout

MaxmakeLab adopts a clean and clear interface design, mainly divided into the following areas:

1. **Menu Bar**: Located at the top of the interface, containing menus such as File, Edit, View, Tools, Help
2. **Toolbar**: Common function shortcut buttons, such as Open File, Save, Run, Pause, etc.
3. **Device Control Area**: Device connection, motion control, spindle control and other device operation functions
4. **Processing Parameters Area**: Set processing speed, spindle speed, feed rate and other parameters
5. **Preview Area**: Real-time display of processing paths and workpiece preview
6. **Status Bar**: Display device status, processing progress, current position and other information

## 🚀 Basic Functions

### File Management
- **Open File**: Support importing G-code files (.nc, .gcode format)
- **Save File**: Save current processing parameters and paths
- **File Preview**: Preview complete processing path before processing

### Device Control
- **Connect Device**: Automatically search and connect HiMill series equipment
- **Manual Control**: Control each axis movement through interface buttons or keyboard
- **Auto Zero Return**: One-click execution of equipment automatic zero return operation
- **Emergency Stop**: Quickly stop all processing operations

### Processing Settings
- **Spindle Control**: Set spindle speed and on/off status
- **Feed Rate Control**: Adjust processing feed speed
- **Processing Origin Setting**: Precisely set workpiece processing origin
- **Tool Compensation**: Set tool compensation parameters

### Processing Monitoring
- **Real-time Position Display**: Display current position coordinates of each axis
- **Processing Progress Monitoring**: Display processing completion percentage
- **Status Log**: Record equipment operation status and operation history

## 🛠️ Operation Process

### Step 1: Connect Device
1. Ensure the device is properly connected to the computer
2. Start MaxmakeLab software
3. Click the "Search Device" button, the software will automatically recognize the device
4. After successful device connection, the status bar will display "Device Connected"

### Step 2: Import File
1. Click "File" → "Open", select your G-code file
2. After file import, the preview area will display the processing path
3. You can use mouse to zoom and pan to preview the processing path

### Step 3: Set Processing Parameters
1. Set appropriate spindle speed and feed rate in the "Processing Parameters" area
2. Choose appropriate processing parameters based on processing materials and tools
3. Set processing origin and tool compensation (if needed)

### Step 4: Start Processing
1. Ensure the workpiece is properly fixed on the equipment workbench
2. Click the "Run" button to start processing
3. During processing, you can pause processing through the "Pause" button, or end processing through the "Stop" button

### Step 5: Processing Complete
1. After processing is complete, the equipment will automatically stop and return to origin
2. Check the processing effect, if satisfied then processing is complete
3. If adjustments are needed, modify processing parameters and run again

## 💡 Usage Tips

1. **Keyboard Shortcuts**:
   - `Ctrl+O`: Open file
   - `Ctrl+S`: Save file
   - `F5`: Start processing
   - `F6`: Pause processing
   - `F7`: Stop processing

2. **Safe Operation**:
   - Before processing, be sure to check if workpiece fixation is secure
   - Do not leave the equipment during processing
   - In case of abnormal situations, immediately press the "Emergency Stop" button

3. **Performance Optimization**:
   - For complex processing files, path optimization can be performed first
   - Regularly clean software cache to keep software running smoothly

## ❓ Frequently Asked Questions

### Q: How to adjust processing speed?
A: Adjust the "Feed Rate" parameter in the processing parameters area. The larger the value, the faster the processing speed.

### Q: What to do if processing path preview is incorrect?
A: Check if the imported G-code file is correct, or reset the processing origin.

### Q: What to do if software response is slow?
A: Close other unnecessary software, or reduce the display accuracy of the preview area.

### Q: How to export processing files?
A: Click "File" → "Export", select the export format.

## 📚 Advanced Learning

If you want to learn more about MaxmakeLab's features in depth, you can refer to:
- [HiMill D1S Processing Control](/en/himill-d1-d1s/hmd1s-processing-control.md)
- [HiMill D1S Laser Processing](/en/himill-d1-d1s/hmd1s-laser-processing.md)
- [HiMill D1S Rotation Axis Processing](/en/himill-d1-d1s/hmd1s-rotation-axis-processing.md)

---

*Document Version: v1.0*
*Update Time: 2024*
*Applicable Software: MaxmakeLab v2.0 and above*