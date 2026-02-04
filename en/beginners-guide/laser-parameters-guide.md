# Laser Processing Parameters Guide

This document provides a detailed introduction to the core parameters in laser processing, helping beginners systematically understand the definition, impact, and application scenarios of each parameter. By mastering the adjustment rules of these parameters, you can quickly get started with laser equipment and achieve ideal processing results.

## 📊 Core Parameters Overview

The effect of laser processing is determined by multiple parameters, among which power, speed, focal length, wavelength, and pulse frequency are the five most critical parameters. These parameters interact and work together, requiring reasonable matching based on specific materials and processing needs.

## 1. Power

### Definition

⚡ **What is Power?**

The amount of laser energy output by the laser equipment per unit time, which directly reflects the "strength" of the equipment, measured in watts (W). Desktop equipment power typically ranges from 10W to 100W, and specific wattages (such as 20W, 50W) can be directly selected in the equipment software during parameter adjustment.

### 🔥 Impact and Application

Power is the core parameter that determines processing depth, speed, and energy density, with a positive correlation among the three. Excessively high power can cause material burning and deformation, while insufficient power results in substandard processing effects.

- **Processing Depth**: The higher the power, the stronger the laser energy, and the deeper the material is melted/vaporized (e.g., 50W can engrave 3mm acrylic, while 20W can only engrave 1mm)
- **Processing Speed**: For the same material, higher power allows for faster processing speeds (more strength means faster movement while still achieving processing)
- **Energy Density**: Higher power results in higher energy per unit area after laser focusing, making it easier to cut through/engrave deeper materials; conversely, energy disperses, resulting in weaker processing effects

### 📱 Desktop Product Adaptation

Desktop models mainly use small/medium power, no high power, precisely matched by purpose:

| Power Range | Application Scenario | Processing Capability |
|------------|---------------------|----------------------|
| 10W-30W    | Shallow Marking     | Metal/plastic LOGO, QR codes, text, small amount of shallow engraving on thin soft non-metals |
| 30W-60W    | General Purpose     | Regular engraving + thin material cutting (acrylic ≤3mm, wood board ≤2mm, thin metal sheet ≤0.5mm) |
| 60W-100W   | Desktop High Power  | Slightly thicker non-metals (acrylic ≤5mm, wood board ≤4mm), some can cut thin stainless steel sheets ≤1mm |

<img src="/eng/beginners-guide/media/laser-parameters-guide/功率影响示意图2.png" alt="Impact of Power on Processing Effects" style="width: 75%; height: auto; border-radius: 10px;" />

## 2. Speed

### Definition

⚡ **What is Speed?**

The moving speed of the laser head (or processing worktable), i.e., the scanning speed of the laser beam on the material surface, measured in millimeters per second (mm/s). Desktop equipment speed adjustment range is mostly between 0-500mm/s, which is one of the parameters that beginners don't know how to start with.

### ⚡ Impact and Application

Speed determines processing efficiency and quality, and must be coordinated with power (adjusting a single parameter will definitely cause problems):

- **Processing Time**: Faster speed means shorter time for the laser to complete the entire processing path, higher efficiency; slower speed means longer processing time, lower efficiency
- **Processing Quality**: Too fast speed → laser stays at a single point on the material for too short a time, insufficient energy, resulting in incomplete cutting, shallow engraving, or blurred patterns; too slow speed → laser stays at a single point for too long, energy accumulation, resulting in material burning, blackened edges, or deformation
- **Power Coordination**: Power and speed are "golden partners"—higher power allows for appropriate speed increase (more strength, can move faster while still achieving processing), lower power requires speed reduction (less strength, need to move slower to ensure sufficient energy)

### 📱 Desktop Product Adaptation

Desktop models determine speed by processing type, not exceeding equipment limits, general adaptation range:

| Processing Type | Recommended Speed Range | Application Scenario |
|----------------|-------------------------|---------------------|
| Laser Marking  | 200-500mm/s             | Quick marking, no deep processing required |
| Shallow Engraving | 100-300mm/s            | Paper, thin leather, metal surfaces |
| Deep Engraving | 30-100mm/s              | Materials requiring depth such as acrylic, wood boards |
| Thin Material Cutting | 50-200mm/s           | Thicker materials require lower speeds |

<img src="/eng/beginners-guide/media/laser-parameters-guide/速度影响示意图2.png" alt="Impact of Speed on Processing Effects" style="width: 75%; height: auto; border-radius: 10px;" />

## 3. Focal Length

### Definition

🎯 **What is Focal Length?**

The optimal vertical distance at which the laser equipment's focusing lens converges the laser beam into the smallest spot (simply put: the "standard distance" from the focusing lens to the material surface), measured in millimeters (mm). Focal length is a fixed property of the focusing lens, cannot be manually adjusted, and can only be aligned with the material surface by raising/lowering the worktable/laser head. Common focal lengths for desktop focusing lenses are 50mm, 63.5mm, and 100mm.

