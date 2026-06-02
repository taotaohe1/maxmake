# HiMill D1S Cannot Power On | MAXMAKE Wiki

Learn how to troubleshoot power-on issues with [MAXMAKE HiMill D1/D1S](https://www.maxmake.com/products) CNC machine. This guide covers power cord checks, voltage adjustment, and step-by-step solutions.

---

### Possible Phenomena
- No response from the device after connecting to power
- Device lights, indicators, and spindle lights are all off
- No response when pressing the power switch
- Smoke coming from the back of the device after connecting to power

### Possible Causes
- Damaged or disconnected power cord
- Faulty power socket or no power supply
- Fault in the internal power module
- Incorrect voltage adjustment that doesn't match the input voltage, e.g., external power supply is 220V but the power module is adjusted to 110V

### Solutions
1. Check if the power cord is obviously damaged or disconnected
2. Replace the power socket and confirm if the socket has normal power supply. Under normal power supply, the internal power indicator should light up. For cover removal steps, refer to the video for replacing the main control board [HiMill D1/D1S Air Cabinet Component Replacement](/en/himill-d1-d1s/hmd1s-replace-air-cabinet.md)

<img src="/eng/himill-d1-d1s/media/hmd1s-cannot-power-on/开关电源指示灯.jpg" alt="Switch Power Indicator" style="width: 400px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

3. Check if the voltage of the power module is adjusted correctly. The adjustment position is shown in the following pictures

<img src="/eng/himill-d1-d1s/media/hmd1s-cannot-power-on/电压调节位置.jpg" alt="Power Module Voltage Adjustment Position" style="width: 400px; height: auto; margin-bottom: 8px; border-radius: 16px;" /> <img src="/eng/himill-d1-d1s/media/hmd1s-cannot-power-on/电压调节位置内部.jpg" alt="Power Module Voltage Adjustment Position" style="width: 400px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

4. If the above methods are ineffective, or if smoke appears, contact support@maxmake.com

---

## FAQPage Schema Markup

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "Why won't my HiMill D1S CNC machine power on?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Possible causes include damaged or disconnected power cord, faulty power socket or no power supply, internal power module fault, or incorrect voltage adjustment. Check power cord, replace power socket, verify voltage setting matches input voltage (110V/220V), and contact support if issues persist."
      }
    },
    {
      "@type": "Question",
      "name": "What should I do if my HiMill D1S shows no response after connecting power?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Check if the power cord is damaged or disconnected. Replace the power socket and confirm normal power supply. Verify the internal power indicator lights up. Check voltage module adjustment matches your local voltage (110V or 220V)."
      }
    },
    {
      "@type": "Question",
      "name": "How do I check the voltage setting on HiMill D1S?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Locate the power module voltage adjustment position inside the device. Ensure the voltage setting matches your local power supply (110V or 220V). Incorrect voltage adjustment can prevent the device from powering on."
      }
    },
    {
      "@type": "Question",
      "name": "What if smoke comes from my HiMill D1S after connecting power?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Immediately disconnect power and do not attempt to use the device. Contact MAXMAKE support at support@maxmake.com for assistance. Smoke indicates a serious electrical issue that requires professional repair."
      }
    }
  ]
}
</script>