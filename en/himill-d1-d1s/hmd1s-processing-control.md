# HiMill D1S CNC Processing Control | MAXMAKE Wiki

Learn how to process with CNC mode on MAXMAKE HiMill D1/D1S CNC machine. This guide covers mode switching, NC program import, origin setting, and processing control.

## 1. Switch to CNC Mode

Switch the mode to CNC mode.

<img src="/eng/himill-d1-d1s/media/hmd1s-processing-control/1-切换cnc模式.webp" alt="MAXMAKE HiMill D1/D1S Switch to CNC Mode" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 2. Import Files

After connecting the equipment, import the prepared NC program.

<img src="/eng/himill-d1-d1s/media/hmd1s-processing-control/1-导入文件.webp" alt="MAXMAKE HiMill D1/D1S Import NC Program Files" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 3. Movement and Positioning

Turn on the spindle and control the tool to move to the processing origin.

<img src="/eng/himill-d1-d1s/media/hmd1s-processing-control/2-转动主轴.webp" alt="MAXMAKE HiMill D1/D1S Turn on Spindle" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />  

<img src="/eng/himill-d1-d1s/media/hmd1s-processing-control/2-移动到原点.webp" alt="MAXMAKE HiMill D1/D1S Move to Origin" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 4. Set Origin

Using the processing origin at the workpiece center point as an example, when the tool is at the workpiece center point, click to set XY0.

<img src="/eng/himill-d1-d1s/media/hmd1s-processing-control/3-设置原点-刀具处于中心点.webp" alt="MAXMAKE HiMill D1/D1S Tool at Center Point" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />  

<img src="/eng/himill-d1-d1s/media/hmd1s-processing-control/3-设置原点-设置xy0点.webp" alt="MAXMAKE HiMill D1/D1S Set XY0 Point" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

Slowly lower the Z-axis. When the tool just contacts the workpiece, click to set Z0.

<img src="/eng/himill-d1-d1s/media/hmd1s-processing-control/3-设置原点-降z轴.webp" alt="MAXMAKE HiMill D1/D1S Lower Z-axis" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />  

<img src="/eng/himill-d1-d1s/media/hmd1s-processing-control/3-设置原点-设置z0点.webp" alt="MAXMAKE HiMill D1/D1S Set Z0 Point" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 5. Preview Simulation

In the 3D interface, you can preview the simulation path.

<img src="/eng/himill-d1-d1s/media/hmd1s-processing-control/4-预览仿真.webp" alt="MAXMAKE HiMill D1/D1S Preview Simulation" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> 📋 **Preview Simulation Tips**:
> 
> - You can adjust the playback rate for real-time preview
> - You can directly drag the progress bar
> 
> {.is-info}

## 6. Transfer File and Start Processing

Click the start processing button to transfer the processing file to the device SD card.

<img src="/eng/himill-d1-d1s/media/hmd1s-processing-control/5-开始.webp" alt="MAXMAKE HiMill D1/D1S Start Processing" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

According to the prompts, wait until the indicator light shows the rainbow rotating light effect, then long press the equipment button for 2 seconds to start processing.

<img src="/eng/himill-d1-d1s/media/hmd1s-processing-control/5-接受文件开始加工.webp" alt="MAXMAKE HiMill D1/D1S Accept File and Start Processing" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **Processing Control Notes**:
> 
> - During processing, single-click the button to pause processing. Long press for 2 seconds to resume processing
> - If the safety door function is enabled, close the door before resuming processing; if the door is not closed, after long pressing for 2 seconds, the resume processing light effect will still be displayed, and finally it will become green steady light but the equipment will have no action
> 
> {.is-warning}

## 7. Parameter Adjustment During Processing

During processing, the feed rate can be changed.

<img src="/eng/himill-d1-d1s/media/hmd1s-processing-control/6-覆写功能，更改转速进给率.webp" alt="MAXMAKE HiMill D1/D1S Override Function Change Spindle Speed and Feed Rate" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **Parameter Adjustment Notes**:
> 
> - During processing, it is not recommended to reduce spindle speed, especially for metal processing, to avoid increased load that could cause tool breakage
> - After changing values, speed will gradually increase or decrease. You need to gradually increase or decrease values based on actual conditions
> 
> {.is-warning}