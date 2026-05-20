# Windows BSOD Troubleshooting Guide

## Common Symptoms
- Blue screen crashes during gaming
- Random system restarts
- Freezing before reboot
- Crashes during Windows startup
- Kernel-Power Event ID 41

---

# Common Causes

## Hardware Related
- Faulty RAM
- Overheating CPU/GPU
- Unstable overclock
- Failing SSD/NVMe
- Power supply instability
- Motherboard issues

## Software Related
- Corrupted drivers
- Windows updates
- GPU driver conflicts
- Corrupted system files
- Antivirus conflicts

---

# Initial Troubleshooting Steps

## 1. Record Error Information
Document:
- BSOD stop code
- Error message
- When crash occurs
- Recent hardware/software changes

Common examples:
- MEMORY_MANAGEMENT
- IRQL_NOT_LESS_OR_EQUAL
- CRITICAL_PROCESS_DIED
- SYSTEM_SERVICE_EXCEPTION

---

# 2. Check Event Viewer

## Open Event Viewer
1. Press Windows + X
2. Select Event Viewer
3. Navigate to:
   Windows Logs > System

Look for:
- Critical events
- Kernel-Power Event ID 41
- Driver-related errors

---

# 3. Monitor Temperatures

## Recommended Tools
- HWInfo64
- MSI Afterburner
- HWMonitor

Check:
- CPU temperatures
- GPU hotspot temperatures
- Idle vs load temperatures

Potential overheating indicators:
- CPU above 90C
- GPU hotspot above 100C

---

# 4. Test RAM

## Windows Memory Diagnostic
1. Press Windows key
2. Search:
   Windows Memory Diagnostic
3. Restart and test

## MemTest86
Use for deeper RAM testing.

Possible indicators:
- Multiple errors
- System instability under load
- Random application crashes

---

# 5. Check System Files

## Run SFC Scan

Open Command Prompt as Administrator:

```powershell
sfc /scannow
```

## Run DISM Repair

```powershell
DISM /Online /Cleanup-Image /RestoreHealth
```

---

# 6. Update Drivers

Focus on:
- GPU drivers
- Chipset drivers
- Network drivers
- Storage drivers

Best practice:
- Download directly from manufacturer websites

Examples:
- NVIDIA
- AMD
- Intel
- ASUS
- MSI

---

# 7. BIOS Troubleshooting

Check:
- BIOS updates
- XMP/EXPO stability
- CPU overclock settings
- Secure Boot configuration

Common fixes:
- Disable unstable overclock
- Reset BIOS to defaults
- Update motherboard BIOS

---

# 8. Storage Troubleshooting

Symptoms:
- Freezing
- Boot issues
- Corrupted files

Check:
- SMART status
- SSD health
- Drive temperatures

Useful tools:
- CrystalDiskInfo
- Manufacturer SSD software

---

# 9. Driver Isolation

## Safe Mode Testing
Boot into Safe Mode to determine if crashes are driver-related.

If stable in Safe Mode:
- likely software/driver issue

---

# 10. Final Isolation Steps

If issue persists:
- Test one RAM stick at a time
- Swap PSU if possible
- Test alternate GPU
- Reinstall Windows
- Test components in another system

---

# Helpful Commands

## System File Checker

```powershell
sfc /scannow
```

## DISM Repair

```powershell
DISM /Online /Cleanup-Image /RestoreHealth
```

## Check Disk

```powershell
chkdsk /f
```

---

# Key Lessons

- Document changes before troubleshooting
- Eliminate one variable at a time
- Prioritize hardware stability first
- Check logs before replacing parts
- Never assume the BSOD message alone identifies the root cause
