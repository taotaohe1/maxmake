# HiMill D1/D1S Limit Switch Troubleshooting: XYZ Homing Sensor Issues Fix

Learn how to troubleshoot limit switch issues on [MAXMAKE HiMill D1/D1S](https://www.maxmake.com/products) CNC machine. This guide covers XY and Z axis homing problems, collision detection, wiring checks, and step-by-step repair solutions.

## Limit Switch Position Diagram

X Limit Switch Position:
<img src="/eng/himill-d1-d1s/media/hmd1s-limit-switch-issue/x限位.jpg" alt="MAXMAKE HiMill D1/D1S X Limit Switch" style="width: 400px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

Y Limit Switch Position:
<img src="/eng/himill-d1-d1s/media/hmd1s-limit-switch-issue/y限位.jpg" alt="MAXMAKE HiMill D1/D1S Y Limit Switch" style="width: 400px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

Z Limit Switch Position:
<img src="/eng/himill-d1-d1s/media/hmd1s-limit-switch-issue/z限位.jpg" alt="MAXMAKE HiMill D1/D1S Z Limit Switch" style="width: 400px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

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
5. Check if the limit switch connection wires are loose and try reconnecting them. For details, refer to the video on replacing XY limits [HiMill D1/D1S Limit Switch Replacement](/en/himill-d1-d1s/hmd1s-replace-limit-switch.md)
6. Check if the limit connection terminals on the main control board are connected properly and try reconnecting them. For cover removal steps, refer to the video for replacing the main control board [HiMill D1/D1S Replace Air Cabinet Components](/en/himill-d1-d1s/hmd1s-replace-air-cabinet.md)
<img src="/eng/himill-d1-d1s/media/hmd1s-limit-switch-issue/主控板未插线限位.jpg" alt="Main Control Board Without Limit Wires" style="width: 350px; height: auto; margin-bottom: 8px; border-radius: 16px;" /> <img src="/eng/himill-d1-d1s/media/hmd1s-limit-switch-issue/主控板插线限位.jpg" alt="Main Control Board With Limit Wires" style="width: 450px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

7. Check if the transmission parts need oiling
8. Restart the device and try again
9. If the issue persists, contact support@maxmake.com

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
9. If the issue persists, contact support@maxmake.com

---

## FAQPage Schema Markup

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "Why won't my HiMill D1S home properly?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Homing issues are often caused by limit switch problems. Check if limit switches are triggered but not sending signals, axes get stuck without rebounding, or there are foreign objects blocking movement. Inspect limit switch wiring, check for mechanical jams, and ensure proper lubrication."
      }
    },
    {
      "@type": "Question",
      "name": "What to do if XY axis keeps colliding during homing?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Immediately stop the device to prevent damage. Check for obstructions, manually adjust axis position to disengage limit switch, verify limit switch rebound is normal, inspect connection wires for looseness, and check main control board terminals."
      }
    },
    {
      "@type": "Question",
      "name": "Why is Z-axis stuck at the top during homing?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Z-axis getting stuck at top indicates limit switch trigger without signal return. Check Z-limit switch wiring for loose connections, verify limit switch isn't blocked by debris, ensure proper lubrication, and inspect main control board connections."
      }
    },
    {
      "@type": "Question",
      "name": "How to check limit switch wiring on HiMill CNC?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Check limit switch connection wires for tightness and reconnection. Also verify limit connection terminals on main control board are properly connected. Refer to official maintenance videos for cover removal procedures."
      }
    }
  ]
}
</script>