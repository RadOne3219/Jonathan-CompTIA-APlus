# HDD / SSD

## CompTIA A+ Core 1 — Objective 1.1

Storage devices provide long-term, non-volatile storage for the operating system, applications, and user data.

For the A+ exam, you should understand common storage technologies, interfaces, form factors, and basic replacement and troubleshooting procedures.

---

# 1. HDD — Hard Disk Drive

A **Hard Disk Drive (HDD)** stores data magnetically on spinning platters.

Major components include:

* Platters
* Spindle motor
* Read/write heads
* Actuator arm

Because an HDD contains moving mechanical components, it is generally more vulnerable to physical shock than an SSD.

### Advantages

* Large capacities
* Generally inexpensive per gigabyte
* Widely available

### Disadvantages

* Mechanical components
* Slower than SSDs
* More sensitive to physical shock
* Produces noise
* Uses more power than many SSDs

---

# 2. SSD — Solid-State Drive

A **Solid-State Drive (SSD)** stores data using flash memory.

SSDs have no spinning platters or mechanical read/write heads.

### Advantages

* Faster than traditional HDDs
* No moving mechanical components
* More resistant to physical shock
* Quiet
* Generally lower power consumption
* Excellent for mobile computers

### Disadvantages

* Can cost more per gigabyte
* Flash memory has a finite write endurance
* Failure can occur without the mechanical warning signs sometimes associated with HDDs

---

# 3. HDD vs. SSD

| Feature           | HDD               | SSD              |
| ----------------- | ----------------- | ---------------- |
| Technology        | Magnetic          | Flash memory     |
| Moving parts      | Yes               | No               |
| Noise             | Possible          | Silent           |
| Shock resistance  | Lower             | Higher           |
| Speed             | Generally slower  | Generally faster |
| Power consumption | Generally higher  | Generally lower  |
| Mobile devices    | Less common today | Very common      |

### A+ Exam Tip

Remember:

**HDD = spinning magnetic platters**

**SSD = flash memory**

---

# 4. SATA

**SATA** stands for:

**Serial ATA — Serial Advanced Technology Attachment**

SATA is an interface used to connect storage devices to a computer.

Common SATA storage devices include:

* 2.5-inch SATA HDDs
* 2.5-inch SATA SSDs

SATA can also be used with other storage-related devices.

---

# 5. 2.5-Inch Drives

The 2.5-inch form factor has historically been common in laptops.

Examples:

* 2.5-inch SATA HDD
* 2.5-inch SATA SSD

These drives are typically connected using:

* SATA data interface
* SATA power interface

In many laptops, a 2.5-inch drive is mounted inside the chassis using a bracket or caddy.

---

# 6. M.2

**M.2** is a compact form factor used for devices such as SSDs and wireless adapters.

M.2 SSDs can use different interfaces.

Common examples include:

* M.2 SATA
* M.2 NVMe

### Important

**M.2 does not automatically mean NVMe.**

M.2 describes the physical form factor.

NVMe describes a storage protocol designed for high-speed flash storage over PCIe.

---

# 7. NVMe

**NVMe** stands for:

**Non-Volatile Memory Express**

NVMe is a storage protocol designed for non-volatile memory, particularly SSDs.

NVMe SSDs commonly communicate over:

**PCI Express (PCIe)**

This allows significantly higher performance than traditional SATA-based storage.

---

# 8. SATA vs. NVMe

| Feature             | SATA SSD       | NVMe SSD                     |
| ------------------- | -------------- | ---------------------------- |
| Interface           | SATA           | PCIe                         |
| Protocol            | SATA/AHCI      | NVMe                         |
| Typical performance | Fast           | Very fast                    |
| Form factors        | 2.5-inch / M.2 | Commonly M.2                 |
| Mobile computers    | Common         | Very common in newer systems |

### Exam Tip

Don't confuse:

**M.2 = form factor**

with:

**NVMe = protocol**

---

# 9. Storage Compatibility

Before replacing a laptop drive, verify:

* Physical form factor
* Interface
* Protocol
* Physical dimensions
* Storage capacity
* Manufacturer requirements
* BIOS/UEFI compatibility
* Operating system requirements

### Example

A laptop may have:

**M.2 NVMe SSD**

You should not automatically assume that every M.2 drive is compatible.

Verify the manufacturer's specifications first.

---

# 10. Signs of Storage Failure

Possible storage failure symptoms include:

* Slow system performance
* Operating system errors
* File corruption
* Applications crashing
* Missing files
* Boot errors
* Drive not detected
* Frequent freezes
* Blue screens
* Unusual HDD noises

---

# 11. HDD Failure Sounds

Traditional HDDs contain moving components.

Potential warning signs include:

* Clicking
* Grinding
* Repeated spinning up/down
* Unusual mechanical noises

A failing HDD may continue to work temporarily, but unusual mechanical sounds should be treated seriously.

### ITAM Response

If important data may be at risk:

**Prioritize data preservation before hardware replacement whenever possible.**

---

# 12. SSD Failure

SSDs don't have moving parts, so they won't produce mechanical clicking or grinding sounds.

Possible SSD failure symptoms include:

* Drive not detected
* Operating system fails to boot
* File corruption
* Read/write errors
* System freezes
* Unexpected crashes

SSD failure can sometimes occur suddenly.

---

# 13. Checking Storage in Windows

You can check storage through:

**Settings → System → Storage**

You can also use:

**Disk Management**

Search Windows for:

**Create and format hard disk partitions**

Disk Management can show:

* Physical drives
* Partitions
* Volumes
* File systems
* Drive letters
* Unallocated space

---

# 14. PowerShell Storage Information

PowerShell can be used to collect storage information.

Example:

```powershell
Get-Disk
```

This can show information about physical disks.

You can also use:

```powershell
Get-PhysicalDisk
```

Depending on the system, this can provide information such as:

* Disk type
* Health status
* Operational status
* Size

---

# 15. Boot Failure Tr
