# 📋 Software Error Query

> This page organizes all software error information for HiMill D1/D1s equipment to help users quickly locate and resolve equipment fault issues.

---

## 📊 Overview Information

| Error Type | Count | Description |
|-----------|-------|-------------|
| 🚨 **Alarm Errors (ALARM)** | 14 | Equipment hardware or safety-related alarm information |
| ❌ **Error Messages (ERROR)** | 85 | Software command, parameter setting related errors |

---

## 🚨 Alarm Errors (ALARM)

> **Description**: These errors are usually related to equipment hardware status, safety settings, and sensor functions, requiring priority handling.

| Error Code | Error Name | Fault Cause | Solution |
|------------|------------|-------------|----------|
| ALARM | Please home the machine. |  |  |
| ALARM1 | Hard limit has been triggered. | 1.Collision causes loss of motor position synchronization, which in turn triggers the limit switch during subsequent movements.<br>2.Accidental contact with the limit switch by hands or foreign objects.<br>3.Abnormal motor operation leads to false triggering of the limit switch.<br>4.Malfunction of the limit switch. | 1.Re-homing is required. Meanwhile, check the fixture, workpiece installation, spindle mounting height and machining file path.<br>2.Re-homing is required. If the limit switch is mistakenly triggered due to object collision, remove the foreign object. Note safety during use; do not insert hands or other objects into the device while it is moving.<br>3.Please check if the motor operation is abnormal, such as abnormal vibration, complete standstill or movement in only one direction. For specific details, refer to the help documentation.<br>4.Enter the "Device Settings" - "Detection" interface to determine if the limit switch is faulty. If so, replace it in a timely manner. |
| ALARM2 | Motion target exceeds machine travel. Alarm during streaming of SD file at line: XXX | The target position in the executed motion code exceeds the device stroke. | Check whether the movement parameters of the XYZ axes in the G-code exceed the travel range. Please re-homing. |
| ALARM2 | Motion target exceeds machine travel. | The target position in the executed motion code exceeds the device stroke. | Check whether the movement parameters of the XYZ axes in the G-code exceed the travel range. Please re-homing. |
| ALARM3 | Reset/E-stop while in motion. | 1.Emergency stop button pressed.<br>2.Reset during movement. | 1.Release the emergency stop; re-homing is required.<br>2.Continue operation after re-homing |
| ALARM4 | Probe fail, The tool setter was triggered before probing. | 1.The tool setter is pressed before probing.<br>2.The tool setter is damaged. | 1.Remove foreign objects to release the tool setter. Please pay attention to operational safety and do not put hands or other objects into the equipment during its operation.<br>2.Enter the "Device Settings" - "Detection" interface to determine if the tool setter is faulty. If so, replace it in a timely manner. |
| ALARM4 | Probe fail, The 3D Probe was triggered before probing. | 1.The probe wire interface is not properly inserted<br>2.3D Probe failure.<br>3.The 3D Probe is already in a triggered state.(indicator light is red) before probing. | 1.Check whether the 3D Probe connection cable is securely connected (ensure it is fully inserted).<br>2.Enter the "Device Settings" - "Detection" interface to determine if the 3D Probe is faulty.<br>3.Before starting probing, ensure the 3D Probe is in a non-triggered state (with the indicator light green). Caution! If the probe is currently in contact with an object, remove the object first and then perform re-zeroing to avoid damaging the 3D Probe. |
| ALARM5 | Probe fail. The tool setter was not triggered within the probing travel. | 1.The tool is too short, or the spindle installation position is too high, resulting in failure to trigger the tool setter within the detection range.<br>2.Tool setter damage. | 1.Adjustments can be made to the spindle height or tool mounting height.<br>2.Enter the "Device Settings" - "Detection" interface to determine if the tool setter is faulty. If so, replace it in a timely manner. |
| ALARM5 | Probe fail. The 3D Probe was not triggered within the probing travel. | 1.The probe is too far from the workpiece, or the set probing distance is too short.<br>2.The 3D probe is malfunctioning. | 1.Move the probe closer to the workpiece, or increase the probing distance.<br>2.Enter the "Device Settings" - "Detection" interface to determine if the 3D Probe is faulty. |
| ALARM6 | Homing fail. The active homing cycle was reset. |  |  |
| ALARM7 | Homing fail. Safety door was opened during homing cycle. | Accidentally opened the safety door during the homing process | Keep the safety door closed during the homing process |
| ALARM8 | Homing fail. Pull off travel failed to clear limit switch. | 1.The limit switch is malfunctioning.<br>2.The motor is operating abnormally. | 1.Enter the "Device Settings" - "Detection" interface to determine if the limit switch is faulty. If so, replace it in a timely manner.<br>2.Check if the motor operation is abnormal (such as severe vibration with loud noise, complete standstill, or movement in only one direction). For details, refer to "How to check if the motor is normal" in the "Help" page.<br>3.Re-homing can be attempted again. |
| ALARM9 | Homing fail. Could not find limit switch within search distances. | 1.A collision occurred, causing movement to be blocked.<br>2.The limit switch is malfunctioning.<br>3.The motor is operating abnormally. | 1.Remove the obstacle and then perform re-homing again.<br>2.Enter the "Device Settings" - "Detection" interface to determine if the limit switch is faulty. If so, replace it in a timely manner.<br>3.Check if the motor operation is abnormal (such as severe vibration with loud noise, complete standstill, or movement in only one direction). For details, refer to "How to check if the motor is normal" in the "Help" page. |
| ALARM10 | EStop asserted. | The emergency stop button has been pressed. | After releasing the emergency stop button, re-homing is required. |
| ALARM11 | Homing required. | There may be a synchronization deviation in the current position. | Re-homing is required. |
| ALARM12 | Limit switch engaged. Clear before continuing. | 1.The limit switch is malfunctioning.<br>2.The motor is operating abnormally. | 1.Enter the "Device Settings" - "Detection" interface to determine if the limit switch is faulty. If so, replace it in a timely manner.<br>2.Check if the motor operation is abnormal (such as severe vibration with loud noise, complete standstill, or movement in only one direction). For details, refer to "How to check if the motor is normal" in the "Help" page.<br>3.Re-homing can be attempted again. |
| ALARM13 | Probe protection triggered. Clear before continuing. |  |  |

