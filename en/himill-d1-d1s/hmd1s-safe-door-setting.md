# MaxmakeLab HiMill D1/D1S Safe Door Setting

## 📋 Safe Door Function Description

- The safe door function can be enabled in the device settings
- When the safe door function is enabled, the processing will automatically pause when the front cover is opened during processing. After closing the door, press and hold the button for 2 seconds to resume processing
- When the safe door function is disabled, opening the front cover during processing will not affect the processing

## ⚠️ Important Notes

> - Even if the safe door function is enabled, you can still start processing with the front cover open. The pause will only be triggered if you close the door and then open it again
> - During pause, the spindle still keeps rotating, please pay attention to safety
>
> {.is-warning}

---

## 📝 Setting Steps

### Step 1: Open Device Settings Interface

After connecting the device, click the device settings button to open the device settings interface.

<img src="/eng/himill-d1-d1s/media/hmd1s-safe-door-setting/1.png" alt="Device Settings Interface" style="max-width: 800px;">

### Step 2: Set Safe Door Function

After entering this interface, the safe door switch will display the current switch status. Turn it on or off as needed.

<img src="/eng/himill-d1-d1s/media/hmd1s-safe-door-setting/2.png" alt="Safe Door Switch Setting" style="max-width: 800px;">

### Step 3: Check Safe Door Status Indicator

The safe door indicator in the workflow status bar only indicates the status of the front cover. You can observe whether the front cover is properly closed through this indicator.

<img src="/eng/himill-d1-d1s/media/hmd1s-safe-door-setting/3.png" alt="Safe Door Status Indicator" style="max-width: 800px;">

- **Indicator light is on**: Indicates that the safe door is closed
- **Indicator light is gray**: Indicates that the front cover is not detected as closed

---

## HowTo Schema Markup

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "HowTo",
  "name": "How to Set Up HiMill D1/D1S Safe Door Function",
  "description": "Complete guide for enabling and configuring the safety door function on MAXMAKE HiMill D1/D1S CNC machine using MaxmakeLab software.",
  "step": [
    {
      "@type": "HowToStep",
      "name": "Open Device Settings Interface",
      "text": "Connect the HiMill device to computer via USB or WiFi. Click the device settings button in MaxmakeLab software to open the settings interface."
    },
    {
      "@type": "HowToStep",
      "name": "Toggle Safe Door Function",
      "text": "In the device settings interface, locate the safe door switch. Toggle it on to enable or off to disable the safety door function as needed."
    },
    {
      "@type": "HowToStep",
      "name": "Verify Safe Door Status",
      "text": "Check the safe door status indicator in the workflow status bar. When enabled, opening front cover during processing will pause operations. Press and hold button for 2 seconds to resume after closing."
    }
  ],
  "tool": [
    {
      "@type": "HowToTool",
      "name": "MaxmakeLab Software"
    }
  ]
}
</script>