# Mobile Device Batteries

## CompTIA A+ Core 1 — Objective 1.1

Understanding batteries is important because mobile devices depend on portable power and battery problems are common IT support issues.

---

## 1. Battery Types

Modern mobile devices primarily use **lithium-ion (Li-ion)** or **lithium-polymer (Li-Po)** batteries.

### Lithium-Ion (Li-ion)

Common characteristics:

* High energy density
* Rechargeable
* Common in laptops and mobile devices
* Gradually loses capacity over time
* Can be damaged by excessive heat or physical damage

### Lithium-Polymer (Li-Po)

Common characteristics:

* Rechargeable
* Lightweight
* Can be manufactured in thin or flexible shapes
* Common in smartphones, tablets, and thin laptops

---

## 2. Removable vs. Non-Removable Batteries

### Removable Battery

A removable battery can be physically removed and replaced by the user or technician.

Advantages:

* Easy replacement
* Can carry a spare battery
* Useful for field workers
* Allows quick battery replacement

### Non-Removable Battery

A non-removable battery is installed inside the device.

Replacement generally requires:

* Opening the device
* Disconnecting the battery
* Removing adhesive or mounting hardware
* Installing the replacement
* Reassembling the device

Many modern laptops, tablets, and smartphones use non-removable batteries.

---

# 3. Battery Health

Battery capacity decreases as a battery ages.

A battery may still report:

**100% charged**

while no longer being capable of holding the same amount of energy it could when new.

### Common signs of degraded battery health

* Shorter battery life
* Rapid percentage drops
* Unexpected shutdowns
* Device shutting down before reaching 0%
* Longer charging times
* Battery overheating

---

# 4. Battery Swelling

A swollen battery occurs when gases build up inside the battery.

This can cause:

* Bulging case
* Raised trackpad
* Keyboard lifting
* Screen separation
* Device chassis distortion

### ⚠️ Safety

A swollen lithium battery should be treated as a **hardware safety issue**.

Do **not**:

* Puncture the battery
* Bend the battery
* Crush the battery
* Continue using a severely swollen battery
* Attempt to force the battery back into position

Follow your organization's approved battery handling and disposal procedures.

---

# 5. Battery Troubleshooting

When a user reports a battery problem, start by identifying the symptoms.

### Problem

**"My laptop dies very quickly."**

Check:

1. Battery health
2. Battery age
3. Power settings
4. Applications consuming excessive power
5. Screen brightness
6. Background processes
7. Charging behavior
8. Whether the battery is physically damaged

---

## 6. Laptop Battery Health in Windows

Windows can generate a battery report.

Open **Command Prompt** or **PowerShell** and run:

```powershell
powercfg /batteryreport
```

Windows will generate a battery report that can provide information such as:

* Design capacity
* Full charge capacity
* Battery usage
* Battery history
* Estimated battery life

### Example

Suppose a laptop has:

**Design Capacity:** 60,000 mWh

**Full Charge Capacity:** 42,000 mWh

The battery is holding significantly less charge than when new.

A rough capacity percentage can be calculated as:

**42,000 ÷ 60,000 × 100 = 70%**

This doesn't automatically mean the battery must be replaced. Always consider the manufacturer's specifications and your organization's replacement standards.

---

# 7. AC Adapter vs. Battery Problems

A laptop that will not power on could have several possible causes.

Possible causes include:

* Dead battery
* Failed AC adapter
* Damaged charging port
* Faulty power cable
* Motherboard failure
* Power management issue

### Troubleshooting approach

Try:

1. Verify the AC adapter is connected.
2. Check whether the charging indicator is active.
3. Test with a known-good compatible charger if available.
4. Inspect the charging port.
5. Check battery status in Windows.
6. Review battery health information.
7. Determine whether the laptop operates correctly while connected to AC power.

---

# 8. ITAM Scenario

### Scenario

A user submits a ServiceNow ticket:

> "My laptop only stays on for about 30 minutes after I unplug it."

Before replacing the laptop, investigate.

### Questions to ask

* How old is the laptop?
* Has the battery life changed recently?
* Does the laptop work normally while plugged in?
* Is the battery physically swollen?
* Is the charger functioning?
* What does the Windows battery report show?

### Possible outcome

If the laptop itself is functioning normally but the battery has significantly degraded, a **battery replacement** may be more appropriate than replacing the entire device.

This saves:

* Money
* Time
* Hardware
* Deployment resources

---

# 9. SysAdmin Connection

Battery troubleshooting is useful for systems administrators because administrators may manage large numbers of laptops.

PowerShell can be used to collect information from devices and automate administrative tasks.

For example, you could eventually create scripts that help identify:

* Battery health
* Device model
* Serial number
* Operating system
* Hardware information

This is where **CompTIA A+ knowledge connects directly to PowerShell and systems administration.**

---

# Key Terms

| Term                 | Meaning                                                 |
| -------------------- | ------------------------------------------------------- |
| Li-ion               | Lithium-ion rechargeable battery                        |
| Li-Po                | Lithium-polymer rechargeable battery                    |
| Design Capacity      | Original rated battery capacity                         |
| Full Charge Capacity | Maximum capacity the battery currently holds            |
| Battery Health       | General condition/capacity of a battery                 |
| Battery Swelling     | Physical expansion caused by internal battery failure   |
| AC Adapter           | Provides external power to the device                   |
| mWh                  | Milliwatt-hour, a unit used to measure battery capacity |

---

# A+ Exam Tip

Remember the difference between:

**Design Capacity**

and

**Full Charge Capacity**

A healthy battery should have a full charge capacity relatively close to its design capacity.

A significantly lower full charge capacity indicates battery degradation.

---

# Quick Check

### Question 1

A laptop's battery is physically swollen. What should you do?

**Answer:** Treat it as a safety issue and follow the organization's approved battery handling/replacement procedure. Do not puncture, bend, or continue using a severely swollen battery.

### Question 2

What command can generate a Windows battery report?

**Answer:**

```powershell
powercfg /batteryreport
```

### Question 3

What is the difference between design capacity and full charge capacity?

**Answer:** Design capacity is the battery's original rated capacity. Full charge capacity is the amount of charge the battery can currently hold.

### Question 4

A laptop works perfectly when connected to AC power but shuts down shortly after being unplugged. What component should you investigate first?

**Answer:** The battery and its health/capacity.

---

## Study Checklist

* [ ] Understand Li-ion batteries
* [ ] Understand Li-Po batteries
* [ ] Understand removable batteries
* [ ] Understand non-removable batteries
* [ ] Recognize battery degradation
* [ ] Recognize battery swelling
* [ ] Understand battery safety
* [ ] Know `powercfg /batteryreport`
* [ ] Understand design capacity
* [ ] Understand full charge capacity
* [ ] Practice troubleshooting battery issues
* [ ] Understand when battery replacement is appropriate

**Status:** 🟡 Learning
