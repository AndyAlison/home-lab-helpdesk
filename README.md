# Home Lab - IT Helpdesk Simulation

This is my home helpdesk lab where I practice troubleshooting like a real IT Support Technician. I document how I would solve common user problems.

## Tools I Use
- Windows 10/11
- Command Prompt (ipconfig, ping, tracert)
- GitHub for documentation

## Ticket 1: User Cannot Access Internet

**Problem:** User says "No internet" on Windows PC.

**How I troubleshoot:**
1. Ask user what they see - check if WiFi icon has warning
2. Run `ipconfig` to check if they have an IP address
3. Run `ping 8.8.8.8` to test internet, and `ping google.com` to test DNS
4. If no IP: run `ipconfig /release` then `ipconfig /renew`
5. If DNS fails: set DNS to 8.8.8.8 and 1.1.1.1
6. Document solution for user

**Result:** User back online. I explain what happened in simple words.
### Evidence
![My troubleshooting on Mac](Check IP.png)

## Ticket 2: Coming Next
- Printer not working
- Slow computer
- Forgot password

## What I Learned
- How to stay calm and ask clear questions
- How to use basic network commands
- How to document fixes so next time is faster

Created by Andy Alison - Aspiring IT Support Technician | Cape Town
