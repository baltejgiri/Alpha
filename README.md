# Project Alpha

**Project Alpha** is a self-hosted infrastructure platform designed to run virtual machines and containers for hosting a wide range of services and applications. The project aims to provide a robust learning and production environment, primarily for personal use and education in networking and systems administration.

## Purpose

- Host essential daily services: VPN, password manager, notes app, phone/computer photo backups (via Immich), music streaming, Plex media server, and more.
- Run virtual labs using tools like EVE-NG and Cisco Modeling Labs for networking education and Linux administration.

## Infrastructure Overview

- **Networking Hardware:**  
  - 2× Cisco Catalyst 2960 switches in a 2-tier architecture  
  - LACP LAG trunk—a dual 1Gb link for increased LAN bandwidth  
  - Network segmentation: VLANs for Production, Servers, Internet Only, and Device Management  
  - Point-to-point uplink to OPNsense firewall (external routing)  
  - PiHole for DNS and Kea for DHCP

- **Virtualization Platform:**  
  - Proxmox VE cluster on dual Dell PowerEdge R630 servers  
  - SAS drives configured in RAIDZ2 for resilience and performance  
  - Management via iDRAC and high-speed LACP connections to core switch

## Target Audience

- Designed for technically-savvy individuals, primarily network administrators interested in learning, testing, and hosting their own services.
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
