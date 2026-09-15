# Wireless Cards

## CompTIA A+ Core 1 — Objective 1.1

Wireless cards allow computers and mobile devices to communicate with wireless networks and other devices.

For the A+ exam, you should understand wireless card functionality, common hardware configurations, symptoms of failure, and basic replacement and troubleshooting techniques.

---

# 1. What Is a Wireless Card?

A wireless network adapter allows a device to connect to wireless networks.

Common wireless technologies include:

* Wi-Fi
* Bluetooth

A wireless card may be:

* Internal
* Replaceable
* Integrated into the motherboard
* Soldered

---

# 2. Wi-Fi

Wi-Fi allows a device to connect to a wireless local area network (WLAN).

A laptop's Wi-Fi adapter communicates with a wireless access point or wireless router.

Typical connection path:

**Laptop → Wi-Fi Adapter → Wireless Access Point → Network**

---

# 3. Bluetooth

Bluetooth is a short-range wireless technology commonly used to connect devices such as:

* Keyboards
* Mice
* Headsets
* Speakers
* Smartphones
* Other peripherals

Bluetooth is generally intended for shorter-range device-to-device communication rather than connecting a computer to a traditional LAN.

---

# 4. Internal Wireless Cards

Many laptops have an internal wireless adapter.

The adapter may be installed:

* On a removable M.2 module
* Directly on the motherboard
* As part of another integrated component

### Important

Do not assume a wireless card is replaceable.

Always check the device's:

* Service manual
* Hardware specifications
* Manufacturer documentation

---

# 5. Wireless Antennas

A wireless card requires antennas to transmit and receive wireless signals.

Laptop antennas are often routed through the display assembly.

A simplified configuration may look like:

**Wireless Card**

↓

**Antenna Cable**

↓

**Display Antenna**

This allows the antenna to be positioned away from other internal components and provides better wireless reception.

---

# 6. Antenna Connectors

Wireless cards commonly use very small antenna connectors.

The antenna cables must be properly connected to the wireless card.

A loose or disconnected antenna can cause:

* Weak Wi-Fi
* Poor range
* Intermittent connectivity
* Slow wireless performance
* Difficulty connecting to distant access points

### Important

A laptop can sometimes still detect Wi-Fi networks with an antenna problem.

Therefore:

**"I can see Wi-Fi" does not automatically mean the antenna is functioning correctly.**

---

# 7. Wireless Card Failure Symptoms

Possible symptoms include:

* Wi-Fi adapter missing
* Wi-Fi option unavailable
* Bluetooth unavailable
* Wireless networks not detected
* Frequent disconnections
* Weak signal
* Poor wireless performance
* Adapter disappearing from Device Manager
* Error codes in Device Manager

---

# 8. Device Manager

In Windows, wireless hardware can be inspected using **Device Manager**.

Open:

**Start → Device Manager**

Look under:

**Network adapters**

You may see an entry representing the wireless adapter.

Examples of information may include:

* Manufacturer
* Adapter model
* Driver
* Status
* Device errors

---

# 9. Device Manager Error

If Windows reports a problem with the wireless adapter, check the device's status.

Possible causes include:

* Driver problem
* Disabled adapter
* Hardware failure
* Incorrect driver
* Device configuration issue

### Troubleshooting

Try:

1. Verify Wi-Fi is enabled.
2. Check Airplane Mode.
3. Open Device Manager.
4. Check the wireless adapter status.
5. Check for driver errors.
6. Restart the computer.
7. Install the appropriate manufacturer driver if necessary.
8. Test with a known-good wireless adapter when appropriate.

---

# 10. Driver Problems vs. Hardware Problems

A missing or non-functioning wireless adapter does not automatically mean the hardware has failed.

### Possible software causes

* Missing driver
* Incorrect driver
* Corrupted driver
* Adapter disabled
* Windows configuration problem
* Network configuration problem

### Possible hardware causes

* Failed wireless card
* Damaged antenna
* Loose antenna connection
* Physical damage
* Motherboard problem

---

# 11. Testing With an External Adapter

A USB Wi-Fi adapter can be useful for troubleshooting.

### Example

A laptop's internal Wi-Fi adapter isn't functioning.

Connect a known-good USB Wi-Fi adapter.

If the USB adapter works:

**Network hardware/software is capable of functioning → investigate the internal wireless adapter.**

This doesn't prove the internal adapter is physically defective, but it helps isolate the problem.

---

# 12. Wi-Fi Signal Strength

Wireless signal strength can be affected by:

* Distance
* Walls
* Building materials
* Interference
* Antenna placement
* Wireless adapter
* Access point
* Network congestion

### Important

Weak Wi-Fi does not automatically mean the wireless card is defective.

Always determine whether other nearby devices experience the same problem.

---

# 13. Is It the Laptop or the Network?

This is an important troubleshooting question.

### One laptop has poor Wi-Fi

Possible causes:

* Laptop wireless card
* Laptop antenna
* Driver
* Configuration
* Physical damage

### Multiple devices have poor Wi-Fi

Possible causes:

* Access point
* Network infrastructure
* Wireless interference
* Internet connection
* Network configuration

