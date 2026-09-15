# Keyboard and Keys

## CompTIA A+ Core 1 — Objective 1.1

Keyboards are a common input device on laptops, tablets with detachable keyboards, and other mobile computing devices.

A technician should be able to identify keyboard problems, determine whether they are hardware or software related, and perform appropriate replacement or troubleshooting procedures.

---

## 1. Types of Mobile Device Keyboards

Mobile devices can use several types of keyboards.

### Built-in Keyboard

A traditional laptop keyboard is physically integrated into the laptop chassis.

Examples include:

* Dell Latitude
* Dell Pro
* Lenovo ThinkPad
* HP business laptops

### Detachable Keyboard

Some tablets use a keyboard that can be physically attached and removed.

The connection may use:

* Proprietary connectors
* Magnetic connectors
* Bluetooth
* USB

### External Keyboard

An external keyboard can connect through:

* USB
* Bluetooth
* Wireless receiver

External keyboards can be useful for troubleshooting.

---

# 2. Common Keyboard Problems

A keyboard problem can affect:

* One key
* Several keys
* An entire keyboard
* Intermittent key presses
* Special function keys
* Backlighting

Common symptoms include:

* Key does not register
* Key gets stuck
* Multiple keys stop working
* Keys type incorrect characters
* Keyboard randomly stops responding
* Keyboard disconnects
* Liquid damage
* Physical damage

---

# 3. Single Key Failure

If only one key is not working, the problem may be localized to that key.

Possible causes:

* Dirt or debris
* Damaged keycap
* Damaged key mechanism
* Liquid damage
* Internal keyboard damage

### Troubleshooting

Try:

1. Test the key in multiple applications.
2. Check whether the key is physically damaged.
3. Inspect for debris.
4. Test an external keyboard.
5. Determine whether the problem follows the operating system or the physical keyboard.

---

# 4. Multiple Keys Not Working

When several keys stop working at the same time, consider a larger hardware or connection problem.

Possible causes:

* Keyboard cable disconnected
* Keyboard cable damaged
* Liquid damage
* Keyboard failure
* Motherboard connection problem
* Driver or operating system issue

### Troubleshooting

Check:

1. Does the keyboard work in the BIOS/UEFI?
2. Does an external keyboard work?
3. Does the problem occur before Windows loads?
4. Is the internal keyboard cable properly connected?
5. Is there visible physical or liquid damage?

---

# 5. Keyboard Cable

Many laptop keyboards connect to the motherboard using a **ribbon cable**.

The cable may use a small locking connector.

When servicing the keyboard:

* Power the device off.
* Disconnect external power.
* Follow the manufacturer's service procedure.
* Carefully release the connector.
* Avoid damaging the ribbon cable.
* Properly secure the connector during reassembly.

### Important

Ribbon cables are delicate and can be easily damaged.

---

# 6. Liquid Damage

Liquid is one of the most common causes of laptop keyboard failure.

Possible symptoms:

* Sticky keys
* Keys not registering
* Multiple keys failing
* Random input
* Corrosion
* Device failure

Liquid damage can extend beyond the keyboard and affect:

* Motherboard
* Touchpad
* Battery
* Storage
* Other internal components

### ITAM Consideration

Document liquid damage carefully.

Depending on company policy and warranty coverage, the device may require:

* Keyboard replacement
* Complete device replacement
* Manufacturer repair
* Damage assessment

---

# 7. Keyboard Layout

Different keyboards can have different layouts.

Examples:

* US English
* UK English
* International layouts
* Specialized layouts

If a user reports that keys produce the wrong characters, the problem may not be hardware.

Check:

* Windows keyboard layout
* Language settings
* Input method
* Physical keyboard layout

### Example

A user presses:

**"**

but receives:

**@**

The physical keyboard may be using a different regional layout.

---

# 8. Function Keys

Laptop keyboards commonly include function keys such as:

* F1
* F2
* F3
* F4
* F5
* F6
* F7
* F8
* F9
* F10
* F11
* F12

They may also provide hardware controls such as:

* Volume
* Brightness
* Screen projection
* Keyboard backlight
* Wireless connectivity
* Microphone mute

These functions may require the correct keyboard or system drivers.

---

# 9. Keyboard Backlight

Many business laptops include keyboard backlighting.

If the keys work but the backlight does not:

Possible causes include:

