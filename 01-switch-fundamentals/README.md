# 01 — Switch Fundamentals

**CCNA Domain:** 1 – Network Fundamentals · **Study plan reference:** Vol 1 Part II (Ch. 4–7)

## Objective

Get comfortable with the Cisco IOS CLI and basic switch administration before anything topology-specific: navigating exec modes, configuring management access, and verifying interface status.

## Topology

2 switches connected by a single trunk-capable link, each with one PC (or loopback) attached to a access port. *(Add topology diagram here once built — export from GNS3 or draw.io into `topology.png`.)*

## Tasks

- [ ] Navigate user EXEC → privileged EXEC → global config → interface config, and back
- [ ] Set hostname, configure `enable secret`, local username/password, and `service password-encryption`
- [ ] Configure SSH access (domain name, RSA key, `line vty` transport input ssh) and disable Telnet
- [ ] Assign a management IP to a switch (SVI on VLAN 1 or a dedicated management VLAN) and verify reachability
- [ ] Configure interface speed/duplex/description on at least one interface, then verify with `show interfaces status`
- [ ] Deliberately misconfigure duplex to trigger a mismatch, observe the symptom, then fix it
- [ ] Save the config and reload one switch to confirm persistence

## Verification Commands

`show running-config`, `show version`, `show ip interface brief`, `show interfaces status`, `show mac address-table`, `show users`

## Configs

Export `show running-config` from each device into `configs/` once the lab is built.

## What I Learned

*(Fill in after completing the lab — what surprised you, what you had to look up, any command syntax that didn't match what you expected from the book.)*
