# 📋 Software Error Query

> This page organizes all software error information for HiMill D1/D1s equipment to help users quickly locate and resolve equipment fault issues.

---

## 📊 Overview Information

| Error Type | Count | Description |
|-----------|-------|-------------|
| 🚨 **Alarm Errors (ALARM)** | 13 | Equipment hardware or safety-related alarm information |
| ❌ **Error Messages (ERROR)** | 84 | Software command, parameter setting related errors |

---

## 🚨 Alarm Errors (ALARM)

> **Description**: These errors are usually related to equipment hardware status, safety settings, and sensor functions, requiring priority handling.

| Error Code | Error Name | Fault Cause | Solution |
|------------|------------|-------------|----------|
| ALARM | Alarm | - | - |
| ALARM1 | Origin position anomaly or homing failure | 1. Origin sensor malfunction or blocked by debris<br>2. Origin position trigger anomaly<br>3. Internal equipment anomaly<br>4. Origin sensor failure | 1. Clear homing obstacles<br>2. Clear debris from equipment bottom origin position<br>3. Check equipment status<br>4. Check if origin position is damaged |
| ALARM2 | Target position exceeds equipment travel range | Target position exceeds equipment travel range when executing motion commands | Check if G-code or XYZ axis movement trajectory exceeds travel range and correct |
| ALARM3 | Sensor failure or self-test failure | 1. Self-test sensor detection failed<br>2. Sensor failure during motion | 1. Resolve self-test failure<br>2. Correct sensor self-test failure |
| ALARM4 | Probe failure, probe tool forward blocked | 1. Probe tool forward position blocked<br>2. Probe tool damaged | 1. Remove blocking objects<br>2. Check if origin position is damaged |
| ALARM4 | Probe failure, 3D probe tool forward blocked | 1. Probe tool interface not properly connected<br>2. 3D probe damaged<br>3. 3D probe in unreleased state before probing | 1. Check 3D Probe connection<br>2. Check if 3D Probe is damaged<br>3. Confirm 3D Probe status |
| ALARM5 | Probe failure, probe tool detection range failed to reach target | 1. Detection tool range or installation position issue<br>2. Probe tool damaged | 1. Move detection range<br>2. Check if origin position is damaged |
| ALARM5 | Probe failure, 3D probe detection range failed to reach target | 1. Detection tool range or installation position issue<br>2. 3D probe damaged | 1. Move detection range<br>2. Check if 3D Probe is damaged |
| ALARM6 | Equipment homing failure during operation, reset failure | - | - |
| ALARM7 | Probe failure, safety door open or safety door not closed | Safety door not closed during equipment operation | Close safety door or safety door opening |
| ALARM8 | Probe failure, origin position not detected | 1. Origin position sensor failure<br>2. Internal equipment anomaly | 1. Check if origin position is damaged<br>2. Check equipment status<br>3. Try executing homing operation again |
| ALARM9 | Probe failure, no detection object found at set position | 1. Equipment bottom motion command failure<br>2. Origin position sensor failure<br>3. Internal equipment anomaly | 1. Remove upper obstacles<br>2. Check if origin position is damaged<br>3. Check equipment status |
| ALARM10 | Self-test failure already stored | Self-test sensor detection failed | Release self-test button, correct sensor |
| ALARM11 | Execute homing | Current position may be the same as offset | Execute homing operation |
| ALARM12 | Origin position already stored in equipment status, detect again | 1. Origin position sensor failure<br>2. Internal equipment anomaly | 1. Check if origin position is damaged<br>2. Check equipment status<br>3. Try executing homing operation again |
| ALARM13 | Probe hold already stored in equipment status, detect again | - | - |

---

## ❌ Error Messages (ERROR)

> **Description**: These errors mainly involve G-code commands, parameter settings, file operations, etc., requiring checking of program code and parameter configuration.

### 📝 G-code Related Errors (ERROR1-ERROR39)

