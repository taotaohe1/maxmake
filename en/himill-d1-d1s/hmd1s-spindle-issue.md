# HiMill D1S Spindle Not Rotating | MAXMAKE Wiki

Learn how to fix spindle problems on [MAXMAKE HiMill D1/D1S](https://www.maxmake.com/products) CNC machine. This guide covers spindle not rotating, motor issues, and step-by-step troubleshooting solutions.


---

## Spindle Not Rotating

### Possible Causes
- Loose motor driver connection wires
- Spindle motor failure
- Software setting issues (e.g., device in laser mode)

### Solutions
1. Check if the motor driver signal wires are loose and try reconnecting them. For cover removal steps, refer to the video for replacing the main control board [HiMill D1/D1S Replace Air Cabinet Components](/en/himill-d1-d1s/hmd1s-replace-air-cabinet.md)
<img src="/eng/himill-d1-d1s/media/hmd1s-spindle-issue/主控未插线电机驱动.jpg" alt="MAXMAKE HiMill D1/D1S Control Board Without Motor Driver Wires" style="width: 350px; height: auto; margin-bottom: 8px; border-radius: 16px;" /> <img src="/eng/himill-d1-d1s/media/hmd1s-spindle-issue/电机驱动.jpg" alt="MAXMAKE HiMill D1/D1S Control Board With Motor Driver Wires" style="width: 450px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

2. Check if the spindle speed settings in the software are reasonable
3. Confirm if the device was just used with the laser and if it is currently in laser mode
4. If the issue persists, contact support@maxmake.com

---

## Spindle Stops Immediately After Starting

### Possible Causes
- Spindle bearing failure
- Motor driver failure
- Excessive processing load

### Solutions
1. Check if the processing load is too high, and appropriately reduce the cutting depth or feed rate
2. Check if the motor driver signal wires are loose and try reconnecting them
3. Restart the device and try again
4. If the issue persists, contact support@maxmake.com

---

## FAQPage Schema Markup

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "Why is my HiMill D1S spindle not rotating?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Possible causes include loose motor driver connection wires, spindle motor failure, or software setting issues (e.g., device in laser mode). Check motor driver signal wires, verify spindle speed settings in software, confirm device is in CNC mode not laser mode, and contact support if issue persists."
      }
    },
    {
      "@type": "Question",
      "name": "How do I fix spindle not rotating on HiMill D1S?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Check if motor driver signal wires are loose and reconnect them. Verify spindle speed settings in software are reasonable. Confirm device is not in laser mode. If issue persists, contact MAXMAKE support at support@maxmake.com."
      }
    },
    {
      "@type": "Question",
      "name": "Why does my HiMill D1S spindle stop immediately after starting?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Possible causes include spindle bearing failure, motor driver failure, or excessive processing load. Reduce cutting depth or feed rate, check motor driver signal wires, restart device, and contact support if issue continues."
      }
    },
    {
      "@type": "Question",
      "name": "What should I do if spindle stops during machining on HiMill D1S?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Check if processing load is too high and reduce cutting depth or feed rate appropriately. Verify motor driver signal wires are connected properly. Restart the device and try again. Contact MAXMAKE support if the problem persists."
      }
    }
  ]
}
</script>