# HiMill D1S USB Connection Issues | MAXMAKE Wiki

Learn how to fix USB connection problems between [MAXMAKE HiMill D1/D1S](https://www.maxmake.com/products) CNC machine and [MaxmakeLab](https://maxmake.com/pages/software) software. This guide covers cable issues, port checks, and driver troubleshooting.

---

## Cable Issues

### Possible Causes
- Damaged USB cable
- Poor USB interface contact
- Signal attenuation due to excessively long USB cable

### Solutions
1. Check if the USB cable has obvious damage or disconnection
2. Replace with a high-quality USB data cable (original equipment cable or shielded USB cable is recommended)
3. Check if the device USB interface and computer USB interface have dust or oxidation
4. Try re-plugging the USB cable to ensure a secure connection
5. Replace the USB interface (try another USB port on the computer)
6. Avoid using excessively long USB extension cables; if necessary, use an extension cable with signal amplification function
7. Check if the USB connection terminal on the main control board is loose or has poor contact; please refer to the video on replacing the main control board for steps to remove the rear cover [HiMill D1/D1S Air Cabinet Component Replacement](/en/himill-d1-d1s/hmd1s-replace-air-cabinet.md)

<img src="/eng/himill-d1-d1s/media/hmd1s-cannot-connect-software-via-usb/主控板未插线usb.jpg" alt="Main Control Board Not Plugged In" style="width: 350px; height: auto; margin-bottom: 8px; border-radius: 16px;" /> <img src="/eng/himill-d1-d1s/media/hmd1s-cannot-connect-software-via-usb/主控板插线usb.jpg" alt="Main Control Board Plugged In" style="width: 450px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

8. If the problem persists, contact support@maxmake.com



---

## Interference Issues

### Possible Causes
- Strong electromagnetic interference sources nearby (such as motors, transformers, wireless devices, etc.)
- USB cable laid parallel to other high-voltage lines
- Insufficient power supply from computer USB port
- Abnormal computer USB driver

### Solutions
1. Keep the device away from strong electromagnetic interference sources (such as high-power motors, microwave ovens, wireless routers, etc.)
2. Avoid laying USB cables parallel to high-voltage lines (such as power cables)
3. Try using a USB hub (with independent power supply) to provide stable power
4. Check if the device USB interface has an electromagnetic shielding cover (if applicable)
5. Update or reinstall the computer USB driver
6. Restart the computer and device, then retry the connection
7. Try connecting the device in a different environment to confirm if it is an environmental interference issue
8. If the problem persists, contact support@maxmake.com

---

## FAQPage Schema Markup

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "Why can't my HiMill D1S connect via USB?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Common causes include damaged USB cable, poor interface contact, signal attenuation from long cables, electromagnetic interference, or USB driver issues. Try replacing the USB cable, checking ports for dust/oxidation, avoiding long extension cables, keeping away from interference sources, updating USB drivers, and restarting both computer and device."
      }
    },
    {
      "@type": "Question",
      "name": "What should I do if USB connection keeps disconnecting?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Ensure the USB cable is securely plugged in, use a shielded or original USB cable, avoid USB hubs without independent power supply, check for electromagnetic interference from motors or wireless devices, and try connecting to a different USB port on your computer."
      }
    },
    {
      "@type": "Question",
      "name": "How to fix USB driver issues for HiMill CNC?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Update or reinstall your computer's USB drivers, restart both the computer and HiMill device, try connecting to a different USB port, and ensure you're using the original USB-B data cable provided with the machine."
      }
    },
    {
      "@type": "Question",
      "name": "When should I contact technical support for USB issues?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Contact support@maxmake.com if you've tried all troubleshooting steps: replacing cables, checking ports, avoiding interference, updating drivers, and verifying the main control board connection, but the USB connection issue still persists."
      }
    }
  ]
}
</script>