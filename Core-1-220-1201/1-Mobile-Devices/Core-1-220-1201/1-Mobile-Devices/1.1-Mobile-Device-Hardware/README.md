# 1.1 Mobile Device Hardware

> **CompTIA A+ Core 1 — 220-1201**

## Objective

Given a scenario, monitor mobile device hardware and use appropriate replacement techniques.

---

## What You Need to Know

For this objective, you should understand the major replaceable components found in mobile devices and recognize common hardware failures.

### Battery

Understand:

* Removable vs. non-removable batteries
* Battery health and capacity
* Battery swelling
* Battery replacement
* Proper battery handling
* Symptoms of battery failure
* Power-related troubleshooting

**Common symptoms:**

* Device shuts down unexpectedly
* Battery drains rapidly
* Device will not hold a charge
* Device becomes unusually hot
* Battery is physically swollen

> ⚠️ A swollen lithium-ion battery is a safety issue. Do not puncture, bend, or continue using a severely swollen battery.

---

## Keyboard and Keys

Mobile devices may use:

* Physical keyboards
* Detachable keyboards
* Laptop-style keyboards
* Individual key mechanisms

Common failures include:

* Missing keys
* Stuck keys
* Keys not registering
* Liquid damage
* Damaged keyboard connectors

### Troubleshooting

Check:

1. Is the keyboard physically damaged?
2. Does the problem affect one key or multiple keys?
3. Does an external keyboard work?
4. Is the keyboard properly connected?
5. Does the problem occur in multiple applications?

---

## RAM

Some mobile devices have removable or replaceable RAM, while many modern devices have memory soldered directly to the motherboard.

Possible symptoms of memory problems include:

* Application crashes
* System instability
* Failure to boot
* Random restarts
* Poor performance

### Important

Always verify whether the specific device supports RAM replacement before attempting a repair.

---

## HDD / SSD

Mobile computers may use:

* 2.5-inch SATA drives
* M.2 SATA SSDs
* M.2 NVMe SSDs
* Proprietary storage solutions
* Soldered storage

Common storage symptoms:

* Slow performance
* Operating system errors
* Boot failures
* Missing files
* Drive not detected

### Replacement Considerations

Before replacing a storage device:

* Verify compatibility
* Back up user data
* Determine whether encryption is enabled
* Verify the replacement drive type
* Determine how the operating system will be restored

---

## Wireless Cards

Wireless cards provide connectivity such as:

* Wi-Fi
* Bluetooth

Depending on the device, the wireless card may be:

* Replaceable
* Integrated into the motherboard
* Soldered

Common symptoms of wireless card problems:

* Wi-Fi unavailable
* Bluetooth unavailable
* Intermittent connectivity
* Weak wireless signal
* Device cannot detect wireless networks

---

## Physical Privacy and Security Components

Modern mobile devices may include hardware designed for authentication and privacy.

### Biometrics

Examples include:

* Fingerprint readers
* Facial recognition
* Other biometric authentication systems

Biometric hardware can be used for:

* Device authentication
* Application authentication
* Secure access

### Near-Field Scanner Features

Near-field technologies allow devices to interact with nearby compatible devices or objects.

Examples include:

* NFC
* Contactless authentication
* Mobile payments
* Access cards

---

## Wi-Fi Antenna

The Wi-Fi antenna allows the wireless adapter to communicate with wireless networks.

Important considerations:

* Antenna placement
* Antenna connectors
* Antenna cables
* Physical damage
* Signal interference

### Symptoms of Antenna Problems

A damaged or disconnected antenna can cause:

* Weak Wi-Fi signal
* Reduced range
* Intermittent connectivity
* Poor wireless performance

---

## Camera / Webcam

Mobile devices commonly include:

* Front-facing cameras
* Rear-facing cameras
* Integrated webcams

Common problems:

* Camera not detected
* Poor image quality
* Camera application crashes
* Privacy settings blocking access
* Physical lens damage

### Troubleshooting

Check:

1. Camera permissions
2. Device privacy settings
3. Application permissions
4. Device Manager on Windows systems
5. Physical damage
6. Whether another application is using the camera

---

## Microphone

Microphones are commonly used for:

