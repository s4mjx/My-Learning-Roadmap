#  **Introduction**

USB (Universal Serial Bus) replaced slow, limited serial connections by enabling high-speed data transfer and simultaneous device connectivity. As a technician, understanding USB versions, cable types, and power delivery is essential for troubleshooting performance and connectivity issues.

# **Layered Explanation**

**Basic:**  
A USB cable connects devices like keyboards, mice, and phones to computers for data transfer and power. It replaced the old serial ports (DB9 and DB25), which could only handle one device and transferred data one bit at a time (max 115 Kbps).

**Intermediate:**  
USB ports allow daisy chaining—up to 127 devices per controller—using hubs. The bandwidth is shared among all connected devices. For example, a USB 3.0 port (5 Gbps) divided among five devices gives roughly 1 Gbps each.

**Advanced:**  
Each USB generation increases speed and power. However, higher speeds require shorter, higher-quality cables to prevent signal degradation. USB also delivers power to charge or run devices, which depends on the version and port type.


# **Operational Steps / Procedures**

1. **Identify USB port version** — look for color or label (blue for USB 3.x, “SS” for SuperSpeed).
2. **Check device requirement** — confirm speed and power needs (e.g., SSD needs USB 3.0 or higher).
3. **Choose correct cable** — match port type (A, B, C) and ensure certified cable quality.
4. **Consider cable length** — under 3 m for USB 3.x and later for full performance.
5. **Use powered hubs** — when connecting many devices to prevent power shortages.
6. **Avoid mixing low/high speed** — using a USB 1.1 device in a USB 3.0 hub slows the whole chain.
7. **Verify power delivery** — use PD ports for tablets or large devices to ensure fast charging.


# **Real-World Examples**

1. **Example 1: Flash Drive Transfer**
    
    - Environment: Office desktop with USB 3.0 ports.
    - Action: Plugging a USB 3.0 flash drive into a USB 3.0 port.
    - Outcome: Achieves ~5 Gbps transfer rate (≈625 MB/s).

2. **Example 2: Long Cable Issue**
    
    - Environment: External hard drive using a 20-ft USB 3.0 cable.
    - Action: File transfer slows dramatically.
    - Outcome: Speed drops to ~3 Gbps due to signal loss; replacing with a 9-ft cable restores full speed.


# **Key Points to Memorize**

- **Serial port speed:** 115 Kbps (very slow).
- **USB 1.0:** 1.5 Mbps (Low Speed).
- **USB 1.1:** 12 Mbps (Full Speed).
- **USB 2.0:** 480 Mbps (High Speed).
- **USB 3.1 Gen 1:** 5 Gbps (SuperSpeed).
- **USB 3.1 Gen 2:** 10 Gbps (SuperSpeed Plus).
- **USB 3.2 Gen 2×2:** 20 Gbps.
- **USB 4.0:** 40 Gbps.
- **Max cable lengths:** 3 m (USB 3.x), 5 m (USB 2.0).
- **Power output:** 0.5 A (USB 2.0), 0.9 A (USB 3.0), up to 1.5 A+ for PD ports.


# **On-the-Job Application (Job-Ready)**

**Checklist:**

- Verify correct USB version for required device speed.
- Use short, certified cables (≤3 m for USB 3.x).
- Confirm adequate power delivery for charging.
- Avoid overloading passive hubs; use powered hubs for multiple devices.
- Replace damaged or uncertified cables immediately.

**Symptom → Cause → Fix:**

- **Slow transfer:** Using old USB 2.0 cable → Replace with USB 3.0/3.1 cable.
- **Device not charging:** Port limits at 0.5 A → Use PD-capable or wall charger.
- **Device disconnects randomly:** Cable too long → Shorten to <3 m or use repeater hub.

**Best Practices:**

- Label ports and cables by version.
- Keep firmware/drivers updated for USB controllers.
- Use braided or shielded cables in noisy electrical environments.


# **Exam Tips**