---

## ❌ Error Messages (ERROR)

> **Description**: These errors mainly involve G-code commands, parameter settings, file operations, etc., requiring checking of program code and parameter configuration.

### 📝 G-code Related Errors (ERROR1-ERROR39)

| Error Code | Error Name | Fault Cause | Solution |
|------------|------------|-------------|----------|
| ERROR1 | G-code words consist of a letter and a value. Letter was not found. Error in SD file at line XXX. | The G-code format is incorrect, with missing letters. | Please check if the G-code format is correct. |
| ERROR1 | G-code words consist of a letter and a value. Letter was not found. |  |  |
| ERROR2 | Missing the expected G-code word value or numeric value format is not valid. Error in SD file at line XXX. | 1.The input value is incorrectly formatted.<br>2.Missing values when writing G-code. | 1.Check if the range and format of values in the G-code are correct.<br>2.Carefully verify the G-code and supplement the missing values. |
| ERROR2 | Missing the expected G-code word value or numeric value format is not valid. |  |  |
| ERROR3 | '$' system command was not recognized or supported. |  |  |
| ERROR4 | Negative value received for an expected positive value. Error in SD file at line XXX. | A negative value was incorrectly entered in the G-code. | 1.Check the value input in the G-code to ensure it meets the requirements.<br>2.Check the relevant calculation logic and correct calculation errors. |
| ERROR4 | Negative value received for an expected positive value. |  |  |
| ERROR5 | Homing cycle failure. Homing is not configured via settings. |  |  |
| ERROR6 | Step pulse time must be greater or equal to 2 microseconds. |  |  |
| ERROR7 | A settings read failed. Auto-restoring affected settings to default values. |  | Please try again |
| ERROR8 | '$' command cannot be used unless controller state is IDLE. |  |  |
| ERROR9 | G-code locked out during alarm or jog state. |  |  |
| ERROR10 | Soft limits cannot be enabled without homing also enabled. |  |  |
| ERROR11 | Max characters per line exceeded. Line was not processed and executed. | 1.The number of characters in a single line of G-code is excessive.<br>2.The file is corrupted.<br>3. An incompatible post-processor is being used. | 1.Shorten the length and streamline the code.<br>2.Check the correctness of the file.<br>3.Check or replace the post-processor. |
| ERROR12 | '$' setting value cause the step rate to exceed the maximum supported. |  |  |
| ERROR13 | Safety door detected as opened and door state initiated. |  |  |
| ERROR14 | Build info or startup line exceeded EEPROM line length limit.Line not stored. |  |  |
| ERROR15 | Jog target exceeds machine travel. Command ignored. |  |  |
| ERROR16 | Jog command with no '=' or contains prohibited g-code. |  |  |
| ERROR17 | Laser mode requires PWM output. |  |  |
| ERROR18 | Reset asserted |  |  |
| ERROR19 | Non positive value |  |  |
| ERROR20 | Unsupported or invalid g-code command found in block. Error in SD file at line XXX. | 1. An unsupported G-code command is used.<br>2.The G-code command is incorrectly written. | 1.Check or replace the post-processor.<br>2.If the file is corrupted, please check the integrity of the file content. |
| ERROR20 | Unsupported or invalid g-code command found in block. |  |  |
| ERROR21 | More than one g-code command from same modal group found in block. Error in SD file at line XXX. | Multiple commands from the same modal group are incorrectly used in the code block (e.g., G1 and G0 exist in the same line). | 1.Check the code to ensure that only one command is used in the same modal group.<br>2.Learn and understand the concepts and usage rules of modal groups.<br>3.Check or replace the post-processor. |
| ERROR21 | More than one g-code command from same modal group found in block. |  |  |
| ERROR22 | Feed rate has not yet been set or is undefined. Error in SD file at line XXX. | The feed rate setting was omitted when writing the G-code. | 1.Check the G-code to confirm whether the feed rate F-value has been added (Example: G1 X10 Y10 Z10 F500).<br>2.Check or replace the post-processor |
| ERROR22 | Feed rate has not yet been set or is undefined. |  |  |
| ERROR23 | G-code command in block requires an integer value. Error in SD file at line XXX. | The value is not an integer. | 1.Please check if the G-code format is correct.<br>2.When writing code, pay attention to the requirements for value types specified by the commands.<br>3.Check or replace the post-processor. |
| ERROR23 | G-code command in block requires an integer value. |  |  |
| ERROR24 | More than one g-code command that requires axis words found in block. Error in SD file at line XXX. | Multiple commands that require the XYZ axes are incorrectly used simultaneously. | 1.Please check the G-code format to see if there are separate G0 or G1 commands<br>2.Check or replace the post-processor. |
| ERROR24 | More than one g-code command that requires axis words found in block. |  |  |
| ERROR25 | Repeated g-code word found in block. Error in SD file at line XXX. | G-code commands are repeated during code writing. | 1.Please check the G-code format and delete duplicate XYZ, F, and S commands.<br>2.Check or replace the post-processor. |
| ERROR25 | Repeated g-code word found in block. |  |  |
| ERROR26 | No axis words found in block for g-code command or current modal state which requires them. Error in SD file at line XXX. | The XYZ axis commands are omitted during code writing, and this issue commonly occurs in arc commands G2 and G3. | 1.Please check the G-code format and supplement the XYZ axis commands.<br>2.Check or replace the post-processor. |
| ERROR26 | No axis words found in block for g-code command or current modal state which requires them. |  |  |
| ERROR27 | Line number value is invalid. | 1.The N line number set during code writing is out of range.<br>2. An error occurred when the program generated the N line number. | 1.Adjust the N line numbers to keep them within the valid range.<br>2.Check or replace the post-processor. |
| ERROR28 | G-code command is missing a required value word. Error in SD file at line XXX. |  | 1.Please check the G-code format and supplement the missing values.<br>2.Check or replace the post-processor. |
| ERROR28 | G-code command is missing a required value word. |  |  |
| ERROR29 | G59.x work coordinate systems are not supported. |  |  |
| ERROR30 | G53 only allowed with G0 and G1 motion modes. Error in SD file at line XXX. |  | 1.Please check the G-code format to ensure that G53 is only used when the current modal state is G0 or G1.<br>2.Check or replace the post-processor. |
| ERROR30 | G53 only allowed with G0 and G1 motion modes. |  |  |
| ERROR31 | Axis words found in block when no command or current modal state uses them. Error in SD file at line XXX. |  | 1.Please check the G-code format to confirm whether there are axis commands after G80.<br>2.Check or replace the post-processor. |
| ERROR31 | Axis words found in block when no command or current modal state uses them. |  |  |
| ERROR32 | G2 and G3 arcs require at least one in-plane axis word. Error in SD file at line XXX. | The XYZ axis parameters are omitted when writing arc commands. | 1.Please check the G-code format and supplement the XYZ axis parameters in the arc commands.<br>2.Check or replace the post-processor. |
| ERROR32 | G2 and G3 arcs require at least one in-plane axis word. |  |  |
| ERROR33 | The motion command has an invalid target. Error in SD file at line XXX. | 1.The G2/G3 arc cannot be generated.<br>2.The probe target coincides with the current position. | 1.Check the arc parameters to ensure an arc can be generated.<br>2.Reset the probe target to avoid coinciding with the current position.<br>3.Check or replace the post-processor. |
| ERROR33 | The motion command has an invalid target. |  |  |
| ERROR34 | A G2 or G3 arc, traced with the radius definition, had a mathematical error when computing the arc geometry. Error in SD file at line XXX. | The radius parameter in the arc is incorrect. | 1.Adjust the radius settings to ensure the calculation is reasonable.<br>2.Check or replace the post-processor. |
| ERROR34 | A G2 or G3 arc, traced with the radius definition, had a mathematical error when computing the arc geometry. |  |  |
| ERROR35 | A G2 or G3 arc, traced with the offset definition, is missing the IJK offset word in the selected plane to trace the arc. Error in SD file at line XXX. | The IJK parameters are omitted when writing arc commands with offset definitions. | 1.Please check the G-code format and supplement the IJK offset parameters.<br>2.Check or replace the post-processor. |
| ERROR35 | A G2 or G3 arc, traced with the offset definition, is missing the IJK offset word in the selected plane to trace the arc. |  |  |
| ERROR36 | There are unused, leftover G-code words that aren't used by any command in the block. Error in SD file at line XXX. | 1.The rapid traverse command G00 contains an extra H parameter.<br>2.The spindle start command M3 contains an extra D parameter.<br>3.The unit setting command G21 contains an extra P parameter.<br>4.The arc interpolation command G02 contains an extra S parameter. | 1.Please check the G-code format and delete redundant G-code parameters.<br>2.Check or replace the post-processor. |
| ERROR36 | There are unused, leftover G-code words that aren't used by any command in the block. |  |  |
| ERROR37 | The G43.1 dynamic tool length offset command cannot apply an offset to an axis other than its configured axis. The Grbl default axis is the Z-axis. |  |  |
| ERROR38 | Tool number greater than max supported value or undefined tool selected. Error in SD file at line XXX. | The entered tool number does not exist or is incorrectly formatted. | 1.Check the entered tool number to ensure it is valid and correctly formatted.<br>2. It is recommended to set the tool number within T0~T8. |
| ERROR38 | Tool number greater than max supported value or undefined tool selected. |  |  |
| ERROR39 | Value out of range. Error in SD file at line XXX. |  |  |
| ERROR39 | Value out of range. |  |  |

