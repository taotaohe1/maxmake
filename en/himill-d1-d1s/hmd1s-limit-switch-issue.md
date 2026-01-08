# HiMill D1S Limit Switch Issues

## Limit Switch Position Diagram

X Limit Switch Position:
<img src="/eng/himill-d1-d1s/media/hmd1s-limit-switch-issue/x限位.jpg" alt="X Limit Switch" style="width: 400px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

Y Limit Switch Position:
<img src="/eng/himill-d1-d1s/media/hmd1s-limit-switch-issue/y限位.jpg" alt="Y Limit Switch" style="width: 400px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

Z Limit Switch Position:
<img src="/eng/himill-d1-d1s/media/hmd1s-limit-switch-issue/z限位.jpg" alt="Z Limit Switch" style="width: 400px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

---

## XY Limit Switch Issues

### Possible Phenomena
- During homing, the XY axes keep colliding, the limit has been triggered but there's no signal
- During homing, the XY axes get stuck and don't rebound, unable to disengage after the limit has been triggered

### Possible Causes
- Loose or poor contact of limit switch connection wires
- Damaged limit switch
- Mechanical structure jammed
- Insufficient lubrication
- Limit switch is blocked by foreign objects

### Solutions
1. If the axes keep colliding, immediately stop the device to avoid further damage
2. Check if there are any objects blocking the axis movement or limit switches
3. Manually turn the lead screw to adjust the axis position and disengage the limit switch from the triggered state
4. Try pressing the limit switch to check if the rebound is normal
5. Check if the limit switch connection wires are loose and try reconnecting them. For details, refer to the video on replacing XY limits [HiMill D1S Limit Switch Replacement](/eng/himill-d1-d1s/hmd1s-replace-limit-switch.md)
6. Check if the limit connection terminals on the main control board are connected properly and try reconnecting them. For cover removal steps, refer to the video for replacing the main control board [HiMill D1S Replace Air Cabinet Components](/eng/himill-d1-d1s/hmd1s-replace-air-cabinet.md)
<img src="/eng/himill-d1-d1s/media/hmd1s-limit-switch-issue/主控板未插线限位.jpg" alt="Main Control Board Without Limit Wires" style="width: 350px; height: auto; margin-bottom: 8px; border-radius: 16px;" /> <img src="/eng/himill-d1-d1s/media/hmd1s-limit-switch-issue/主控板插线限位.jpg" alt="Main Control Board With Limit Wires" style="width: 450px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

7. Check if the transmission parts need oiling
8. Restart the device and try again
9. If the issue persists, contact support@maxmaketech.com

---

## Z Limit Switch Issues

### Possible Phenomena
- During homing, the Z-axis keeps colliding upwards, the limit has been triggered but there's no signal
- During homing, the Z-axis moves to the top and gets stuck without rebounding, unable to disengage after the limit has been triggered

### Possible Causes
- Loose Z-axis limit switch connection wires
- Damaged Z-axis limit switch
- Z-axis mechanical structure jammed
- Insufficient lubrication
- Limit switch is blocked by foreign objects

### Solutions
1. If the axis keeps colliding, immediately stop the device to avoid further damage
2. Check if there are any objects blocking the axis movement or limit switch
3. Manually turn the lead screw to adjust the axis position and disengage the limit switch from the triggered state
4. Try pressing the limit switch to check if the rebound is normal
5. Check if the limit switch connection wires are loose and try reconnecting them. For details, refer to the video on replacing Z limit
6. Check if the limit connection terminals on the main control board are connected properly and try reconnecting them
7. Check if the transmission parts need oiling
8. Restart the device and try again
9. If the issue persists, contact support@maxmaketech.com