- **Expect version-speed questions:** e.g., “Which USB version supports 10 Gbps?” → _USB 3.1 Gen 2._
- **Trick questions:** “How many devices can connect via USB?” → _127 per controller._
- **Power delivery traps:** USB 2.0 provides only _0.5 A._
- **Mnemonic:** _“1-1-2-3-4 → 1.5 M, 12 M, 480 M, 5 G, 40 G”_ (for version-speed order).
- **Identify labeling:** “SS” = SuperSpeed (USB 3.x).


# **Mini-Quiz**

**Multiple-Choice**

1. USB 2.0 supports which maximum speed?  
    A. 12 Mbps B. 480 Mbps C. 5 Gbps D. 40 Gbps  
    **→ B**
2. The maximum number of devices per USB controller is:  
    A. 64 B. 127 C. 255 D. 512  
    **→ B**
3. USB 3.1 Gen 2×2 can transfer up to:  
    A. 10 Gbps B. 20 Gbps C. 5 Gbps D. 40 Gbps  
    **→ B**

**Short Answer**  
4. What is the max cable length for USB 2.0?  
**→ 5 meters (≈15 feet).**

5. How much power can a USB 3.0 port supply?  
    **→ 900 mA or 0.9 A (≈4.5 W).**


# **Short Glossary**

- **Serial Port:** Legacy interface transmitting one bit at a time (DB9/DB25).
- **Daisy Chain:** Connecting multiple devices in sequence via hubs.
- **Host Controller:** Hardware managing USB connections and bandwidth.
- **SuperSpeed:** Marketing term for USB 3.x speeds (5 Gbps+).
- **PD (Power Delivery):** Standard for higher-wattage USB charging.
- **Bandwidth:** Maximum data rate capacity shared among devices.
- **Resistance:** Electrical opposition in cables causing signal loss.
- **Signal Integrity:** Quality of transmitted data over a cable.
- **Hub:** Device expanding a single USB port into several.
- **Gigabit:** 1 billion bits per second (Gbps), unit for data transfer rate.

USB hubs share one USB “lane” of bandwidth. When you plug devices of different speeds into the same hub, the hub has to slow down communication for compatibility. This can reduce the performance of all devices connected through that hub.

## **Layered Explanation**

# **Basic**

USB hubs act like traffic intersections. If one slow car gets in the lane, every car behind it must slow down.  
A USB 1.1 device is extremely slow (12 Mbps).  
A USB 3.0 device is very fast (5 Gbps).  
If they share the same hub, the hub switches into “slow mode” for compatibility.

# **Intermediate**

USB uses a **shared bus architecture**, meaning that all devices connected to the same USB controller or hub must follow a communication cycle.  
When a low-speed device joins the hub, the hub allocates slower “time slices” for communication. This forces faster devices to wait longer between transfer cycles.

Result:  
Your USB 3.0 device **cannot maintain full 5 Gbps**, even though the port supports it.

# **Advanced**

Older USB speeds (1.1 and 2.0) use **different signaling methods** from USB 3.0+ (SuperSpeed).  
When a slow device is detected:

1. The hub creates a **transaction translator (TT)** to handle old protocols.
2. If the hub has **only one TT**, all devices share the same downgraded signaling cycle.
3. The whole hub behaves like a USB 2.0/1.1 chain until the slow device stops talking.

Most cheap hubs have **one TT**, so everything slows down.  
High-quality hubs have **multi-TT**, which isolates slow devices so faster ones stay fast.


## **Operational Steps / Procedure**

1. Identify the hub speed (USB 2.0, USB 3.0, or USB 3.1).
2. Check if the hub is single-TT or multi-TT (most cheap hubs = single-TT).
3. Look at what you’re plugging in:
    - If ANY device is USB 1.1 in a single-TT hub → entire hub drops to slow timing.
4. Separate slow devices:
    - Use a different port on the computer or a different hub.
5. Keep fast devices (SSD, cameras) on USB 3.x ports alone.


## **Real-World Examples**

# **Example 1: External SSD slows down**

Environment: Laptop USB 3.0 port → cheap 4-port hub → SSD + old USB keyboard.  
Action: Plug in a USB 1.1 keyboard.  
Outcome: SSD drops from 5 Gbps to < 12 Mbps because the hub enters a low-speed cycle.

