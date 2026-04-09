# Alarm2 Error Issue

## Problem Description

When the device shows an Alarm2 error during processing, it is usually caused by insufficient Z-axis travel. This guide will detail how to troubleshoot and resolve this issue.

## Troubleshooting Steps

### Step 1: Connect the Device

**Operation Steps**:
Ensure the device is correctly connected to the computer and open MaxmakeLab software.

**Operation Video**:
<img src="/eng/himill-d1-d1s/media/hmd1s-alarm2-error/1连接设备.gif" alt="Connect Device Video" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

### Step 2: Click Workflow to Enter Processing Interface

**Operation Steps**:
1. In MaxmakeLab software, click the "Workflow" button in the top navigation bar
2. Enter the processing interface to prepare for subsequent operations

**Operation Video**:
<img src="/eng/himill-d1-d1s/media/hmd1s-alarm2-error/2进入加工界面.gif" alt="Enter Processing Interface Video" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

**Reference Image**:
<img src="/eng/himill-d1-d1s/media/hmd1s-alarm2-error/1.jpg" alt="Enter Processing Interface" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### Step 3: Execute Tool Change Command to Install 3D Probe

**Operation Steps**:
1. In the processing interface, find and click the "Tool Change" button
2. Wait for the device to reach the tool change position and install the 3D probe
3. Ensure the 3D probe is securely installed

**Operation Video**:
<img src="/eng/himill-d1-d1s/media/hmd1s-alarm2-error/3换上三坐标.gif" alt="Install 3D Probe Video" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

**Reference Image**:
<img src="/eng/himill-d1-d1s/media/hmd1s-alarm2-error/2.jpg" alt="Install 3D Probe" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### Step 4: Set XYZ Zero Point

**Operation Steps**:
1. Use the 3D probe to detect the workpiece surface
2. Set the XYZ zero point coordinates in the software
3. Confirm the zero point is set correctly

**Operation Video**:
<img src="/eng/himill-d1-d1s/media/hmd1s-alarm2-error/4设置零点.gif" alt="Set XYZ Zero Point Video" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

**Reference Image**:
<img src="/eng/himill-d1-d1s/media/hmd1s-alarm2-error/3.jpg" alt="Set XYZ Zero Point" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### Step 5: Execute Tool Change Command to Install Processing Tool

**Operation Steps**:
1. Click the "Tool Change" button again
2. Wait for the device to automatically install the processing tool
3. Ensure the tool is securely installed

**Operation Video**:
<img src="/eng/himill-d1-d1s/media/hmd1s-alarm2-error/5换上加工刀具.gif" alt="Install Processing Tool Video" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

**Reference Image**:
<img src="/eng/himill-d1-d1s/media/hmd1s-alarm2-error/4.jpg" alt="Install Processing Tool" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### Step 6: Verify Height Compensation After Tool Change

**Operation Steps**:
1. Check the height compensation value displayed in the software
2. Confirm the compensation value is set correctly
3. Make adjustments if necessary

**Operation Video**:
<img src="/eng/himill-d1-d1s/media/hmd1s-alarm2-error/6检验高度补偿.gif" alt="Verify Height Compensation Video" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

**Reference Image**:
<img src="/eng/himill-d1-d1s/media/hmd1s-alarm2-error/5.jpg" alt="Verify Height Compensation" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### Step 7: Check Z-axis Travel

**Operation Steps**:
1. Load your processing file
2. Observe the Z travel range in the 3D preview
3. Confirm whether the Z travel range is within the device's allowable range
4. If the Z travel range exceeds the device's allowable range, adjust the Z zero point position

**Operation Video**:
<img src="/eng/himill-d1-d1s/media/hmd1s-alarm2-error/7加工报错.gif" alt="Processing Error Video" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

**Reference Image**:
<img src="/eng/himill-d1-d1s/media/hmd1s-alarm2-error/6.jpg" alt="Check Z-axis Travel" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

**Problem Analysis**:
In the video, you can see that the Z travel in the bottom left corner of the 3D preview is -10.5 to 5. This means the Z zero point requires a maximum of 5mm upward travel and 10.5mm downward travel.

If the Z zero point is set to 73mm and the device's maximum Z travel is 80mm, the available travel is 80mm - 73mm = 7mm, which is far insufficient for the 10.5mm downward travel required for processing, so an error will definitely occur during processing.

## Solution

When this happens, you need to reserve sufficient processing distance for the Z-axis travel:

1. **Adjust Z zero point position**: Set the Z zero point in a more appropriate position to ensure sufficient travel space
2. **Check workpiece height**: If the workpiece is too low, consider using a垫块 or adjusting the processing strategy
3. **Observe travel range**: Before processing, always observe the Z travel range in the 3D preview to ensure it is within the device's allowable range
4. **Reserve safety distance**: When setting the zero point, it is recommended to reserve at least 5-10mm of safety distance

## Preventive Measures

1. **Pre-processing check**: Before each processing, always check the travel range in the 3D preview
2. **Zero point setting**: Set the zero point reasonably to avoid approaching the device's travel limit
3. **Tool length**: Use tools of appropriate length to avoid insufficient travel due to overly long tools
4. **Workpiece clamping**: Ensure the workpiece is clamped securely and at an appropriate height

> 💡 **Tip**: If you still encounter Alarm2 error, please check if the device's limit switches are working properly and if the firmware version is up to date.
> {.is-info}