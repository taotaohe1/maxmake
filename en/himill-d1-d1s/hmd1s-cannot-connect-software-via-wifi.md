# MaxmakeLab HiMill D1/D1S Cannot Connect to Software via WiFi

---

## 🔌 Connection Issues

### ❓ Possible Causes
- Device not properly restarted or homed
- WiFi account or password entered incorrectly
- Computer IP address configuration error
- Router settings abnormal
- Device antenna connection poor


### ✅ Solutions

1. **🔄 Restart Device**
   - Turn off device power
   - Wait 10 seconds before restarting the device
   - Ensure device is homed after restart, then enter settings interface
   - Try reconnecting to WiFi network


2. **🔑 Check WiFi Account and Password**
   - Confirm WiFi account and password are entered correctly
   - Pay attention to password case sensitivity and special characters
   - Re-enter password

3. **🌐 Check IP Address Configuration**
   - Select your computer's IP address from the "Local IP Address" dropdown menu (usually there is only one option; if there are multiple, check the wireless network adapter IP address in your computer's network settings)
   - Enter the device IP address in the field below

4. **📡 Check Router Settings**
   - Check if the router has blocked the device
   - View the router's MAC address filtering configuration
   - Confirm the router's WiFi frequency band (2.4GHz) configuration [This device only supports the 2.4GHz frequency band]
   - Restart the router

5. **📱 Test Device Hotspot Function**
   - Switch the device to hotspot mode (for specific operation steps, refer to the "Switch to Hotspot Mode" section in [HiMill D1/D1S Network Configuration](/en/himill-d1-d1s/hmd1s-network-configuration.md))
   - Use your computer to search and connect to the device hotspot
   - If your computer can connect to the hotspot, it indicates that the device WiFi module is working properly

6. **📡 Check Device Antenna Connection**
   - Remove the back cover and check if the antenna on the main control board has fallen off or is loose
   - For back cover removal steps, please refer to the video for replacing the main control board [HiMill D1/D1S Replace Component Cabinet](/en/himill-d1-d1s/hmd1s-replace-air-cabinet.md)
   - (If the top cover was previously removed, the antenna may have been pulled off during disassembly)
   - Open the top cover and check the antenna connection status
   - For top cover removal steps, please refer to the video for replacing the moving axis motor [HiMill D1/D1S Replace Moving Axis Motor](/en/himill-d1-d1s/hmd1s-replace-moving-axis-motor.md), specifically the Z-axis motor replacement section, as removing the top cover is similar to replacing the Z-axis motor

> ⚠️ **Important Notice**：
> - When opening the top cover, be very careful not to pull on the antenna!!!
> 
> {.is-warning}

**Antenna Location on Main Control Board:**

<img src="/eng/himill-d1-d1s/media/hmd1s-cannot-connect-software-via-wifi/主控板.jpg" alt="Antenna Not Connected" style="width: 50%; height: auto; margin-bottom: 8px; border-radius: 16px;" /> <img src="/eng/himill-d1-d1s/media/hmd1s-cannot-connect-software-via-wifi/wifi天线.png" alt="Antenna Connected" style="width: 50%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

7. **📧 If the problem persists, please contact support@maxmake.com**

---

## 📶 Interference Issues

### ❓ Possible Causes
- Strong electromagnetic interference sources nearby
- WiFi signal blocked or attenuated
- Device too far from router

### ✅ Solutions
1. Move the device away from strong electromagnetic interference sources (such as microwave ovens, wireless routers, Bluetooth devices, etc.)
2. Reduce WiFi signal obstructions, ensure no metal barriers between device and router
3. Move the device closer to the router, or use a WiFi signal amplifier
4. Try switching WiFi frequency bands (2.4GHz), this device only supports the 2.4GHz frequency band, if using 5GHz frequency band, only hotspot connection is available
5. Restart the router and device, then retry connection
6. If the problem persists, please contact support@maxmake.com