### 🔍 Impact and Application

Focal length determines laser spot size, energy density, processing precision, and processing range, and has different sensitivities to "defocus error" (the distance the material surface deviates from the optimal focal length):

- **Short Focal Length (e.g., 50mm)**: Produces smaller spots, higher energy density, extremely high processing precision, but smaller processing range and extremely sensitive to defocus error (material surface slightly higher/lower by 1-2mm, spot becomes larger, energy disperses, processing effect drops sharply)
- **Long Focal Length (e.g., 100mm)**: Produces slightly larger spots, slightly lower energy density, slightly reduced processing precision, but larger processing range and less sensitive to defocus error (slight height variations on material surface have little effect on spot and energy)
- **Medium Focal Length (e.g., 63.5mm)**: Balances precision, energy, and processing range, is the "universal model" for desktop use, suitable for most processing scenarios

### 📱 Desktop Product Adaptation

| Focal Length | Application Scenario | Features |
|-------------|---------------------|----------|
| 50mm        | Fine Processing     | Metal small character marking, micro pattern engraving, narrow gap thin material cutting, high precision required scenarios |
| 63.5mm      | General Purpose     | Can do marking, engraving, and thin cutting, beginner's first choice, no need to frequently replace focusing lenses |
| 100mm       | Large Area Processing | Whole board acrylic/wood engraving, batch processing of large-size workpieces, precision meets daily needs |

<img src="/eng/beginners-guide/media/laser-parameters-guide/焦距对比示意图.png" alt="Comparison of Different Focal Length Effects" style="width:75%; height: auto; border-radius: 10px;" />

## 4. Wavelength

### Definition

🌈 **What is Wavelength?**

The exclusive physical characteristic of laser, which is the "frequency identifier" of the laser beam, measured in nanometers (nm). Wavelength is determined by the core component of the laser equipment (laser), and cannot be manually adjusted (wavelength is fixed when selecting equipment, and remains fixed during processing). Common wavelengths for desktop use are 450nm (blue light), 1064nm (fiber), and 10600nm (CO₂, i.e., 10.6μm).

### 🌈 Impact and Application

The core function of wavelength is to determine material absorption characteristics (whether the material can "absorb" laser energy), while also having clear safety restrictions, making it the core basis for equipment selection:

- **Material Absorption Characteristics**: Laser energy can only achieve processing when absorbed by the material. Different materials are only "sensitive" to specific wavelengths:
  - Non-metals (wood, plastic, acrylic, leather) have extremely high absorption efficiency for 10600nm (CO₂)
  - Metals (steel, aluminum, copper) have high absorption efficiency for 1064nm (fiber), 450nm (blue light)
  - 450nm (blue light) can balance part of thin non-metals and metals, making it the "all-round wavelength"

- **Safety Restrictions**:
  - 10600nm (CO₂) laser is invisible to the naked eye, easy to cause burns if touched by mistake, need to take proper protection during operation
  - 450nm (blue light), 1064nm (fiber) laser is visible to the naked eye, can intuitively see the optical path, safer for beginners to operate

### 📱 Desktop Product Adaptation

| Wavelength | Suitable Materials | Features |
|------------|-------------------|----------|
| 450nm (Blue Light) | Thin non-metals + all metals | Desktop "all-round model", suitable for beginners, small equipment size, low power consumption |
| 1064nm (Fiber) | Metals | Metal processing special, focused on metal marking/thin cutting, poor non-metal processing effect |
| 10600nm (CO₂) | Non-metals | Non-metal processing main force, focused on non-metal engraving/cutting (depth and efficiency are much higher than blue light), cannot process metals |

<img src="/eng/beginners-guide/media/laser-parameters-guide/波长吸收特性2.png" alt="Material Absorption Characteristics of Different Wavelengths" style="width: 75%; height: auto; border-radius: 10px;" />

## 5. Pulse Frequency

### Definition

🔄 **What is Pulse Frequency?**

Only for pulse laser equipment (desktop mainstream, different from continuous laser), refers to the number of times the laser emits laser beams per second, measured in hertz (Hz). It can be manually adjusted in the equipment software, and the desktop adjustment range is mostly between 0-500kHz. Continuous laser equipment does not have this parameter.

### 🔄 Impact and Application

Pulse frequency determines the energy distribution, fineness, and heat-affected zone (the area around the material affected by laser heating) of the laser:

- **Energy Control**: Higher frequency → more emissions per second → greater total laser energy → deeper processing depth, higher efficiency; lower frequency → fewer emissions → smaller total energy → shallower processing depth, but more concentrated energy at single points
- **Heat-Affected Zone**: Lower frequency → longer interval between laser emissions → material has time to dissipate heat → smaller heat-affected zone (material not easy to deform, edges not blackened); higher frequency → shorter emission interval → heat accumulation → larger heat-affected zone, suitable for batch processing with low precision requirements

