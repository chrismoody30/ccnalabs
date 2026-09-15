# 09 — Wireless LAN Concepts

**CCNA Domain:** 2 – Network Access · **Study plan reference:** Vol 1 Part VIII (Ch. 26–29)

## Objective

Wireless is the one domain area that's hard to fully lab without a real WLC and APs, so this folder is deliberately lighter on CLI and heavier on documented understanding — plus whatever you *can* touch.

## What's Realistically Labbable

- If GNS3/EVE-NG supports a WLC image in your environment, build a basic autonomous-vs-controller-based comparison and configure a WLAN/SSID with WPA2/WPA3 on the WLC
- Otherwise: use a real consumer AP or your own home Wi-Fi router's admin UI to configure and compare WPA2-Personal vs. WPA3-Personal, and document the differences in the settings available
- Packet capture: use Wireshark against your own home Wi-Fi to observe the 802.11 association/authentication exchange (a legitimate, legal target since it's your own network)

## Tasks

- [ ] Document the difference between autonomous and controller-based (split-MAC) architectures in your own words
- [ ] Configure WPA2 and then WPA3 on an available AP/WLC and note every settings difference
- [ ] Capture and briefly analyze the 802.11 association process on your own home network with Wireshark
- [ ] Write up how a WLC-based deployment (multiple APs, one controller) would differ operationally from the autonomous AP you have access to

## What I Learned

*(Fill in after completing the lab.)*