### **Example 2: Webcam becomes choppy**

Environment: USB 3.0 webcam + USB 1.1 printer on the same hub.  
Action: Printer starts polling (communicating).  
Outcome: Webcam lags because all devices share slow signaling.


## **Key Points to Memorize**

- USB hubs share bandwidth; slow devices reduce performance.
- USB 1.1 = 12 Mbps; USB 3.0 = 5 Gbps.
- Single-TT hubs downgrade all devices to slow cycle timing.
- Multi-TT hubs isolate speeds (keep fast devices fast).
- Always separate legacy devices from high-speed chains.
- Use direct USB 3.0 ports for SSDs, webcams, audio interfaces.
- Cheap hubs = most common cause of USB slowdowns.


## **On-the-Job Application (Job-Ready)**

# **Checklist**

- For storage devices, always use USB 3.x ports directly.
- Avoid mixing old devices (USB 1.1/2.0) on the same hub as fast ones.
- Check hub specifications for “multi-TT.”
- Replace old hubs; they bottleneck modern devices.

# **Symptom → Cause → Fix**

- **Symptom:** SSD speed drops dramatically  
    **Cause:** USB 1.1 or 2.0 device in same hub  
    **Fix:** Move slow device to another port

- **Symptom:** Webcam lag or audio glitches  
    **Cause:** Bandwidth contention on hub  
    **Fix:** Use a dedicated USB 3 port

- **Symptom:** Device disconnects  
    **Cause:** Hub overloaded or slow cycle  
    **Fix:** Use powered, multi-TT hub


## **Exam Tips**

- CompTIA often asks:  
    “What happens when you connect a USB 1.1 device in a USB 3.0 hub?”  
    Correct answer: **The hub slows communication and can reduce effective bandwidth for all devices.*
- Watch for questions about **“transaction translators.”**
- Remember: **single-TT slows everything, multi-TT keeps speeds separated.**


## **Mini-Quiz**

# Multiple Choice

1. What happens in a single-TT hub when a USB 1.1 device is connected?  
    A. Nothing changes  
    B. All devices share slow cycle  
    C. Only USB 1.1 slows  
    D. Only USB 3.0 slows  
    **→ B**

2. USB 1.1 max speed is:  
    A. 1.5 Mbps  
    B. 12 Mbps  
    C. 480 Mbps  
    D. 5 Gbps  
    **→ B**

3. Why do devices slow down?  
    A. USB controllers fail  
    B. Shared communication cycle  
    C. Wrong cable  
    D. USB is outdated  
    **→ B**

# Short Answer

4. What hardware inside a hub handles speed differences?  
    **→ Transaction Translator (TT).**

5. How do you keep fast devices from slowing down?  
    **→ Use a multi-TT hub or separate ports.**


## **Short Glossary**

- **USB 1.1:** Full-speed legacy standard (12 Mbps).
- **USB 3.0:** SuperSpeed, 5 Gbps.
- **Hub:** Device that expands one USB port into many.
- **Transaction Translator:** Chip handling communication between different USB speeds.
- **Single-TT Hub:** One translator; all devices slow down.
- **Multi-TT Hub:** Multiple translators; speeds isolated.



USB ports do two jobs: transfer data and deliver electrical power. Each USB version has a maximum amount of power it can send to a device. This affects charging speed and whether a device works properly.


## **Layered Explanation**

# **Basic**

When you plug in a device, the USB port sends electricity to power it or charge it.  
Different USB versions send different amounts of power:

- USB 2.0 → **0.5 amps**
- USB 3.0 → **0.9 amps**
- USB Power Delivery (PD) ports → **1.5 amps or more**

More amps = faster and stronger charging.

# **Intermediate**

A USB port has a **current limit** (amps).  
Devices like phones or tablets need more current to charge quickly.  
Low-current ports will charge very slowly or not at all.

Examples:

- USB 2.0 (0.5 A) is too weak for modern tablets.
- USB 3.0 (0.9 A) is better, but still slower than a wall charger.
- PD ports (1.5 A to 5 A) are designed for fast charging and even powering laptops.

# **Advanced**