* Voice calls
* Video conferencing
* Voice commands
* Recording

Common symptoms:

* Other people cannot hear the user
* Recording contains no audio
* Audio is distorted
* Microphone works in one application but not another

### Troubleshooting

Check:

1. Microphone permissions
2. Default input device
3. Application settings
4. Physical obstruction
5. External microphones/headsets
6. Device drivers when applicable

---

# Real-World ITAM Connection

Mobile hardware troubleshooting is directly relevant to IT asset management.

When a user reports a hardware problem, you may need to determine whether the issue is:

**User issue → Configuration issue → Software issue → Hardware issue → Replacement**

For example:

> User reports that their laptop Wi-Fi is extremely weak.

Possible causes:

* Incorrect Wi-Fi settings
* Driver problem
* Wireless card failure
* Damaged antenna
* Physical damage
* Network issue

The goal is to identify the cause before replacing hardware.

---

# SysAdmin Connection

Understanding mobile hardware also helps with systems administration because administrators frequently support:

* Laptops
* Mobile computers
* Wireless connectivity
* Docking stations
* Cameras
* Microphones
* Authentication hardware
* Remote workers

A strong SysAdmin doesn't immediately replace hardware.

They first determine:

**What is failing?**

**Why is it failing?**

**Can it be repaired?**

**Should the device be replaced?**

---

# Hands-On Labs

Future labs for this section will include:

* Identify laptop hardware
* Identify replaceable components
* Check Windows battery health
* Identify Wi-Fi hardware
* Troubleshoot a webcam
* Troubleshoot a microphone
* Diagnose weak Wi-Fi signal
* Determine whether a device needs repair or replacement
* Document hardware replacement in a ticket

---

# Troubleshooting Scenarios

### Scenario 1 — Rapid Battery Drain

A user's laptop battery drops from 100% to 30% within an hour.

Determine:

* Is the battery defective?
* Is an application consuming excessive power?
* Is the device overheating?
* Is the battery health degraded?

---

### Scenario 2 — Weak Wi-Fi

A laptop connects to Wi-Fi but has extremely poor signal strength compared with nearby computers.

Potential causes:

* Antenna problem
* Wireless card problem
* Driver issue
* Physical obstruction
* Hardware damage

---

### Scenario 3 — Webcam Not Working

A user reports that their webcam doesn't work in Microsoft Teams.

Before replacing the camera:

* Check privacy settings
* Check application permissions
* Check Device Manager
* Test another application
* Check whether the camera is physically damaged

---

### Scenario 4 — Microphone Not Working

A user can hear everyone during a Teams meeting, but nobody can hear them.

Possible causes:

* Wrong input device selected
* Microphone muted
* Application permission problem
* Driver issue
* Hardware failure

---

# Key Terms

| Term          | Definition                                                                 |
| ------------- | -------------------------------------------------------------------------- |
| Battery       | Provides portable power to the device                                      |
| RAM           | Temporary working memory used by the operating system and applications     |
| SSD           | Solid-state storage device                                                 |
| Wireless Card | Hardware used for wireless communication                                   |
| Antenna       | Sends and receives wireless signals                                        |
| Biometrics    | Authentication using physical characteristics                              |
| NFC           | Short-range wireless communication technology                              |
| Webcam        | Camera used for video capture                                              |
| Microphone    | Hardware used to capture audio                                             |
| Soldered      | Permanently attached to the motherboard and generally not user-replaceable |

---

# Study Checklist

* [ ] Understand mobile device batteries
* [ ] Understand battery failure symptoms
* [ ] Understand keyboard and key replacement
* [ ] Understand mobile RAM
* [ ] Understand HDD/SSD replacement
* [ ] Understand wireless cards
* [ ] Understand biometrics
* [ ] Understand NFC
* [ ] Understand Wi-Fi antennas
* [ ] Understand webcams
* [ ] Understand microphones
* [ ] Understand basic mobile hardware troubleshooting
* [ ] Complete hands-on hardware identification lab
* [ ] Complete troubleshooting scenarios
* [ ] Pass practice questions for this objective

---

## Progress

**Status:** 🟡 In Progress

**Next objective:** `1.2 Accessories & Connectivity`
