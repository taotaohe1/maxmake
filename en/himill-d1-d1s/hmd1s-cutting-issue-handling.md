# 🔧 Broken Tool Handling Guide

> This page provides handling methods and solutions for HiMill D1/D1s equipment when encountering tool breakage during processing.

---

## ⚠️ Important Notice

> **Attention**:
> - After tool breakage, stop the equipment operation immediately and remove the broken tool shank
> - After power off, origin information will be retained, but tool compensation information will be reset to zero
> {.is-warning}

---

## 🔍 Tool Breakage Handling Methods

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
<td>Restart equipment, after homing, pull down the handle and directly replace the tool, reset Z0, and start processing.</td>
</tr>
<tr>
<td>Power On</td>
<td>After homing, replace the tool, pull down the handle and directly replace the tool, reset Z0, and start processing.</td>
</tr>
<tr>
<td rowspan="2">2</td>
<td rowspan="2">Only one tool processing, but with tool change code T1M6<br><br>Example:<br><br>M5<br>T1 M6<br>M3 S13000<br>(Processing)<br>M5<br>M30</td>
<td>Power Off</td>
<td>Restart equipment, after homing, click the tool change button in software, replace tool and auto-measure height, reset Z0, then start processing</td>
</tr>
<tr>
<td>Power On</td>
<td>After homing, click the tool change button in software, replace tool and auto-measure height, can start processing directly</td>
</tr>
<tr>
<td rowspan="2">3</td>
<td rowspan="2">Multiple tools processing, and first tool breaks<br><br>Example:<br><br>M5<br>T1 M6<br>(Processing)<br>T2 M6<br>(Processing)<br>T3 M6<br>(Processing)<br>M5<br>M30</td>
<td>Power Off</td>
<td>Restart equipment, after homing, click the tool change button in software, replace tool and auto-measure height, reset Z0, then start processing</td>
</tr>
<tr>
<td>Power On</td>
<td>After homing, click the tool change button in software, replace tool and auto-measure height, can start processing directly</td>
</tr>
<tr>
<td rowspan="2">4</td>
<td rowspan="2">Multiple tools processing, and tool X breaks during processing<br><br>Example:<br><br>M5<br>T1 M6<br>(Processing)<br>T2 M6<br>(Processing)<br>TX M6<br>(Processing)<br>T8 M6<br>(Processing)<br>M5<br>M30</td>
<td>Power Off</td>
<td>Open NC file with computer, delete all code before TXM6 (keep TXM6 and all subsequent code)<br><br>After homing, import modified code, click tool change button in software, replace tool and auto-measure height, reset Z0, then start processing</td>
</tr>
<tr>
<td>Power On</td>
<td>Open NC file with computer, delete all code before TXM6 (keep TXM6 and all subsequent code)<br><br>After homing, import modified code, click tool change button in software, replace tool and auto-measure height, can start processing directly</td>
</tr>
</table>

---

## 💡 Preventive Measures

- Regularly check tool wear conditions
- Select appropriate cutting parameters
- Ensure tool installation is firm
- Monitor abnormal conditions during processing