USB Power Delivery (PD) is a negotiated system.  
The device and the port “talk” to decide how much power is safe.  
PD can increase voltage too (5V → 9V → 15V → 20V), allowing up to 100 watts or more.

Example:

- A laptop might negotiate 20V × 3A = **60W**
- A phone might negotiate 9V × 2A = **18W**

USB 2.0 and USB 3.0 **cannot negotiate power**, so they stay at 5V with fixed current limits.


## **Operational Steps / Procedure**

1. Identify the USB port: USB 2.0 (black), USB 3.0 (blue), USB-C (PD capable).
2. Check device power needs (phone, tablet, SSD, laptop).
3. Match device to proper port:
    - Low power: USB 2.0/3.0
    - Charging: Prefer USB 3.0 or PD
    - High power: Use PD or wall charger
4. If charging is slow, move device to PD or higher-amp port.
5. Avoid charging demanding devices through USB hubs.


## **Real-World Examples**

# **Example 1: Slow iPad Charging**

Environment: Plugging an iPad into a USB 2.0 port (0.5 A).  
Outcome: iPad battery increases extremely slowly or not at all.  
Reason: iPad needs at least 1.5 A.  
Fix: Plug into a PD port or wall charger.

# **Example 2: External Hard Drive Disconnects**

Environment: USB-powered HDD connected to USB 2.0 port.  
Outcome: Random disconnections.  
Reason: Drive requires more than 0.5 A to maintain spin.  
Fix: Connect to USB 3.0 or powered hub.


## **Key Points to Memorize**

- USB 2.0 → **0.5 A** (very weak).
- USB 3.0 → **0.9 A** (moderate).
- USB-C PD → **1.5 A to 5 A**, depending on negotiation.
- More current = faster charging.
- Device and port must agree on voltage and current (PD only).
- High-power devices require PD or a wall adapter.
- Weak ports cause slow charging, errors, or disconnects.


## **On-the-Job Application (Job-Ready)**

# **Checklist**

- Always check port type before troubleshooting power issues.
- Use PD ports for phones, tablets, or external drives.
- Use powered USB hubs for multiple devices.
- Replace weak or damaged ports causing brownouts.

# **Symptom → Cause → Fix**

- **Slow phone charging**  
    Cause: USB 2.0 port (0.5 A)  
    Fix: Use PD port or dedicated charger

- **External SSD unstable**  
    Cause: Insufficient power  
    Fix: Connect directly to USB 3.0/PD

- **Laptop won’t charge over USB-C**  
    Cause: Port is USB-C data only, no PD  
    Fix: Use PD-capable USB-C port


## **Exam Tips**

- CompTIA LOVES these numbers:
    - **USB 2.0 = 500 mA**
    - **USB 3.0 = 900 mA**
    - **PD = 1.5 A or higher**

- USB 2.0 and 3.0 deliver fixed 5V; PD can go up to 20V.
- If the question mentions _negotiation_ → the answer is **USB Power Delivery**.


## **Mini-Quiz**

# Multiple Choice

1. How much power does USB 2.0 provide?  
    A. 0.5 A  
    B. 0.9 A  
    C. 1.5 A  
    D. 3 A  
    → **A**

2. USB 3.0 provides:  
    A. 300 mA  
    B. 500 mA  
    C. 900 mA  
    D. 1500 mA  
    → **C**

3. Which port supports negotiated fast charging?  
    A. USB 2.0  
    B. USB 3.0  
    C. USB-C PD  
    D. Serial DB9  
    → **C**

# Short Answer

4. Why does a tablet charge slowly on USB 2.0?  
    → USB 2.0 only gives 0.5 A, which is too weak.

5. What happens when a device needs more current than the port provides?  
    → It charges slowly or disconnects.


## **Short Glossary**

- **Amp (A):** Amount of electrical current.
- **Watt (W):** Power, calculated as volts × amps.
- **PD (Power Delivery):** USB fast-charging standard.
- **Negotiation:** Device and charger agree on safe power levels.
- **USB 2.0/3.0:** Fixed 5V power.
- **USB-C:** Connector type; may or may not include PD.
