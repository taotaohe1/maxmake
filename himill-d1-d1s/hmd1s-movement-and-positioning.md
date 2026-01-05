# MaxmakeLab Movement and Positioning

## Movement and Positioning in CNC Machining

Before machining, it is generally necessary to determine the machining origin. Control spindle movement through movement buttons. After moving to the workpiece machining origin, set the equipment machining origin. (Determined by NC program, for example, if the machining origin in the NC program is the center point, then find the workpiece center point and set it as the machining origin)

### 1. X-axis Movement Control

In movement control, clicking this button can control X-axis left and right movement.

<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-录屏-主轴向右移动.gif" alt="Spindle moving right" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />
<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-拍摄-主轴向右移动.gif" alt="Spindle moving right" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />  

<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-录屏-主轴向左移动.gif" alt="Spindle moving left" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />
<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-拍摄-主轴向左移动.gif" alt="Spindle moving left" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 2. Y-axis Movement Control

Click this button to control Y-axis front and back movement.

<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-录屏-垫板向内移动.gif" alt="Base plate moving inward" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />
<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-拍摄-垫板向内移动.gif" alt="Base plate moving inward" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />  

<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-录屏-垫板向外移动.gif" alt="Base plate moving outward" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />
<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-拍摄-垫板向外移动.gif" alt="Base plate moving outward" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />  

> ⚠️ **Y-axis Movement Note**:
> 
> Here the Y-axis is the base plate movement, the spindle moves relative to the base plate. So when clicking forward movement, it is the spindle moving relatively forward, and the Y-axis base plate moves backward
> 
> {.is-warning}

### 3. Z-axis Movement Control

Click this button to control Z-axis up and down movement.

<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-录屏-主轴向下移动.gif" alt="Spindle moving down" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />
<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-拍摄-主轴向下移动.gif" alt="Spindle moving down" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />  

<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-录屏-主轴向上移动.gif" alt="Spindle moving up" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />
<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-拍摄-主轴向上移动.gif" alt="Spindle moving up" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 4. A-axis (Rotary Axis) Movement Control

Click this button to control A-axis (rotary axis) movement.

<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/2-A轴移动.gif" alt="Rotary axis movement" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 5. Step Size and Feed Rate Settings

When moving, you can set step size and feed rate.
- Step Size: The distance the spindle moves each time
- Feed Rate: The speed at which the spindle moves each time (HiMill equipment maximum speed is 1000mm/min, setting over 1000mm/min will move according to 1000mm/min)

<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/3-设置步距和进给率.jpg" alt="Step size and feed rate settings" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 6. Set XY0 Point

When the tool moves to the workpiece center, click this button to set the XY0 point.

<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/4-设置XY0点.gif" alt="Set XY0 point" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 7. Set Z0 Point

When the tool just contacts the workpiece, click this button to set the Z0 point.

<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/4-设置Z0点.gif" alt="Set Z0 point" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

---

## Movement and Positioning in Laser Machining

### 1. Laser Movement Operation

During laser machining, you can also use movement buttons to move above objects.

<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/5-2-激光移动界面截图.jpg" alt="Laser movement interface" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 2. Quick Movement Positioning

You can also use quick movement, left-click on a position in the canvas, and the spindle will move to the corresponding coordinate location.

<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/5-3-快速移动.jpg" alt="Quick movement positioning" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 3. Laser Border Positioning

After activating the laser button, click the border button, and the laser will walk out the machining range with weak light.

<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/5-4-激光激活+边框定位.jpg" alt="Laser activation + border positioning" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />  

<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/5-5-拍摄边框定位.gif" alt="Border positioning effect" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **Laser Border Positioning Precautions**:
> 
> - Generally set to current position, will walk out the machining range from the current laser position for easy adjustment at any time; if set to absolute coordinates, the border walk range will be fixed, requiring adjustment of the machining material position
> - If out of bounds, the interface will pop up an out-of-bounds prompt, please move the spindle forward and try the border walk again
> - Since the laser is installed on the front side of the spindle, the machining range actually moves forward. If necessary, open the safety door to prevent material from hitting the safety door
> 
> {.is-warning}