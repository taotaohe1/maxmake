# Emergency Stop Interface

## 1. Interface Introduction

The interface labeled **E-Stop** on the back panel of the device is the external emergency stop interface, located next to the TP IN interface:

<img src="/eng/himill-d1-d1s/media/hmd1s-emergency-stop-interface/1-emergency-stop-interface.png" alt="E-Stop emergency stop interface on the back panel" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

- **Interface specification**: GX12 2-pin male aviation connector
- **Matching plug**: GX12 2-pin female aviation connector
- **Trigger method**: The emergency stop signal is triggered when the two pins are electrically closed (shorted)

Through this interface, you can connect an external emergency stop button or other safety device to stop the machine immediately in an emergency.

## 2. Trigger and Recovery

| Status | Interface Signal | Machine Behavior |
|--------|------------------|------------------|
| Normal | Two pins open | Machine operates normally |
| Emergency stop triggered | Two pins shorted (closed) | Motion output stops and machining is aborted immediately; JOG movement and spindle activation are disabled while the emergency stop is active |
| Reset and recover | Two pins return to open | After releasing the emergency stop, homing must be performed again before the machine can be used |

> ℹ️ **What to do after an emergency stop**:
> After the emergency stop is triggered, the software will display an ALARM3 / ALARM10 message. First reset the external emergency stop device, then perform homing again. The alarm will be cleared and normal operation can resume.
> {.is-info}

You can also verify the external emergency stop signal in the detection interface of MaxMakeLab: the status indicator turns green when the external emergency stop is triggered and turns gray when released (firmware V1.0.34 or later required).

## 3. Self-Adaptation Guide

No official emergency stop device is available yet. You may purchase and adapt one yourself according to the specifications below.

### 3.1 Required Materials

| Item | Specification / Requirement |
|------|------------------------------|
| Aviation connector | GX12 2-pin (2-contact) female aviation connector |
| Emergency stop button | Mushroom-head self-locking button with one normally open (NO) contact |
| Cable | 2-core sheathed cable; choose an appropriate wire gauge for the actual routing distance |

### 3.2 Wiring and Installation Steps

1. **Power off**: Before wiring, make sure to turn off the machine and unplug the power cord.
2. **Connect the button**: Wire one **normally open (NO) contact** of the emergency stop button to the two pins of the GX12 female connector — the two pins conduct when the button is pressed and open when the button is rotated or pulled out.
3. **Mount the button**: Install the emergency stop button where the operator can reach it quickly and directly, without being blocked by workpieces, materials, or chips.
4. **Check the signal**: Connect the interface and power on. In the MaxMakeLab detection interface, press and release the button and confirm that the emergency stop status indicator changes accordingly.
5. **No-load verification**: Simulate an emergency stop without a tool installed and without machining: confirm that the machine stops immediately; after resetting, re-home as prompted and confirm the machine returns to normal.

> ⚠️ **Wiring notes**:
> - This machine triggers on **contact closure**, so use the **normally open (NO) contact** of the button. This differs from the normally closed (NC) emergency stop circuits commonly used on industrial equipment — do not copy wiring methods from other machines.
> - Since the open state is the normal state, an accidental cable break will not trigger the emergency stop. Route the cable away from moving parts to prevent pinching and abrasion, and inspect the cable regularly.
> {.is-warning}

## 4. Precautions

> ⚠️ **Safety warnings**:
> - Plugging/unplugging the connector and all wiring operations must be performed with the **power off**.
> - The interface determines the emergency stop state solely by the continuity of its two pins. **Do not apply external voltage or connect other signal sources** to the interface, as this may damage the machine.
> - The reliability of a self-made emergency stop device is the responsibility of the maker. Please use reliable buttons, connectors, and cables, and test the function regularly.
> - The external emergency stop is a supplementary safety measure and cannot replace proper operation and routine safety checks.
> - We recommend updating the machine firmware to the latest version (V1.0.37 and later fix the issue where JOG movement or spindle activation was still possible after an external emergency stop was triggered).
> {.is-warning}

## 5. Official Accessory

An official emergency stop device is still in planning. Once its design and verification are completed, a ready-to-use accessory will be listed in the official Maxmake store — no self-wiring required. The purchase link will be updated here when available:

- 🔗 Official store emergency stop accessory: **Coming soon**

## 6. Related Documents

- [Detection Function Description](/en/himill-d1-d1s/hmd1s-detection-function.md)
- [Software Error Query](/en/himill-d1-d1s/hmd1s-software-error-query.md)
