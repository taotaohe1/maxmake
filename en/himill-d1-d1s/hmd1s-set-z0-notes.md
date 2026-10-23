---
title: "HiMill D1S Setting Z0 Notes"
description: "Learn how to set the Z0 (Z-axis machining origin) on the MAXMAKE HiMill D1S CNC machine."
---

# HiMill D1S Setting Z0 Notes | MAXMAKE Wiki

Learn how to set the Z0 (Z-axis machining origin) on the [MAXMAKE HiMill D1S](https://www.maxmake.com/products/himill-d1s) CNC machine. This guide explains the G-code logic behind the Set Z0 function, the required height measurement step, power-off compensation behavior, and precautions for third-party control software.

---

## 1. G-Code Logic Behind Setting Z0

When you click the "Set Z0" button in MaxmakeLab, the software sends the following G-codes to the machine in sequence:

```
[SET_OFFSET]
G10L1P1Z0
G43H1
G92Z0
```

Description of each command:
- `G10L1P1Z0`: Writes the current tool length compensation value into the active coordinate system
- `G43H1`: Applies the H1 tool length compensation
- `G92Z0`: Sets the current Z-axis position as the Z0 point

> 📋 **Note**:
> 
> - MaxmakeLab has this logic built in, so you can simply click the "Set Z0" button — no manual entry required.
> - If you are using a third-party control software (not MaxmakeLab), you must create your own macro program that contains these G-codes and use it as the "Set Z0" function.
> 
> {.is-info}

---

## 2. Always Measure Tool Height Before Setting Z0

> ⚠️ **Important Precautions**:
> 
> - Tool height measurement must be completed before setting Z0.
> - If you set Z0 and start machining without measuring tool height first, the tool length compensation will be incorrect, which may lead to machining errors or a collision between the tool and the workpiece.
> 
> {.is-warning}

After height measurement, the current tool is set as the reference tool. When a subsequent `T*M6` tool change command is executed in the machining program, the machine automatically runs the tool change macro, completes height measurement for the new tool, and writes the new tool length compensation value into the active coordinate system.

---

## 3. Compensation Value Behavior After Power Off

> ⚠️ **Power-Off Precautions**:
> 
> - After the machine is powered off, all written tool length compensation values are cleared.
> - The Z value retained in the coordinate system after power-off corresponds to the tool that was measured and had Z0 set before the power was cut.
> - If an unexpected power loss occurs, you must re-run the height measurement and set Z0 again before resuming machining.
> 
> {.is-warning}

---

## 4. Height Measurement When Using the 3D Probe

When using the 3D probe for detection, the first step is always height measurement. Click the "Tool Change" button in the software and the machine will automatically complete the height measurement process before you proceed with further detection and Z0 setting.

For detailed instructions, refer to: [How to Use HiMill D1S 3D Probe](./hmd1s-3d-probe-using.md)

---

## 📋 Setting Z0 Key Points Summary

> 🚨 **Key Points**:
> 
> 1. After installing a tool, always complete height measurement before setting Z0.
> 2. Once height measurement is done, move the tool to the workpiece surface and click "Set Z0".
> 3. When using third-party control software, create your own macro program and send the G-codes strictly in this order: `[SET_OFFSET]` → `G10L1P1Z0` → `G43H1` → `G92Z0`.
> 4. After a power loss, re-run height measurement and set Z0 again.
> 5. When using the 3D probe, click "Tool Change" first to complete height measurement.
> 
> {.is-warning}
