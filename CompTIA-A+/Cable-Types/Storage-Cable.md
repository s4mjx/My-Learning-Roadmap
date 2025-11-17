# Storage Cables — Mental Model (OBJ 3.4)

## What Storage Cables Really Do

Storage cables move data between the drive (HDD/SSD/optical) and the system.  
Different cables = different speeds, connectors, and use cases.  
Modern systems mainly use SATA internally and USB/Thunderbolt externally.  
Enterprise systems use SAS. SCSI is legacy.


## Core Mental Map

# Thunderbolt

- Versions 1–2 use DisplayPort connector.
- Versions 3–4 use **USB-C connector**.
- Thunderbolt 4 = **40 Gbps**, fully compatible with USB-C/USB4.
- A Thunderbolt device will not fully work on a regular USB-C port unless the port supports Thunderbolt.
- Short cables (usually 0.5 m).

**Think:** “USB-C shape, Thunderbolt speed.”


# Lightning (Apple)

- Reversible connector.
- Only on older iPhones/iPads/AirPods.
- Data + charging.
- One end Lightning, the other USB-A or USB-C.

**Think:** “Apple’s old connector before USB-C.”


# SATA (Internal Drives)

- Standard for HDDs, SATA SSDs, and internal optical drives.
- Requires **two cables**:
    - 7-pin data
    - 15-pin power
- Revisions:
    - SATA I: 1.5 Gbps
    - SATA II: 3 Gbps
    - SATA III: 6 Gbps
- Real speed depends on the drive, not the cable (HDDs bottleneck long before 6 Gbps).

**Think:** “L-shaped connector, separate power + data.”


# eSATA (External SATA)

- External version of SATA.
- Data only (no power).
- Was fast before USB 3.0 existed.
- Today largely obsolete because USB 3.2 and Thunderbolt are much faster.

**Think:** “Old external SATA before fast USB.”


# SCSI (Legacy)

- Parallel, old, bulky connectors.
- Narrow: 7 devices
- Wide: 15 devices
- Max speed: 320 Mbps
- Power uses separate Molex or combined 80-pin SCA connector.
- Still found in very old servers.

**Think:** “Old server tech—slow, parallel, gone.”


# SAS (Enterprise)

- Modern serial successor to SCSI.
- Up to **24 Gbps**, full duplex.
- Supports up to **128 devices per controller**.
- Enterprise reliability (redundancy, dual-port drives).
- Backward compatible with SATA drives.

**Think:** “Enterprise storage—fast, reliable, scalable.”


## When Each Type Is Used Today

- **Home/Office Internal** → SATA
- **Home External** → USB 3.x, USB4, Thunderbolt
- **Mac/High-End** → Thunderbolt 3/4
- **Enterprise Servers** → SAS
- **Legacy Companies** → SCSI (rare)
- **Old Apple Devices** → Lightning


## Shortcuts

- USB-C ≠ Thunderbolt. Same shape, different speed.
- SATA always = **data + power separate**.
- Thunderbolt 4 = **40 Gbps**, full USB4 compatibility.
- SCSI = **dead tech**, SAS = **living version**.
- SAS accepts SATA; SATA does **not** accept SAS.