| Error Code | Error Name | Fault Cause | Solution |
|------------|------------|-------------|----------|
| ERROR1 | Some character values in G-code command not detected as character type | G-code format error, missing characters | Check if G-code format is correct |
| ERROR2 | Numerical format valid digits lack preset values | Numerical format error, missing numerical values | 1. Check numerical format range in G-code<br>2. Check if motion G-code missing numerical values |
| ERROR3 | System unknown '$' not supported | - | - |
| ERROR4 | Received numerical value mismatch received numerical value | G-code input command value mismatch | 1. Check numerical values in G-code<br>2. Check critical or logical processing commands |
| ERROR5 | Probe failure, tool did not complete function | - | - |
| ERROR6 | Equipment communication equipment exists or 2 seconds | - | - |
| ERROR7 | Equipment read failure, auto-execute image parameters not set to default value | - | - |
| ERROR8 | System unknown '$' unknown equipment unknown status executing | - | - |
| ERROR9 | Current G-code not in safe point motion status executing | - | - |
| ERROR10 | Equipment not completed moving to target position | - | - |
| ERROR11 | Check daily file address, data not completed executing | 1. G-code file address incorrect<br>2. File path corrupted<br>3. Used unmatched merge parameters | 1. Check program re-run<br>2. Check file path correctness<br>3. Check merge parameters |
| ERROR12 | Numerical format incorrect or parameters incompatible | - | - |
| ERROR13 | Detected all open, stored equipment stop parameters | - | - |
| ERROR14 | Equipment information unable to read program EEPROM read program name | - | - |
| ERROR15 | Movement target position exceeds equipment travel range | - | - |
| ERROR16 | Jog movement error missing: wrong key, wrong execute G-code | - | - |
| ERROR17 | Equipment mode needs PWM error | - | - |
| ERROR18 | Equipment already stored | - | - |
| ERROR19 | Numerical error | - | - |
| ERROR20 | Detected unsupported base G-code command | 1. Used unsupported G-code command<br>2. Error in G-code command<br>3. Used unmatched merge parameters | 1. Check equipment parameters<br>2. Check file corruption |
| ERROR21 | Two G-code commands in same mode simultaneously | Multiple commands from same mode used simultaneously in storage | 1. Clear, confirm only one command per mode<br>2. Learn program mode various commands<br>3. Check merge parameters |
| ERROR22 | Execute code not completed user not completed | Missing storage command ' when storing G-code | 1. Check G-code, confirm F value<br>2. Check merge parameters |
| ERROR23 | G-code command in storage missing values | Numerical command format error | 1. Check G-code format<br>2. Note command value types<br>3. Check merge parameters |
| ERROR24 | Detected G-code missing XYZ command | Motion simultaneous use requires XYZ axis commands | 1. Check G-code format contains motion commands<br>2. Check merge parameters |
| ERROR25 | Duplicate G-code command in storage | G-code command duplicate during write | 1. Delete duplicate XYZ, F and S commands<br>2. Check merge parameters |
| ERROR26 | Motion command not found in storage | Missing XYZ axis commands during write | 1. Confirm contains motion commands XYZ axis commands<br>2. Check merge parameters |
| ERROR27 | Program line number error | 1. N program line number exceeds range<br>2. Write program N program line number error | 1. Check N program line number range<br>2. Check merge parameters |
| ERROR28 | Missing base values | G-code missing base parameters | 1. Confirm contains missing base parameters<br>2. Check merge parameters |
| ERROR29 | G59.x coordinate system not supported | - | - |
| ERROR30 | G53 coordinate system, cannot use G0 or G1 motion mode | Check G-code format confirm if using G53 when current mode is G0 or G1 | 1. Check G-code format<br>2. Check merge parameters |
| ERROR31 | Storage command, no indication of current mode state using it | Current mode has no motion mode | 1. Confirm add storage command after G80<br>2. Check merge parameters |
| ERROR32 | G2 or G3 command missing selected XYZ arc center | Missing XYZ arc center when writing arc command | 1. Confirm arc command contains XYZ arc center<br>2. Check merge parameters |
| ERROR33 | Motion command target position invalid | 1. G2/G3 arc unable to complete<br>2. Detection target and current position angle | 1. Check arc parameters<br>2. Check detection target angle<br>3. Check merge parameters |
| ERROR34 | Using radius equal to 0 G2/G3 arc and angle execution failure | Radius in arc equal to 0 | 1. Check radius parameters<br>2. Check merge parameters |
| ERROR35 | Using eccentric motion G2/G3 arc missing selected IJK eccentric parameters | Missing IJK eccentric parameters when writing eccentric motion arc command | 1. Include IJK eccentric parameters<br>2. Check merge parameters |
| ERROR36 | No command found in storage using other G-code | 1. Contains undefined H parameters<br>2. Contains undefined D parameters<br>3. Contains undefined P parameters<br>4. Contains undefined S parameters | 1. Delete undefined G-code parameters<br>2. Check merge parameters |
| ERROR37 | G43.1 dynamic tool length offset command offset cannot be applied to equipment (default Z-axis) | - | - |
| ERROR38 | Tool number and length in command exceed supported values or undefined tool | Specified tool number not in range or format error | 1. Check specified tool number<br>2. Check tool parameters T1~T8 |
| ERROR39 | Value exceeds range | - | - |

### 🔧 Equipment Related Errors (ERROR40-ERROR58)

| Error Code | Error Name | Fault Cause | Solution |
|------------|------------|-------------|----------|
| ERROR40 | Tool magazine change parameter execution failure G-code command | - | - |
| ERROR41 | In constant speed, CSS different mode, storage motion parameter undefined | - | - |
| ERROR42 | Equipment processing plane defined as ZX plane | - | - |
| ERROR43 | Equipment speed exceeds range | - | - |
| ERROR44 | Rotation exceeds range | - | - |
| ERROR45 | Origin position beyond return, equipment motion | - | - |
| ERROR46 | Need multiple equipment to continue | - | - |
| ERROR47 | Auto detect ATC or unused front tool, use M61 detect current tool | - | - |