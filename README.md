# Home Lab Helpdesk - IT Support Tickets

Real-world L1 Helpdesk troubleshooting documented from macOS.

## Tickets Completed: 3/10

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

## Skills Demonstrated
macOS troubleshooting, Terminal, CUPS printing, networking, L1 documentation, GitHub

**By Andiswa Pongoma | IT Helpdesk | Cape Town**
## What I Learned
- How to stay calm and ask clear questions
- How to use basic network commands
- How to document fixes so next time is faster

Created by Andy Alison - IT Support Technician | Cape Town
