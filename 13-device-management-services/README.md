# 13 — Device Management Services

**CCNA Domain:** 4 – IP Services · **Study plan reference:** Vol 2 Ch. 9, 12

## Objective

Wire up the operational-visibility protocols that make a network manageable and that show up constantly in real IT support work: syslog, NTP, CDP/LLDP for topology discovery, SNMP, and HSRP for gateway redundancy.

## Topology

2–3 routers/switches, a syslog server (can be a simple listener on a lab host), redundant gateway routers for HSRP. *(Add topology diagram.)*

## Tasks

- [ ] Configure NTP client/server relationships and verify clock sync with `show ntp status`/`show ntp associations`
- [ ] Configure syslog to send to an external server and set an appropriate severity level, then trigger a log message on purpose and confirm it arrives
- [ ] Enable CDP and/or LLDP and use it to map a topology you didn't already have diagrammed — a nice small proof this is genuinely useful, not just exam trivia
- [ ] Configure SNMP (v2c to start, note where v3 would add security) and pull a value with an SNMP tool from the lab host
- [ ] Configure HSRP between two routers acting as redundant default gateways, fail the active one, and time how fast the standby takes over

## Verification Commands

`show ntp status`, `show logging`, `show cdp neighbors detail`, `show lldp neighbors detail`, `show standby brief`

## What I Learned

*(Fill in after completing the lab.)*
