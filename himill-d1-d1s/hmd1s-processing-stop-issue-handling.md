# ⚠️ Processing Stop Due to Issues Handling Guide

> This page provides handling methods and solutions for HiMill D1/D1s equipment when processing stops due to various issues during processing.

---

## ⚠️ Important Notice

> **Attention**:
> - First troubleshoot the problem; if it's not a hardware issue, you can proceed with the following operations
> - After power off, origin information will be retained, but tool compensation information will be reset to zero
> - In most cases when processing stops, the tool is not broken, so after clicking tool change, there's no need to actually change the tool; just press the button to let the tool complete auto height measurement
> {.is-warning}

---

## 🔍 Processing Stop Handling Methods

<table>
<tr>
<th>No.</th>
<th>Code Form</th>
<th>Equipment Status</th>
<th>Operation</th>
</tr>
<tr>
<td rowspan="2">1</td>
<td rowspan="2">Only one tool processing, no tool change code<br><br>Example:<br><br>M3 S13000<br>(Processing)<br>M5<br>M30</td>
<td>Power Off</td>
<td>Restart equipment, after homing, re-import file and start processing.</td>
</tr>
<tr>
<td>Power On</td>
<td>After homing, re-import file and start processing.</td>
</tr>
<tr>
<td rowspan="2">2</td>
<td rowspan="2">Only one tool processing, but with tool change code T1M6<br><br>Example:<br><br>M5<br>T1 M6<br>M3 S13000<br>(Processing)<br>M5<br>M30</td>
<td>Power Off</td>
<td>1. Restart equipment, after homing, click the tool change button in software, after auto height measurement, reset Z0, then start processing<br><br>2. Also can modify NC file, delete T1M6 code. Import modified file and can start processing directly.</td>
</tr>
<tr>
<td>Power On</td>
<td>After homing, re-import file and start processing.</td>
</tr>
<tr>
<td rowspan="2">3</td>
<td rowspan="2">Multiple tools processing, and first tool stops during processing<br><br>Example:<br><br>M5<br>T1 M6<br>M3 S13000<br>(Processing)<br>T2 M6<br>(Processing)<br>T3 M6<br>...<br>M5<br>M30</td>
<td>Power Off</td>
<td>Restart equipment, after homing, click the tool change button in software, after auto height measurement, reset Z0, then start processing</td>
</tr>
<tr>
<td>Power On</td>
<td>After homing, re-import file and start processing.</td>
</tr>
<tr>
<td rowspan="2">4</td>
<td rowspan="2">Multiple tools processing, and tool X stops during processing<br><br>Example:<br><br>M5<br>T1 M6<br>M3 S13000<br>(Processing)<br>T2 M6<br>(Processing)<br>TX M6<br>(Processing)<br>T8 M6<br>(Processing)<br>M5<br>M30</td>
<td>Power Off</td>
<td>Open NC file with computer, delete all code before TXM6 (keep TXM6 and all subsequent code)<br><br>After homing, import modified code, click tool change button in software, after auto height measurement, reset Z0, then start processing</td>
</tr>
<tr>
<td>Power On</td>
<td>Open NC file with computer, delete all code before TXM6 (keep TXM6 and all subsequent code)<br><br>After homing, import modified code, can start processing directly</td>
</tr>
</table>

---

## 💡 Important Reminders

- **Tool Breakage Judgment**: In most cases when processing stops, the tool is not broken, avoid unnecessary tool change operations
- **Auto Height Measurement**: After tool change, no actual tool replacement is needed, just complete the auto height measurement process
- **Origin Retention**: After equipment power off, origin information is retained, which can reduce the need to reset XY0, but please operate Z0 setting according to the actual situation in the table
- **File Backup**: It is recommended to backup the original file before modifying NC files