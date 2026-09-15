# 00 — Lab Environment Setup

## Goal

Stand up a repeatable network simulation environment on the same VMware host that already runs Kali/Metasploitable, capable of running real Cisco IOS behavior — not just Packet Tracer's simplified simulation — so the CLI output in this repo reflects genuine device behavior.

## Recommended Path

**GNS3 (free, open source) + Cisco IOS images**

GNS3 emulates real network topologies and, unlike Packet Tracer, can run actual Cisco IOS/IOSv images rather than a simplified simulation — the CLI behavior, `show` output, and edge cases match what you'll see on real gear. Two ways to get legitimate IOS images to run inside it:

1. **Cisco Modeling Labs (CML) Personal / Student license** (~$199/yr, steep student/NetAcad discounts often available) — the officially licensed way to get IOSv and IOSvL2 reference platform images. Once installed, the IOSv/IOSvL2 disk images can be imported into GNS3 as custom Qemu appliances.
2. **Cisco Packet Tracer** (free, official, from the Cisco Networking Academy) as a lower-cost starting point — it covers the full CCNA syllabus (VLANs, STP, OSPF, ACLs, NAT, DHCP, port security) well enough for exam prep and early labs, just with Cisco's simplified CLI simulation rather than real IOS. A reasonable plan: start here for Labs 01–04 (switching/VLANs/STP) while deciding whether to invest in CML, then move to GNS3 + real IOS for Labs 06+ (routing/OSPF/NAT/ACLs) where CLI realism matters more for the portfolio.

### Setup Steps (GNS3 on VMware)

1. Download the GNS3 VM appliance (`.ova`) from gns3.com and import it into VMware Workstation/Player alongside the existing Kali/Metasploitable VMs — put it on its own host-only or NAT network segment so lab traffic never touches the production network.
2. Install the GNS3 GUI client on the host machine (or another VM) and point it at the GNS3 VM's management IP.
3. Import IOSv/IOSvL2 images (from a licensed CML install) as Qemu-based appliances in GNS3's appliance manager.
4. Build a "smoke test" topology — two routers back to back — and confirm you can reach privileged EXEC, save a config, and reload without losing it. That confirms the environment is solid before Lab 01 starts.

## Alternative: EVE-NG

EVE-NG Community Edition is a comparable option (also a VM appliance, also supports IOSv/IOSvL2), with a slightly steeper learning curve but a more polished web UI and easier multi-topology management if the lab list grows. Worth considering if GNS3 starts feeling limiting after a few labs.

## What to Document Here Once Set Up

- [ ] Screenshot of the GNS3 VM running alongside the existing lab VMs (VMware library view)
- [ ] Screenshot of the smoke-test topology with both routers reachable
- [ ] Note the exact IOS/IOSv versions used, for reproducibility
- [ ] Note the virtual network segment used for lab traffic (should be isolated from the production home network)
