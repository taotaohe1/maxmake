# HiMill D1S Rotation Axis Processing Guide: 4th Axis Setup & Machining Tutorial

Learn how to use the [rotation axis](https://maxmake.com/products/4th-axis-module) for 4th axis machining on [MAXMAKE HiMill D1S](https://www.maxmake.com/products/himill-d1s) CNC machine.

## 1. Switch to CNC Mode

Switch the mode to CNC mode.

<img src="/eng/himill-d1-d1s/media/hmd1s-rotation-axis-processing/1-切换cnc模式.webp" alt="Switch to CNC Mode" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 2. Import Files

After connecting the equipment, import the prepared NC program.

<img src="/eng/himill-d1-d1s/media/hmd1s-rotation-axis-processing/1-导入文件.webp" alt="Import Files" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 3. Raise Spindle

Due to the relatively high height of the rotation axis itself, the spindle may need to be raised. Loosen the 4 fixing screws of the spindle, move it up, and then refix it.

<img src="/eng/himill-d1-d1s/media/hmd1s-rotation-axis-processing/2-上调主轴.webp" alt="Raise Spindle" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 4. Movement and Positioning

Turn on the spindle and control the tool to move to the processing origin.

<img src="/eng/himill-d1-d1s/media/hmd1s-rotation-axis-processing/3-移动定位-打开主轴.webp" alt="Turn on Spindle" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1s-rotation-axis-processing/3-移动定位-移动.webp" alt="Movement" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 5. Set Origin

When the tool is at the processing origin, click to set XY0.

<img src="/eng/himill-d1-d1s/media/hmd1s-rotation-axis-processing/4-设置原点-1-刀具位于原点时.webp" alt="Tool at Origin" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1s-rotation-axis-processing/4-设置原点-1-设置xy0点.webp" alt="Set XY0 Point" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

Slowly lower the Z-axis. When the tool just contacts the workpiece, click to set Z0.

<img src="/eng/himill-d1-d1s/media/hmd1s-rotation-axis-processing/4-设置原点-2-降下z轴.webp" alt="Lower Z-axis" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1s-rotation-axis-processing/4-设置原点-2-设置z0点.webp" alt="Set Z0 Point" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **Origin Setting Notes**:
> 
> - In this case, the Z0 of the NC program is at the corner edge of the square workpiece, so when setting Z0, the corner needs to be adjusted to be directly above
> - Before rotation axis processing, when designing the toolpath, it is recommended to clamp the workpiece first. Be sure to consider the clamping position carefully. The generated toolpath must avoid the chuck jaws to prevent collision
> - At the same time, the Z-axis processing range needs to be determined in advance, and the tool length needs to be calculated in advance to avoid insufficient tool length that would prevent processing
> 
> {.is-warning}

## 6. Preview Simulation

In the 3D interface, you can preview the simulation path.

<img src="/eng/himill-d1-d1s/media/hmd1s-rotation-axis-processing/5-预览仿真.webp" alt="Preview Simulation" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> 📋 **Preview Simulation Tips**:
> 
> - You can adjust the playback rate for real-time preview
> - You can directly drag the progress bar
> 
> {.is-info}

## 7. Transfer File and Start Processing

Click the start processing button to transfer the processing file to the device SD card.

<img src="/eng/himill-d1-d1s/media/hmd1s-rotation-axis-processing/6-点击开始.webp" alt="Click Start" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

According to the prompts, wait until the indicator light shows the rainbow rotating light effect, then long press the equipment button for 2 seconds to start processing.

<img src="/eng/himill-d1-d1s/media/hmd1s-rotation-axis-processing/6-接受文件开始加工.webp" alt="Accept File and Start Processing" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **Processing Control Notes**:
> 
> - During processing, single-click the button to pause processing. Long press for 2 seconds to resume processing
> - If the safety door function is enabled, close the door before resuming processing
> 
> {.is-warning}

## 8. During Processing, Spindle Speed and Feed Rate Can Be Changed

During processing, the spindle speed and feed rate can be changed.

<img src="/eng/himill-d1-d1s/media/hmd1s-rotation-axis-processing/7-覆写功能.webp" alt="Override Function" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **Parameter Adjustment Notes**:
> 
> - During processing, it is not recommended to reduce spindle speed, especially for metal processing, to avoid increased load that could cause tool breakage
> - After changing values, speed will gradually increase or decrease. You need to gradually increase or decrease values based on actual conditions
> 
> {.is-warning}