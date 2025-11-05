# Project Alpha

**Project Alpha** is a self-hosted infrastructure platform designed to run virtual machines and containers for hosting a wide range of services and applications. The project aims to provide a robust learning simulating production environment, primarily for personal and educational use leveraging open source softwares, applications and recycled hardware. Project Alpha's backbone run on Proxmox Virtual Environment using Dell Servers and Cisco hardware using two tier network architecture to deliver high availability and scalability.

## Purpose

- Host essential daily services: Cloud photos & files backup, media/music streaming, password manager, home automation, communication applications. 
- Network management and monitoring, network tools i.e. DNS, DHCP.
- Docker containers for application hosting.

## Infrastructure Overview

- **Networking Hardware:**  
  - Cisco Catalyst Switches in a 2-tier architecture  
  - LACP LAG trunk—a dual 1Gb link for increased LAN bandwidth between Core and Access switches.  
  - Network segmentation to segregate the traffic for groups. 
  - Point-to-point uplink to OPNsense firewall (external routing)
  - Pi-hole server for DNS and Kea for DHCP

- **Virtualization Platform:**  
  - Proxmox VE for primary and backup server using Enterprise grade Dell PowerEdge servers.
  - SAS drives configured in RAIDZ2 for resilience and performance.
  - Management via iDRAC and LACP LAG to network switch for high bandwidth passthrough.

## Target Audience

- Designed for technically-savvy individuals, primarily system and network administrators interested in learning, testing, and hosting their own services.
- Secondary purpose: Enable friends and family to access virtual labs for learning—**not for commercial use**.

## Goals

- Deliver a highly available, resilient, and scalable home datacenter environment.
- Focus on future-proof design and hardware longevity.

## Features

- Segmented LAN for security and management
- High-bandwidth backbone and redundancy
- Self-hosted, privacy-respecting applications
- Expandable virtualization for labs and real-world service hosting

---

This project combines hands-on learning, self-hosted service reliability, and advanced networking practices.  
**Project Alpha** is designed for those who trust in doing things themselves—and want the best for their everyday digital needs.
