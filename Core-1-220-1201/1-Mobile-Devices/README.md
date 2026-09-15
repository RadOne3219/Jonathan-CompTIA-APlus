ore-1-220-1201/1-Mobile-Devices/1.1-Mobile-Device-Hardware/README.md


# 1.1 Mobile Device Hardware — Final Review

## CompTIA A+ Core 1 — Final Review

This page summarizes the hardware covered by Objective 1.1.

The goal is not simply to memorize components. You should be able to recognize a problem, identify the likely component, and choose an appropriate troubleshooting or replacement approach.

---

# Hardware Covered

| Component                 | Know This                                                     |
| ------------------------- | ------------------------------------------------------------- |
| Battery                   | Types, health, replacement, swelling, charging problems       |
| Keyboard/Keys             | Failure symptoms, connection, replacement                     |
| RAM                       | Capacity, SO-DIMM, soldered vs. replaceable, failure symptoms |
| HDD/SSD                   | HDD vs. SSD, SATA, M.2, NVMe, failure symptoms                |
| Wireless Card             | Wi-Fi/Bluetooth, drivers, replacement                         |
| Physical Privacy/Security | Biometrics, privacy features, NFC                             |
| Wi-Fi Antennas            | Antenna placement, connectors, cables, MIMO                   |
| Camera/Webcam             | Privacy shutter, permissions, drivers, hardware               |
| Microphone                | Input device, permissions, mute, drivers, hardware            |

---

# Troubleshooting Mindset

When troubleshooting mobile device hardware, avoid immediately replacing the component.

Use a logical process:

**Identify → Inspect → Test → Isolate → Repair/Replace → Verify → Document**

### 1. Identify

Determine exactly what the user is experiencing.

Example:

> "The laptop won't connect to Wi-Fi."

This doesn't automatically mean the wireless card has failed.

---

### 2. Inspect

Check for obvious physical problems.

Examples:

* Damaged cables
* Loose connectors
* Broken ports
* Swollen battery
* Damaged display
* Privacy shutter
* Blocked microphone
* Damaged keyboard

---

### 3. Test

Use the operating system and available tools to determine whether the device is being detected.

Examples:

* Device Manager
* Windows Settings
* Camera application
* Sound settings
* Network settings
* Disk Management

---

### 4. Isolate

Determine whether the problem is:

**Hardware → Driver → Operating System → Application → Network → User configuration**

---

### 5. Repair or Replace

Only replace hardware after troubleshooting indicates that replacement is appropriate.

---

### 6. Verify

After repairing or replacing the component:

* Test the original problem.
* Confirm normal operation.
* Verify related functions.

---

### 7. Document

In a corporate IT environment, document:

* Symptoms
* Troubleshooting performed
* Resolution
* Hardware replaced
* Asset information
* User impact

For your environment, this would typically be reflected in the appropriate **ServiceNow** ticket and asset records.

---

# Component Identification Review

## Battery

Remember:

* Provides portable power.
* Battery health can affect runtime.
* Swollen batteries are a safety concern.
* Charging problems don't always mean the battery itself has failed.

### Key Command

```powershell
powercfg /batteryreport
```

---

# Keyboard

Remember:

* Individual keys can fail.
* Entire keyboards can fail.
* Internal connections can become loose.
* Liquid damage can cause keyboard problems.
* External keyboards can help isolate hardware problems.

---

# RAM

Remember:

* RAM is volatile memory.
* RAM is different from storage.
* SO-DIMM is common in laptops.
* Some modern devices have soldered RAM.
* Insufficient RAM and defective RAM are different problems.

### Key Command

```powershell
Get-CimInstance Win32_PhysicalMemory
```

---

# HDD / SSD

Remember:

* HDDs use spinning magnetic disks.
* SSDs use flash memory.
* SATA is an interface.
* M.2 is a physical form factor.
* NVMe is a storage protocol commonly used over PCIe.
* Not every M.2 drive is NVMe.

### Key Commands

```powershell
Get-Disk
```

```powershell
Get-PhysicalDisk
```

---

# Wireless Card

Remember:

* Wireless cards commonly provide Wi-Fi and Bluetooth.
* Drivers can cause connectivity problems.
* A wireless card can be detected even when there are antenna problems.
* External adapters can help isolate hardware problems.

### Key Command

```powershell
Get-NetAdapter
```

---

# Physical Privacy and Security

Remember:

### Biometrics

Biometrics are:

**Something you are**

Examples:

* Fingerprint
* Facial recognition

### NFC

Near Field Communication provides short-range wireless communication.

Common uses include:

* Contactless payments
* Access control
* Device interactions
* Short-range pairing/data exchange

---

# Wi-Fi Antennas

