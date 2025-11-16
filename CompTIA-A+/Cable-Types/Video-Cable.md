# Video Cables

## Introduction  
Video cables connect computers and devices to displays such as monitors, TVs, and projectors. Each cable type supports different resolutions, refresh rates, speeds, and signal types. Understanding them is essential for choosing the right cable and troubleshooting display issues.


# Mental Model  
- HDMI = universal digital video/audio standard.
<img width="400" height="300" alt="image" src="https://github.com/user-attachments/assets/08a5c552-548a-48b4-b576-dba09374702e" />

- DisplayPort = PC/gaming/professional standard with higher refresh rates.
<img width="400" height="300" alt="image" src="https://github.com/user-attachments/assets/a7c48879-06d2-4a8e-8c3c-dabba3b090c8" />
  
- DVI and VGA = legacy interfaces.
<img width="400" height="300" alt="image" src="https://github.com/user-attachments/assets/884f5fa5-a19a-487f-b2b8-925e7d1fcfe7" />
  
- Thunderbolt and USB-C = can transmit video using DisplayPort technology internally.
<img width="400" height="300" alt="image" src="https://github.com/user-attachments/assets/d992305b-53e2-4586-a4e1-f618de02821d" />
 
- Newer cables = more bandwidth → higher resolution → higher refresh rate.


# HDMI

## Overview  
HDMI is a digital interface for video + audio. Supports 1080p up to 8K and includes HDCP for content protection.

## Connector Types  
- **Type A** – Standard full-size  
- **Type C** – Mini HDMI
<img width="400" height="300" alt="image" src="https://github.com/user-attachments/assets/e8a45e76-c12b-4cf3-80cd-e9f4ba64caa0" />

- **Type D** – Micro HDMI
<img width="400" height="300" alt="image" src="https://github.com/user-attachments/assets/af307456-da69-478f-817e-334da659dec5" />
  

## Cable Categories  
- **Standard HDMI** → up to 1080p  
- **High-Speed HDMI** → 4K / 8K  

## Versions  
- **HDMI 2.0** → 18 Gbps (4K 60 Hz)  
- **HDMI 2.1** → 48 Gbps (4K 120 Hz / 8K 60 Hz)

## Notes  
HDMI fits only one direction. Used in TVs, consoles, laptops, desktops.


# DisplayPort (DP)

## Overview  
DisplayPort is a VESA-designed digital interface used mainly on PCs and professional monitors.

## Key Features  
- Full-size DisplayPort includes a **locking latch**  
- Mini DisplayPort used on older Macs/laptops  
- Supports 4K/8K + high refresh rates  
- **DP 2.0** reaches up to **80 Gbps**  
- Supports **daisy chaining** (MST – Multi-Stream Transport)


# DVI

## Overview  
Mixed digital/analog interface from the late 1990s.

## Types  
- **DVI-A** → Analog only  
- **DVI-D** → Digital only  
- **DVI-I** → Digital + Analog  

## Notes  
Uses pin connectors. No audio. Seen mainly on older GPUs and projectors.


# VGA

## Overview  
Legacy fully analog 15-pin interface.

## Key Notes  
- Prone to interference  
- Bent pins = color issues  
- Considered legacy technology


# Thunderbolt

## Overview  
High-speed interface that carries video, data, and power.

## Versions  
- **Thunderbolt 1/2** → Mini DisplayPort connector
<img width="400" height="300" alt="image" src="https://github.com/user-attachments/assets/91f020cb-c960-42cd-a437-59985d5cc7da" />

- **Thunderbolt 3/4** → USB-C connector (40 Gbps)
<img width="400" height="300" alt="image" src="https://github.com/user-attachments/assets/942ac698-0192-4d50-a729-25ac4ff3f05a" />


## Key Notes  
- Supports 4K/8K displays  
- Fully compatible with USB-C devices  
- Can daisy chain  
- Rule: **Thunderbolt ports accept USB-C → USB-C ports do NOT always accept Thunderbolt**


# USB-C (DisplayPort Alt Mode)

## Overview  
Reversible connector that can transmit video if the port supports **DisplayPort Alternate Mode**.

## Key Notes  
- Sends video, data, and power  
- Supports 4K/8K depending on hardware  
- Common in modern laptops  
- Not all USB-C ports output video


# Comparison Table

| Cable Type | Signal | Max Resolution | Audio | Reversible | Status |
|-----------|--------|----------------|--------|------------|--------|
| HDMI | Digital | 1080p–8K | Yes | No | Current |
| DisplayPort | Digital | 1440p–8K | Yes | No | Current/Pro |
| DVI | Digital/Analog | Up to 1080p | No | No | Legacy |
| VGA | Analog | 480p–1080p | No | No | Legacy |
| Thunderbolt 3/4 | Digital | 4K–8K | Yes | Yes | Current |
| USB-C Alt Mode | Digital | 4K–8K | Yes | Yes | Current |


# Key Points to Memorize  
- HDMI Types: A, C, D  
- HDMI Categories: Standard (1080p), High-Speed (4K/8K)  
- HDMI 2.1 = 48 Gbps  
- DisplayPort has a locking connector  
- DisplayPort supports daisy chaining  
- DVI-I = digital + analog  
- VGA = analog, 15 pins  
- Thunderbolt 3/4 = USB-C @ 40 Gbps  
- USB-C video requires **DisplayPort Alt Mode**
<img width="400" height="300" alt="image" src="https://github.com/user-attachments/assets/f41bb6f9-08e2-4717-991f-d33d22bde850" />
 
- Not all USB-C ports output video


# Think About this

- Modern systems → HDMI or DisplayPort  
- Gaming + high refresh → DisplayPort preferred  
- Laptops → USB-C Alt Mode or Thunderbolt  
- Old systems → DVI or VGA  
- 4K/8K → check bandwidth (HDMI 2.0/2.1, DP 1.4/2.0)  
- Streaming error → possible HDCP issue  