* Backlight disabled
* Keyboard shortcut
* System configuration
* Driver/firmware issue
* Hardware failure

Before replacing the keyboard, verify that the backlight hasn't simply been disabled.

---

# 10. External Keyboard Troubleshooting

An external keyboard can be an excellent diagnostic tool.

### Example

A laptop's built-in keyboard isn't working.

Connect a known-good USB keyboard.

If the external keyboard works:

**Operating system is probably functional → investigate the internal keyboard.**

If neither keyboard works:

**Investigate software, USB, motherboard, or broader system issues.**

This helps isolate the problem.

---

# 11. BIOS/UEFI Testing

Testing the keyboard before Windows loads can help determine whether the problem is hardware or software.

If the keyboard works in BIOS/UEFI but fails inside Windows:

Possible causes include:

* Driver problem
* Operating system configuration
* Accessibility settings
* Software conflict

If the keyboard does not work in BIOS/UEFI:

A hardware problem becomes more likely.

---

# 12. Keyboard Replacement

If the keyboard has failed and is replaceable, the technician may need to:

1. Shut down the device.
2. Disconnect AC power.
3. Follow the manufacturer's service manual.
4. Remove the required panels/components.
5. Disconnect the keyboard cable.
6. Remove the keyboard.
7. Install the replacement.
8. Reconnect the cable.
9. Reassemble the device.
10. Test every key.

### Always Test After Replacement

Test:

* Alphabetic keys
* Numbers
* Function keys
* Modifier keys
* Arrow keys
* Enter
* Backspace
* Spacebar
* Keyboard shortcuts
* Backlight if applicable

---

# Real-World ITAM Scenario

### Scenario

A user submits a ServiceNow ticket:

> "Several keys on my Dell laptop aren't working."

Before ordering a replacement keyboard:

### Step 1 — Gather Information

Ask:

* Which keys are affected?
* Did the problem start suddenly?
* Was anything spilled on the laptop?
* Was the device dropped?
* Does an external keyboard work?
* Does the keyboard work before Windows loads?

### Step 2 — Isolate the Problem

Determine whether the issue is:

**Hardware → Software → Configuration → Physical Damage**

### Step 3 — Determine Resolution

Possible resolutions:

* Clean the keyboard
* Correct keyboard layout
* Resolve a software issue
* Reseat the keyboard cable
* Replace the keyboard
* Replace the entire device

---

# SysAdmin Connection

Keyboard troubleshooting teaches an important systems administration principle:

> **Isolate the failure before changing the hardware.**

The same methodology applies to:

* Network adapters
* Storage
* Memory
* Displays
* Docking stations
* Printers
* USB devices
* Wireless devices

---

# A+ Exam Tips

### Remember:

**One key fails**

→ Investigate the key itself.

**Multiple keys fail**

→ Investigate the keyboard, cable, liquid damage, or system.

**Keyboard works in BIOS but not Windows**

→ Software/configuration becomes more likely.

**Keyboard fails everywhere**

→ Hardware becomes more likely.

**External keyboard works**

→ Investigate the internal keyboard.

---

# Quick Check

### Question 1

A laptop's built-in keyboard does not work, but a USB keyboard works normally. What should you investigate?

**Answer:** The internal keyboard, its cable/connection, or the keyboard hardware.

### Question 2

A keyboard works in BIOS but stops working once Windows starts. What should you investigate?

**Answer:** Windows drivers, configuration, accessibility settings, or software conflicts.

### Question 3

Several keys stopped working immediately after a drink was spilled on the laptop. What is the likely cause?

**Answer:** Liquid damage.

### Question 4

What component commonly connects a laptop keyboard to the motherboard?

**Answer:** A ribbon cable.

---

# Study Checklist

* [ ] Understand built-in keyboards
* [ ] Understand detachable keyboards
* [ ] Understand external keyboards
* [ ] Identify common keyboard failures
* [ ] Understand ribbon cables
* [ ] Recognize liquid damage
* [ ] Understand keyboard layouts
* [ ] Understand function keys
* [ ] Understand keyboard backlighting
* [ ] Use an external keyboard for troubleshooting
* [ ] Understand BIOS/UEFI keyboard testing
* [ ] Understand keyboard replacement
* [ ] Practice keyboard troubleshooting scenarios

**Status:** 🟡 Learning