Remember:

* The wireless card and antenna are different components.
* Laptop antennas may be located inside the display assembly.
* Antenna cables connect the wireless card to the antennas.
* Multiple antennas can support MIMO.
* Damaged or disconnected antennas can cause poor wireless performance.

---

# Camera / Webcam

Remember:

* Cameras can be integrated or external.
* Privacy shutters physically block the camera.
* Windows permissions control camera access.
* Device Manager can help identify device/driver problems.
* A camera working in one application but not another often points toward application settings or permissions.

---

# Microphone

Remember:

* Microphones can be integrated or external.
* Multiple microphones can form an array.
* Check mute status first.
* Verify the correct input device.
* Check Windows privacy permissions.
* Test outside the affected application.
* Check drivers before assuming hardware failure.

---

# A+ Troubleshooting Scenarios

## Scenario 1 — Battery

A laptop shuts down shortly after being disconnected from AC power.

Possible causes:

* Battery failure
* Battery degradation
* Charging problem
* Power-management issue

**First steps:**

Check battery health and charging behavior.

---

## Scenario 2 — RAM

A laptop becomes extremely slow when several applications are open.

Possible causes:

* Insufficient RAM
* Excessive background processes
* Storage performance
* Other system issues

**Don't automatically assume RAM has failed.**

---

## Scenario 3 — SSD

A laptop reports that its storage device is missing.

Possible causes:

* Drive failure
* Connection problem
* BIOS/UEFI configuration
* Storage controller issue

**Determine whether the drive is detected before replacing it.**

---

## Scenario 4 — Wi-Fi

A laptop has poor wireless performance while other devices work normally.

Possible causes:

* Wireless driver
* Wireless card
* Antenna
* Antenna cable
* Local interference

**Isolate the laptop from the network itself as the source of the problem.**

---

## Scenario 5 — Camera

The camera works in Windows Camera but not Teams.

Most likely areas:

* Teams configuration
* Camera selection
* Permissions
* Application issue

---

## Scenario 6 — Microphone

The user can hear everyone but nobody can hear them.

Investigate:

1. Mute status
2. Input device
3. Windows permissions
4. Application settings
5. Driver
6. Hardware

---

# Replacement Decision

Before replacing hardware, ask:

### Is the device detected?

If **no**:

Investigate:

* Connection
* Driver
* BIOS/UEFI
* Hardware

### Is the device detected but malfunctioning?

Investigate:

* Configuration
* Driver
* Software
* Hardware

### Does it work on another system?

If **yes**:

The original computer's configuration, drivers, ports, or operating system may be the problem.

If **no**:

Hardware failure becomes more likely.

---

# Exam Strategy

When CompTIA gives you a hardware troubleshooting scenario:

### Don't jump to the most expensive answer.

Look for the answer that:

1. Checks the simplest cause.
2. Is least invasive.
3. Confirms the failure.
4. Is appropriate for the symptoms.

For example:

> User's webcam isn't working.

Don't immediately choose:

**Replace the motherboard.**

First consider:

**Privacy shutter → permissions → selected camera → application → driver → hardware**

---

# 1.1 Master Checklist

Before marking Objective 1.1 complete, make sure you can explain:

* [ ] Battery types and troubleshooting
* [ ] Battery replacement considerations
* [ ] Keyboard and key failures
* [ ] Keyboard replacement
* [ ] Laptop RAM
* [ ] RAM troubleshooting
* [ ] HDD vs. SSD
* [ ] SATA vs. NVMe
* [ ] M.2 form factor
* [ ] Storage troubleshooting
* [ ] Wireless cards
* [ ] Wi-Fi/Bluetooth troubleshooting
* [ ] Biometrics
* [ ] NFC
* [ ] Physical privacy features
* [ ] Wi-Fi antennas
* [ ] Antenna connectors
* [ ] Camera/webcam troubleshooting
* [ ] Camera privacy shutters
* [ ] Microphone troubleshooting
* [ ] Microphone permissions
* [ ] Hardware replacement decisions

---

# 1.1 Completion Standard

You are ready to move forward when you can do three things:

### 1. Identify

Look at a scenario and identify the likely component.

### 2. Troubleshoot

Explain what you would check first, second, and third.

### 3. Explain

Explain **why** you selected that troubleshooting step.

That third skill is especially important.

Don't just memorize:

> "Check Device Manager."

Understand **why**:

> Device Manager can help determine whether Windows detects the hardware and whether a device or driver problem exists.

---

# Final 1.1 Takeaway

Mobile-device hardware troubleshooting is about **isolating the failure**.

Think:

**Physical → Detection → Configuration → Driver → Application → Hardware**

And remember:

> **Test before you replace.**
