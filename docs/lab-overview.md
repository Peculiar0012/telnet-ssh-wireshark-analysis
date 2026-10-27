# Lab Overview

**Title:** Practical Lab: Comparing Telnet and SSH Traffic in Wireshark  
**Skill level:** Beginner  
**Focus:** Network security, packet capture, encryption

## Goal
Capture local remote-access sessions with Wireshark and compare what can be observed when one session uses Telnet and the other SSH.

## Objectives
- Capture on a loopback interface.
- Identify Telnet packets and follow a Telnet TCP stream.
- Identify SSH packets and follow an SSH TCP stream.
- Compare plaintext visibility and encryption.
- Explain why SSH is preferred for secure remote administration.

## Required environment
- Linux VM or lab workstation with Wireshark.
- Working local Telnet service.
- Working local SSH service.
- Terminal permission to start Wireshark and connect to `localhost`.

## Safety
Use dedicated lab accounts and passwords. Do not place real credentials or production secrets in captures or screenshots. Only capture systems and accounts you are authorized to use.
