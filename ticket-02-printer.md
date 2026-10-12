# Ticket 02 - Printer Not Working

**User reports:** "I try to print but nothing happens, no printer showing"

**Environment:** macOS - RE220 (andiswapongoma@RE220)

### Diagnosis Steps:
1. Checked installed printers:
   Result: `No destinations added. no system default destination`

2. Checked CUPS scheduler status:
      Result: `scheduler is running` + `no system default destination` + `No destinations added.`

3. Checked print queue:
      Result: `lpq: Error - no default destination available.`

### Root Cause:
Printer subsystem (CUPS) is running, but no printer is configured and no default destination set. User cannot print because system has no target.

### Resolution Workflow (What L1 would do):
1. Confirm user on correct network / VPN
2. System Settings > Printers & Scanners > Add Printer (IP / AirPrint)
3. Install driver if needed
4. Set as default: `lpadmin -d <printer_name>` or via GUI
5. Test: `lp -d <printer_name> /etc/hosts` or print test page
6. If fails after add: restart CUPS, check driver compatibility

### Evidence:
- `evidence-03-printer-all.png` - Complete chain: lpstat -p -d, lpstat -t, lpq
- Shows diagnostic thinking, not just one command

### Skills demonstrated:
CUPS, lpstat, lpq, macOS printing, L1 troubleshooting, documentation