### 📱 Desktop Product Adaptation

| Frequency Range | Application Scenario | Features |
|----------------|---------------------|----------|
| Low Frequency (20kHz-100kHz) | Fine Processing     | Metal small character/pattern marking, micro engraving, thin material narrow gap cutting, small heat-affected zone, smooth edges |
| Medium Frequency (100kHz-300kHz) | Regular Processing | Most marking, engraving, thin cutting, balancing efficiency and fineness, desktop general gear |
| High Frequency (300kHz-500kHz) | Fast Batch Processing | Large area simple patterns, thin material fast cutting, high efficiency, suitable for scenarios with low fineness requirements |

<img src="/eng/beginners-guide/media/laser-parameters-guide/脉冲频率影响2.png" alt="Impact of Pulse Frequency on Processing Effects" style="width: 75%; height: auto; border-radius: 10px;" />

## 6. Parameter Coordination and Optimization Strategy

⚙️ **How Do Parameters Work Together?**

Laser processing has no "universal parameters"—even if a single parameter is adjusted perfectly, it cannot guarantee ideal results. The core is the coordination of the three adjustable parameters: power, speed, and frequency, combined with fixed focal length and wavelength.

### 🔄 Power-Speed-Frequency Triangle Relationship

The three are the "core adjustment group" for processing, with each change affecting the others. The adjustment logic is as follows:

1. **Set Power**: Determine basic power based on material thickness/processing depth (select high power for thick materials/deep engraving, low power for thin materials/shallow marking)
2. **Match Speed**: Higher power allows for speed increase, lower power requires speed reduction, avoiding "high power slow speed burning" and "low power fast speed insufficient processing"
3. **Adjust Frequency**: Select low frequency for fine processing (small heat-affected zone), high frequency for batch processing (high efficiency), and medium frequency for regular processing. Frequency should be adjusted synchronously with speed (increase frequency for fast speed to ensure sufficient energy; decrease frequency for slow speed to avoid heat accumulation)

### 🧪 Material Testing Process (Must Do for Beginners)

Different materials and different thicknesses of the same material have different parameters. Be sure to test samples before processing finished products:

1. Take material samples (same material and thickness as finished products, 5cm×5cm is sufficient)
2. Fix focal length and wavelength (these two are fixed equipment properties, no need to adjust)
3. Set basic parameters according to "medium power + medium speed + medium frequency" (desktop recommended 30W+100mm/s+200kHz)
4. Test process on the sample with basic parameters, observe the effect:
   - Incomplete cutting/shallow engraving → increase power/decrease speed/increase frequency (choose one, beginners prioritize increasing power)
   - Burning/deformation → decrease power/increase speed/decrease frequency (choose one, beginners prioritize decreasing power)
   - Low precision/rough edges → decrease frequency/change to short focal length (beginners prioritize decreasing frequency)
5. Fine-tune 1-2 times repeatedly until the sample effect is satisfactory, save the parameters, and directly apply them to finished product processing

## 📋 Laser Parameters Reference

> ⚠️ **Important Note**:
> 
> - There is no universal parameter standard for laser processing, each device has its unique parameter characteristics
> - Different materials, thicknesses, and processing requirements will affect the final parameter selection
> - Beginners are advised to use scrap materials for trial and error, and gradually master parameter adjustment rules after accumulating experience
> - The following is the laser parameter reference table for our Maxmake devices, for reference only, actual use still needs to be adjusted according to specific conditions
> 
> {.is-info}

- **Maxmake Laser Parameters Reference Table**: [View Detailed Parameters](/en/laser-parameters.md)

## Summary

The core of laser processing parameters is not "how high/low to adjust", but "matching"—precisely matching parameters with materials and processing needs. For desktop beginners, remember the following core points:

1. **Fixed parameters do not need adjustment**: Wavelength (determined when selecting equipment), focal length (selected according to processing precision, beginners use 63.5mm general model)
2. **Core parameters determined by needs**: Power determines depth, speed determines efficiency, frequency determines fineness
3. **Adjustment sequence matters**: First set power, then match speed, finally fine-tune frequency, do not adjust a single parameter alone
4. **Must do for beginners**: Test samples first, then process finished products, make good use of the equipment software's preset parameter library

Laser parameter adjustment is not complicated. Beginners can use scrap materials for trial and error, then try different materials later, summarize the rules of "what materials match what parameters", and gradually achieve "one glance to determine parameters". The core is to practice more, test more, don't be afraid to adjust incorrectly, and the cost of sample trial and error is extremely low.

---

*📝 This document is continuously updated. If you have any suggestions or questions, please contact us.*