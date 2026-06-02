# HiMill CNC FAQ | MAXMAKE Wiki

Find answers to common questions about [MAXMAKE HiMill D1/D1S](https://www.maxmake.com/products) CNC machines. Comprehensive troubleshooting, setup, software, and maintenance FAQ for all skill levels.

This document summarizes common questions and answers about [MAXMAKE HiMill](https://www.maxmake.com/products) series equipment, helping you quickly solve problems encountered during use.

---

## HiMill CNC Cannot Power On - Troubleshooting Guide
**Problem**: The device cannot power on after being connected, and the indicator light does not turn on.

**Solution**:
- Check if the power cord is obviously damaged or broken
- Replace the power socket and confirm if the socket has normal power supply
- Check if the device voltage level matches the local voltage (110V/230V)
- If the above methods are ineffective, or if smoke appears, please contact technical support

**Related Documents**: [HiMill D1/D1S Cannot Power On](/en/himill-d1-d1s/hmd1s-cannot-power-on.md)

---

## HiMill CNC Connection Issues - USB & WiFi Troubleshooting
**Problem**: Unable to connect the device to the computer via USB or WiFi.

**Solution**:
- **USB Connection**:
  - Use the original USB-B data cable
  - Ensure both ends are fully inserted
  - Avoid using low-quality USB hubs
  - Try replacing the USB port
  - Check if the device USB interface and computer USB interface have dust or oxidation
- **WiFi Connection**:
  - Ensure the device WiFi function is enabled in MaxmakeLab software
  - Check if the network configuration is correct (SSID and password)
  - Ensure the computer and device are in the same WiFi network environment

**Related Documents**:
- [HiMill D1/D1S Cannot Connect Software via USB](/en/himill-d1-d1s/hmd1s-cannot-connect-software-via-usb.md)
- [HiMill D1/D1S Cannot Connect Software via WiFi](/en/himill-d1-d1s/hmd1s-cannot-connect-software-via-wifi.md)
- [HiMill D1S Connection Guide](/en/himill-d1-d1s/hmd1s-connection.md)

---

## HiMill CNC Power Voltage Switching - 110V/230V Guide
**Problem**: How to adjust the device's power voltage to adapt to voltage standards in different regions?

**Solution**:
- Toggle the voltage switch to the left to switch to 230V (Europe, Asia)
- Toggle the voltage switch to the right to switch to 110V (USA, Japan)
- The voltage adjustment position is on the device power module
- Be sure to adjust the voltage level before powering on to ensure it matches the local voltage

**Related Documents**: [HiMill D1S Basic Operation and Usage Safety](/en/himill-d1-d1s/hmd1s-basic-operation-and-usage-safety.md)

---

## HiMill CNC Software - MaxmakeLab Guide
**Problem**: What software is used for controlling and programming HiMill series equipment?

**Solution**:
- HiMill series equipment uses MaxmakeLab software for control and programming
- MaxmakeLab is an intelligent control software designed specifically for HiMill series CNC equipment
- The software supports both CNC machining and laser processing modes
- It has complete design, toolpath generation, and processing control functions

**Related Documents**:
- [MaxmakeLab Software Introduction](/en/maxmakelab/maxmakelab-introduction.md)
- [MaxmakeLab Software Installation Guide](/en/maxmakelab/maxmakelab-installation.md)
- [MaxmakeLab Software Manual](/en/maxmakelab/maxmakelab-software-manual.md)

---

## HiMill CAM Function & Tool Library - Availability Status
**Problem**: The software includes CAM function and tool library function, but it cannot be used normally.

**Solution**:
CAM-related functions are under active development. Once development is complete and available, we will update them on the relevant pages of the software. You can use external CAM software (such as Fusion 360, Vectric Aspire) to generate toolpaths.

**Related Documents**:
- [MaxmakeLab Software Manual](/en/maxmakelab/maxmakelab-software-manual.md)
- [HiMill D1S Tool Installation Guide](/en/himill-d1-d1s/hmd1s-tool-installation.md)

---

## HiMill CNC Safety Door Function - Enable & Setup Guide
**Problem**: How to enable and set the safety door function?

**Solution**:
- After connecting the device, click the device settings button to open the device settings interface
- In the device settings interface, find the safety door setting option
- Turn on or off the safety door function as needed
- After enabling the safety door function, if the front cover is opened during processing, processing will automatically pause
- After closing the door, long press the button for 2 seconds to continue processing

**Related Documents**: [MaxmakeLab HiMill D1/D1S Safety Door Setting](/en/himill-d1-d1s/hmd1s-safe-door-setting.md)

---

## HiMill CNC Tool Change Process - Automatic Height Measurement
**Problem**: What is the tool change process and logic of HiMill equipment?

**Solution**:
- Click the tool change button in MaxmakeLab software
- The device enters tool change state, and the spindle moves to the tool change position (X140,Y0)
- The indicator light shows yellow flashing, indicating that tool change is possible
- Pull down the handle, insert the tool, and the tool clamping depth should be ≥15mm
- Slowly release the handle to ensure the tool is securely installed
- After confirming correct installation, click the button, and the spindle will move to the height gauge to complete automatic height measurement
- Before starting processing, it is recommended to click tool change for the first tool to complete automatic height measurement

**Related Documents**: [HiMill D1S Tool Installation Guide](/en/himill-d1-d1s/hmd1s-tool-installation.md)

---

## HiMill CNC Tool Breakage & Processing Stop - Troubleshooting
**Problem**: How to handle tool breakage or unexpected stop during processing?

**Solution**:
- **Tool Breakage Handling**:
  - After tool breakage, stop the device operation immediately and be sure to remove the broken tool handle
  - Take different processing methods according to the G-code form and device status
  - Restart the device, after homing, replace the tool, reset Z0, and restart processing
  - If there is tool change code, click the tool change button in the software to replace the tool and automatically measure height
- **Unexpected Stop Handling**:
  - Check the stop reason (such as safety door opening, power failure, etc.)
  - After troubleshooting, long press the device button for 2 seconds to resume processing
  - If power is lost, after restarting the device, it is necessary to re-home and set the origin

**Related Documents**:
- [Guide for Handling Tool Breakage During Processing](/en/himill-d1-d1s/hmd1s-cutting-issue-handling.md)
- [HiMill D1S Processing Stop Issue Handling](/en/himill-d1-d1s/hmd1s-processing-stop-issue-handling.md)

---

## HiMill CNC Abnormal Noise - Troubleshooting & Maintenance
**Problem**: The device makes abnormally loud noise during operation.

**Solution**:
- Check if the guide rails and lead screws need lubrication (use recommended lubricant)
- Confirm if the moving axis is jammed by foreign objects or debris
- Check if the spindle bearings are worn or damaged
- Ensure the device is placed stably on a level surface without resonance

**Related Documents**: [HiMill D1 Guide Rail Lead Screw Maintenance](/en/himill-d1-d1s/hmd1-guide-rail-lead-screw-maintenance.md)

---

## FAQPage Schema Markup

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "Why won't my HiMill CNC machine power on?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "If your MAXMAKE HiMill D1/D1S CNC machine cannot power on, check if the power cord is damaged, replace the power socket, verify the voltage setting matches local standards (110V/230V), and ensure the device voltage level is correctly adjusted. If smoke appears or issues persist, contact technical support."
      }
    },
    {
      "@type": "Question",
      "name": "How to connect HiMill CNC to computer via USB or WiFi?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "For USB connection: use the original USB-B data cable, ensure both ends are fully inserted, avoid low-quality USB hubs, try different USB ports, and check for dust or oxidation. For WiFi: enable WiFi in MaxmakeLab software, verify network configuration (SSID and password), and ensure both devices are on the same network."
      }
    },
    {
      "@type": "Question",
      "name": "How to switch HiMill CNC power voltage between 110V and 230V?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Toggle the voltage switch to the left for 230V (Europe, Asia) or to the right for 110V (USA, Japan). The voltage adjustment switch is located on the device power module. Always adjust before powering on to match local voltage standards."
      }
    },
    {
      "@type": "Question",
      "name": "What software controls HiMill CNC machines?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "HiMill series CNC machines use MaxmakeLab software for control and programming. MaxmakeLab is specifically designed for HiMill equipment, supporting both CNC machining and laser processing modes with complete design, toolpath generation, and processing control functions."
      }
    },
    {
      "@type": "Question",
      "name": "Why can't I use CAM function and tool library in MaxmakeLab?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "CAM-related functions are currently under active development. Once completed and available, updates will be released through software updates. In the meantime, use external CAM software like Fusion 360 or Vectric Aspire to generate toolpaths for your HiMill CNC machine."
      }
    },
    {
      "@type": "Question",
      "name": "How to enable safety door function on HiMill CNC?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Connect the device, click device settings button, find the safety door setting option, and toggle it on or off. When enabled, opening the front cover during processing automatically pauses operations. After closing, long press the button for 2 seconds to resume."
      }
    },
    {
      "@type": "Question",
      "name": "What is the tool change process for HiMill CNC?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Click tool change button in MaxmakeLab. The spindle moves to tool change position (X140,Y0), indicator flashes yellow. Pull down handle, insert tool with ≥15mm clamping depth, release handle. Click button to complete automatic height measurement before processing."
      }
    },
    {
      "@type": "Question",
      "name": "How to handle tool breakage or unexpected stop during processing?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "For tool breakage: stop immediately, remove broken tool, restart device, re-home, replace tool, reset Z0, and restart. For unexpected stops: check reason (safety door, power failure), troubleshoot, then long press button 2 seconds to resume. After power loss, re-home and set origin."
      }
    },
    {
      "@type": "Question",
      "name": "Why is my HiMill CNC making abnormal noise?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Abnormal noise may indicate guide rails or lead screws need lubrication, foreign objects jamming the moving axis, worn spindle bearings, or unstable placement. Ensure proper lubrication, clean debris, check bearings, and place machine on a stable level surface."
      }
    }
  ]
}
</script>

