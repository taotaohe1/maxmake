# MaxmakeLab 3D Probe Usage

## 1. Installing 3D Probe

After installing the 3D probe, switch to the tool setting (3D probe) interface in the software. You need to click the "Tool Change" button and wait for the 3D probe to complete automatic height measurement before proceeding with subsequent operations.

Click the "Tool Change" button:

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/1-安装测头-换刀-01-录屏换刀.gif" alt="Tool Change" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

Install the 3D probe, click the button, and complete automatic height measurement

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/1-安装测头-组装-02-组装测头.webp" alt="Assemble 3D Probe" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/1-安装测头-测高-03-完成测高.webp" alt="Complete Automatic Height Measurement" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **Tool Change Operation Precautions**:
> 
> - If the workpiece is tall, please adjust the spindle height upward as necessary
> - If you need to use the 3D probe to automatically set Z0, this step must be completed, otherwise subsequent tool compensation will be incorrect. After use, you need to click tool change, replace the tool and automatically measure tool height before processing
> - If only used for centering or corner detection (setting XY0), this step can be skipped, but when changing the first tool, you still need to click tool change and complete automatic height measurement. Then manually set Z0
> - After inserting the 3D probe, do not open the spindle, otherwise it will cause damage to the 3D probe!!!
> 
> {.is-warning}

## 2. Interface Button Function Introduction

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/0-界面-按钮-00-界面功能.jpg" alt="Interface Button Functions" style="width: 300px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

Control:
- Tool Change: Click before installation and install 3D probe, after measurement click and replace with processing tool
- Set XY0: Set current position as XY0 point, used for manual setting. Ignore if using automatic centering
- Set Z0: Set current position as Z0 point, used for manual setting. Ignore if using automatic centering

Move to Position: Center X, Center Y, Center XY. After using 3D probe to set XY0, the corresponding icon will be lit, click to automatically go to the set X0 or Y0 position (also applies to corner detection).

Tool Setting:
- Tool Distance: The distance the probe will move during detection. If no workpiece is detected within the set distance, a popup will prompt
- Tool Speed: The probe will move at the speed set here during detection
- Ball Radius: The ball tip radius of the probe. This is the default value, no changes needed

## 3. Corner Detection

Select corner detection in the software to detect the corner position of the material and automatically set the corner as XY0. Take the bottom-left corner as an example.

### X-axis Detection

Use the movement function to move the 3D probe to the left side of the workpiece.

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/2-角点-X轴-移动-01-移动到工件左侧.jpg" alt="X-axis Movement" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

Click detect, after detecting the workpiece, it will automatically set the detected position as X0.

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/2-角点-X轴-探测-02-X轴探测截图.jpg" alt="X-axis Detection Screenshot" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />
<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/2-角点-X轴-探测-03-X轴探测过程.webp" alt="X-axis Detection Process" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### Y-axis Detection

Use the movement function to move the probe to the front side of the workpiece.

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/2-角点-Y轴-移动-01-移动到工件前侧.webp" alt="Y-axis Movement" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

Click detect, after detecting the workpiece, it will automatically set the detected position as Y0.

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/2-角点-Y轴-探测-02-Y轴探测结果.jpg" alt="Y-axis Detection" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />
<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/2-角点-Y轴-探测-03-Y轴探测过程.webp" alt="Y-axis Detection Process" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### Z-axis Detection

Use the movement function to move the 3D probe above the workpiece.

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/2-角点-Z轴-移动-01-移动到工件上方.webp" alt="Z-axis Movement" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

Click Z-plane detection, after detecting the workpiece, it will automatically set the detected position as Z0.

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/2-角点-Z轴-探测-02-Z轴探测成功.jpg" alt="Z-axis Detection Success" style="width: 300px; height: auto; margin-bottom: 8px; border-radius: 16px;" />
<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/2-角点-Z轴-探测-03-Z轴探测过程.webp" alt="Z-axis Detection Process" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### Tool Change

After all settings are complete, click tool change to replace the first tool to be used and complete automatic height measurement.

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/5-换刀-点击-01-录屏点击换刀.gif" alt="Click Tool Change" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/5-换刀-过程-02-换刀过程.webp" alt="Tool Change Process" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 4. Rectangular External Centering

Select rectangular external centering in the software to detect and automatically calculate the center position, manually set the detected center as XY0 point.

### X-axis Left Side Detection

Use the movement function to move the 3D probe to the left side of the workpiece.

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/3-矩形外-X左-移动-01-移动到工件左侧.jpg" alt="X-axis Left Side Movement" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

And click detect, wait for detection to complete.

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/3-矩形外-X左-探测-02-左侧探测成功.jpg" alt="X-axis Left Side Detection Success" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/3-矩形外-X左-探测-03-左侧探测过程.webp" alt="X-axis Left Side Detection Process" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### X-axis Right Side Detection

After detecting the workpiece, manually raise the Z-axis to a safe height, then move to the right side of the workpiece.

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/3-矩形外-X右-移动-01-移动到工件右侧.webp" alt="X-axis Right Side Movement" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

