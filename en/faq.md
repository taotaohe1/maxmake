# Frequently Asked Questions (FAQ)

This document summarizes common questions and answers about HiMill series equipment, helping you quickly solve problems encountered during use.

---

## 1. What to do if the device cannot power on?
**Problem**: The device cannot power on after being connected, and the indicator light does not turn on.

**Solution**:
- Check if the power cord is obviously damaged or broken
- Replace the power socket and confirm if the socket has normal power supply
- Check if the device voltage level matches the local voltage
- If the above methods are ineffective, or if smoke appears, please contact technical support

**Related Documents**: [HiMill D1/D1S Cannot Power On](/en/himill-d1-d1s/hmd1s-cannot-power-on.md)

---

## 2. Cannot connect, how to connect correctly?
**Problem**: Unable to connect the device to the computer via USB or WiFi.

**Solution**:
- **USB Connection**:
  - Use the original USB-B data cable
  - Ensure both ends are fully inserted
  - Avoid using low-quality USB hubs
  - Try replacing the USB port
  - Check if the device USB interface and computer USB interface have dust or oxidation
- **WiFi Connection**:
  - Ensure the device WiFi function is enabled
  - Check if the network configuration is correct
  - Ensure the computer and device are in the same network environment

**Related Documents**:
- [HiMill D1/D1S Cannot Connect Software via USB](/en/himill-d1-d1s/hmd1s-cannot-connect-software-via-usb.md)
- [HiMill D1/D1S Cannot Connect Software via WiFi](/en/himill-d1-d1s/hmd1s-cannot-connect-software-via-wifi.md)
- [HiMill D1S Connection Guide](/en/himill-d1-d1s/hmd1s-connection.md)

---

## 3. How to switch power voltage?
**Problem**: How to adjust the device's power voltage to adapt to voltage standards in different regions?

**Solution**:
- Toggle the voltage switch to the left to switch to 230V
- Toggle the voltage switch to the right to switch to 110V
- The voltage adjustment position is on the device power module
- Be sure to adjust the voltage level before powering on to ensure it matches the local voltage

**Related Documents**: [HiMill D1S Basic Operation and Usage Safety](/en/himill-d1-d1s/hmd1s-basic-operation-and-usage-safety.md)

---

## 4. What software to use?
**Problem**: What software is used for controlling and programming HiMill series equipment?

**Solution**:
- HiMill series equipment uses MaxmakeLab software for control and programming
- MaxmakeLab is an intelligent control software designed specifically for HiMill series CNC equipment
- The software supports both CNC processing and laser processing modes
- It has complete design, toolpath generation, and processing control functions

**Related Documents**:
- [MaxmakeLab Software Introduction](/en/maxmakelab/maxmakelab-introduction.md)
- [MaxmakeLab Software Installation Guide](/en/maxmakelab/maxmakelab-installation.md)
- [MaxmakeLab Software Manual](/en/maxmakelab/maxmakelab-software-manual.md)

---

## 5. CAM function includes tool library function, why can't it be used?
**Problem**: The software includes CAM function and tool library function, but it cannot be used normally.

**Solution**:
CAM-related functions are under development. Once development is complete and available, we will update them on the relevant pages of the software.

**Related Documents**:
- [MaxmakeLab Software Manual](/en/maxmakelab/maxmakelab-software-manual.md)
- [HiMill D1S Tool Installation Guide](/en/himill-d1-d1s/hmd1s-tool-installation.md)

---

## 6. How to enable the safety door function?
**Problem**: How to enable and set the safety door function?

**Solution**:
- After connecting the device, click the device settings button to open the device settings interface
- In the device settings interface, find the safety door setting option
- Turn on or off the safety door function as needed
- After enabling the safety door function, if the front cover is opened during processing, processing will automatically pause
- After closing the door, long press the button for 2 seconds to continue processing

**Related Documents**: [MaxmakeLab HiMill D1/D1S Safety Door Setting](/en/himill-d1-d1s/hmd1s-safe-door-setting.md)

---

## 7. What is the tool change logic of the device?
**Problem**: What is the tool change process and logic of HiMill equipment?

**Solution**:
- Click the tool change button in the software
- The device enters tool change state, and the spindle moves to a position convenient for tool change (X140,Y0)
- The indicator light shows yellow flashing, indicating that tool change is possible
- Pull down the handle, insert the tool, and the tool clamping depth should be ≥15mm
- Slowly release the handle to ensure the tool is securely installed
- After confirming correct installation, click the button (either internal or external), and the spindle will move to the top of the height gauge to complete height measurement
- Before starting processing, it is recommended to click tool change for the first tool to complete automatic height measurement

**Related Documents**: [HiMill D1S Tool Installation Guide](/en/himill-d1-d1s/hmd1s-tool-installation.md)

---

## 8. How to handle tool breakage and unexpected stop during processing?
**Problem**: How to handle tool breakage or unexpected stop during processing?

**Solution**:
- **Tool Breakage Handling**:
  - After tool breakage, stop the device operation immediately and be sure to remove the broken tool handle
  - Take different processing methods according to the processing code form and device status
  - Restart the device, after homing, replace the tool, reset Z0, and start processing
  - If there is tool change code, click the tool change button in the software to replace the tool and automatically measure height
- **Unexpected Stop Handling**:
  - Check the stop reason (such as safety door opening, power failure, etc.)
  - After troubleshooting, long press the device button for 2 seconds to resume processing
  - If power is lost, after restarting the device, it is necessary to re-home and set the origin

**Related Documents**:
- [Guide for Handling Tool Breakage During Processing](/en/himill-d1-d1s/hmd1s-cutting-issue-handling.md)
- [HiMill D1S Processing Stop Issue Handling](/en/himill-d1-d1s/hmd1s-processing-stop-issue-handling.md)

---

## 9. What to do if the device is too noisy?
**Problem**: The device makes abnormally loud noise during operation.

**Solution**:
- Check if the guide rails and lead screws need lubrication
- Confirm if the moving axis is jammed by foreign objects
- Check if the spindle bearings are worn
- Ensure the device is placed stably without resonance

**Related Documents**: [HiMill D1 Guide Rail Lead Screw Maintenance](/en/himill-d1-d1s/hmd1-guide-rail-lead-screw-maintenance.md)

---

## 10. How to use the dust collection system?
**Problem**: How to correctly use and maintain the device's dust collection system?

**Solution**:
- Ensure the dust collection pipeline is tightly connected
- Regularly clean the vacuum cleaner filter
- Check if the dust collection port is blocked
- Ensure the vacuum cleaner has sufficient power
- Keep the dust collection system on during processing

**Related Documents**:
- [HiMill D1 Dust Collection System](/en/himill-d1-d1s/hmd1-dust-collection-system.md)
- [HiMill D1S Dust Collection System](/en/himill-d1-d1s/hmd1s-dust-collection-system.md)

---

## 11. Where to find tutorials for different accessories purchased?
**Related Documents**:
- [HiMill D1S 3D Probe Using](/en/himill-d1-d1s/hmd1s-3d-probe-using.md)
- [HiMill D1S Laser Module](/en/himill-d1-d1s/hmd1s-laser-module.md)
- [HiMill D1S Rotation Axis](/en/himill-d1-d1s/hmd1s-rotation-axis.md)
- [HiMill D1S Side Clamp](/en/himill-d1-d1s/hmd1s-side-clamp.md)
- [HiMill D1S Vacuum Platform](/en/himill-d1-d1s/hmd1s-vacuum-platform.md)