# Storage Cables — Mental Model (OBJ 3.4)

## Overview
Storage cables move data between drives (HDDs, SSDs, optical) and the motherboard.  
Different cable types offer different connectors, speeds, and use cases.  
Modern systems rely on SATA (internal), USB/Thunderbolt (external), and SAS (enterprise).  
Legacy systems used SCSI.


## Thunderbolt

**Key Ideas**
- TB1–TB2 use DisplayPort connectors.  
- TB3–TB4 use **USB-C connectors**.  
- **Thunderbolt 4 = 40 Gbps**.  
- USB-C shape doesn’t guarantee Thunderbolt speed.  
- Thunderbolt devices require Thunderbolt support on the port.

```text
Thunderbolt 4
Connector: USB-C
Speed: 40 Gbps
Compatibility: Fully compatible with USB-C & USB4

Lightning (Apple)
Reversible: Yes
Platform: Apple-only
Use Case: Charging + Data (older devices)

SATA
Data: 7-pin
Power: 15-pin
Rev 3 Speed: 6 Gbps
Used For: HDDs, SATA SSDs, DVD/Blu-ray drives

eSATA
Power: No
Speed: Up to 6 Gbps
Status: Largely obsolete

SCSI
Type: Parallel (legacy)
Max Speed: 320 Mbps
Devices: 7 (narrow), 15 (wide)
Status: Legacy hardware only

SAS
Speed: Up to 24 Gbps
Compatibility: Supports SATA drives
Use Case: Enterprise servers
Scalability: Up to 128 devices

## Modern Use Cases
Internal Consumer PCs  → SATA
External Home Storage  → USB 3.x / USB4 / Thunderbolt
Mac & Creator Devices  → Thunderbolt 3/4
Enterprise Servers     → SAS
Legacy Systems         → SCSI
Old Apple Devices      → Lightning

## Shortcuts:
- USB-C shape ≠ Thunderbolt protocol.
- SATA always requires separate power and data cables.
- Thunderbolt 4 = 40 Gbps and full USB4 compatibility.
- SAS accepts SATA drives, but SATA does NOT accept SAS.
- SCSI is legacy; SAS is modern.
