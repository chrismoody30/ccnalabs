# 14 — Network Automation (Stretch Lab)

**CCNA Domain:** 6 – Automation and Programmability · **Study plan reference:** Vol 2 Ch. 16–19

## Objective

The CCNA exam only expects conceptual understanding here (what REST/JSON/Ansible/Puppet/Chef are, not how to write them), but this is the domain that differentiates a portfolio from a certification — actually automating something against the lab devices built in earlier labs.

## Tasks

- [ ] Enable the RESTCONF or NETCONF interface on a lab device (if the IOS image supports it) and pull device data with a simple Python `requests` script
- [ ] Write a basic Ansible playbook that connects to 2–3 lab routers/switches over SSH and pulls `show version` / backs up the running-config to local files
- [ ] Document, in plain language, the difference between Ansible (agentless, push-based) and Puppet/Chef (agent-based, pull-based) — this is exam-testable and worth having in your own words
- [ ] Bonus: extend the Ansible playbook to push a small config change (e.g., add a syslog server) across multiple devices at once and verify it landed

## What I Learned

*(Fill in after completing the lab — this is the strongest "employer-facing" lab in the repo, worth writing up in the most detail.)*
