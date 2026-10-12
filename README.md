# Home Lab Helpdesk - IT Support Tickets

Real-world L1 Helpdesk troubleshooting documented from macOS.

## Tickets Completed: 10/10

### Ticket 01 - No Internet / Network Troubleshooting
- Diagnosis: `ifconfig`, `ping 8.8.8.8`,ping google.com, `traceroute`, DNS checks
- Evidence: `evidence-network.png`
- File: `ticket-01-network.md`
- Status: Done

### Ticket 02 - Printer Not Working
- Diagnosis: `lpstat -p -d`, `lpstat -t`, `lpq` - CUPS scheduler running but no destinations
- Root Cause: No printer configured, no default destination
- Evidence: `evidence-printer.png` (full chain in one screenshot)
- File: `ticket-02-printer.md`
- Status: Done

### Ticket 03 - Slow Computer / Disk Full
- Diagnosis: df -h (6.5Gi free), top (71M free, Load 5.08), du -sh (23G in Downloads)
- Evidence: evidence-slow-disk.png, evidence-slow-top.png, evidence-slow-du.png
- Status: Done

### Ticket 04 - User Access Denied / Permissions
- Diagnosis: whoami, id, ls -la, sudo -l, last
- Evidence: evidence-permissions.png
- Status: Done

### Ticket 05 - Software Won't Install / App Blocked
- Diagnosis: ls Downloads, xattr, spctl --status, ls -la /Applications, ps aux
- Evidence: evidence-software.png
- Status: Done

###  Ticket 06 - User Login Failure
- Diagnosis: ls -la, who, dscl list/Users, id (whoami), dscl read/Users 
- Evidence: evidence-login.png
- Status: Done

###  Ticket 07 - Incorrect Date/Time Causing SSL/Login Failures
- Diagnosis: date, sudo sntp, sudo systemsetup timezone, sudo systemsetup networktimeserver
- Evidence: evidence-daztetime.png
- Status: Done
  
###  Ticket 08 - No Sound / Audio Not Outputting
- Diagnosis: system_profiler SPAudioDataType, osascript, ps aux
- Evidence: evidence-audio.png
- Status: Done
  
###  Ticket 09 - Bluetooth Not Working / Device Won't Pair
- Diagnosis: system_profiler SPBluetoothDataType, defaults read, ps aux 
- Evidence: evidence-bluetooth.png
- Status: Done

###  Ticket 10 - Slow Boot / Too Many Startup Items / Boot Failure 
- Diagnosis: pmset -g log, launchctl list, ls -la
- Evidence: evidence-startup.png
- Status: Done

## Core Skills Demonstrated
Terminal, Network Diagnostics, CUPS Printing, Performance Triage, User Management, macOS Gatekeeper, Permissions, pfctl, system_profiler, launchctl, sntp, dscl, cupsctl

**By Andiswa Alison Pongoma | IT Helpdesk | Cape Town**
## What I Learned
- How to stay calm and ask clear questions
- How to use basic network commands
- How to document fixes so next time is faster

Created by Andy Alison - IT Support Technician | Cape Town
