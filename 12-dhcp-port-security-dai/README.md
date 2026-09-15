# 12 — DHCP, Port Security, DHCP Snooping & Dynamic ARP Inspection

**CCNA Domain:** 5 – Security Fundamentals · **Study plan reference:** Vol 2 Ch. 6–8

## Objective

Chain together the access-layer security features that actually get deployed together in practice: port security to control which devices can even connect, then DHCP snooping and Dynamic ARP Inspection to stop the two classic Layer 2 attacks (rogue DHCP server, ARP spoofing).

## Topology

A switch with a DHCP server (router or dedicated), 2+ client access ports, one port set up to simulate a rogue device. *(Add topology diagram.)*

## Tasks

- [ ] Configure a router or switch as a DHCP server for a client subnet, verify a client leases an address, and check `show ip dhcp binding`
- [ ] Configure port security on an access port (max MAC count, sticky learning, violation mode) and trigger a violation on purpose by connecting a second device — document shutdown vs. restrict vs. protect behavior
- [ ] Enable DHCP snooping, mark the correct uplink as trusted, and simulate a rogue DHCP server on an untrusted port — confirm its offers get dropped
- [ ] Enable Dynamic ARP Inspection using the DHCP snooping binding table, then simulate a gratuitous/spoofed ARP from Kali (this is a natural bridge to the existing cybersecurity lab) and confirm DAI blocks it

## Verification Commands

`show ip dhcp binding`, `show port-security`, `show port-security interface <if>`, `show ip dhcp snooping`, `show ip dhcp snooping binding`, `show ip arp inspection`

## What I Learned

*(Fill in after completing the lab — this is a great one to cross-reference with the Kali/Metasploitable lab for an attacker's-eye view of what these controls actually stop.)*
