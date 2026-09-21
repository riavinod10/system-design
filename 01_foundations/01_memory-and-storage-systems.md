### Computer Memory & Storage

Computer memory and storage are both used to hold data, but they serve different purposes.

**Memory** is mainly used for data that the computer needs to access quickly while it is running, whereas **storage** is used to retain data for longer periods.

### Memory

Memory can be divided into **RAM** and **ROM**.

**RAM (Random Access Memory)** stores the programs and data that are currently being used by the computer. It is fast, but it is **volatile**, meaning its contents are lost when the power is switched off.

**ROM (Read-Only Memory)** is **non-volatile**, so it retains its contents even when the computer is powered off. It stores important information required to start and operate the hardware, such as firmware and BIOS.

### Types of RAM

RAM is mainly of two types:

**1. SRAM — Static RAM**

SRAM is faster and more expensive than DRAM. It does not need to be constantly refreshed and is therefore suitable for applications where very fast access is required.

→ **Used in CPU caches**

**2. DRAM — Dynamic RAM**

DRAM is slower and cheaper than SRAM. It needs to be periodically refreshed to retain its data.

Different forms of DRAM include **FPM DRAM, EDO DRAM, SDRAM and DDR SDRAM**. Many older types are now obsolete, while modern systems commonly use **DDR4 and DDR5**.

**GDDR** is a type of DRAM designed for high data-transfer rates and is commonly used by GPUs because GPUs need to process large amounts of data in parallel.

### SRAM vs DRAM

```text
              RAM
               │
       ┌───────┴───────┐
       │               │
      SRAM            DRAM
       │               │
   Faster            Slower
   Expensive         Cheaper
   No refresh        Needs refresh
       │               │
   CPU Cache       Main Memory
```

---

### Firmware and BIOS

**Firmware** is software stored in non-volatile memory that controls the operation of hardware and allows hardware components to work correctly.

**BIOS (Basic Input/Output System)** is firmware that runs when the computer is powered on. It initializes the hardware and starts the boot process before handing control over to the operating system.

```text
Power ON
   ↓
BIOS starts
   ↓
Hardware initialized
   ↓
Operating System loaded
```

---

### Storage

Storage is generally **non-volatile**, so data remains even after the computer is switched off.

The main types discussed are:

- HDD
- SSD
- USB / Flash Drive
- SD Card

### HDD — Hard Disk Drive

HDDs store data on **spinning magnetic disks**.

They provide large storage capacities at a relatively low cost, but they are slower because they contain moving mechanical parts.

```text
HDD
 ↓
Spinning magnetic disks
 ↓
Moving parts
 ↓
Slower access
```

### SSD — Solid State Drive

SSDs use **NAND-based flash memory** instead of spinning disks.

Compared with HDDs, SSDs provide:

- Faster access to data
- Lower power consumption
- Better resistance to physical shock
- No moving mechanical parts
- Lower latency

The trade-off is that SSDs generally cost more for the same amount of storage.

```text
HDD → Magnetic disks + Moving parts
SSD → NAND flash + No moving parts
```

### NVMe

**NVMe (Non-Volatile Memory Express)** is a high-performance interface/protocol designed for SSDs.

Unlike traditional SATA-based SSDs, NVMe SSDs communicate through **PCIe lanes**, which allows higher data-transfer rates and lower latency.

```text
SATA SSD
SSD → SATA → System

NVMe SSD
SSD → PCIe → CPU
          ↓
    Lower latency
    Higher speed
```

---

### Flash Drives and SD Cards

**Flash drives**, also called USB drives or thumb drives, are small portable storage devices connected through USB. They are commonly used for transferring files between computers.

**SD cards** are also flash-based storage and are commonly used in cameras, smartphones and other portable devices.

They are available in different physical sizes:

```text
SD
├── miniSD
└── microSD
```

---

### Overall Picture

```text
                  COMPUTER MEMORY & STORAGE
                           │
              ┌────────────┴────────────┐
              │                         │
           MEMORY                    STORAGE
              │                         │
       ┌──────┴──────┐          ┌───────┼────────┐
       │             │          │       │        │
      RAM           ROM         HDD     SSD     Flash
       │             │                   │        │
  ┌────┴────┐    Firmware              NVMe    ┌─┴─┐
  │         │    / BIOS                  │     USB SD
 SRAM      DRAM                         PCIe
  │         │
CPU Cache   │
            ├── SDRAM
            ├── DDR4
            ├── DDR5
            └── GDDR → GPU
```

### Quick Revision

- **RAM** → Fast, temporary and volatile
- **SRAM** → Faster, expensive → CPU cache
- **DRAM** → Cheaper, needs refresh → Main memory
- **GDDR** → High bandwidth → GPU
- **ROM** → Non-volatile → Firmware / BIOS
- **HDD** → Magnetic disks + moving parts → Cheap, large storage
- **SSD** → NAND flash + no moving parts → Faster storage
- **NVMe** → Uses PCIe → High-performance SSD storage
- **USB Drive** → Portable flash storage
- **SD Card** → Small portable flash storage

> **Memory → fast access while working**  
> **Storage → persistent data for the long term**