### Troubleshooting Principle

**Compare the affected device with a known-good device.**

This is one of the simplest ways to isolate a problem.

---

# 14. Power Management

Windows may use power-management settings that affect wireless hardware.

A laptop may disable or reduce certain hardware functions to conserve battery power.

When troubleshooting intermittent wireless problems, check:

* Power settings
* Adapter properties
* Device Manager
* Manufacturer power-management software

---

# 15. Bluetooth Troubleshooting

Bluetooth problems can appear similar to wireless card problems.

Check:

1. Is Bluetooth enabled?
2. Is Airplane Mode disabled?
3. Is the device discoverable?
4. Is the peripheral powered on?
5. Is the device already paired with another computer?
6. Is the Bluetooth driver functioning?
7. Can another Bluetooth device connect?

---

# 16. Wireless Card Replacement

If the wireless card is replaceable and has been determined to be defective:

1. Shut down the computer.
2. Disconnect AC power.
3. Follow the manufacturer's service documentation.
4. Use appropriate ESD precautions.
5. Remove the required access panel.
6. Disconnect the antenna cables carefully.
7. Remove the wireless card.
8. Install the compatible replacement.
9. Reconnect the antenna cables.
10. Reassemble the device.
11. Install the appropriate driver if necessary.
12. Test Wi-Fi and Bluetooth.

---

# 17. Antenna Cable Identification

Wireless cards may have multiple antenna connections.

The cables may be labeled or color-coded by the manufacturer.

### Important

Follow the manufacturer's documentation when reconnecting antenna cables.

Incorrect routing or connection can result in:

* Poor signal
* Reduced range
* Intermittent connectivity
* Physical damage to connectors

---

# 18. ITAM Scenario

### Scenario

A user submits a ServiceNow ticket:

> "My laptop barely gets Wi-Fi in the conference room, but everyone else's laptop works fine."

Before replacing the laptop:

### Investigate

1. Compare the affected laptop with a known-good laptop.
2. Check wireless signal strength.
3. Check Device Manager.
4. Verify the wireless driver.
5. Test another location.
6. Check the antenna connection if appropriate.
7. Test with a known-good external Wi-Fi adapter.

### Possible Cause

If other laptops work normally in the same location, the issue is more likely isolated to the affected device.

Potential causes include:

* Wireless driver
* Wireless card
* Antenna
* Configuration

---

# 19. SysAdmin Connection

Wireless adapters are important in enterprise environments.

Systems administrators may manage:

* Wireless drivers
* Device configurations
* Wi-Fi profiles
* Endpoint policies
* Network troubleshooting
* Device hardware standards

This becomes especially relevant when managing large numbers of Windows devices through enterprise management platforms.

---

# 20. PowerShell Connection

PowerShell can be used to gather network adapter information.

For example:

```powershell id="i9q42m"
Get-NetAdapter
```

This can display network adapters and their status.

You can also use:

```powershell id="q5d6zi"
Get-NetAdapter | Format-Table Name, InterfaceDescription, Status, LinkSpeed
```

This can help identify:

* Adapter name
* Hardware description
* Connection status
* Link speed

---

# A+ Exam Tips

Remember:

### Wireless card

Provides wireless connectivity.

### Antenna

Transmits and receives the wireless signal.

### Driver

Allows the operating system to communicate with the hardware.

### Weak signal

Could be:

* Antenna
* Wireless card
* Distance
* Interference
* Access point
* Environment

### Multiple devices affected

Think:

**Network infrastructure**

### One device affected

Think:

**Device hardware, driver, or configuration**

---

# Quick Check

### Question 1

What hardware allows a laptop to connect to Wi-Fi?

**Answer:** A wireless network adapter/card.

### Question 2

What component helps transmit and receive the wireless signal?

**Answer:** The antenna.

### Question 3

A laptop cannot connect to Wi-Fi, but a USB Wi-Fi adapter works correctly. What should you investigate?

**Answer:** The internal wireless adapter, its driver, configuration, or antenna.

### Question 4

Several users lose Wi-Fi at the same time. Should you immediately replace their wireless cards?

**Answer:** No. Investigate the wireless network infrastructure first.

### Question 5

What PowerShell command displays network adapters?

**Answer:**

```powershell id="0r9g8b"
Get-NetAdapter
```

---

# Study Checklist

* [ ] Understand wireless network adapters
* [ ] Understand Wi-Fi
* [ ] Understand Bluetooth
* [ ] Understand internal wireless cards
* [ ] Understand wireless antennas
* [ ] Understand antenna connectors
* [ ] Recognize wireless card failure symptoms
* [ ] Use Device Manager to inspect wireless hardware
* [ ] Understand driver vs. hardware problems
* [ ] Understand external adapter troubleshooting
* [ ] Understand Wi-Fi signal problems
* [ ] Know how to isolate device vs. network problems
* [ ] Understand Bluetooth troubleshooting
* [ ] Understand wireless card replacement
* [ ] Know `Get-NetAdapter`
* [ ] Practice wireless troubleshooting scenarios

**Status:** 🟡 Learning