---

## HiMill CNC Dust Collection System - Usage & Maintenance
**Problem**: How to correctly use and maintain the device's dust collection system?

**Solution**:
- Ensure the dust collection pipeline is tightly connected to the machine
- Regularly clean the vacuum cleaner filter to maintain suction power
- Check if the dust collection port is blocked by debris
- Ensure the vacuum cleaner has sufficient power (recommended 1000W+)
- Keep the dust collection system on during processing to maintain clean working environment

**Related Documents**:
- [HiMill D1 Dust Collection System](/en/himill-d1-d1s/hmd1-dust-collection-system.md)
- [HiMill D1S Dust Collection System](/en/himill-d1-d1s/hmd1s-dust-collection-system.md)

---

## HiMill CNC Accessories - Tutorials & User Guides
**Problem**: Where to find tutorials for different accessories purchased?

**Solution**:
Below are the tutorials for HiMill D1/D1S accessories:

**Related Documents**:
- [HiMill D1S 3D Probe Usage Guide](/en/himill-d1-d1s/hmd1s-3d-probe-using.md)
- [HiMill D1S Laser Module Guide](/en/himill-d1-d1s/hmd1s-laser-module.md)
- [HiMill D1S Rotation Axis Guide](/en/himill-d1-d1s/hmd1s-rotation-axis.md)
- [HiMill D1S Side Clamp Guide](/en/himill-d1-d1s/hmd1s-side-clamp.md)
- [HiMill D1S Vacuum Platform Guide](/en/himill-d1-d1s/hmd1s-vacuum-platform.md)