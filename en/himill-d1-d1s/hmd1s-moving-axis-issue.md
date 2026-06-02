# HiMill D1S Axis Movement Issues | MAXMAKE Wiki

Learn how to fix axis movement problems on [MAXMAKE HiMill D1/D1S](https://www.maxmake.com/products) CNC machine. This guide covers axis not moving, stuttering, and free movement issues with step-by-step solutions.

## Precautions
>- **Emergency Handling**: In case of continuous axis collision or jamming, immediately stop the device and power it off to avoid further damage to mechanical components
>- **Safe Operation**: Before conducting any inspections or repairs, ensure the device is completely powered off
>- **Operation Specifications**: When manually adjusting axis positions, operate slowly
>- **Protective Measures**: When handling mechanical components, it is recommended to wear protective gloves to prevent scratches
> {.is-warning}
---

## Possible Phenomena
- **Not Locked After Power-On**: After the device is powered on, the axis is not in a locked state and may move freely
- **Axis Does Not Move**: When operating the controller, the axis shows no movement response
- **Axis Movement Stutters**: The axis experiences stuttering, shaking, or abnormal noise during movement

## Possible Causes
### Electrical Faults
- Motor driver failure or damage
- Loose, poor contact, or disconnected motor wires
- Motor itself has failed

### Mechanical Faults
- Mechanical transmission parts (such as lead screws, guide rails) are faulty or have foreign objects stuck
- Insufficient lubrication of guide rails or lead screws leading to increased friction

### Control System Issues
- Limit switches are triggered or damaged
- Incorrect parameter settings
- Controller software abnormality

## Solutions

### 1. Exclude Limit Switch Abnormalities
- After powering on, try the homing operation to check if it can move normally
- If homing fails, refer to the [HiMill D1/D1S Limit Switch Issues](/en/himill-d1-d1s/hmd1s-limit-switch-issue.md)

### 2. Check Mechanical Transmission Parts
- Carefully check if there are any foreign objects stuck in the transmission path
- If jamming is found, immediately power off and remove the foreign objects

### 3. Check Motor Connection Wires

#### X Motor Connection Wires
The spindle needs to be moved to the right for inspection. Try reconnecting:
<img src="/eng/himill-d1-d1s/media/hmd1s-moving-axis-issue/x电机.jpg" alt="MAXMAKE HiMill D1/D1S X Motor" style="width: 400px; height: auto; margin-bottom: 8px; border-radius: 16px;" /> <img src="/eng/himill-d1-d1s/media/hmd1s-moving-axis-issue/x电机线.jpg" alt="MAXMAKE HiMill D1/D1S X Motor Wires" style="width: 400px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

#### Y Motor Connection Wires
The device needs to be placed sideways for inspection. Try reconnecting:
<img src="/eng/himill-d1-d1s/media/hmd1s-moving-axis-issue/y电机线.jpg" alt="MAXMAKE HiMill D1/D1S Y Motor Wires" style="width: 400px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

#### Z Motor Connection Wires
Check the position as follows. Try reconnecting:
<img src="/eng/himill-d1-d1s/media/hmd1s-moving-axis-issue/z电机线.jpg" alt="MAXMAKE HiMill D1/D1S Z Motor Wires" style="width: 400px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 4. Check Lubrication Status
- Check if the guide rails and lead screws are insufficiently lubricated
- If not lubricated for a long time, noise and jamming will occur during movement

### 5. Restart the Device
- Turn off the device power, wait 30 seconds, and then restart
- Observe if the axis movement returns to normal

### 6. Restore Parameter Settings
- If the movement still stutters with abnormal noise, try restoring the device to factory parameters. After connecting the device, try clicking the restore button after homing
<img src="/eng/himill-d1-d1s/media/hmd1s-moving-axis-issue/恢复参数.png" alt="MAXMAKE HiMill D1/D1S Restore Parameters" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 7. Check Main Control Board Motor Wires
- Check if the motor connection wires on the main control board are loose or have poor contact. For cover removal steps, refer to the video for replacing the main control board [HiMill D1/D1S Replace Air Cabinet Components](/en/himill-d1-d1s/hmd1s-replace-air-cabinet.md)
<img src="/eng/himill-d1-d1s/media/hmd1s-moving-axis-issue/主控板未插线电机.jpg" alt="MAXMAKE HiMill D1/D1S Main Control Board Without Motor Wires" style="width: 350px; height: auto; margin-bottom: 8px; border-radius: 16px;" /> <img src="/eng/himill-d1-d1s/media/hmd1s-moving-axis-issue/主控板插线电机.jpg" alt="MAXMAKE HiMill D1/D1S Main Control Board With Motor Wires" style="width: 450px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 8. Contact Technical Support
If none of the above methods work, please contact support@maxmake.com for further assistance

---

## FAQPage Schema Markup

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "Why won't my HiMill D1S axis move?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Common causes include motor driver failure, loose motor wires, mechanical jamming from foreign objects, insufficient lubrication, limit switch issues, or incorrect parameter settings. Try homing operation, checking for obstructions, verifying motor connections, and restarting the device."
      }
    },
    {
      "@type": "Question",
      "name": "What causes axis movement stuttering on HiMill CNC?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Axis stuttering can be caused by loose motor connections, insufficient guide rail/lead screw lubrication, mechanical jamming, or controller software issues. Check motor wires, lubricate moving parts, remove any obstructions, and try restoring factory parameters."
      }
    },
    {
      "@type": "Question",
      "name": "Why is my HiMill axis not locked after power-on?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "If the axis moves freely after power-on, this indicates a motor driver issue, disconnected motor wires, or controller software problem. Check motor connections on X, Y, Z axes, verify main control board wiring, and restart the device."
      }
    },
    {
      "@type": "Question",
      "name": "How to check motor connections on HiMill D1S?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "For X motor: move spindle right and inspect connections. For Y motor: place device sideways. For Z motor: check upper connections. Also verify wiring on main control board. Refer to official maintenance videos for cover removal procedures."
      }
    }
  ]
}
</script>