### 🔧 Equipment Related Errors (ERROR40-ERROR58)

| Error Code | Error Name | Fault Cause | Solution |
|------------|------------|-------------|----------|
| ERROR40 | G-code command not allowed when tool change is pending. Error in SD file at line XXX. |  |  |
| ERROR40 | G-code command not allowed when tool change is pending. |  |  |
| ERROR41 | Spindle not running when motion commanded in CSS or spindle sync mode. Error in SD file at line XXX. |  |  |
| ERROR41 | Spindle not running when motion commanded in CSS or spindle sync mode. |  |  |
| ERROR42 | Plane must be ZX for threading. Error in SD file at line XXX. |  |  |
| ERROR42 | Plane must be ZX for threading. |  |  |
| ERROR43 | Max. feed rate exceeded. Error in SD file at line XXX. |  |  |
| ERROR43 | Max. feed rate exceeded. |  |  |
| ERROR44 | RPM out of range. Error in SD file at line XXX. |  |  |
| ERROR44 | RPM out of range. |  |  |
| ERROR45 | Only homing is allowed when a limit switch is engaged. |  |  |
| ERROR46 | Home machine to continue. |  |  |
| ERROR47 | ATC: current tool is not set. Set current tool with M61. |  |  |
| ERROR48 | Value word conflict. |  |  |
| ERROR49 | Power on self test failed. A hard reset is required. |  |  |
| ERROR50 | Emergency stop active. |  |  |
| ERROR51 | Motor fault. |  |  |
| ERROR52 | Setting value is out of range. |  |  |
| ERROR53 | Setting is not available, possibly due to limited driver support. |  |  |
| ERROR54 | Retract position is less than drill depth. |  | 1.Please check the G-code format to ensure that the R coordinate is greater than the Z coordinate.<br>2.Check or replace the post-processor. |
| ERROR54 | Retract position is less than drill depth. |  |  |
| ERROR55 | Attempt to home two auto squared axes at the same time. |  |  |
| ERROR56 | Coordinate system is locked. |  |  |
| ERROR57 | Unexpected file demarcation. |  |  |
| ERROR58 | Port is not available |  |  |

