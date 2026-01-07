# MaxmakeLab Laser Processing

## ⚠️ Usage Reminder

Please be sure to check the laser usage specifications before use!!!

[Link to How to Use Laser Module](hmd1s-laser-module.md)

---

## 1. Switch to Laser Mode

Click the laser mode option in the software interface:

<img src="/eng/himill-d1-d1s/media/hmd1s-laser-processing/1-切换激光模式.webp" alt="Switch to Laser Mode" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 2. Add Files

You can design your own graphics or import graphics from the material library or add images:

<img src="/eng/himill-d1-d1s/media/hmd1s-laser-processing/1-导入文件.webp" alt="Import Files" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 3. Activate Laser Mode

Click the activate laser button to enable laser mode:

<img src="/eng/himill-d1-d1s/media/hmd1s-laser-processing/1-点击激光模式.webp" alt="Click Laser Mode" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **Laser Activation Notes**:
> 
> - After activating the laser, the motor enters high-speed mode with a maximum processing speed of 2000mm/min. There will be some noise during operation, which is normal
> - After processing is complete, when switching back to CNC mode, you need to click the activation button again to cancel laser mode
> 
> {.is-warning}

## 4. Parameter Settings

In laser mode, the maximum speed is 2000mm/min (approximately 33mm/s). Adjust the power reasonably based on test results:

<img src="/eng/himill-d1-d1s/media/hmd1s-laser-processing/2-设置参数.webp" alt="Parameter Settings" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 5. Movement and Positioning

Control the laser to move above the material:

<img src="/eng/himill-d1-d1s/media/hmd1s-laser-processing/3-移动.webp" alt="Movement and Positioning" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 6. Border Positioning

Click the border button, and the laser will trace the processing range with weak light:

<img src="/eng/himill-d1-d1s/media/hmd1s-laser-processing/4-边框定位.webp" alt="Border Positioning" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 7. Adjust Focus

5mm from the bottom of the light shield to the material is the optimal focal position for laser processing. You can use the focus assist block from the laser accessories box and slowly lower the Z-axis until the focus assist block just passes through the gap:

<img src="/eng/himill-d1-d1s/media/hmd1s-laser-processing/5-对焦辅助片.webp" alt="Focus Assist Block" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 8. Transfer File and Start Processing

Click the start processing button to transfer the processing file to the device SD card. Long press the button for 2 seconds to start processing:

<img src="/eng/himill-d1-d1s/media/hmd1s-laser-processing/6-点击开始.webp" alt="Click Start" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<br>

<img src="/eng/himill-d1-d1s/media/hmd1s-laser-processing/6-接受文件开始加工.webp" alt="Accept File and Start Processing" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **Processing Notes**:
> 
> Due to the laser and spindle not being coaxial, the actual processing range is offset by approximately 20mm forward. When processing large graphics, the laser may exceed the equipment. At this time, you need to open the safety door, and the safety door function should be turned off in software settings
> 
> {.is-warning}