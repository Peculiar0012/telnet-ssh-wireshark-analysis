# Telnet vs SSH Traffic Analysis with Wireshark

## Recommended GitHub repository
- **Name:** `telnet-vs-ssh-wireshark-lab`
- **Description:** A beginner-friendly Wireshark lab comparing Telnet plaintext traffic with SSH-encrypted sessions on localhost, with commands, screenshots, observations, and security lessons.

## Overview
This project follows the supplied *Practical Lab: Comparing Telnet and SSH Traffic in Wireshark*. Capture local Telnet and SSH sessions on the loopback interface, apply Wireshark display filters, follow TCP streams, and document the differences.

## Learning objectives
- Capture traffic on a loopback interface (often `lo`).
- Identify a local Telnet session and inspect its TCP stream.
- Observe that Telnet application data may be readable as plaintext.
- Identify a local SSH session and inspect its TCP stream.
- Compare the results and explain why SSH is preferred for secure remote administration.

## Repository structure
```text
telnet-vs-ssh-wireshark-lab/
├── README.md
├── .gitignore
├── commands_used.txt
├── commands/
├── docs/
├── evidence/
├── notes/
└── screenshots/
```

## Required environment
- Linux VM or lab workstation with Wireshark installed.
- Working local Telnet service.
- Working local SSH service.
- Terminal permission to start Wireshark and connect to `localhost`.

Use dedicated lab accounts and harmless test commands. Only capture systems and accounts you are authorized to use.

## Workflow
1. Read `docs/lab-overview.md`.
2. Follow `docs/procedure.md`.
3. Record your actual findings in `docs/observations.md`.
4. Answer the questions in `docs/reflection-questions.md`.
5. Add your own sanitized screenshots to `screenshots/`.
6. Complete `evidence/evidence-checklist.md`.
7. Review staged files for sensitive information before pushing.

## Push to GitHub using Git Bash
Create an empty GitHub repository named `telnet-vs-ssh-wireshark-lab`. Extract this ZIP, open Git Bash in the extracted folder, then run:

```bash
git init
git add .
git status
git commit -m "Add Telnet vs SSH Wireshark lab documentation"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/telnet-vs-ssh-wireshark-lab.git
git push -u origin main
```

Replace `YOUR-USERNAME` with your GitHub username. Review `git status` before committing. If the remote already exists, inspect it with `git remote -v`.

## Portfolio summary
This lab demonstrates packet capture and protocol analysis using Wireshark. It compares Telnet's plaintext application data with SSH's encrypted session traffic and documents the security implications for remote administration.

## Suggested screenshots
- `screenshots/telnet-filter.png`
- `screenshots/telnet-stream.png`
- `screenshots/ssh-filter.png`
- `screenshots/ssh-stream.png`

Only add screenshots you actually captured. Never commit packet captures or screenshots exposing passwords, tokens, authentication data, private IP addresses, hostnames, or other sensitive information. `.gitignore` excludes common capture file extensions.

## Completion checklist
- [ ] Captured Telnet traffic on loopback.
- [ ] Applied `telnet` filter and inspected Follow TCP Stream.
- [ ] Captured SSH traffic on loopback.
- [ ] Applied `ssh` filter and inspected Follow TCP Stream.
- [ ] Answered reflection questions and completed observations.
- [ ] Added genuine, sanitized screenshots.
- [ ] Checked for secrets and capture files before pushing.