Click detect, wait for detection to complete.

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/3-矩形外-X右-探测-02-右侧探测成功.jpg" alt="X-axis Right Side Detection Success" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/3-矩形外-X右-探测-03-右侧探测过程.webp" alt="X-axis Right Side Detection Process" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

After detecting the workpiece, you will get the X coordinates of both sides of the workpiece, click Zero X below, automatically calculate the center, and set the center as X0.

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/3-矩形外-X右-分中-04-点击X轴分中.jpg" alt="Click Centering" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### Y-axis Detection

Detect the front and back sides of the workpiece using the same method, click Zero Y, automatically calculate the center, and set the center as Y0.

### Z-axis Detection

Use the movement function to move the 3D probe above the workpiece.

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/3-矩形外-Z轴-移动-01-移动到工件上方.webp" alt="Z-axis Movement" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

Click Z-plane detection, wait for detection to complete.

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/3-矩形外-Z轴-探测-02-Z轴探测成功.jpg" alt="Z-axis Detection Success" style="width: 300px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

After detecting the workpiece, it will automatically set the detected position as Z0.

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/3-矩形外-Z轴-探测-03-Z轴探测过程.webp" alt="Z-axis Detection Process" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### Tool Change

After all settings are complete, click tool change to replace the first tool to be used and complete automatic height measurement.

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/5-换刀-点击-01-录屏点击换刀.gif" alt="Click Tool Change" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/5-换刀-过程-02-换刀过程.webp" alt="Tool Change Process" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **Rectangular External Centering Precautions**:
> 
> Circular external centering and rectangular external centering operations are similar. However, note that when detecting the X center point, the Y-axis coordinate cannot be changed. When detecting the Y center point, the X-axis coordinate cannot be changed. For example: after detecting the X left side, raise the Z-axis, then move to the X right side, during which the Y-axis cannot move.
> 
> {.is-warning}

## 5. Circular Internal Centering

Select circular internal centering in the software to detect and automatically calculate the center position, manually set the detected center as XY0 point.

### X-axis Left Side Detection

Use the movement function to move the probe inside the workpiece, close to the left side inside the workpiece.

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/4-圆形内-X左-移动-01-移动到内部左侧.webp" alt="X-axis Left Side Movement" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

Click left detection, wait for detection to complete.

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/4-圆形内-X左-探测-02-内部左侧探测成功.jpg" alt="X-axis Left Side Detection Success" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/4-圆形内-X左-探测-03-内部左侧探测过程.webp" alt="X-axis Left Side Detection Process" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### X-axis Right Side Detection

After detecting the workpiece, move close to the right side of the workpiece (do not move the Y-axis during this time).

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/4-圆形内-X右-移动-01-移动到内部右侧.webp" alt="X-axis Right Side Movement" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

Click right detection, wait for detection to complete.

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/4-圆形内-X右-探测-02-内部右侧探测成功.jpg" alt="X-axis Right Side Detection Success" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/4-圆形内-X右-探测-03-内部右侧探测过程.webp" alt="X-axis Right Side Detection Process" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

After detecting the workpiece, you will get the X coordinates of both internal sides of the workpiece, click Zero X below, automatically calculate the center, and set the center as X0.

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/4-圆形内-X右-分中-04-点击X轴分中.jpg" alt="Click Centering" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### Y-axis Detection

Detect the front and back sides inside the workpiece using the same method, click Zero Y, automatically calculate the center, and set the center as Y0.

### Z-axis Detection

Use the movement function to move the 3D probe above the workpiece.

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/4-圆形内-Z轴-移动-01-移动到工件上方.webp" alt="Z-axis Movement" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

And click Z-plane detection, wait for detection to complete.

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/4-圆形内-Z轴-探测-02-Z轴探测成功.jpg" alt="Z-axis Detection Success" style="width: 300px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

After detecting the workpiece, it will automatically set the detected position as Z0.

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/4-圆形内-Z轴-探测-03-Z轴探测过程.webp" alt="Z-axis Detection Process" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### Tool Change

After all settings are complete, click tool change to replace the first tool to be used and complete automatic height measurement.

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/5-换刀-点击-01-录屏点击换刀.gif" alt="Click Tool Change" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/5-换刀-过程-02-换刀过程.webp" alt="Tool Change Process" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> 📋 **Centering Operation Tips**:
> 
> Rectangular internal centering and circular internal centering operations are similar.
> 
> {.is-info}

## Precautions

> ⚠️ **3D Probe Usage Safety Precautions**:
> 
> - Centering is suitable for workpieces with regular shapes, such as circles or rectangles. Not recommended for irregular workpieces
> - During Z-axis surface detection, select the highest surface of the workpiece
> - When moving the 3D probe, keep the ball tip slightly below the workpiece, not too low
> - Observe in advance if there are objects that may obstruct the 3D probe movement, avoid the 3D probe being hit and damaged before the probe contacts
> - The 3D probe is a precision and easily damaged accessory, please move the 3D probe slowly
> - If the alarm is triggered by accidental contact during movement, please remove the obstacle in time, return to zero and retry
> 
> {.is-warning}