### 💾 SD Card Related Errors (ERROR60-ERROR66)

| Error Code | Error Name | Fault Cause | Solution |
|------------|------------|-------------|----------|
| ERROR60 | Status_SDMountError | 1.The SD card has poor contact.<br>2.The SD card is damaged<br>3.The SD card format is not supported<br>4.The firmware cannot recognize and mount the SD card | 1.Please restart the device. If the issue persists, try formatting the SD card.<br>2.If the SD card is damaged, refer to the tutorial for replacing the SD card. |
| ERROR61 | Status_FileReadError | 1.Target file is corrupted.<br>2.The file path is incorrect.<br>3.The SD card connection was interrupted during reading.<br>4.The file content does not conform to the expected format. | 1.Please restart the device and try again.<br>2.If the issue persists, try formatting the SD card.<br>3.If formatting proves ineffective, refer to the tutorial for replacing the SD card. |
| ERROR62 | Status_FsFailedOpenDir | 1.The directory name is incorrect.<br>2.The directory itself is corrupted. | 1.Please restart the device and try again.<br>2.If the issue persists, try formatting the SD card.<br>3.If formatting proves ineffective, refer to the tutorial for replacing the SD card. |
| ERROR63 | Status_FSDirNotFound | 1.The directory path is incorrect.<br>2.The directory was accidentally deleted. | 1.Please restart the device and try again.<br>2.If the issue persists, try formatting the SD card.<br>3.If formatting proves ineffective, refer to the tutorial for replacing the SD card. |
| ERROR64 | Status_SDNotMounted | 1. No SD card is inserted.<br>2.The mounting process was not triggered after the SD card was inserted.<br>3. No remount was performed after a previous mounting attempt failed.<br>4.Any operation on the SD card at this point (such as reading files or listing directories) will trigger this error. | 1.Please restart the device and try again.<br>2.If the issue persists, try formatting the SD card.<br>3.If formatting proves ineffective, refer to the tutorial for replacing the SD card. |
| ERROR65 | Status_FsNotMounted | The file system that the firmware needs to access is not fully mounted, resulting in the inability to perform file/directory operations. | 1.Please restart the device and try again.<br>2.If the issue persists, try formatting the SD card.<br>3.If formatting proves ineffective, refer to the tutorial for replacing the SD card. |
| ERROR66 | Status_FsReadOnly | The file system is corrupted. | 1.Please restart the device and try again.<br>2.If the issue persists, try formatting the SD card.<br>3.If formatting proves ineffective, refer to the tutorial for replacing the SD card. |

