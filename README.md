# NetworkWalks | Week 1 – Project 1: Cybersecurity Lab Setup

> A hands-on learning project documenting the preparation of a cybersecurity lab with Oracle VM VirtualBox and Kali Linux.

## Project overview

This repository records the setup process for a beginner cybersecurity lab. It is intended to document the installation, configuration, verification, and troubleshooting work completed during NetworkWalks Week 1, Project 1.

**Project status:** Installation and documentation in progress. Update each section only after verifying it on your own system.

## Objectives

- Prepare a virtualization environment using Oracle VM VirtualBox.
- Install and boot Kali Linux in a virtual machine.
- Review VM hardware and storage settings.
- Configure the required virtual network and verify connectivity.
- Capture implementation screenshots.
- Record real troubleshooting steps and learning outcomes.

## Tools and technologies

| Tool | Purpose |
|---|---|
| Oracle VM VirtualBox | Run the virtual machine |
| Kali Linux | Linux environment for cybersecurity learning |
| Windows host | Host operating system |
| GitHub | Version-controlled project documentation |

Record the exact versions used in `documentation/environment-details.md`.

## Lab architecture

```text
Windows Host
└── Oracle VM VirtualBox
    └── Kali Linux Virtual Machine
        └── Virtual network (record the actual mode and settings)
```

This is a logical overview. Add other virtual machines or network components only if you actually deploy and verify them.

## Implementation record

### 1. VirtualBox preparation
Document the VirtualBox version, VM name, allocated CPU/RAM, and virtual disk size in `documentation/environment-details.md`.

### 2. Kali Linux installation
The installation workflow includes selecting the desktop environment and software collections, configuring the virtual disk, installing GRUB, and completing the first boot.

Record the Kali release and installation outcome after the VM boots successfully.

### 3. Network configuration
Record the actual adapter mode, network name, CIDR, guest interface, IP address, default gateway, and DNS resolver in `documentation/network-configuration.md`.

Useful commands inside Kali:

```bash
ip a
ip route
cat /etc/resolv.conf
```

Connectivity checks (use the actual gateway shown by `ip route`):

```bash
ping -c 4 <gateway-ip>
getent hosts kali.org
```

A failed ping alone does not prove the network is unavailable; ICMP traffic may be filtered.

### 4. Shared folder and snapshot
If these are part of your completed setup, document the host folder, guest mount location, permissions, and snapshot name in `documentation/verification-checklist.md`. Do not mark them complete until verified.

## Screenshots

Place your own implementation screenshots in the matching folders:

- `screenshots/installation/` – Kali installer, GRUB, completion, first boot
- `screenshots/virtualbox/` – VM settings and VirtualBox version
- `screenshots/network/` – adapter settings, `ip a`, routes, DNS
- `screenshots/verification/` – connectivity, shared folder, snapshot

Use descriptive filenames such as `01-kali-installer.png` and `02-grub-installation.png`.

## Troubleshooting

A troubleshooting log template is available at `documentation/troubleshooting.md`. Record only issues you personally encountered and the resolution you verified.

## Learning outcomes

Complete this section after testing the lab. Potential topics include virtualization, Linux installation, VM storage, network interface inspection, routing, DNS, and technical documentation. Mention only the skills demonstrated by your own work.

## Security and ethical use

Use this lab for education and authorized testing only. Test only systems you own or have explicit permission to assess. Keep intentionally vulnerable targets isolated.

## Official resources

- [Kali Linux documentation](https://www.kali.org/docs/)
- [Kali Linux downloads](https://www.kali.org/get-kali/)
- [Oracle VM VirtualBox](https://www.virtualbox.org/)
- [VirtualBox User Manual](https://www.virtualbox.org/manual/)

## Author and submission details

- **Author:** [Enter your name]
- **NetworkWalks ID:** [Enter your assigned ID, if applicable]
- **Program:** NetworkWalks
- **Week:** 1
- **Project:** 1 – Cybersecurity Lab Setup
- **GitHub repository:** [Add repository URL after creating it]
- **LinkedIn post:** [Add post URL after publishing]

---

**Evidence standard:** This README is a project template. Replace placeholders, add your own screenshots, and update completion statuses only after checking the actual lab.
