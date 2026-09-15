# 02 — VLANs and Trunking

**CCNA Domain:** 2 – Network Access · **Study plan reference:** Vol 1 Part III (Ch. 8), Vol 2 Ch. 13

## Objective

Build a multi-switch VLAN topology with trunking and inter-VLAN routing, matching the kind of segmentation you'd actually deploy at a small office (e.g., separating advisor workstations from guest/voice traffic).

## Topology

2 switches trunked together, 3 VLANs (e.g., 10-Staff, 20-Guest, 99-Native/Management), a router-on-a-stick or L3 switch for inter-VLAN routing, one PC per VLAN. *(Add topology diagram.)*

## Tasks

- [ ] Create VLANs and assign access ports on both switches
- [ ] Configure the trunk link (802.1Q, explicit native VLAN, allowed VLAN list)
- [ ] Configure router-on-a-stick (or SVIs on an L3 switch) for inter-VLAN routing
- [ ] Verify PCs in different VLANs can reach their default gateway but not each other without routing
- [ ] Break the native VLAN match on purpose (mismatch it on one side) and observe/document the symptom in `show interfaces trunk` and CDP warnings
- [ ] Add a voice VLAN on one access port and verify with `show interfaces switchport`

## Verification Commands

`show vlan brief`, `show interfaces trunk`, `show interfaces switchport`, `show ip route`, `ping`/`traceroute` between VLANs

## What I Learned

*(Fill in after completing the lab.)*
