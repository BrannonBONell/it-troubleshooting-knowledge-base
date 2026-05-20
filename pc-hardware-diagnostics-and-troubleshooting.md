# PC Hardware Diagnostics and Troubleshooting

# Introduction

PC hardware troubleshooting is an essential IT skill used in:
- help desk
- desktop support
- data center environments
- hardware repair
- system administration
- gaming PC support

Effective troubleshooting requires:
- isolating variables
- documenting symptoms
- testing components methodically

---

# Common Hardware Components

# CPU
Processes instructions and system operations.

Common issues:
- overheating
- instability
- bent pins
- thermal throttling

---

# RAM
Temporary system memory.

Common issues:
- crashes
- BSODs
- instability
- boot failures

---

# GPU
Handles graphics rendering and display output.

Common issues:
- overheating
- artifacting
- driver crashes
- black screens

---

# Power Supply (PSU)
Provides power to all components.

Common issues:
- random shutdowns
- no power
- instability under load

---

# Motherboard
Connects and manages communication between components.

Common issues:
- failed ports
- POST failures
- BIOS corruption
- faulty VRMs

---

# Storage Devices

Examples:
- SATA SSD
- NVMe SSD
- HDD

Common issues:
- drive detection failures
- corruption
- slow performance
- boot issues

---

# Initial Troubleshooting Process

# 1. Identify Symptoms

Examples:
- no display
- no power
- random restarts
- overheating
- freezing
- boot loops

Document:
- exact symptoms
- frequency
- recent changes
- error messages

---

# 2. Check Physical Connections

Verify:
- power cables
- RAM seating
- GPU seating
- storage cables
- front panel connectors

Loose connections are common causes of issues.

---

# 3. Check for POST Behavior

POST = Power-On Self-Test

Possible symptoms:
- beep codes
- debug LEDs
- no display
- reboot loops

Common indicators:
- DRAM light
- CPU light
- VGA light
- BOOT light

---

# Common Hardware Troubleshooting Scenarios

# Scenario 1
System powers on but no display.

Possible causes:
- loose GPU
- faulty RAM
- incorrect monitor input
- failed GPU
- BIOS issue

Troubleshooting:
1. Reseat GPU
2. Test integrated graphics
3. Test another monitor/cable
4. Test RAM individually
5. Clear CMOS

---

# Scenario 2
Random shutdowns during gaming.

Possible causes:
- overheating
- PSU instability
- GPU hotspot temperatures
- unstable overclock

Check:
- CPU temperatures
- GPU temperatures
- Event Viewer logs

---

# Scenario 3
NVMe SSD not detected.

Possible causes:
- faulty M.2 slot
- BIOS settings
- lane sharing conflicts
- failed SSD

Troubleshooting:
1. Reseat drive
2. Test alternate slot
3. Update BIOS
4. Verify BIOS detection
5. Test drive in another system

---

# Scenario 4
Frequent BSODs.

Possible causes:
- RAM instability
- corrupted drivers
- overheating
- storage corruption

Check:
- MemTest86
- Event Viewer
- temperatures
- SMART data

---

# Temperature Monitoring

# Common Monitoring Tools

- HWInfo64
- HWMonitor
- MSI Afterburner

---

# Temperature Guidelines

# CPU
Typical safe range:
- idle: 30C–50C
- load: under 90C preferred

---

# GPU
Typical safe range:
- load: 65C–85C
- hotspot ideally under 100C

---

# RAM Troubleshooting

# Common Symptoms
- random crashes
- BSODs
- instability under load
- failure to boot

---

# Troubleshooting Steps

1. Reseat RAM
2. Test one stick at a time
3. Disable XMP/EXPO
4. Run MemTest86
5. Test alternate DIMM slots

---

# BIOS and CMOS Troubleshooting

# Clear CMOS

Useful for:
- failed overclocks
- boot loops
- BIOS corruption symptoms

Methods:
- CMOS button
- jumper pins
- CMOS battery removal

---

# BIOS Updates

Can improve:
- CPU compatibility
- RAM stability
- storage compatibility

Always follow manufacturer instructions carefully.

---

# Storage Diagnostics

# SMART Monitoring

Useful tools:
- CrystalDiskInfo
- Samsung Magician
- WD Dashboard

Signs of failure:
- bad sectors
- health warnings
- slow performance
- disappearing drives

---

# Power Supply Troubleshooting

# Common Symptoms
- random shutdowns
- no power
- instability under load
- reboot loops

---

# Basic Checks
- verify PSU switch
- check cables
- test alternate outlet
- inspect for burning smell

If possible:
- test known-good PSU

---

# Important Troubleshooting Principles

1. Change one variable at a time
2. Start with simplest explanations
3. Verify physical connections first
4. Monitor temperatures
5. Read logs and indicators
6. Document findings

---

# Why Hardware Troubleshooting Matters

Hardware troubleshooting skills are valuable for:
- IT support
- desktop support
- cloud infrastructure
- data centers
- AI infrastructure
- gaming hardware support

Understanding hardware fundamentals improves:
- system administration
- networking
- cloud troubleshooting
- performance analysis