### 🔍 Other System Errors (ERROR71-ERROR84, ERROR253)

| Error Code | Error Name | Fault Cause | Solution |
|------------|------------|-------------|----------|
| ERROR71 | Unknown operation found in expression. |  |  |
| ERROR72 | Divide by zero in expression attempted. |  |  |
| ERROR73 | Too large or too small argrument provided. |  |  |
| ERROR74 | Argument is not valid for the operation |  |  |
| ERROR75 | Expression is not valid. |  |  |
| ERROR76 | Either NAN (not a number) or infinity was returned from expression. |  |  |
| ERROR77 | Authentication required. |  |  |
| ERROR78 | Access denied. |  |  |
| ERROR79 | Not allowed while critical event is active. |  |  |
| ERROR80 | Flow statement only allowed in filesystem macro. |  |  |
| ERROR81 | Unknown flow statement. |  |  |
| ERROR82 | Stack overflow while executing flow statement. |  |  |
| ERROR83 | Out of memory while executing flow statement. |  |  |
| ERROR84 | Could not open file. |  |  |
| ERROR253 | User defined error occured. |  |  |

---

## 🛠️ Troubleshooting Guide

### 🔴 Priority Order
1. **ALARM Errors** - Priority handling, affects equipment safety operation
2. **ERROR40-ERROR58** - Equipment related errors
3. **ERROR1-ERROR39** - G-code related errors
4. **ERROR60-ERROR66** - SD card related errors
5. **ERROR71-ERROR84, ERROR253** - Other system errors

### 💡 Common Solutions
- Check equipment status and connections
- Verify G-code format correctness
- Confirm parameter setting ranges
- Restart equipment or re-initialize
- Check hardware sensor status

---

*📝 This document is continuously updated. If you encounter any errors not listed here, please contact technical support.*